# Comparing `tmp/alacorder-80.1.2.tar.gz` & `tmp/alacorder-80.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.1.2.tar", max compression
+gzip compressed data, was "alacorder-80.1.3.tar", max compression
```

## Comparing `alacorder-80.1.2.tar` & `alacorder-80.1.3.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.1.2/LICENSE
--rw-r--r--   0        0        0     6889 2023-04-30 22:20:34.472204 alacorder-80.1.2/README.md
--rw-r--r--   0        0        0      697 2023-05-02 14:23:36.762018 alacorder-80.1.2/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-05-02 14:23:56.879572 alacorder-80.1.2/src/alacorder/.DS_Store
--rw-r--r--   0        0        0     1784 2023-04-21 19:12:38.269775 alacorder-80.1.2/src/alacorder/__init__.py
--rw-r--r--   0        0        0   213086 2023-05-02 14:23:45.359435 alacorder-80.1.2/src/alacorder/__main__.py
--rw-r--r--   0        0        0   213086 2023-05-02 14:23:13.445437 alacorder-80.1.2/src/alacorder/alac.py
--rw-r--r--   0        0        0     7818 1970-01-01 00:00:00.000000 alacorder-80.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.1.3/LICENSE
+-rw-r--r--   0        0        0     6889 2023-04-30 22:20:34.472204 alacorder-80.1.3/README.md
+-rw-r--r--   0        0        0      697 2023-05-02 17:22:11.238178 alacorder-80.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.1.3/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   213086 2023-05-02 17:21:47.228463 alacorder-80.1.3/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   213086 2023-05-02 17:21:55.202860 alacorder-80.1.3/src/alacorder/alac.py
+-rw-r--r--   0        0        0     7818 1970-01-01 00:00:00.000000 alacorder-80.1.3/PKG-INFO
```

### Comparing `alacorder-80.1.2/LICENSE` & `alacorder-80.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.1.2/README.md` & `alacorder-80.1.3/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-80.1.2/pyproject.toml` & `alacorder-80.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.1.2"
+version = "80.1.3"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.1.2/src/alacorder/__main__.py` & `alacorder-80.1.3/src/alacorder/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.1.2"
+version = "80.1.3"
 
 autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
```

### Comparing `alacorder-80.1.2/src/alacorder/alac.py` & `alacorder-80.1.3/src/alacorder/alac.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.1.2"
+version = "80.1.3"
 
 autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
```

### Comparing `alacorder-80.1.2/PKG-INFO` & `alacorder-80.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.1.2
+Version: 80.1.3
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

