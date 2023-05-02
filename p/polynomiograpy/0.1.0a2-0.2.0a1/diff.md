# Comparing `tmp/polynomiograpy-0.1.0a2.tar.gz` & `tmp/polynomiograpy-0.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polynomiograpy-0.1.0a2.tar", max compression
+gzip compressed data, was "polynomiograpy-0.2.0a1.tar", max compression
```

## Comparing `polynomiograpy-0.1.0a2.tar` & `polynomiograpy-0.2.0a1.tar`

### file list

```diff
@@ -1,9 +1,13 @@
--rw-r--r--   0        0        0     1070 2023-05-01 01:47:51.256690 polynomiograpy-0.1.0a2/LICENSE
--rw-r--r--   0        0        0       68 2023-05-01 01:39:06.537562 polynomiograpy-0.1.0a2/README.md
--rw-r--r--   0        0        0     1998 2023-05-01 03:42:21.865965 polynomiograpy-0.1.0a2/polynomiograpy/__init__.py
--rw-r--r--   0        0        0     2444 2023-05-01 03:32:22.349878 polynomiograpy-0.1.0a2/polynomiograpy/cli/__init__.py
--rw-r--r--   0        0        0     1458 2023-05-01 02:13:32.052248 polynomiograpy-0.1.0a2/polynomiograpy/common/polynomial.py
--rw-r--r--   0        0        0     1256 2023-05-01 02:27:18.245511 polynomiograpy-0.1.0a2/polynomiograpy/compute_screen.py
--rw-r--r--   0        0        0     2279 2023-05-01 03:18:42.322827 polynomiograpy-0.1.0a2/polynomiograpy/methods/iter.py
--rw-r--r--   0        0        0      738 2023-05-01 03:42:08.187485 polynomiograpy-0.1.0a2/pyproject.toml
--rw-r--r--   0        0        0      738 1970-01-01 00:00:00.000000 polynomiograpy-0.1.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-01 01:47:51.256690 polynomiograpy-0.2.0a1/LICENSE
+-rw-r--r--   0        0        0       68 2023-05-01 01:39:06.537562 polynomiograpy-0.2.0a1/README.md
+-rw-r--r--   0        0        0      414 2023-05-02 08:46:19.553798 polynomiograpy-0.2.0a1/polynomiograpy/__init__.py
+-rw-r--r--   0        0        0     4851 2023-05-02 08:45:57.985613 polynomiograpy-0.2.0a1/polynomiograpy/cli/__init__.py
+-rw-r--r--   0        0        0      970 2023-05-02 08:39:43.286847 polynomiograpy-0.2.0a1/polynomiograpy/common/finite_field.py
+-rw-r--r--   0        0        0     1458 2023-05-01 02:13:32.052248 polynomiograpy-0.2.0a1/polynomiograpy/common/polynomial.py
+-rw-r--r--   0        0        0     1991 2023-05-02 08:14:34.251805 polynomiograpy-0.2.0a1/polynomiograpy/iterations/__init__.py
+-rw-r--r--   0        0        0     1266 2023-05-02 07:52:35.745113 polynomiograpy-0.2.0a1/polynomiograpy/iterations/helpers.py
+-rw-r--r--   0        0        0     2279 2023-05-02 07:44:10.901452 polynomiograpy-0.2.0a1/polynomiograpy/iterations/methods.py
+-rw-r--r--   0        0        0      915 2023-05-02 08:43:46.491492 polynomiograpy-0.2.0a1/polynomiograpy/roots/__init__.py
+-rw-r--r--   0        0        0      931 2023-05-02 08:15:06.208942 polynomiograpy-0.2.0a1/polynomiograpy/roots/helpers.py
+-rw-r--r--   0        0        0      738 2023-05-02 08:46:46.725578 polynomiograpy-0.2.0a1/pyproject.toml
+-rw-r--r--   0        0        0      738 1970-01-01 00:00:00.000000 polynomiograpy-0.2.0a1/PKG-INFO
```

### Comparing `polynomiograpy-0.1.0a2/LICENSE` & `polynomiograpy-0.2.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `polynomiograpy-0.1.0a2/polynomiograpy/__init__.py` & `polynomiograpy-0.2.0a1/polynomiograpy/iterations/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from typing import Literal, Callable
-from polynomiograpy.common.polynomial import Polynomial
-from polynomiograpy.compute_screen import compute_screen
-from polynomiograpy.methods import iter
 import numpy as np
-
-__version__ = "0.1.0.a2"
-
-__all__ = ["compute_screen_for_single_poly", "Polynomial"]
+from polynomiograpy.common.polynomial import Polynomial
+from . import helpers
+from . import methods
+from .methods import available_methods
+
+__all__ = [
+    "compute_screen_for_single_poly",
+    "available_methods",
+]
 
 
 def compute_screen_for_single_poly(
     method: Literal["newton", "halley", "steffensen"],
     poly: Polynomial,
     delta: float,
     width: int,
@@ -22,53 +24,53 @@
     scale_y: float = 1,
     shift_x: float = 0,
     shift_y: float = 0,
     max_value: int = 16,
     reverse_color=False,
     channel: int = 0,
 ):
-    assert method in iter.available_methods, "Unknown method"
+    assert method in available_methods, "Unknown method"
     func: Callable[[complex], int]
     if method == "newton":
 
         def func(val: complex) -> int:
-            new_val, iter_count = iter.newton_method(
+            new_val, iter_count = methods.newton_method(
                 poly,
                 val,
                 delta,
                 max_iter_count=max_value,
             )
             return iter_count
 
     elif method == "halley":
 
         def func(val: complex) -> int:
-            new_val, iter_count = iter.halley_method(
+            new_val, iter_count = methods.halley_method(
                 poly,
                 val,
                 delta,
                 max_iter_count=max_value,
             )
             return iter_count
 
     elif method == "steffensen":
 
         def func(val: complex) -> int:
-            new_val, iter_count = iter.steffensen_method(
+            new_val, iter_count = methods.steffensen_method(
                 poly,
                 val,
                 delta,
                 max_iter_count=max_value,
             )
             return iter_count
 
     else:
         # cannot happen
         raise Exception("wtf")
-    return compute_screen(
+    return helpers.compute_np_screen(
         func,
         width,
         height,
         screen,
         screen_buffer,
         scale_x=scale_x,
         scale_y=scale_y,
```

