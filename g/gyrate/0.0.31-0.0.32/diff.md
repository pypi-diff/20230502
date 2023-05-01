# Comparing `tmp/gyrate-0.0.31.tar.gz` & `tmp/gyrate-0.0.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gyrate-0.0.31.tar", last modified: Mon May  1 23:13:48 2023, max compression
+gzip compressed data, was "gyrate-0.0.32.tar", last modified: Mon May  1 23:18:17 2023, max compression
```

## Comparing `gyrate-0.0.31.tar` & `gyrate-0.0.32.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 23:13:48.501605 gyrate-0.0.31/
--rw-rw-rw-   0        0        0     1069 2023-05-01 18:04:17.000000 gyrate-0.0.31/LICENSE
--rw-rw-rw-   0        0        0     1359 2023-05-01 23:13:48.501605 gyrate-0.0.31/PKG-INFO
--rw-rw-rw-   0        0        0      760 2023-05-01 23:13:04.000000 gyrate-0.0.31/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 23:13:48.476672 gyrate-0.0.31/gyrate/
--rw-rw-rw-   0        0        0      195 2023-05-01 23:02:18.000000 gyrate-0.0.31/gyrate/__init__.py
--rw-rw-rw-   0        0        0     2997 2023-05-01 23:02:18.000000 gyrate-0.0.31/gyrate/_utils.py
--rw-rw-rw-   0        0        0     1321 2023-05-01 18:04:18.000000 gyrate-0.0.31/gyrate/cursor.py
--rw-rw-rw-   0        0        0    16617 2023-05-01 23:02:18.000000 gyrate-0.0.31/gyrate/gyrate.py
--rw-rw-rw-   0        0        0     3221 2023-05-01 23:03:01.000000 gyrate-0.0.31/gyrate/notebook.py
-drwxrwxrwx   0        0        0        0 2023-05-01 23:13:48.497616 gyrate-0.0.31/gyrate.egg-info/
--rw-rw-rw-   0        0        0     1359 2023-05-01 23:13:48.000000 gyrate-0.0.31/gyrate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      321 2023-05-01 23:13:48.000000 gyrate-0.0.31/gyrate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 23:13:48.000000 gyrate-0.0.31/gyrate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      299 2023-05-01 23:13:48.000000 gyrate-0.0.31/gyrate.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-01 23:13:48.000000 gyrate-0.0.31/gyrate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-05-01 23:13:48.503600 gyrate-0.0.31/setup.cfg
--rw-rw-rw-   0        0        0     1241 2023-05-01 23:12:36.000000 gyrate-0.0.31/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-01 23:13:48.500608 gyrate-0.0.31/tests/
--rw-rw-rw-   0        0        0    21363 2023-05-01 23:02:18.000000 gyrate-0.0.31/tests/test_halo.py
--rw-rw-rw-   0        0        0    14198 2023-05-01 23:02:18.000000 gyrate-0.0.31/tests/test_halo_notebook.py
+drwxrwxrwx   0        0        0        0 2023-05-01 23:18:17.233723 gyrate-0.0.32/
+-rw-rw-rw-   0        0        0     1069 2023-05-01 18:04:17.000000 gyrate-0.0.32/LICENSE
+-rw-rw-rw-   0        0        0     1359 2023-05-01 23:18:17.234719 gyrate-0.0.32/PKG-INFO
+-rw-rw-rw-   0        0        0      760 2023-05-01 23:13:04.000000 gyrate-0.0.32/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 23:18:17.201488 gyrate-0.0.32/gyrate/
+-rw-rw-rw-   0        0        0      193 2023-05-01 23:16:34.000000 gyrate-0.0.32/gyrate/__init__.py
+-rw-rw-rw-   0        0        0     2997 2023-05-01 23:02:18.000000 gyrate-0.0.32/gyrate/_utils.py
+-rw-rw-rw-   0        0        0     1321 2023-05-01 18:04:18.000000 gyrate-0.0.32/gyrate/cursor.py
+-rw-rw-rw-   0        0        0    16617 2023-05-01 23:02:18.000000 gyrate-0.0.32/gyrate/gyrate.py
+-rw-rw-rw-   0        0        0     3221 2023-05-01 23:03:01.000000 gyrate-0.0.32/gyrate/notebook.py
+drwxrwxrwx   0        0        0        0 2023-05-01 23:18:17.226768 gyrate-0.0.32/gyrate.egg-info/
+-rw-rw-rw-   0        0        0     1359 2023-05-01 23:18:16.000000 gyrate-0.0.32/gyrate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      355 2023-05-01 23:18:16.000000 gyrate-0.0.32/gyrate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 23:18:16.000000 gyrate-0.0.32/gyrate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      299 2023-05-01 23:18:16.000000 gyrate-0.0.32/gyrate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-01 23:18:16.000000 gyrate-0.0.32/gyrate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-01 23:18:17.235716 gyrate-0.0.32/setup.cfg
+-rw-rw-rw-   0        0        0     1239 2023-05-01 23:16:49.000000 gyrate-0.0.32/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 23:18:17.232725 gyrate-0.0.32/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-01 18:04:18.000000 gyrate-0.0.32/tests/__init__.py
+-rw-rw-rw-   0        0        0     1317 2023-05-01 23:16:34.000000 gyrate-0.0.32/tests/_utils.py
+-rw-rw-rw-   0        0        0    21359 2023-05-01 23:16:35.000000 gyrate-0.0.32/tests/test_halo.py
+-rw-rw-rw-   0        0        0    14196 2023-05-01 23:16:35.000000 gyrate-0.0.32/tests/test_halo_notebook.py
```

### Comparing `gyrate-0.0.31/LICENSE` & `gyrate-0.0.32/LICENSE`

 * *Files identical despite different names*

### Comparing `gyrate-0.0.31/PKG-INFO` & `gyrate-0.0.32/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gyrate
-Version: 0.0.31
+Version: 0.0.32
 Summary: create beautiful and elegant terminal spinners
 License: MIT
 Keywords: console,spinner,loading,cli,spinners,terminal
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `gyrate-0.0.31/README.md` & `gyrate-0.0.32/README.md`

 * *Files identical despite different names*

