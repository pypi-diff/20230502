# Comparing `tmp/asgihandler-0.3.9.tar.gz` & `tmp/asgihandler-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asgihandler-0.3.9.tar", last modified: Sat Aug  6 00:52:42 2022, max compression
+gzip compressed data, was "asgihandler-0.4.0.tar", last modified: Tue May  2 06:13:01 2023, max compression
```

## Comparing `asgihandler-0.3.9.tar` & `asgihandler-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2022-08-06 00:52:42.954872 asgihandler-0.3.9/
--rw-rw-rw-   0        0        0     1067 2022-07-16 23:50:52.000000 asgihandler-0.3.9/LICENSE
--rw-rw-rw-   0        0        0       27 2022-07-16 23:50:52.000000 asgihandler-0.3.9/MANIFEST.in
--rw-rw-rw-   0        0        0     3035 2022-08-06 00:52:42.954872 asgihandler-0.3.9/PKG-INFO
--rw-rw-rw-   0        0        0     2403 2022-07-16 23:50:52.000000 asgihandler-0.3.9/README.md
-drwxrwxrwx   0        0        0        0 2022-08-06 00:52:42.939844 asgihandler-0.3.9/asgihandler/
--rw-rw-rw-   0        0        0       21 2022-07-16 23:50:52.000000 asgihandler-0.3.9/asgihandler/__init__.py
--rw-rw-rw-   0        0        0       68 2022-07-16 23:55:07.000000 asgihandler-0.3.9/asgihandler/__version__.py
--rw-rw-rw-   0        0        0     1287 2022-08-05 19:34:25.000000 asgihandler-0.3.9/asgihandler/core.py
--rw-rw-rw-   0        0        0      425 2022-08-06 00:52:39.000000 asgihandler-0.3.9/asgihandler/userCheck.py
-drwxrwxrwx   0        0        0        0 2022-08-06 00:52:42.953843 asgihandler-0.3.9/asgihandler.egg-info/
--rw-rw-rw-   0        0        0     3035 2022-08-06 00:52:42.000000 asgihandler-0.3.9/asgihandler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      308 2022-08-06 00:52:42.000000 asgihandler-0.3.9/asgihandler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-06 00:52:42.000000 asgihandler-0.3.9/asgihandler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2022-08-06 00:52:42.000000 asgihandler-0.3.9/asgihandler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2022-08-06 00:52:42.000000 asgihandler-0.3.9/asgihandler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-08-06 00:52:42.954872 asgihandler-0.3.9/setup.cfg
--rw-rw-rw-   0        0        0     3878 2022-08-06 00:52:39.000000 asgihandler-0.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 06:13:01.905166 asgihandler-0.4.0/
+-rw-rw-rw-   0        0        0     1067 2022-07-16 23:50:52.000000 asgihandler-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0       27 2022-07-16 23:50:52.000000 asgihandler-0.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3035 2023-05-02 06:13:01.896166 asgihandler-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2403 2022-07-16 23:50:52.000000 asgihandler-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 06:13:01.683133 asgihandler-0.4.0/asgihandler/
+-rw-rw-rw-   0        0        0       21 2022-07-16 23:50:52.000000 asgihandler-0.4.0/asgihandler/__init__.py
+-rw-rw-rw-   0        0        0       68 2022-07-16 23:55:07.000000 asgihandler-0.4.0/asgihandler/__version__.py
+-rw-rw-rw-   0        0        0     1287 2022-08-05 19:34:25.000000 asgihandler-0.4.0/asgihandler/core.py
+-rw-rw-rw-   0        0        0      425 2022-08-06 00:52:39.000000 asgihandler-0.4.0/asgihandler/userCheck.py
+drwxrwxrwx   0        0        0        0 2023-05-02 06:13:01.884166 asgihandler-0.4.0/asgihandler.egg-info/
+-rw-rw-rw-   0        0        0     3035 2023-05-02 06:13:01.000000 asgihandler-0.4.0/asgihandler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      308 2023-05-02 06:13:01.000000 asgihandler-0.4.0/asgihandler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 06:13:01.000000 asgihandler-0.4.0/asgihandler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-02 06:13:01.000000 asgihandler-0.4.0/asgihandler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-02 06:13:01.000000 asgihandler-0.4.0/asgihandler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 06:13:01.906167 asgihandler-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     3878 2023-05-02 06:09:16.000000 asgihandler-0.4.0/setup.py
```

### Comparing `asgihandler-0.3.9/LICENSE` & `asgihandler-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asgihandler-0.3.9/PKG-INFO` & `asgihandler-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: asgihandler
-Version: 0.3.9
+Version: 0.4.0
 Summary: ASGIHandler
 Home-page: https://github.com/GreaterWMS/GreaterWMS
 Author: Singosgu
 Author-email: singosgu@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.9.0
+Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 📦 setup.py (for humans)
 =======================
```

### Comparing `asgihandler-0.3.9/README.md` & `asgihandler-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `asgihandler-0.3.9/asgihandler/core.py` & `asgihandler-0.4.0/asgihandler/core.py`

 * *Files identical despite different names*

### Comparing `asgihandler-0.3.9/asgihandler.egg-info/PKG-INFO` & `asgihandler-0.4.0/asgihandler.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: asgihandler
-Version: 0.3.9
+Version: 0.4.0
 Summary: ASGIHandler
 Home-page: https://github.com/GreaterWMS/GreaterWMS
 Author: Singosgu
 Author-email: singosgu@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.9.0
+Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 📦 setup.py (for humans)
 =======================
```

### Comparing `asgihandler-0.3.9/setup.py` & `asgihandler-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 
 # Package meta-data.
 NAME = 'asgihandler'
 DESCRIPTION = 'ASGIHandler'
 URL = 'https://github.com/GreaterWMS/GreaterWMS'
 EMAIL = 'singosgu@gmail.com'
 AUTHOR = 'Singosgu'
-REQUIRES_PYTHON = '>=3.9.0'
-VERSION = '0.3.9'
+REQUIRES_PYTHON = '>=3.7.0'
+VERSION = '0.4.0'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'requests',
 ]
 
 # What packages are optional?
```