### Comparing `polynomiograpy-0.1.0a2/polynomiograpy/common/polynomial.py` & `polynomiograpy-0.2.0a1/polynomiograpy/common/polynomial.py`

 * *Files identical despite different names*

### Comparing `polynomiograpy-0.1.0a2/polynomiograpy/compute_screen.py` & `polynomiograpy-0.2.0a1/polynomiograpy/iterations/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Callable
 import numpy as np
 
 
-def compute_screen(
+def compute_np_screen(
     func: Callable[[complex], int],
     width: int,
     height: int,
     screen: np.ndarray,
     screen_buffer: np.ndarray,
     *,
     scale_x: float = 1,
@@ -14,15 +14,15 @@
     shift_x: float = 0,
     shift_y: float = 0,
     max_value: int = 16,
     reverse_color: bool = False,
     channel: int = 0,
 ):
     assert len(screen.shape) >= 3, "Wrong shape for screen"
-    assert len(screen_buffer.shape) >= 3, "Wrong shape for screen"
+    assert len(screen_buffer.shape) >= 3, "Wrong shape for screen buffer"
     assert screen.shape == screen_buffer.shape, "screen shape != screen buffer shape"
     origin_x = width / 2
     origin_y = height / 2
     for j in range(height):
         for i in range(width):
             x = (i - origin_x) * scale_x + shift_x
             y = -(j - origin_y) * scale_y + shift_y
```

### Comparing `polynomiograpy-0.1.0a2/polynomiograpy/methods/iter.py` & `polynomiograpy-0.2.0a1/polynomiograpy/iterations/methods.py`

 * *Files identical despite different names*

### Comparing `polynomiograpy-0.1.0a2/pyproject.toml` & `polynomiograpy-0.2.0a1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "polynomiograpy"
-version = "0.1.0.a2"
+version = "0.2.0.a1"
 description = ""
 authors = ["İsmail Tapan <ismltpn@gmail.com>"]
 maintainers = ["İsmail Tapan <ismltpn@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = ""
 repository = "https://github.com/ismltpn/polynomiograpy/"
```

### Comparing `polynomiograpy-0.1.0a2/PKG-INFO` & `polynomiograpy-0.2.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polynomiograpy
-Version: 0.1.0a2
+Version: 0.2.0a1
 Summary: 
 Home-page: https://github.com/ismltpn/polynomiograpy/
 License: MIT
 Keywords: Polynomiography,Polynomials,Visual Art
 Author: İsmail Tapan
 Author-email: ismltpn@gmail.com
 Maintainer: İsmail Tapan
```

