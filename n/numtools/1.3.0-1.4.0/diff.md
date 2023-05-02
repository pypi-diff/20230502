# Comparing `tmp/numtools-1.3.0.tar.gz` & `tmp/numtools-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numtools-1.3.0.tar", last modified: Mon Mar 13 09:32:21 2023, max compression
+gzip compressed data, was "numtools-1.4.0.tar", last modified: Tue May  2 04:15:19 2023, max compression
```

## Comparing `numtools-1.3.0.tar` & `numtools-1.4.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-03-13 09:32:21.233077 numtools-1.3.0/
--rw-r--r--   0 nic       (1001) nic       (1001)      172 2019-11-19 09:06:07.000000 numtools-1.3.0/AUTHORS.rst
--rw-r--r--   0 nic       (1001) nic       (1001)      221 2019-11-19 09:06:07.000000 numtools-1.3.0/CONTRIBUTING.rst
--rw-r--r--   0 nic       (1001) nic       (1001)      285 2019-12-16 06:53:49.000000 numtools-1.3.0/HISTORY.rst
--rw-r--r--   0 nic       (1001) nic       (1001)     1074 2019-12-13 10:28:35.000000 numtools-1.3.0/LICENSE
--rw-r--r--   0 nic       (1001) nic       (1001)      262 2019-11-19 09:06:07.000000 numtools-1.3.0/MANIFEST.in
--rw-rw-r--   0 nic       (1001) nic       (1001)     1521 2023-03-13 09:32:21.233077 numtools-1.3.0/PKG-INFO
--rw-r--r--   0 nic       (1001) nic       (1001)      681 2019-12-16 06:52:44.000000 numtools-1.3.0/README.rst
-drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-03-13 09:32:21.229077 numtools-1.3.0/docs/
--rw-r--r--   0 nic       (1001) nic       (1001)      609 2019-11-19 09:06:07.000000 numtools-1.3.0/docs/Makefile
-drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-03-13 09:32:21.225077 numtools-1.3.0/docs/_build/
-drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-03-13 09:32:21.225077 numtools-1.3.0/docs/_build/html/
-drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-03-13 09:32:21.229077 numtools-1.3.0/docs/_build/html/_static/
--rw-r--r--   0 nic       (1001) nic       (1001)      286 2019-12-16 16:19:06.000000 numtools-1.3.0/docs/_build/html/_static/file.png
--rw-r--r--   0 nic       (1001) nic       (1001)       90 2019-12-16 16:19:06.000000 numtools-1.3.0/docs/_build/html/_static/minus.png
--rw-r--r--   0 nic       (1001) nic       (1001)       90 2019-12-16 16:19:06.000000 numtools-1.3.0/docs/_build/html/_static/plus.png
--rw-r--r--   0 nic       (1001) nic       (1001)       28 2019-11-19 09:06:07.000000 numtools-1.3.0/docs/authors.rst
--rwxr-xr-x   0 nic       (1001) nic       (1001)     4900 2022-10-12 15:49:49.000000 numtools-1.3.0/docs/conf.py
--rw-r--r--   0 nic       (1001) nic       (1001)       33 2019-11-19 09:06:07.000000 numtools-1.3.0/docs/contributing.rst
--rw-r--r--   0 nic       (1001) nic       (1001)       28 2019-11-19 09:06:07.000000 numtools-1.3.0/docs/history.rst
--rw-r--r--   0 nic       (1001) nic       (1001)      305 2019-11-19 09:06:07.000000 numtools-1.3.0/docs/index.rst
--rw-r--r--   0 nic       (1001) nic       (1001)      102 2019-11-19 09:06:07.000000 numtools-1.3.0/docs/installation.rst
--rw-r--r--   0 nic       (1001) nic       (1001)      770 2019-11-19 09:06:07.000000 numtools-1.3.0/docs/make.bat
--rw-r--r--   0 nic       (1001) nic       (1001)       61 2020-01-15 10:31:32.000000 numtools-1.3.0/docs/modules.rst
--rw-r--r--   0 nic       (1001) nic       (1001)      136 2020-01-15 10:31:32.000000 numtools-1.3.0/docs/numtools.csyslib.rst
--rw-r--r--   0 nic       (1001) nic       (1001)      133 2020-01-15 10:31:32.000000 numtools-1.3.0/docs/numtools.intzip.rst
--rw-r--r--   0 nic       (1001) nic       (1001)      270 2020-01-15 10:31:32.000000 numtools-1.3.0/docs/numtools.rst
--rw-r--r--   0 nic       (1001) nic       (1001)      145 2020-01-15 10:31:32.000000 numtools-1.3.0/docs/numtools.serializer.rst
--rw-r--r--   0 nic       (1001) nic       (1001)      145 2020-01-15 10:31:32.000000 numtools-1.3.0/docs/numtools.vgextended.rst
--rw-r--r--   0 nic       (1001) nic       (1001)       27 2019-11-19 09:06:07.000000 numtools-1.3.0/docs/readme.rst
--rw-r--r--   0 nic       (1001) nic       (1001)       71 2019-11-19 09:06:07.000000 numtools-1.3.0/docs/usage.rst
-drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-03-13 09:32:21.229077 numtools-1.3.0/numtools/
--rw-rw-r--   0 nic       (1001) nic       (1001)      167 2023-03-13 09:31:51.000000 numtools-1.3.0/numtools/__init__.py
--rw-r--r--   0 nic       (1001) nic       (1001)    18150 2023-03-13 09:10:36.000000 numtools-1.3.0/numtools/csyslib.py
--rw-r--r--   0 nic       (1001) nic       (1001)     5932 2022-10-12 15:49:45.000000 numtools-1.3.0/numtools/intzip.py
--rw-rw-r--   0 nic       (1001) nic       (1001)     4348 2022-11-26 09:10:46.000000 numtools-1.3.0/numtools/pandas_tk.py
--rw-rw-r--   0 nic       (1001) nic       (1001)     9152 2022-10-12 15:49:49.000000 numtools-1.3.0/numtools/serializer.py
--rw-r--r--   0 nic       (1001) nic       (1001)     5315 2023-03-13 09:11:17.000000 numtools-1.3.0/numtools/vgextended.py
-drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-03-13 09:32:21.233077 numtools-1.3.0/numtools.egg-info/
--rw-rw-r--   0 nic       (1001) nic       (1001)     1521 2023-03-13 09:32:21.000000 numtools-1.3.0/numtools.egg-info/PKG-INFO
--rw-rw-r--   0 nic       (1001) nic       (1001)      950 2023-03-13 09:32:21.000000 numtools-1.3.0/numtools.egg-info/SOURCES.txt
--rw-rw-r--   0 nic       (1001) nic       (1001)        1 2023-03-13 09:32:21.000000 numtools-1.3.0/numtools.egg-info/dependency_links.txt
--rw-rw-r--   0 nic       (1001) nic       (1001)        1 2023-03-13 09:32:21.000000 numtools-1.3.0/numtools.egg-info/not-zip-safe
--rw-rw-r--   0 nic       (1001) nic       (1001)        9 2023-03-13 09:32:21.000000 numtools-1.3.0/numtools.egg-info/top_level.txt
--rw-r--r--   0 nic       (1001) nic       (1001)      483 2023-03-13 09:32:21.233077 numtools-1.3.0/setup.cfg
--rw-rw-r--   0 nic       (1001) nic       (1001)     1229 2023-03-13 09:31:51.000000 numtools-1.3.0/setup.py
-drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-03-13 09:32:21.233077 numtools-1.3.0/tests/
--rw-r--r--   0 nic       (1001) nic       (1001)       63 2019-11-19 09:06:07.000000 numtools-1.3.0/tests/__init__.py
--rw-r--r--   0 nic       (1001) nic       (1001)     2559 2022-10-12 15:49:45.000000 numtools-1.3.0/tests/test_csyslib.py
--rw-rw-r--   0 nic       (1001) nic       (1001)      967 2022-10-12 09:19:37.000000 numtools-1.3.0/tests/test_intzip.py
--rw-rw-r--   0 nic       (1001) nic       (1001)     1469 2023-03-13 09:09:12.000000 numtools-1.3.0/tests/test_matrix.py
--rw-rw-r--   0 nic       (1001) nic       (1001)     2567 2023-01-19 14:44:08.000000 numtools-1.3.0/tests/test_pandas_tk.py
--rw-rw-r--   0 nic       (1001) nic       (1001)     3529 2022-10-12 15:49:49.000000 numtools-1.3.0/tests/test_serializer.py
--rw-rw-r--   0 nic       (1001) nic       (1001)     3599 2022-10-12 15:49:45.000000 numtools-1.3.0/tests/test_serializer.py.orig
+drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-05-02 04:15:19.777738 numtools-1.4.0/
+-rw-r--r--   0 nic       (1001) nic       (1001)      172 2019-11-19 09:06:07.000000 numtools-1.4.0/AUTHORS.rst
+-rw-r--r--   0 nic       (1001) nic       (1001)      221 2019-11-19 09:06:07.000000 numtools-1.4.0/CONTRIBUTING.rst
+-rw-r--r--   0 nic       (1001) nic       (1001)      285 2019-12-16 06:53:49.000000 numtools-1.4.0/HISTORY.rst
+-rw-r--r--   0 nic       (1001) nic       (1001)     1074 2019-12-13 10:28:35.000000 numtools-1.4.0/LICENSE
+-rw-r--r--   0 nic       (1001) nic       (1001)      262 2019-11-19 09:06:07.000000 numtools-1.4.0/MANIFEST.in
+-rw-rw-r--   0 nic       (1001) nic       (1001)     1521 2023-05-02 04:15:19.777738 numtools-1.4.0/PKG-INFO
+-rw-r--r--   0 nic       (1001) nic       (1001)      681 2019-12-16 06:52:44.000000 numtools-1.4.0/README.rst
+drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-05-02 04:15:19.773738 numtools-1.4.0/docs/
+-rw-r--r--   0 nic       (1001) nic       (1001)      609 2019-11-19 09:06:07.000000 numtools-1.4.0/docs/Makefile
+drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-05-02 04:15:19.765738 numtools-1.4.0/docs/_build/
+drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-05-02 04:15:19.769738 numtools-1.4.0/docs/_build/html/
+drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-05-02 04:15:19.773738 numtools-1.4.0/docs/_build/html/_static/
+-rw-r--r--   0 nic       (1001) nic       (1001)      286 2019-12-16 16:19:06.000000 numtools-1.4.0/docs/_build/html/_static/file.png
+-rw-r--r--   0 nic       (1001) nic       (1001)       90 2019-12-16 16:19:06.000000 numtools-1.4.0/docs/_build/html/_static/minus.png
+-rw-r--r--   0 nic       (1001) nic       (1001)       90 2019-12-16 16:19:06.000000 numtools-1.4.0/docs/_build/html/_static/plus.png
+-rw-r--r--   0 nic       (1001) nic       (1001)       28 2019-11-19 09:06:07.000000 numtools-1.4.0/docs/authors.rst
+-rwxr-xr-x   0 nic       (1001) nic       (1001)     4900 2022-10-12 15:49:49.000000 numtools-1.4.0/docs/conf.py
+-rw-r--r--   0 nic       (1001) nic       (1001)       33 2019-11-19 09:06:07.000000 numtools-1.4.0/docs/contributing.rst
+-rw-r--r--   0 nic       (1001) nic       (1001)       28 2019-11-19 09:06:07.000000 numtools-1.4.0/docs/history.rst
+-rw-r--r--   0 nic       (1001) nic       (1001)      305 2019-11-19 09:06:07.000000 numtools-1.4.0/docs/index.rst
+-rw-r--r--   0 nic       (1001) nic       (1001)      102 2019-11-19 09:06:07.000000 numtools-1.4.0/docs/installation.rst
+-rw-r--r--   0 nic       (1001) nic       (1001)      770 2019-11-19 09:06:07.000000 numtools-1.4.0/docs/make.bat
+-rw-r--r--   0 nic       (1001) nic       (1001)       61 2020-01-15 10:31:32.000000 numtools-1.4.0/docs/modules.rst
+-rw-r--r--   0 nic       (1001) nic       (1001)      136 2020-01-15 10:31:32.000000 numtools-1.4.0/docs/numtools.csyslib.rst
+-rw-r--r--   0 nic       (1001) nic       (1001)      133 2020-01-15 10:31:32.000000 numtools-1.4.0/docs/numtools.intzip.rst
+-rw-r--r--   0 nic       (1001) nic       (1001)      270 2020-01-15 10:31:32.000000 numtools-1.4.0/docs/numtools.rst
+-rw-r--r--   0 nic       (1001) nic       (1001)      145 2020-01-15 10:31:32.000000 numtools-1.4.0/docs/numtools.serializer.rst
+-rw-r--r--   0 nic       (1001) nic       (1001)      145 2020-01-15 10:31:32.000000 numtools-1.4.0/docs/numtools.vgextended.rst
+-rw-r--r--   0 nic       (1001) nic       (1001)       27 2019-11-19 09:06:07.000000 numtools-1.4.0/docs/readme.rst
+-rw-r--r--   0 nic       (1001) nic       (1001)       71 2019-11-19 09:06:07.000000 numtools-1.4.0/docs/usage.rst
+drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-05-02 04:15:19.773738 numtools-1.4.0/numtools/
+-rw-rw-r--   0 nic       (1001) nic       (1001)      167 2023-05-02 04:15:03.000000 numtools-1.4.0/numtools/__init__.py
+-rw-r--r--   0 nic       (1001) nic       (1001)    18150 2023-03-13 09:10:36.000000 numtools-1.4.0/numtools/csyslib.py
+-rw-r--r--   0 nic       (1001) nic       (1001)     5932 2022-10-12 15:49:45.000000 numtools-1.4.0/numtools/intzip.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)     4406 2023-05-02 04:11:56.000000 numtools-1.4.0/numtools/pandas_tk.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)     9152 2022-10-12 15:49:49.000000 numtools-1.4.0/numtools/serializer.py
+-rw-r--r--   0 nic       (1001) nic       (1001)     5315 2023-03-13 09:11:17.000000 numtools-1.4.0/numtools/vgextended.py
+drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-05-02 04:15:19.773738 numtools-1.4.0/numtools.egg-info/
+-rw-rw-r--   0 nic       (1001) nic       (1001)     1521 2023-05-02 04:15:19.000000 numtools-1.4.0/numtools.egg-info/PKG-INFO
+-rw-rw-r--   0 nic       (1001) nic       (1001)      950 2023-05-02 04:15:19.000000 numtools-1.4.0/numtools.egg-info/SOURCES.txt
+-rw-rw-r--   0 nic       (1001) nic       (1001)        1 2023-05-02 04:15:19.000000 numtools-1.4.0/numtools.egg-info/dependency_links.txt
+-rw-rw-r--   0 nic       (1001) nic       (1001)        1 2023-05-02 04:15:19.000000 numtools-1.4.0/numtools.egg-info/not-zip-safe
+-rw-rw-r--   0 nic       (1001) nic       (1001)        9 2023-05-02 04:15:19.000000 numtools-1.4.0/numtools.egg-info/top_level.txt
+-rw-r--r--   0 nic       (1001) nic       (1001)      483 2023-05-02 04:15:19.777738 numtools-1.4.0/setup.cfg
+-rw-rw-r--   0 nic       (1001) nic       (1001)     1229 2023-05-02 04:15:03.000000 numtools-1.4.0/setup.py
+drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-05-02 04:15:19.777738 numtools-1.4.0/tests/
+-rw-r--r--   0 nic       (1001) nic       (1001)       63 2019-11-19 09:06:07.000000 numtools-1.4.0/tests/__init__.py
+-rw-r--r--   0 nic       (1001) nic       (1001)     2559 2022-10-12 15:49:45.000000 numtools-1.4.0/tests/test_csyslib.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)      967 2022-10-12 09:19:37.000000 numtools-1.4.0/tests/test_intzip.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)     1469 2023-03-13 09:09:12.000000 numtools-1.4.0/tests/test_matrix.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)     2567 2023-01-19 14:44:08.000000 numtools-1.4.0/tests/test_pandas_tk.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)     3529 2022-10-12 15:49:49.000000 numtools-1.4.0/tests/test_serializer.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)     3599 2022-10-12 15:49:45.000000 numtools-1.4.0/tests/test_serializer.py.orig
```

### Comparing `numtools-1.3.0/LICENSE` & `numtools-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `numtools-1.3.0/PKG-INFO` & `numtools-1.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numtools
-Version: 1.3.0
+Version: 1.4.0
 Summary: numeric-gmbH toolbox
 Home-page: https://framagit.org/numenic/numtools
 Author: numenic
 Author-email: info@numeric-gmbh.ch
 Keywords: numtools
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `numtools-1.3.0/README.rst` & `numtools-1.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `numtools-1.3.0/docs/Makefile` & `numtools-1.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `numtools-1.3.0/docs/conf.py` & `numtools-1.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `numtools-1.3.0/docs/make.bat` & `numtools-1.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `numtools-1.3.0/numtools/csyslib.py` & `numtools-1.4.0/numtools/csyslib.py`

 * *Files identical despite different names*

### Comparing `numtools-1.3.0/numtools/intzip.py` & `numtools-1.4.0/numtools/intzip.py`

 * *Files identical despite different names*

### Comparing `numtools-1.3.0/numtools/pandas_tk.py` & `numtools-1.4.0/numtools/pandas_tk.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import numpy as np
 import pandas as pd
 
 from numtools.intzip import hunzip, hzip
 
 
