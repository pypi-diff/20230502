# Comparing `tmp/pybrat-0.1.6.tar.gz` & `tmp/pybrat-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybrat-0.1.6.tar", max compression
+gzip compressed data, was "pybrat-0.1.7.tar", max compression
```

## Comparing `pybrat-0.1.6.tar` & `pybrat-0.1.7.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0       69 2022-10-09 01:35:06.967715 pybrat-0.1.6/pybrat/__init__.py
--rw-r--r--   0        0        0    12796 2022-10-09 01:34:31.924925 pybrat-0.1.6/pybrat/parser.py
--rw-r--r--   0        0        0        0 2022-09-06 05:39:52.502627 pybrat-0.1.6/pybrat/py.typed
--rw-r--r--   0        0        0     1476 2022-09-06 05:39:52.502939 pybrat-0.1.6/pybrat/utils.py
--rw-r--r--   0        0        0      420 2022-10-09 01:35:01.412163 pybrat-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      548 1970-01-01 00:00:00.000000 pybrat-0.1.6/setup.py
--rw-r--r--   0        0        0      390 1970-01-01 00:00:00.000000 pybrat-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       69 2023-05-02 14:12:01.282267 pybrat-0.1.7/pybrat/__init__.py
+-rw-r--r--   0        0        0    13837 2023-05-02 14:06:46.086420 pybrat-0.1.7/pybrat/parser.py
+-rw-r--r--   0        0        0        0 2022-09-06 05:39:52.502627 pybrat-0.1.7/pybrat/py.typed
+-rw-r--r--   0        0        0     1476 2022-09-06 05:39:52.502939 pybrat-0.1.7/pybrat/utils.py
+-rw-r--r--   0        0        0      420 2023-05-02 14:12:06.196320 pybrat-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      441 1970-01-01 00:00:00.000000 pybrat-0.1.7/PKG-INFO
```

### Comparing `pybrat-0.1.6/pybrat/parser.py` & `pybrat-0.1.7/pybrat/parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import collections
 import dataclasses
 import itertools
 import os
 import re
 from collections.abc import Iterable
-from typing import Optional, Union
+from typing import Callable, Optional, Union
 
 from pybrat.utils import iter_file_groups
 
 
 @dataclasses.dataclass
 class Reference(object):
     rid: str
@@ -313,22 +313,25 @@
                 self._raise(
                     RuntimeError(
                         "Detected identical span for"
                         f" different entities: [{id_}, {entity.id}]"
                     )
                 )
 
-    def _parse_ann(self, ann, encoding):
+    def _parse_ann(self, ann, encoding, preprocess_function):
         # Parser entities and store required data for parsing relations
         # and events.
         entity_matches, relation_matches, event_matches = [], [], []
         references = collections.defaultdict(list)
 
-        with open(ann, mode="r") as f:
+        with open(ann, mode="r", encoding=encoding) as f:
             for line in f:
+                if preprocess_function is not None:
+                    line = preprocess_function(line)
+
                 line = line.rstrip()
                 if not line or line.startswith("#") or self._should_ignore_line(line):
                     continue
 
                 if line.startswith("T"):
                     if match := self._parse_entity(line):
                         entity_matches += [match]
@@ -366,42 +369,64 @@
 
         return {
             "entities": list(entities.values()),
             "relations": relations,
             "events": list(events.values()),
         }
 
-    def _parse_text(self, txt, encoding):  # pylint: disable=no-self-use
+    def _parse_text(
+        self, txt, encoding, preprocess_function
+    ):  # pylint: disable=no-self-use
         with open(txt, mode="r", encoding=encoding) as f:
-            return f.read()
+            text = f.read()
+            if preprocess_function is not None:
+                text = preprocess_function(text)
+
+            return text
 
     def parse(
-        self, dirname: Union[str, bytes, os.PathLike], encoding: str = "utf-8"
+        self,
+        dirname: Union[str, bytes, os.PathLike],
+        encoding: str = "utf-8",
+        text_preprocess_function: Optional[Callable[[str], str]] = None,
+        ann_preprocess_function: Optional[Callable[[str], str]] = None,
     ) -> list[Example]:
         """Parse examples in given directory.
 
         Args:
             dirname (Union[str, bytes, os.PathLike]): Directory
                 containing brat examples.
             encoding (str): Encoding for reading text files and
                 ann files
+            text_preprocess_function (Optional[Callable[[str], str]]):
+                Function for text pre-processing, will be call on the
+                whole text file before parsing
+            ann_preprocess_function (Optional[Callable[[str], str]]):
+                Function for annotation pre-processing, will be call on
+                each annotation line before parsing
 
         Returns:
             examples (list[Example]): Parsed examples.
         """
 
         examples = []
 
         file_groups = iter_file_groups(
             dirname,
             self.exts,
             missing="error" if self.error == "raise" else "ignore",
         )
 
         for key, (ann_file, txt_file) in file_groups:
-            txt = self._parse_text(txt_file, encoding=encoding)
-            ann = self._parse_ann(ann_file, encoding=encoding)
+            txt = self._parse_text(
+                txt_file,
+                encoding=encoding,
+                preprocess_function=text_preprocess_function,
+            )
+            ann = self._parse_ann(
+                ann_file, encoding=encoding, preprocess_function=ann_preprocess_function
+            )
             examples += [Example(text=txt, **ann, id=key)]
 
         examples.sort(key=lambda x: x.id if x.id is not None else "")
 
         return examples
```

### Comparing `pybrat-0.1.6/pybrat/utils.py` & `pybrat-0.1.7/pybrat/utils.py`

 * *Files identical despite different names*

