# Comparing `tmp/hyundai_kia_connect_api-3.2.0.tar.gz` & `tmp/hyundai_kia_connect_api-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyundai_kia_connect_api-3.2.0.tar", last modified: Mon May  1 20:57:43 2023, max compression
+gzip compressed data, was "hyundai_kia_connect_api-3.3.0.tar", last modified: Tue May  2 17:24:19 2023, max compression
```

## Comparing `hyundai_kia_connect_api-3.2.0.tar` & `hyundai_kia_connect_api-3.3.0.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:57:43.402552 hyundai_kia_connect_api-3.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-01 20:57:11.000000 hyundai_kia_connect_api-3.2.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-05-01 20:57:11.000000 hyundai_kia_connect_api-3.2.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-01 20:57:11.000000 hyundai_kia_connect_api-3.2.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-01 20:57:11.000000 hyundai_kia_connect_api-3.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-01 20:57:11.000000 hyundai_kia_connect_api-3.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-05-01 20:57:43.402552 hyundai_kia_connect_api-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-05-01 20:57:11.000000 hyundai_kia_connect_api-3.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:57:43.398551 hyundai_kia_connect_api-3.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-01 20:57:11.000000 hyundai_kia_connect_api-3.2.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-01 20:57:11.000000 hyundai_kia_connect_api-3.2.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-05-01 20:57:11.000000 hyundai_kia_connect_api-3.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-01 20:57:11.000000 hyundai_kia_connect_api-3.2.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-01 20:57:11.000000 hyundai_kia_connect_api-3.2.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-01 20:57:11.000000 hyundai_kia_connect_api-3.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-01 20:57:11.000000 hyundai_kia_connect_api-3.2.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-01 20:57:11.000000 hyundai_kia_connect_api-3.2.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-01 20:57:11.000000 hyundai_kia_connect_api-3.2.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-01 20:57:11.000000 hyundai_kia_connect_api-3.2.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:57:43.402552 hyundai_kia_connect_api-3.2.0/hyundai_kia_connect_api/
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-05-01 20:57:11.000000 hyundai_kia_connect_api-3.2.0/hyundai_kia_connect_api/ApiImpl.py
--rw-r--r--   0 runner    (1001) docker     (123)    23907 2023-05-01 20:57:11.000000 hyundai_kia_connect_api-3.2.0/hyundai_kia_connect_api/HyundaiBlueLinkAPIUSA.py
--rw-r--r--   0 runner    (1001) docker     (123)    27449 2023-05-01 20:57:11.000000 hyundai_kia_connect_api-3.2.0/hyundai_kia_connect_api/KiaUvoAPIUSA.py
--rw-r--r--   0 runner    (1001) docker     (123)    30644 2023-05-01 20:57:11.000000 hyundai_kia_connect_api-3.2.0/hyundai_kia_connect_api/KiaUvoApiCA.py
--rw-r--r--   0 runner    (1001) docker     (123)    53887 2023-05-01 20:57:11.000000 hyundai_kia_connect_api-3.2.0/hyundai_kia_connect_api/KiaUvoApiEU.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-01 20:57:11.000000 hyundai_kia_connect_api-3.2.0/hyundai_kia_connect_api/Token.py
--rw-r--r--   0 runner    (1001) docker     (123)    12772 2023-05-01 20:57:11.000000 hyundai_kia_connect_api-3.2.0/hyundai_kia_connect_api/Vehicle.py
--rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-05-01 20:57:11.000000 hyundai_kia_connect_api-3.2.0/hyundai_kia_connect_api/VehicleManager.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-01 20:57:11.000000 hyundai_kia_connect_api-3.2.0/hyundai_kia_connect_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-01 20:57:11.000000 hyundai_kia_connect_api-3.2.0/hyundai_kia_connect_api/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-01 20:57:11.000000 hyundai_kia_connect_api-3.2.0/hyundai_kia_connect_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-01 20:57:11.000000 hyundai_kia_connect_api-3.2.0/hyundai_kia_connect_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:57:43.402552 hyundai_kia_connect_api-3.2.0/hyundai_kia_connect_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-05-01 20:57:43.000000 hyundai_kia_connect_api-3.2.0/hyundai_kia_connect_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-01 20:57:43.000000 hyundai_kia_connect_api-3.2.0/hyundai_kia_connect_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 20:57:43.000000 hyundai_kia_connect_api-3.2.0/hyundai_kia_connect_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 20:57:43.000000 hyundai_kia_connect_api-3.2.0/hyundai_kia_connect_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-01 20:57:43.000000 hyundai_kia_connect_api-3.2.0/hyundai_kia_connect_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-01 20:57:43.000000 hyundai_kia_connect_api-3.2.0/hyundai_kia_connect_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-01 20:57:11.000000 hyundai_kia_connect_api-3.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-01 20:57:43.402552 hyundai_kia_connect_api-3.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-01 20:57:31.000000 hyundai_kia_connect_api-3.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:57:43.402552 hyundai_kia_connect_api-3.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 20:57:11.000000 hyundai_kia_connect_api-3.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-01 20:57:11.000000 hyundai_kia_connect_api-3.2.0/tests/ca_login_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-01 20:57:11.000000 hyundai_kia_connect_api-3.2.0/tests/eu_check_response_for_errors_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-01 20:57:11.000000 hyundai_kia_connect_api-3.2.0/tests/eu_login_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:24:19.080946 hyundai_kia_connect_api-3.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-05-02 17:24:19.080946 hyundai_kia_connect_api-3.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:24:19.076946 hyundai_kia_connect_api-3.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:24:19.080946 hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api/ApiImpl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23907 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api/HyundaiBlueLinkAPIUSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27449 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api/KiaUvoAPIUSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30644 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api/KiaUvoApiCA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51320 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api/KiaUvoApiCN.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53887 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api/KiaUvoApiEU.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api/Token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12772 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api/Vehicle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9083 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api/VehicleManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:24:19.080946 hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-05-02 17:24:19.000000 hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-02 17:24:19.000000 hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 17:24:19.000000 hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 17:24:18.000000 hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-02 17:24:19.000000 hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-02 17:24:19.000000 hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-02 17:24:19.080946 hyundai_kia_connect_api-3.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-02 17:24:03.000000 hyundai_kia_connect_api-3.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:24:19.080946 hyundai_kia_connect_api-3.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/tests/ca_login_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/tests/eu_check_response_for_errors_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-02 17:23:32.000000 hyundai_kia_connect_api-3.3.0/tests/eu_login_test.py
```

### Comparing `hyundai_kia_connect_api-3.2.0/CONTRIBUTING.rst` & `hyundai_kia_connect_api-3.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.2.0/LICENSE` & `hyundai_kia_connect_api-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.2.0/PKG-INFO` & `hyundai_kia_connect_api-3.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyundai_kia_connect_api
-Version: 3.2.0
+Version: 3.3.0
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/fuatakgun/hyundai_kia_connect_api
 Author: Fuat Akgun
 Author-email: fuatakgun@gmail.com
 License: MIT license
 Keywords: hyundai_kia_connect_api
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `hyundai_kia_connect_api-3.2.0/README.rst` & `hyundai_kia_connect_api-3.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.2.0/docs/Makefile` & `hyundai_kia_connect_api-3.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.2.0/docs/conf.py` & `hyundai_kia_connect_api-3.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.2.0/docs/installation.rst` & `hyundai_kia_connect_api-3.3.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.2.0/docs/make.bat` & `hyundai_kia_connect_api-3.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.2.0/hyundai_kia_connect_api/ApiImpl.py` & `hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api/ApiImpl.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.2.0/hyundai_kia_connect_api/HyundaiBlueLinkAPIUSA.py` & `hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api/HyundaiBlueLinkAPIUSA.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.2.0/hyundai_kia_connect_api/KiaUvoAPIUSA.py` & `hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api/KiaUvoAPIUSA.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.2.0/hyundai_kia_connect_api/KiaUvoApiCA.py` & `hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api/KiaUvoApiCA.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.2.0/hyundai_kia_connect_api/KiaUvoApiEU.py` & `hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api/KiaUvoApiEU.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.2.0/hyundai_kia_connect_api/Vehicle.py` & `hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api/Vehicle.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.2.0/hyundai_kia_connect_api/VehicleManager.py` & `hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api/VehicleManager.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,24 +7,26 @@
 import pytz
 
 from .ApiImpl import ApiImpl, ClimateRequestOptions
 from .HyundaiBlueLinkAPIUSA import HyundaiBlueLinkAPIUSA
 from .KiaUvoAPIUSA import KiaUvoAPIUSA
 from .KiaUvoApiCA import KiaUvoApiCA
 from .KiaUvoApiEU import KiaUvoApiEU
+from .KiaUvoApiCN import KiaUvoApiCN
 from .Token import Token
 from .Vehicle import Vehicle
 from .const import (
     BRAND_HYUNDAI,
     BRAND_KIA,
     BRANDS,
     DOMAIN,
     REGION_CANADA,
     REGION_EUROPE,
     REGION_USA,
+    REGION_CHINA,
     REGIONS,
     VEHICLE_LOCK_ACTION,
     CHARGE_PORT_ACTION,
     OrderStatus,
 )
 
 _LOGGER = logging.getLogger(__name__)
@@ -233,7 +235,9 @@
             return KiaUvoApiCA(region, brand, language)
         elif REGIONS[region] == REGION_EUROPE:
             return KiaUvoApiEU(region, brand, language)
         elif REGIONS[region] == REGION_USA and BRANDS[brand] == BRAND_HYUNDAI:
             return HyundaiBlueLinkAPIUSA(region, brand, language)
         elif REGIONS[region] == REGION_USA and BRANDS[brand] == BRAND_KIA:
             return KiaUvoAPIUSA(region, brand, language)
+        elif REGIONS[region] == REGION_CHINA:
+            return KiaUvoApiCN(region, brand, language)
```

