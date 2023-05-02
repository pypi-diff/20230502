# Comparing `tmp/xev-data-0.0.4.tar.gz` & `tmp/xev-data-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xev-data-0.0.4.tar", last modified: Wed Feb 22 20:30:09 2023, max compression
+gzip compressed data, was "xev-data-0.0.5.tar", last modified: Tue May  2 15:43:42 2023, max compression
```

## Comparing `xev-data-0.0.4.tar` & `xev-data-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2023-02-22 20:30:09.240692 xev-data-0.0.4/
--rw-r--r--   0 vdelfave (669582709) staff       (20)      660 2023-02-22 20:30:09.240579 xev-data-0.0.4/PKG-INFO
--rw-r--r--   0 vdelfave (669582709) staff       (20)      421 2023-02-10 20:46:49.000000 xev-data-0.0.4/README.md
--rw-r--r--   0 vdelfave (669582709) staff       (20)       74 2023-02-01 18:07:17.000000 xev-data-0.0.4/pyproject.toml
--rw-r--r--   0 vdelfave (669582709) staff       (20)       38 2023-02-22 20:30:09.240724 xev-data-0.0.4/setup.cfg
--rw-r--r--   0 vdelfave (669582709) staff       (20)     3933 2023-02-22 20:29:53.000000 xev-data-0.0.4/setup.py
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2023-02-22 20:30:09.238853 xev-data-0.0.4/src/
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2023-02-22 20:30:09.239503 xev-data-0.0.4/src/xdata/
--rw-r--r--   0 vdelfave (669582709) staff       (20)       36 2022-10-25 16:06:50.000000 xev-data-0.0.4/src/xdata/__init__.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)    35579 2023-02-22 20:28:24.000000 xev-data-0.0.4/src/xdata/database.py
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2023-02-22 20:30:09.240090 xev-data-0.0.4/src/xev_data.egg-info/
--rw-r--r--   0 vdelfave (669582709) staff       (20)      660 2023-02-22 20:30:09.000000 xev-data-0.0.4/src/xev_data.egg-info/PKG-INFO
--rw-r--r--   0 vdelfave (669582709) staff       (20)      320 2023-02-22 20:30:09.000000 xev-data-0.0.4/src/xev_data.egg-info/SOURCES.txt
--rw-r--r--   0 vdelfave (669582709) staff       (20)        1 2023-02-22 20:30:09.000000 xev-data-0.0.4/src/xev_data.egg-info/dependency_links.txt
--rw-r--r--   0 vdelfave (669582709) staff       (20)       25 2023-02-22 20:30:09.000000 xev-data-0.0.4/src/xev_data.egg-info/requires.txt
--rw-r--r--   0 vdelfave (669582709) staff       (20)        6 2023-02-22 20:30:09.000000 xev-data-0.0.4/src/xev_data.egg-info/top_level.txt
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2023-02-22 20:30:09.240435 xev-data-0.0.4/tests/
--rw-r--r--   0 vdelfave (669582709) staff       (20)     9813 2023-02-22 20:28:50.000000 xev-data-0.0.4/tests/test_database.py
--rwxr-xr-x   0 vdelfave (669582709) staff       (20)      331 2023-02-01 18:58:47.000000 xev-data-0.0.4/tests/test_hello.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)      224 2023-02-06 21:29:27.000000 xev-data-0.0.4/tests/test_import.py
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2023-05-02 15:43:42.930965 xev-data-0.0.5/
+-rw-r--r--   0 vdelfave (669582709) staff       (20)       30 2023-05-02 15:39:00.000000 xev-data-0.0.5/MANIFEST.in
+-rw-r--r--   0 vdelfave (669582709) staff       (20)      660 2023-05-02 15:43:42.930858 xev-data-0.0.5/PKG-INFO
+-rw-r--r--   0 vdelfave (669582709) staff       (20)      421 2023-02-10 20:46:49.000000 xev-data-0.0.5/README.md
+-rw-r--r--   0 vdelfave (669582709) staff       (20)       74 2023-02-01 18:07:17.000000 xev-data-0.0.5/pyproject.toml
+-rw-r--r--   0 vdelfave (669582709) staff       (20)       38 2023-05-02 15:43:42.930995 xev-data-0.0.5/setup.cfg
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     3932 2023-05-02 15:40:02.000000 xev-data-0.0.5/setup.py
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2023-05-02 15:43:42.929045 xev-data-0.0.5/src/
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2023-05-02 15:43:42.929793 xev-data-0.0.5/src/xdata/
+-rw-r--r--   0 vdelfave (669582709) staff       (20)       36 2022-10-25 16:06:50.000000 xev-data-0.0.5/src/xdata/__init__.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    35579 2023-02-22 20:28:24.000000 xev-data-0.0.5/src/xdata/database.py
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2023-05-02 15:43:42.930379 xev-data-0.0.5/src/xev_data.egg-info/
+-rw-r--r--   0 vdelfave (669582709) staff       (20)      660 2023-05-02 15:43:42.000000 xev-data-0.0.5/src/xev_data.egg-info/PKG-INFO
+-rw-r--r--   0 vdelfave (669582709) staff       (20)      332 2023-05-02 15:43:42.000000 xev-data-0.0.5/src/xev_data.egg-info/SOURCES.txt
+-rw-r--r--   0 vdelfave (669582709) staff       (20)        1 2023-05-02 15:43:42.000000 xev-data-0.0.5/src/xev_data.egg-info/dependency_links.txt
+-rw-r--r--   0 vdelfave (669582709) staff       (20)       25 2023-05-02 15:43:42.000000 xev-data-0.0.5/src/xev_data.egg-info/requires.txt
+-rw-r--r--   0 vdelfave (669582709) staff       (20)        6 2023-05-02 15:43:42.000000 xev-data-0.0.5/src/xev_data.egg-info/top_level.txt
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2023-05-02 15:43:42.930714 xev-data-0.0.5/tests/
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     9813 2023-02-22 20:28:50.000000 xev-data-0.0.5/tests/test_database.py
+-rwxr-xr-x   0 vdelfave (669582709) staff       (20)      331 2023-02-01 18:58:47.000000 xev-data-0.0.5/tests/test_hello.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)      224 2023-02-06 21:29:27.000000 xev-data-0.0.5/tests/test_import.py
```

### Comparing `xev-data-0.0.4/PKG-INFO` & `xev-data-0.0.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xev-data
-Version: 0.0.4
+Version: 0.0.5
 Home-page: https://gitlab.com/xevra/xev-data
 Author: Vera Delfavero
 Author-email: xevra86@gmail.com
 Maintainer: Vera Delfavero
 Maintainer-email: xevra86@gmail.com
 License: MIT Lisence
 Keywords: hdf5