### Comparing `gyrate-0.0.31/gyrate/_utils.py` & `gyrate-0.0.32/gyrate/_utils.py`

 * *Files identical despite different names*

### Comparing `gyrate-0.0.31/gyrate/cursor.py` & `gyrate-0.0.32/gyrate/cursor.py`

 * *Files identical despite different names*

### Comparing `gyrate-0.0.31/gyrate/gyrate.py` & `gyrate-0.0.32/gyrate/gyrate.py`

 * *Files identical despite different names*

### Comparing `gyrate-0.0.31/gyrate/notebook.py` & `gyrate-0.0.32/gyrate/notebook.py`

 * *Files identical despite different names*

### Comparing `gyrate-0.0.31/gyrate.egg-info/PKG-INFO` & `gyrate-0.0.32/gyrate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gyrate
-Version: 0.0.31
+Version: 0.0.32
 Summary: create beautiful and elegant terminal spinners
 License: MIT
 Keywords: console,spinner,loading,cli,spinners,terminal
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `gyrate-0.0.31/setup.py` & `gyrate-0.0.32/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 
 
 with io.open("README.md", encoding="utf-8") as infile:
     long_description = infile.read()
 
 setup(
     name="gyrate",
-    packages=find_packages(exclude=("tests", "examples")),
-    version="0.0.31",
+    packages=find_packages(exclude=("ext", "examples")),
+    version="0.0.32",
     license="MIT",
     classifiers=[
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3 :: Only",
```

### Comparing `gyrate-0.0.31/tests/test_halo.py` & `gyrate-0.0.32/tests/test_halo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-"""This module tests Halo spinners.
+"""This module ext Halo spinners.
 """
 import io
 import os
 import re
 import sys
 import requests
 import time
@@ -32,15 +32,15 @@
     default_spinner = Spinners['dots'].value
 else:
     frames = [get_coded_text(frame) for frame in Spinners['line'].value['frames']]
     default_spinner = Spinners['line'].value
 
 
 class SpecificException(Exception):
-    """A unique exc class we know only our tests would raise"""
+    """A unique exc class we know only our ext would raise"""
 
 
 class TestHalo(unittest.TestCase):
     """Test Halo enum for attribute values.
     """
     TEST_FOLDER = os.path.dirname(os.path.abspath(__file__))
```

### Comparing `gyrate-0.0.31/tests/test_halo_notebook.py` & `gyrate-0.0.32/tests/test_halo_notebook.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-"""This module tests HaloNotebook spinners.
+"""This module ext HaloNotebook spinners.
 """
 import os
 import re
 import sys
 import time
 import unittest
```

