# Comparing `tmp/core-braincube-dev-0.0.1.tar.gz` & `tmp/core-braincube-dev-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core-braincube-dev-0.0.1.tar", last modified: Tue May  2 09:53:35 2023, max compression
+gzip compressed data, was "core-braincube-dev-0.0.2.tar", last modified: Tue May  2 11:07:05 2023, max compression
```

## Comparing `core-braincube-dev-0.0.1.tar` & `core-braincube-dev-0.0.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 09:53:35.784641 core-braincube-dev-0.0.1/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1066 2023-05-02 09:45:18.000000 core-braincube-dev-0.0.1/LICENSE
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      643 2023-05-02 09:53:35.784104 core-braincube-dev-0.0.1/PKG-INFO
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     4275 2023-05-02 09:47:16.000000 core-braincube-dev-0.0.1/README.md
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 09:53:35.771048 core-braincube-dev-0.0.1/core/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.1/core/__init__.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 09:53:35.774130 core-braincube-dev-0.0.1/core/dal/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.1/core/dal/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1289 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.1/core/dal/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      281 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.1/core/dal/database_errors.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1497 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.1/core/dal/postgres_connection.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)    20547 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.1/core/dal/postgres_repository.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 09:53:35.776248 core-braincube-dev-0.0.1/core/di/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.1/core/di/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      623 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.1/core/di/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     3472 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.1/core/di/injector.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 09:53:35.778907 core-braincube-dev-0.0.1/core/rest/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.1/core/rest/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1112 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.1/core/rest/app_controller.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     3026 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.1/core/rest/app_module.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     3631 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.1/core/rest/data.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 09:53:35.780782 core-braincube-dev-0.0.1/core/utils/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.1/core/utils/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      580 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.1/core/utils/convert.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1111 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.1/core/utils/data.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 09:53:35.783442 core-braincube-dev-0.0.1/core_braincube_dev.egg-info/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      643 2023-05-02 09:53:35.000000 core-braincube-dev-0.0.1/core_braincube_dev.egg-info/PKG-INFO
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      594 2023-05-02 09:53:35.000000 core-braincube-dev-0.0.1/core_braincube_dev.egg-info/SOURCES.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        1 2023-05-02 09:53:35.000000 core-braincube-dev-0.0.1/core_braincube_dev.egg-info/dependency_links.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)       24 2023-05-02 09:53:35.000000 core-braincube-dev-0.0.1/core_braincube_dev.egg-info/requires.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        5 2023-05-02 09:53:35.000000 core-braincube-dev-0.0.1/core_braincube_dev.egg-info/top_level.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)       38 2023-05-02 09:53:35.784808 core-braincube-dev-0.0.1/setup.cfg
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      848 2023-05-02 09:36:50.000000 core-braincube-dev-0.0.1/setup.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:07:05.687977 core-braincube-dev-0.0.2/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1066 2023-05-02 09:45:18.000000 core-braincube-dev-0.0.2/LICENSE
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      643 2023-05-02 11:07:05.687486 core-braincube-dev-0.0.2/PKG-INFO
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     4275 2023-05-02 09:47:16.000000 core-braincube-dev-0.0.2/README.md
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:07:05.668061 core-braincube-dev-0.0.2/core/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.2/core/__init__.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:07:05.670118 core-braincube-dev-0.0.2/core/dal/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.2/core/dal/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1289 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.2/core/dal/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      281 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.2/core/dal/database_errors.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1497 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.2/core/dal/postgres_connection.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)    20547 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.2/core/dal/postgres_repository.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:07:05.672361 core-braincube-dev-0.0.2/core/di/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.2/core/di/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      623 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.2/core/di/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     3472 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.2/core/di/injector.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:07:05.675272 core-braincube-dev-0.0.2/core/rest/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.2/core/rest/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1112 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.2/core/rest/app_controller.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     3026 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.2/core/rest/app_module.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     3631 2023-05-02 11:05:30.000000 core-braincube-dev-0.0.2/core/rest/data.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:07:05.678242 core-braincube-dev-0.0.2/core/utils/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.2/core/utils/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      580 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.2/core/utils/convert.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1111 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.2/core/utils/data.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:07:05.684795 core-braincube-dev-0.0.2/core_braincube_dev.egg-info/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      643 2023-05-02 11:07:05.000000 core-braincube-dev-0.0.2/core_braincube_dev.egg-info/PKG-INFO
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      594 2023-05-02 11:07:05.000000 core-braincube-dev-0.0.2/core_braincube_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        1 2023-05-02 11:07:05.000000 core-braincube-dev-0.0.2/core_braincube_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)       24 2023-05-02 11:07:05.000000 core-braincube-dev-0.0.2/core_braincube_dev.egg-info/requires.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        5 2023-05-02 11:07:05.000000 core-braincube-dev-0.0.2/core_braincube_dev.egg-info/top_level.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)       38 2023-05-02 11:07:05.688129 core-braincube-dev-0.0.2/setup.cfg
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      848 2023-05-02 11:02:02.000000 core-braincube-dev-0.0.2/setup.py
```

### Comparing `core-braincube-dev-0.0.1/LICENSE` & `core-braincube-dev-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.1/PKG-INFO` & `core-braincube-dev-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: core-braincube-dev
-Version: 0.0.1
+Version: 0.0.2
 Summary: Microframework for aws lambdas
 Author: Boudis Evangelos
 Author-email: <evangelos.boudis@gmail.com>
 Keywords: amazon,aws,lambda,routing,dal,injection
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `core-braincube-dev-0.0.1/README.md` & `core-braincube-dev-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.1/core/dal/data.py` & `core-braincube-dev-0.0.2/core/dal/data.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.1/core/dal/postgres_connection.py` & `core-braincube-dev-0.0.2/core/dal/postgres_connection.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.1/core/dal/postgres_repository.py` & `core-braincube-dev-0.0.2/core/dal/postgres_repository.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.1/core/di/data.py` & `core-braincube-dev-0.0.2/core/di/data.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.1/core/di/injector.py` & `core-braincube-dev-0.0.2/core/di/injector.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.1/core/rest/app_controller.py` & `core-braincube-dev-0.0.2/core/rest/app_controller.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.1/core/rest/app_module.py` & `core-braincube-dev-0.0.2/core/rest/app_module.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.1/core/rest/data.py` & `core-braincube-dev-0.0.2/core/rest/data.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.1/core/utils/convert.py` & `core-braincube-dev-0.0.2/core/utils/convert.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.1/core/utils/data.py` & `core-braincube-dev-0.0.2/core/utils/data.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.1/core_braincube_dev.egg-info/PKG-INFO` & `core-braincube-dev-0.0.2/core_braincube_dev.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: core-braincube-dev
-Version: 0.0.1
+Version: 0.0.2
 Summary: Microframework for aws lambdas
 Author: Boudis Evangelos
 Author-email: <evangelos.boudis@gmail.com>
 Keywords: amazon,aws,lambda,routing,dal,injection
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `core-braincube-dev-0.0.1/core_braincube_dev.egg-info/SOURCES.txt` & `core-braincube-dev-0.0.2/core_braincube_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.1/setup.py` & `core-braincube-dev-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="core-braincube-dev",
-    version="0.0.1",
+    version="0.0.2",
     author="Boudis Evangelos",
     author_email="<evangelos.boudis@gmail.com>",
     description="Microframework for aws lambdas",
     long_description_content_type="text/markdown",
     long_description="core-braincube-dev is a developer toolkit to implement Serverless best practices.",
     packages=find_packages(),
     install_requires=["asyncpg", "pypika", "pydantic"],
```

