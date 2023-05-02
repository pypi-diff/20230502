# Comparing `tmp/core-braincube-dev-0.0.4.tar.gz` & `tmp/core-braincube-dev-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core-braincube-dev-0.0.4.tar", last modified: Tue May  2 11:40:37 2023, max compression
+gzip compressed data, was "core-braincube-dev-0.0.5.tar", last modified: Tue May  2 11:46:08 2023, max compression
```

## Comparing `core-braincube-dev-0.0.4.tar` & `core-braincube-dev-0.0.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:40:37.606597 core-braincube-dev-0.0.4/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1066 2023-05-02 09:45:18.000000 core-braincube-dev-0.0.4/LICENSE
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      903 2023-05-02 11:40:37.606817 core-braincube-dev-0.0.4/PKG-INFO
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     4291 2023-05-02 11:38:16.000000 core-braincube-dev-0.0.4/README.md
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:40:37.595172 core-braincube-dev-0.0.4/core/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.4/core/__init__.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:40:37.598300 core-braincube-dev-0.0.4/core/dal/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.4/core/dal/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1289 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.4/core/dal/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      281 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.4/core/dal/database_errors.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1497 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.4/core/dal/postgres_connection.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)    20547 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.4/core/dal/postgres_repository.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:40:37.600300 core-braincube-dev-0.0.4/core/di/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.4/core/di/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      623 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.4/core/di/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     3472 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.4/core/di/injector.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:40:37.602472 core-braincube-dev-0.0.4/core/rest/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.4/core/rest/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1112 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.4/core/rest/app_controller.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     3026 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.4/core/rest/app_module.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     3631 2023-05-02 11:05:30.000000 core-braincube-dev-0.0.4/core/rest/data.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:40:37.603910 core-braincube-dev-0.0.4/core/utils/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.4/core/utils/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      580 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.4/core/utils/convert.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1111 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.4/core/utils/data.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:40:37.606230 core-braincube-dev-0.0.4/core_braincube_dev.egg-info/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      903 2023-05-02 11:40:37.000000 core-braincube-dev-0.0.4/core_braincube_dev.egg-info/PKG-INFO
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      604 2023-05-02 11:40:37.000000 core-braincube-dev-0.0.4/core_braincube_dev.egg-info/SOURCES.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        1 2023-05-02 11:40:37.000000 core-braincube-dev-0.0.4/core_braincube_dev.egg-info/dependency_links.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)       48 2023-05-02 11:40:37.000000 core-braincube-dev-0.0.4/core_braincube_dev.egg-info/requires.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        5 2023-05-02 11:40:37.000000 core-braincube-dev-0.0.4/core_braincube_dev.egg-info/top_level.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      940 2023-05-02 11:40:37.607685 core-braincube-dev-0.0.4/setup.cfg
--rw-r--r--   0 evangelosboudis   (501) staff       (20)       38 2023-05-02 11:28:19.000000 core-braincube-dev-0.0.4/setup.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:46:08.678353 core-braincube-dev-0.0.5/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1066 2023-05-02 09:45:18.000000 core-braincube-dev-0.0.5/LICENSE
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      903 2023-05-02 11:46:08.678626 core-braincube-dev-0.0.5/PKG-INFO
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     4291 2023-05-02 11:38:16.000000 core-braincube-dev-0.0.5/README.md
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:46:08.665964 core-braincube-dev-0.0.5/core/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.5/core/__init__.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:46:08.669549 core-braincube-dev-0.0.5/core/dal/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.5/core/dal/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1289 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.5/core/dal/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      281 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.5/core/dal/database_errors.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1497 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.5/core/dal/postgres_connection.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)    20547 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.5/core/dal/postgres_repository.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:46:08.671592 core-braincube-dev-0.0.5/core/di/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.5/core/di/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      623 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.5/core/di/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     3472 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.5/core/di/injector.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:46:08.673962 core-braincube-dev-0.0.5/core/rest/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.5/core/rest/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1112 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.5/core/rest/app_controller.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     3026 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.5/core/rest/app_module.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     3631 2023-05-02 11:05:30.000000 core-braincube-dev-0.0.5/core/rest/data.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:46:08.675492 core-braincube-dev-0.0.5/core/utils/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.5/core/utils/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      580 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.5/core/utils/convert.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1111 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.5/core/utils/data.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:46:08.677802 core-braincube-dev-0.0.5/core_braincube_dev.egg-info/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      903 2023-05-02 11:46:08.000000 core-braincube-dev-0.0.5/core_braincube_dev.egg-info/PKG-INFO
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      604 2023-05-02 11:46:08.000000 core-braincube-dev-0.0.5/core_braincube_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        1 2023-05-02 11:46:08.000000 core-braincube-dev-0.0.5/core_braincube_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)       48 2023-05-02 11:46:08.000000 core-braincube-dev-0.0.5/core_braincube_dev.egg-info/requires.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        5 2023-05-02 11:46:08.000000 core-braincube-dev-0.0.5/core_braincube_dev.egg-info/top_level.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      969 2023-05-02 11:46:08.679529 core-braincube-dev-0.0.5/setup.cfg
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)       38 2023-05-02 11:28:19.000000 core-braincube-dev-0.0.5/setup.py
```

### Comparing `core-braincube-dev-0.0.4/LICENSE` & `core-braincube-dev-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.4/PKG-INFO` & `core-braincube-dev-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: core-braincube-dev
-Version: 0.0.4
+Version: 0.0.5
 Summary: Microframework for python aws lambdas
 Home-page: https://bitbucket.org/braincube-common/core-aws.git
 Author: Braincube
 Author-email: spresvias@braincube.gr
 License: MIT
 Keywords: python,amazon,aws,lambda,routing,dal,injection
 Classifier: Intended Audience :: Developers
