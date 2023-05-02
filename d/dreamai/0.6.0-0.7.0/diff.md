# Comparing `tmp/dreamai-0.6.0.tar.gz` & `tmp/dreamai-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dreamai-0.6.0.tar", last modified: Tue May  2 01:43:38 2023, max compression
+gzip compressed data, was "dreamai-0.7.0.tar", last modified: Tue May  2 13:54:14 2023, max compression
```

## Comparing `dreamai-0.6.0.tar` & `dreamai-0.7.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-02 01:43:38.862010 dreamai-0.6.0/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)    11337 2022-09-05 16:31:43.000000 dreamai-0.6.0/LICENSE
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      111 2022-09-05 16:31:43.000000 dreamai-0.6.0/MANIFEST.in
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      869 2023-05-02 01:43:38.862010 dreamai-0.6.0/PKG-INFO
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      130 2023-05-02 01:42:31.000000 dreamai-0.6.0/README.md
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-02 01:43:38.858010 dreamai-0.6.0/dreamai/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       22 2023-05-02 01:43:22.000000 dreamai-0.6.0/dreamai/__init__.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     7897 2023-05-02 01:43:22.000000 dreamai-0.6.0/dreamai/_modidx.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     8737 2023-05-02 01:43:22.000000 dreamai-0.6.0/dreamai/core.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      811 2023-05-02 01:33:15.000000 dreamai-0.6.0/dreamai/imports.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     8258 2023-05-02 01:43:22.000000 dreamai-0.6.0/dreamai/vision.py
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-02 01:43:38.862010 dreamai-0.6.0/dreamai.egg-info/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      869 2023-05-02 01:43:38.000000 dreamai-0.6.0/dreamai.egg-info/PKG-INFO
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      361 2023-05-02 01:43:38.000000 dreamai-0.6.0/dreamai.egg-info/SOURCES.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-05-02 01:43:38.000000 dreamai-0.6.0/dreamai.egg-info/dependency_links.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       36 2023-05-02 01:43:38.000000 dreamai-0.6.0/dreamai.egg-info/entry_points.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-01-18 11:49:09.000000 dreamai-0.6.0/dreamai.egg-info/not-zip-safe
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      483 2023-05-02 01:43:38.000000 dreamai-0.6.0/dreamai.egg-info/requires.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)        8 2023-05-02 01:43:38.000000 dreamai-0.6.0/dreamai.egg-info/top_level.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     1143 2023-05-02 01:43:12.000000 dreamai-0.6.0/settings.ini
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       38 2023-05-02 01:43:38.862010 dreamai-0.6.0/setup.cfg
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     2641 2023-01-25 20:45:57.000000 dreamai-0.6.0/setup.py
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-02 13:54:14.443136 dreamai-0.7.0/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)    11337 2022-09-05 16:31:43.000000 dreamai-0.7.0/LICENSE
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      111 2022-09-05 16:31:43.000000 dreamai-0.7.0/MANIFEST.in
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      869 2023-05-02 13:54:14.443136 dreamai-0.7.0/PKG-INFO
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      130 2023-05-02 01:42:31.000000 dreamai-0.7.0/README.md
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-02 13:54:14.443136 dreamai-0.7.0/dreamai/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       22 2023-05-02 13:54:09.000000 dreamai-0.7.0/dreamai/__init__.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     7897 2023-05-02 13:54:09.000000 dreamai-0.7.0/dreamai/_modidx.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     8737 2023-05-02 13:54:09.000000 dreamai-0.7.0/dreamai/core.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      821 2023-05-02 13:53:30.000000 dreamai-0.7.0/dreamai/imports.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     8258 2023-05-02 13:54:09.000000 dreamai-0.7.0/dreamai/vision.py
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-02 13:54:14.443136 dreamai-0.7.0/dreamai.egg-info/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      869 2023-05-02 13:54:14.000000 dreamai-0.7.0/dreamai.egg-info/PKG-INFO
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      361 2023-05-02 13:54:14.000000 dreamai-0.7.0/dreamai.egg-info/SOURCES.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-05-02 13:54:14.000000 dreamai-0.7.0/dreamai.egg-info/dependency_links.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       36 2023-05-02 13:54:14.000000 dreamai-0.7.0/dreamai.egg-info/entry_points.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-01-18 11:49:09.000000 dreamai-0.7.0/dreamai.egg-info/not-zip-safe
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      483 2023-05-02 13:54:14.000000 dreamai-0.7.0/dreamai.egg-info/requires.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)        8 2023-05-02 13:54:14.000000 dreamai-0.7.0/dreamai.egg-info/top_level.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     1143 2023-05-02 13:54:03.000000 dreamai-0.7.0/settings.ini
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       38 2023-05-02 13:54:14.443136 dreamai-0.7.0/setup.cfg
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     2641 2023-01-25 20:45:57.000000 dreamai-0.7.0/setup.py
```

### Comparing `dreamai-0.6.0/LICENSE` & `dreamai-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dreamai-0.6.0/PKG-INFO` & `dreamai-0.7.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreamai
-Version: 0.6.0
+Version: 0.7.0
 Summary: A bunch of cool and convenient utility functions.
 Home-page: https://github.com/HamzaFarhan/dreamai
 Author: HamzaFarhan
 Author-email: thehamza96@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dreamai-0.6.0/dreamai/_modidx.py` & `dreamai-0.7.0/dreamai/_modidx.py`

 * *Files identical despite different names*

### Comparing `dreamai-0.6.0/dreamai/core.py` & `dreamai-0.7.0/dreamai/core.py`

 * *Files identical despite different names*

### Comparing `dreamai-0.6.0/dreamai/imports.py` & `dreamai-0.7.0/dreamai/imports.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # import torch
 # from torch import nn
 
+import re
 import os
 import cv2
 import json
 import copy
 import pickle
 import random
 import imutils
```

### Comparing `dreamai-0.6.0/dreamai/vision.py` & `dreamai-0.7.0/dreamai/vision.py`

 * *Files identical despite different names*

### Comparing `dreamai-0.6.0/dreamai.egg-info/PKG-INFO` & `dreamai-0.7.0/dreamai.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreamai
-Version: 0.6.0
+Version: 0.7.0
 Summary: A bunch of cool and convenient utility functions.
 Home-page: https://github.com/HamzaFarhan/dreamai
 Author: HamzaFarhan
 Author-email: thehamza96@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dreamai-0.6.0/settings.ini` & `dreamai-0.7.0/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = dreamai
 lib_name = %(repo)s
-version = 0.6.0
+version = 0.7.0
 min_python = 3.8
 license = apache2
 doc_path = _docs
 lib_path = dreamai
 nbs_path = nbs
 recursive = True
 tst_flags = notest
```

### Comparing `dreamai-0.6.0/setup.py` & `dreamai-0.7.0/setup.py`

 * *Files identical despite different names*