-def signed_absmax(df, axis=0, origin=False):
+def signed_absmax(df, axis=0, origin=False, mode="max"):
     """retrieve the critical values from a dataframe by series or column,
     keeping correct signed values
 
     return a series, if origin is False
     return a dataframe if origin is True
 
     >>> df = pd.DataFrame(
@@ -46,15 +46,16 @@
     100  -6.0      C
     110   4.0      D
     111  -9.0      C
     """
     if axis == 0:
         df = df.T
         axis = 1
-    ixs = np.nanargmax(df**2, axis=axis)  # row index if axis=0
+    f = {"max": np.nanargmax, "min": np.nanargmin}[mode]
+    ixs = f(df**2, axis=axis)  # row index if axis=0
     crit = df.values[range(df.shape[0]), ixs]
     index = df.index if axis == 1 else df.columns
     values = pd.Series(crit, index=index, name="crit")
     if origin:
         origin = pd.Series(dict(zip(df.index, df.columns[ixs])), name="orig")
         df = pd.concat((values, origin), axis=1)
         return df
```

### Comparing `numtools-1.3.0/numtools/serializer.py` & `numtools-1.4.0/numtools/serializer.py`

 * *Files identical despite different names*

### Comparing `numtools-1.3.0/numtools/vgextended.py` & `numtools-1.4.0/numtools/vgextended.py`

 * *Files identical despite different names*

### Comparing `numtools-1.3.0/numtools.egg-info/PKG-INFO` & `numtools-1.4.0/numtools.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numtools
-Version: 1.3.0
+Version: 1.4.0
 Summary: numeric-gmbH toolbox
 Home-page: https://framagit.org/numenic/numtools
 Author: numenic
 Author-email: info@numeric-gmbh.ch
 Keywords: numtools
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `numtools-1.3.0/numtools.egg-info/SOURCES.txt` & `numtools-1.4.0/numtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `numtools-1.3.0/setup.py` & `numtools-1.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,11 +39,11 @@
     include_package_data=True,
     keywords="numtools",
     name="numtools",
     packages=find_packages(include=["numtools", "numtools.*"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
-    version="1.3.0",
+    version="1.4.0",
     zip_safe=False,
     url="https://framagit.org/numenic/numtools",
 )
```

### Comparing `numtools-1.3.0/tests/test_csyslib.py` & `numtools-1.4.0/tests/test_csyslib.py`

 * *Files identical despite different names*

### Comparing `numtools-1.3.0/tests/test_intzip.py` & `numtools-1.4.0/tests/test_intzip.py`

 * *Files identical despite different names*

### Comparing `numtools-1.3.0/tests/test_matrix.py` & `numtools-1.4.0/tests/test_matrix.py`

 * *Files identical despite different names*

### Comparing `numtools-1.3.0/tests/test_pandas_tk.py` & `numtools-1.4.0/tests/test_pandas_tk.py`

 * *Files identical despite different names*

### Comparing `numtools-1.3.0/tests/test_serializer.py` & `numtools-1.4.0/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `numtools-1.3.0/tests/test_serializer.py.orig` & `numtools-1.4.0/tests/test_serializer.py.orig`

 * *Files identical despite different names*