```

### Comparing `core-braincube-dev-0.0.4/README.md` & `core-braincube-dev-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.4/core/dal/data.py` & `core-braincube-dev-0.0.5/core/dal/data.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.4/core/dal/postgres_connection.py` & `core-braincube-dev-0.0.5/core/dal/postgres_connection.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.4/core/dal/postgres_repository.py` & `core-braincube-dev-0.0.5/core/dal/postgres_repository.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.4/core/di/data.py` & `core-braincube-dev-0.0.5/core/di/data.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.4/core/di/injector.py` & `core-braincube-dev-0.0.5/core/di/injector.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.4/core/rest/app_controller.py` & `core-braincube-dev-0.0.5/core/rest/app_controller.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.4/core/rest/app_module.py` & `core-braincube-dev-0.0.5/core/rest/app_module.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.4/core/rest/data.py` & `core-braincube-dev-0.0.5/core/rest/data.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.4/core/utils/convert.py` & `core-braincube-dev-0.0.5/core/utils/convert.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.4/core/utils/data.py` & `core-braincube-dev-0.0.5/core/utils/data.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.4/core_braincube_dev.egg-info/PKG-INFO` & `core-braincube-dev-0.0.5/core_braincube_dev.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: core-braincube-dev
-Version: 0.0.4
+Version: 0.0.5
 Summary: Microframework for python aws lambdas
 Home-page: https://bitbucket.org/braincube-common/core-aws.git
 Author: Braincube
 Author-email: spresvias@braincube.gr
 License: MIT
 Keywords: python,amazon,aws,lambda,routing,dal,injection
 Classifier: Intended Audience :: Developers
```

### Comparing `core-braincube-dev-0.0.4/core_braincube_dev.egg-info/SOURCES.txt` & `core-braincube-dev-0.0.5/core_braincube_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.4/setup.cfg` & `core-braincube-dev-0.0.5/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [metadata]
 name = core-braincube-dev
-version = 0.0.4
+version = 0.0.5
 url = https://bitbucket.org/braincube-common/core-aws.git
 author = Braincube
 author_email = spresvias@braincube.gr
 license = MIT
 license_files = LICENSE
 description = Microframework for python aws lambdas
+description-file = README.md
 classifiers = 
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
```

