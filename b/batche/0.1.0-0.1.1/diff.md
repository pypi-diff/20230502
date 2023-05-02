# Comparing `tmp/batche-0.1.0.tar.gz` & `tmp/batche-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batche-0.1.0.tar", max compression
+gzip compressed data, was "batche-0.1.1.tar", max compression
```

## Comparing `batche-0.1.0.tar` & `batche-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1070 2023-04-27 11:02:47.864806 batche-0.1.0/LICENSE
--rw-r--r--   0        0        0      185 2023-04-27 15:35:13.913284 batche-0.1.0/README.md
--rw-r--r--   0        0        0      107 2023-04-27 15:43:11.636266 batche-0.1.0/batche/__init__.py
--rw-r--r--   0        0        0     4116 2023-04-27 15:43:07.496310 batche-0.1.0/batche/batche.py
--rw-r--r--   0        0        0      665 2023-04-27 15:45:39.502697 batche-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      863 1970-01-01 00:00:00.000000 batche-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-27 11:02:47.864806 batche-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3527 2023-05-01 10:47:30.821158 batche-0.1.1/README.md
+-rw-r--r--   0        0        0       77 2023-04-28 09:12:18.324279 batche-0.1.1/batche/__init__.py
+-rw-r--r--   0        0        0     4557 2023-05-01 10:41:47.028362 batche-0.1.1/batche/batche.py
+-rw-r--r--   0        0        0     4162 2023-04-28 16:21:20.066020 batche-0.1.1/batche/lrucache.py
+-rw-r--r--   0        0        0      694 2023-05-02 15:06:57.845216 batche-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4163 1970-01-01 00:00:00.000000 batche-0.1.1/PKG-INFO
```

### Comparing `batche-0.1.0/LICENSE` & `batche-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `batche-0.1.0/batche/batche.py` & `batche-0.1.1/batche/batche.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,81 +1,97 @@
 import inspect
-from collections import OrderedDict
 from functools import wraps
 from typing import Any, Callable, Dict, List, Optional, TypeVar
 
-from pydantic import ValidationError, parse_obj_as
+from .lrucache import LRUCache
 
 R = TypeVar("R")
 
-batche_cache: Dict[Any, List[R]] = OrderedDict()
+
+class BatcheException(Exception):
+    pass
 
 
 def is_list_annotation(annotation: Any):
-    if annotation is list or (
+    """
+    Check if annotation is a list or a generic list
+    """
+    return annotation is list or (
         hasattr(annotation, "__origin__") and issubclass(list, annotation.__origin__)
-    ):
-        return True
-    return False
+    )
 
 
-def cache_batch_variable(
-    batch_variable_name: Optional[str] = None, max_size: Optional[int] = None
-):
+def validate_function_annotations(
+    func: Callable[..., List[Any]], batch_variable_name: str
+) -> int:
+    """
+    Validate that the batch function has the correct annotations on the batch variable and return value
+    Batch variable must be a list of hashable objects
+    Return value must be a list of Any type
+
+    If annotations are not provided then ignores validation
+    """
+    # validate batch_func
+    function_argspec = inspect.getfullargspec(func)
+    index = -1
+
+    # validate batch_variable_name is a valid argument
+    if (
+        batch_variable_name not in function_argspec.args
+        and function_argspec.varkw is None
+    ):
+        raise BatcheException(
+            f"{batch_variable_name} must be a valid argument of the batch function"
+        )
+
+    # get index of batch_variable argument
+    if batch_variable_name in function_argspec.args:
+        index = function_argspec.args.index(batch_variable_name)
+
+    # validate batch_arg annotation must be list
+    batch_arg_annotations = function_argspec.annotations.get(batch_variable_name)
+    if batch_arg_annotations and not is_list_annotation(batch_arg_annotations):
+        raise BatcheException(
+            f"{batch_variable_name} annotation must be a list of hashable objects"
+        )
+
+    # validate return annotation must be list
+    return_annotation = function_argspec.annotations.get("return")
+    if return_annotation and not is_list_annotation(return_annotation):
+        raise BatcheException("return annotation must be a list")
+
+    return index
+
+
+def cache_batch_variable(batch_variable_name: str, maxsize: Optional[int] = None):
+    batche_cache: Dict[Any, List[R]] = {}
+    if maxsize is not None:
+        batche_cache = LRUCache(maxsize=maxsize)
+
     def internal_cache_batch_decorator(
         func: Callable[..., List[R]]
     ) -> Callable[..., List[R]]:
-        # validate batch_func
-        function_function_argspec = inspect.getfullargspec(func)
-        if batch_variable_name is not None:
-            assert (
-                batch_variable_name in function_function_argspec.args
-            ), f"{batch_variable_name} must be a valid argument of the batch function"
-
-            batch_arg_annotations = function_function_argspec.annotations.get(
-                batch_variable_name
-            )
-            if batch_arg_annotations:
-                assert is_list_annotation(
-                    batch_arg_annotations
-                ), f"{batch_variable_name} annotation must be a list of hashable objects"
-
-        return_annotation = function_function_argspec.annotations.get("return")
-        if return_annotation:
-            assert is_list_annotation(
-                return_annotation
-            ), "return annotation must be a list"
+        arg_index = validate_function_annotations(
+            func, batch_variable_name=batch_variable_name
+        )
 
         @wraps(func)
         def batch_function_wrapper(*args, **kwargs):
             args = list(args)
-            in_args = False
+            in_args = False  # tracks where the batch_variable is (in args or kwargs)
 
-            # check if batch_variable is in args or kwargs
+            # check if batch_variable is in kwargs
             batch_variable = kwargs.get(batch_variable_name)
-            if batch_variable is not None:
-                batch_variable = parse_obj_as(
-                    func.__annotations__.get(batch_variable_name), batch_variable
-                )
-            else:
-                for arg_index, arg in enumerate(args):
-                    try:
-                        # check if batch_variable meets the annotation provided
-                        # NOTE: this will fail if more than one argument
-                        # meets the annotation before batch_variable
-                        batch_variable = parse_obj_as(
-                            func.__annotations__.get(batch_variable_name), arg
-                        )
-                        in_args = True
-                        break
-                    except ValidationError:
-                        continue
-            assert (
-                batch_variable is not None
-            ), f"{batch_variable_name} must be a valid argument of the batch function"
+            if batch_variable is None:
+                if arg_index < 0 or arg_index >= len(args):
+                    raise BatcheException(
+                        f"{batch_variable_name} must be a valid argument of the batch function"
+                    )
+                batch_variable = args[arg_index]
+                in_args = True
 
             # new_batch will contain only the items that are not in cache
             new_batch, new_indices = [], []
 
             # initialize predictions with empty lists
             predictions = [[] for _ in range(len(batch_variable))]
 
@@ -93,18 +109,22 @@
             if in_args:
                 args[arg_index] = new_batch
             else:
                 kwargs[batch_variable_name] = new_batch
 
             # call the function with the new batch
             out = func(*args, **kwargs)
-            assert len(out) == len(
-                new_batch
-            ), "batch function must return a list of predictions of the same length as the batch"
 
+            # validate that the function returns a list of the same length as the new batch
+            if len(out) != len(new_batch):
+                raise BatcheException(
+                    "batch function must return a list of predictions of the same length as the batch"
+                )
+
+            # update the cache and outputs
             for i, prediction in zip(new_indices, out):
                 predictions[i] = prediction
                 batche_cache[batch_variable[i]] = prediction
 
             return predictions
 
         return batch_function_wrapper
```

### Comparing `batche-0.1.0/pyproject.toml` & `batche-0.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 [tool.poetry]
 name = "batche"
-version = "0.1.0"
+version = "0.1.1"
 description = "batch caching decorator"
 authors = ["Gautier Dagan <gautier.dagan@ed.ac.uk>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/gautierdag/batche"
 repository = "https://github.com/gautierdag/batche"
 include = [
     "LICENSE",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-pydantic = "^1.10.7"
 
 [tool.poetry.dev-dependencies]
 pre-commit = "^3.2.2"
 ruff = "^0.0.263"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
@@ -26,8 +25,10 @@
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
 
 [tool.ruff]
+line-length = 88
+select = ["F", "E", "W", "I001"]
 ignore = ["F722", "E501"]
```

