# Comparing `tmp/core-braincube-dev-0.0.6.tar.gz` & `tmp/core-braincube-dev-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core-braincube-dev-0.0.6.tar", last modified: Tue May  2 11:56:01 2023, max compression
+gzip compressed data, was "core-braincube-dev-0.0.7.tar", last modified: Tue May  2 11:57:12 2023, max compression
```

## Comparing `core-braincube-dev-0.0.6.tar` & `core-braincube-dev-0.0.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:56:01.466226 core-braincube-dev-0.0.6/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1066 2023-05-02 09:45:18.000000 core-braincube-dev-0.0.6/LICENSE
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      903 2023-05-02 11:56:01.466472 core-braincube-dev-0.0.6/PKG-INFO
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     4291 2023-05-02 11:38:16.000000 core-braincube-dev-0.0.6/README.md
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:56:01.458122 core-braincube-dev-0.0.6/core/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.6/core/__init__.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:56:01.459758 core-braincube-dev-0.0.6/core/dal/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.6/core/dal/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1289 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.6/core/dal/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      281 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.6/core/dal/database_errors.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1497 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.6/core/dal/postgres_connection.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)    20547 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.6/core/dal/postgres_repository.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:56:01.461043 core-braincube-dev-0.0.6/core/di/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.6/core/di/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      623 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.6/core/di/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     3472 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.6/core/di/injector.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:56:01.462600 core-braincube-dev-0.0.6/core/rest/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.6/core/rest/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1112 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.6/core/rest/app_controller.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     3026 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.6/core/rest/app_module.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     3631 2023-05-02 11:05:30.000000 core-braincube-dev-0.0.6/core/rest/data.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:56:01.463737 core-braincube-dev-0.0.6/core/utils/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.6/core/utils/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      580 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.6/core/utils/convert.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1111 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.6/core/utils/data.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:56:01.465825 core-braincube-dev-0.0.6/core_braincube_dev.egg-info/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      903 2023-05-02 11:56:01.000000 core-braincube-dev-0.0.6/core_braincube_dev.egg-info/PKG-INFO
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      604 2023-05-02 11:56:01.000000 core-braincube-dev-0.0.6/core_braincube_dev.egg-info/SOURCES.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        1 2023-05-02 11:56:01.000000 core-braincube-dev-0.0.6/core_braincube_dev.egg-info/dependency_links.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)       48 2023-05-02 11:56:01.000000 core-braincube-dev-0.0.6/core_braincube_dev.egg-info/requires.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        5 2023-05-02 11:56:01.000000 core-braincube-dev-0.0.6/core_braincube_dev.egg-info/top_level.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      969 2023-05-02 11:56:01.467456 core-braincube-dev-0.0.6/setup.cfg
--rw-r--r--   0 evangelosboudis   (501) staff       (20)       38 2023-05-02 11:28:19.000000 core-braincube-dev-0.0.6/setup.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:57:12.711250 core-braincube-dev-0.0.7/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1066 2023-05-02 09:45:18.000000 core-braincube-dev-0.0.7/LICENSE
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      903 2023-05-02 11:57:12.711952 core-braincube-dev-0.0.7/PKG-INFO
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     4291 2023-05-02 11:38:16.000000 core-braincube-dev-0.0.7/README.md
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:57:12.702925 core-braincube-dev-0.0.7/core/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.7/core/__init__.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:57:12.704481 core-braincube-dev-0.0.7/core/dal/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.7/core/dal/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1289 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.7/core/dal/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      281 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.7/core/dal/database_errors.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1497 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.7/core/dal/postgres_connection.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)    20547 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.7/core/dal/postgres_repository.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:57:12.705650 core-braincube-dev-0.0.7/core/di/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.7/core/di/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      623 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.7/core/di/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     3472 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.7/core/di/injector.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:57:12.707071 core-braincube-dev-0.0.7/core/rest/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.7/core/rest/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1112 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.7/core/rest/app_controller.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     3026 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.7/core/rest/app_module.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     3631 2023-05-02 11:05:30.000000 core-braincube-dev-0.0.7/core/rest/data.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:57:12.708216 core-braincube-dev-0.0.7/core/utils/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.7/core/utils/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      580 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.7/core/utils/convert.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1111 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.7/core/utils/data.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:57:12.710298 core-braincube-dev-0.0.7/core_braincube_dev.egg-info/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      903 2023-05-02 11:57:12.000000 core-braincube-dev-0.0.7/core_braincube_dev.egg-info/PKG-INFO
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      604 2023-05-02 11:57:12.000000 core-braincube-dev-0.0.7/core_braincube_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        1 2023-05-02 11:57:12.000000 core-braincube-dev-0.0.7/core_braincube_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)       48 2023-05-02 11:57:12.000000 core-braincube-dev-0.0.7/core_braincube_dev.egg-info/requires.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        5 2023-05-02 11:57:12.000000 core-braincube-dev-0.0.7/core_braincube_dev.egg-info/top_level.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      974 2023-05-02 11:57:12.713625 core-braincube-dev-0.0.7/setup.cfg
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)       38 2023-05-02 11:28:19.000000 core-braincube-dev-0.0.7/setup.py
```

### Comparing `core-braincube-dev-0.0.6/LICENSE` & `core-braincube-dev-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.6/PKG-INFO` & `core-braincube-dev-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: core-braincube-dev
-Version: 0.0.6
+Version: 0.0.7
 Summary: Microframework for python aws lambdas
 Home-page: https://bitbucket.org/braincube-common/core-aws.git
 Author: Braincube
 Author-email: spresvias@braincube.gr
 License: MIT
 Keywords: python,amazon,aws,lambda,routing,dal,injection
 Classifier: Intended Audience :: Developers