### Comparing `hyundai_kia_connect_api-3.2.0/hyundai_kia_connect_api/const.py` & `hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api/const.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 BRAND_KIA = "Kia"
 BRAND_HYUNDAI = "Hyundai"
 BRANDS = {1: BRAND_KIA, 2: BRAND_HYUNDAI}
 
 REGION_EUROPE = "Europe"
 REGION_CANADA = "Canada"
 REGION_USA = "USA"
-REGIONS = {1: REGION_EUROPE, 2: REGION_CANADA, 3: REGION_USA}
+REGION_CHINA = "China"
+REGIONS = {1: REGION_EUROPE, 2: REGION_CANADA, 3: REGION_USA, 4: REGION_CHINA}
 
 LENGTH_KILOMETERS = "km"
 LENGTH_MILES = "mi"
 DISTANCE_UNITS = {None: None, 0: None, 1: LENGTH_KILOMETERS, 3: LENGTH_MILES}
 
 TEMPERATURE_C = "°C"
 TEMPERATURE_F = "°F"
```

### Comparing `hyundai_kia_connect_api-3.2.0/hyundai_kia_connect_api/exceptions.py` & `hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.2.0/hyundai_kia_connect_api/utils.py` & `hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api/utils.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.2.0/hyundai_kia_connect_api.egg-info/PKG-INFO` & `hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyundai-kia-connect-api
-Version: 3.2.0
+Version: 3.3.0
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/fuatakgun/hyundai_kia_connect_api
 Author: Fuat Akgun
 Author-email: fuatakgun@gmail.com
 License: MIT license
 Keywords: hyundai_kia_connect_api
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `hyundai_kia_connect_api-3.2.0/hyundai_kia_connect_api.egg-info/SOURCES.txt` & `hyundai_kia_connect_api-3.3.0/hyundai_kia_connect_api.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 docs/make.bat
 docs/readme.rst
 docs/usage.rst
 hyundai_kia_connect_api/ApiImpl.py
 hyundai_kia_connect_api/HyundaiBlueLinkAPIUSA.py
 hyundai_kia_connect_api/KiaUvoAPIUSA.py
 hyundai_kia_connect_api/KiaUvoApiCA.py
+hyundai_kia_connect_api/KiaUvoApiCN.py
 hyundai_kia_connect_api/KiaUvoApiEU.py
 hyundai_kia_connect_api/Token.py
 hyundai_kia_connect_api/Vehicle.py
 hyundai_kia_connect_api/VehicleManager.py
 hyundai_kia_connect_api/__init__.py
 hyundai_kia_connect_api/const.py
 hyundai_kia_connect_api/exceptions.py
```

### Comparing `hyundai_kia_connect_api-3.2.0/setup.py` & `hyundai_kia_connect_api-3.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,10 +40,10 @@
     name="hyundai_kia_connect_api",
     packages=find_packages(
         include=["hyundai_kia_connect_api", "hyundai_kia_connect_api.*"]
     ),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/fuatakgun/hyundai_kia_connect_api",
-    version="3.2.0",
+    version="3.3.0",
     zip_safe=False,
 )
```

### Comparing `hyundai_kia_connect_api-3.2.0/tests/ca_login_test.py` & `hyundai_kia_connect_api-3.3.0/tests/ca_login_test.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.2.0/tests/eu_check_response_for_errors_test.py` & `hyundai_kia_connect_api-3.3.0/tests/eu_check_response_for_errors_test.py`

 * *Files identical despite different names*