```

### Comparing `xev-data-0.0.4/setup.py` & `xev-data-0.0.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from datetime import date
 
 #----------------------------------------------------------------
 # General
 #----------------------------------------------------------------
 
 __name__        = "xev-data"
-__version__     = "0.0.4"
-__date__        = date(2023, 2, 10)
+__version__     = "0.0.5"
+__date__        = date(2023, 5, 2)
 __keywords__    = [
      "hdf5",
     ]
 __status__      = "Alpha"
 
 #----------------------------------------------------------------
 # URLs
```

### Comparing `xev-data-0.0.4/src/xdata/database.py` & `xev-data-0.0.5/src/xdata/database.py`

 * *Files identical despite different names*

### Comparing `xev-data-0.0.4/src/xev_data.egg-info/PKG-INFO` & `xev-data-0.0.5/src/xev_data.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xev-data
-Version: 0.0.4
+Version: 0.0.5
 Home-page: https://gitlab.com/xevra/xev-data
 Author: Vera Delfavero
 Author-email: xevra86@gmail.com
 Maintainer: Vera Delfavero
 Maintainer-email: xevra86@gmail.com
 License: MIT Lisence
 Keywords: hdf5
```

### Comparing `xev-data-0.0.4/tests/test_database.py` & `xev-data-0.0.5/tests/test_database.py`

 * *Files identical despite different names*