```

### Comparing `core-braincube-dev-0.0.6/README.md` & `core-braincube-dev-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.6/core/dal/data.py` & `core-braincube-dev-0.0.7/core/dal/data.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.6/core/dal/postgres_connection.py` & `core-braincube-dev-0.0.7/core/dal/postgres_connection.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.6/core/dal/postgres_repository.py` & `core-braincube-dev-0.0.7/core/dal/postgres_repository.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.6/core/di/data.py` & `core-braincube-dev-0.0.7/core/di/data.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.6/core/di/injector.py` & `core-braincube-dev-0.0.7/core/di/injector.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.6/core/rest/app_controller.py` & `core-braincube-dev-0.0.7/core/rest/app_controller.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.6/core/rest/app_module.py` & `core-braincube-dev-0.0.7/core/rest/app_module.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.6/core/rest/data.py` & `core-braincube-dev-0.0.7/core/rest/data.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.6/core/utils/convert.py` & `core-braincube-dev-0.0.7/core/utils/convert.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.6/core/utils/data.py` & `core-braincube-dev-0.0.7/core/utils/data.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.6/core_braincube_dev.egg-info/PKG-INFO` & `core-braincube-dev-0.0.7/core_braincube_dev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: core-braincube-dev
-Version: 0.0.6
+Version: 0.0.7
 Summary: Microframework for python aws lambdas
 Home-page: https://bitbucket.org/braincube-common/core-aws.git
 Author: Braincube
 Author-email: spresvias@braincube.gr
 License: MIT
 Keywords: python,amazon,aws,lambda,routing,dal,injection
 Classifier: Intended Audience :: Developers
```

### Comparing `core-braincube-dev-0.0.6/core_braincube_dev.egg-info/SOURCES.txt` & `core-braincube-dev-0.0.7/core_braincube_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.6/setup.cfg` & `core-braincube-dev-0.0.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [metadata]
 name = core-braincube-dev
-version = 0.0.6
+version = 0.0.7
 url = https://bitbucket.org/braincube-common/core-aws.git
 author = Braincube
 author_email = spresvias@braincube.gr
 license = MIT
 license_files = LICENSE
 description = Microframework for python aws lambdas
-description-file = README.md
+long-description-file = README.md
 classifiers = 
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
```

