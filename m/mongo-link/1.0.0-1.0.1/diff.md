# Comparing `tmp/mongo_link-1.0.0.tar.gz` & `tmp/mongo_link-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongo_link-1.0.0.tar", last modified: Sun Apr 30 19:39:40 2023, max compression
+gzip compressed data, was "mongo_link-1.0.1.tar", last modified: Mon May  1 22:27:16 2023, max compression
```

## Comparing `mongo_link-1.0.0.tar` & `mongo_link-1.0.1.tar`

### file list

```diff
@@ -1,40 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 19:39:40.272672 mongo_link-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-30 19:39:26.000000 mongo_link-1.0.0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-30 19:39:40.272672 mongo_link-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-04-30 19:39:26.000000 mongo_link-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 19:39:40.264672 mongo_link-1.0.0/mongo_link/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 19:39:26.000000 mongo_link-1.0.0/mongo_link/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-30 19:39:26.000000 mongo_link-1.0.0/mongo_link/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 19:39:40.268672 mongo_link-1.0.0/mongo_link/mongo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 19:39:26.000000 mongo_link-1.0.0/mongo_link/mongo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 19:39:40.268672 mongo_link-1.0.0/mongo_link/mongo/driver/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-30 19:39:26.000000 mongo_link-1.0.0/mongo_link/mongo/driver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-30 19:39:26.000000 mongo_link-1.0.0/mongo_link/mongo/driver/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-30 19:39:26.000000 mongo_link-1.0.0/mongo_link/mongo/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 19:39:40.268672 mongo_link-1.0.0/mongo_link/mongo/indexes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 19:39:26.000000 mongo_link-1.0.0/mongo_link/mongo/indexes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-30 19:39:26.000000 mongo_link-1.0.0/mongo_link/mongo/indexes/mongo_index.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 19:39:40.268672 mongo_link-1.0.0/mongo_link/mongo/model/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-30 19:39:26.000000 mongo_link-1.0.0/mongo_link/mongo/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-30 19:39:26.000000 mongo_link-1.0.0/mongo_link/mongo/model/mongo_embedded_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-30 19:39:26.000000 mongo_link-1.0.0/mongo_link/mongo/model/mongo_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 19:39:40.268672 mongo_link-1.0.0/mongo_link/mongo/motor/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-30 19:39:26.000000 mongo_link-1.0.0/mongo_link/mongo/motor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-30 19:39:26.000000 mongo_link-1.0.0/mongo_link/mongo/motor/motor_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-04-30 19:39:26.000000 mongo_link-1.0.0/mongo_link/mongo/motor/motor_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 19:39:40.268672 mongo_link-1.0.0/mongo_link/mongo/repository/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-30 19:39:26.000000 mongo_link-1.0.0/mongo_link/mongo/repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-30 19:39:26.000000 mongo_link-1.0.0/mongo_link/mongo/repository/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-30 19:39:26.000000 mongo_link-1.0.0/mongo_link/mongo/repository/repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-30 19:39:26.000000 mongo_link-1.0.0/mongo_link/mongo/repository/repository_decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 19:39:40.272672 mongo_link-1.0.0/mongo_link/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 19:39:26.000000 mongo_link-1.0.0/mongo_link/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-30 19:39:26.000000 mongo_link-1.0.0/mongo_link/utils/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 19:39:40.268672 mongo_link-1.0.0/mongo_link.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-30 19:39:40.000000 mongo_link-1.0.0/mongo_link.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-30 19:39:40.000000 mongo_link-1.0.0/mongo_link.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 19:39:40.000000 mongo_link-1.0.0/mongo_link.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-30 19:39:40.000000 mongo_link-1.0.0/mongo_link.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-30 19:39:40.000000 mongo_link-1.0.0/mongo_link.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 19:39:40.272672 mongo_link-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-04-30 19:39:26.000000 mongo_link-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:27:16.723693 mongo_link-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-01 22:26:59.000000 mongo_link-1.0.1/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-01 22:27:16.723693 mongo_link-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-05-01 22:26:59.000000 mongo_link-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:27:16.715693 mongo_link-1.0.1/mongo_link/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 22:26:59.000000 mongo_link-1.0.1/mongo_link/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-01 22:26:59.000000 mongo_link-1.0.1/mongo_link/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:27:16.719693 mongo_link-1.0.1/mongo_link/mongo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 22:26:59.000000 mongo_link-1.0.1/mongo_link/mongo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:27:16.719693 mongo_link-1.0.1/mongo_link/mongo/driver/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-01 22:26:59.000000 mongo_link-1.0.1/mongo_link/mongo/driver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-01 22:26:59.000000 mongo_link-1.0.1/mongo_link/mongo/driver/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-01 22:26:59.000000 mongo_link-1.0.1/mongo_link/mongo/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:27:16.719693 mongo_link-1.0.1/mongo_link/mongo/indexes/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-01 22:26:59.000000 mongo_link-1.0.1/mongo_link/mongo/indexes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-01 22:26:59.000000 mongo_link-1.0.1/mongo_link/mongo/indexes/mongo_index.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:27:16.719693 mongo_link-1.0.1/mongo_link/mongo/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-01 22:26:59.000000 mongo_link-1.0.1/mongo_link/mongo/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-01 22:26:59.000000 mongo_link-1.0.1/mongo_link/mongo/model/mongo_embedded_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-01 22:26:59.000000 mongo_link-1.0.1/mongo_link/mongo/model/mongo_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:27:16.719693 mongo_link-1.0.1/mongo_link/mongo/motor/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-01 22:26:59.000000 mongo_link-1.0.1/mongo_link/mongo/motor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-01 22:26:59.000000 mongo_link-1.0.1/mongo_link/mongo/motor/motor_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-05-01 22:26:59.000000 mongo_link-1.0.1/mongo_link/mongo/motor/motor_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:27:16.719693 mongo_link-1.0.1/mongo_link/mongo/repository/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-01 22:26:59.000000 mongo_link-1.0.1/mongo_link/mongo/repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-01 22:26:59.000000 mongo_link-1.0.1/mongo_link/mongo/repository/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-01 22:26:59.000000 mongo_link-1.0.1/mongo_link/mongo/repository/repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-01 22:26:59.000000 mongo_link-1.0.1/mongo_link/mongo/repository/repository_decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:27:16.719693 mongo_link-1.0.1/mongo_link/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 22:26:59.000000 mongo_link-1.0.1/mongo_link/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-01 22:26:59.000000 mongo_link-1.0.1/mongo_link/utils/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:27:16.715693 mongo_link-1.0.1/mongo_link.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-01 22:27:16.000000 mongo_link-1.0.1/mongo_link.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-01 22:27:16.000000 mongo_link-1.0.1/mongo_link.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 22:27:16.000000 mongo_link-1.0.1/mongo_link.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-01 22:27:16.000000 mongo_link-1.0.1/mongo_link.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 22:27:16.000000 mongo_link-1.0.1/mongo_link.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 22:27:16.723693 mongo_link-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-01 22:26:59.000000 mongo_link-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:27:16.719693 mongo_link-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 22:26:59.000000 mongo_link-1.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-01 22:26:59.000000 mongo_link-1.0.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:27:16.719693 mongo_link-1.0.1/tests/functionality/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 22:26:59.000000 mongo_link-1.0.1/tests/functionality/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-01 22:26:59.000000 mongo_link-1.0.1/tests/functionality/create_index.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:27:16.723693 mongo_link-1.0.1/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 22:26:59.000000 mongo_link-1.0.1/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-01 22:26:59.000000 mongo_link-1.0.1/tests/utils/config.py
```

### Comparing `mongo_link-1.0.0/LICENCE` & `mongo_link-1.0.1/LICENCE`

 * *Files identical despite different names*

### Comparing `mongo_link-1.0.0/PKG-INFO` & `mongo_link-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongo_link
-Version: 1.0.0
+Version: 1.0.1
 Summary: Mongo link is a orm wrapper for motor and pymongo
 Home-page: https://github.com/kovtunov-oleksandr/MongoLink
 Author: Kovtunov Oleksandr
 Author-email: kovtunov.oleksandr.00@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `mongo_link-1.0.0/README.md` & `mongo_link-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,21 +9,22 @@
 Seamless integration of MongoDB with Pydantic models
 Asynchronous support for efficient and scalable operations
 Customizable schema validation and alias handling
 Clean, expressive, and easy-to-use API
 
 Get started with MongoLink today and streamline your data management workflow with Python and MongoDB!
 
+Full documentation is available at [doc](./doc/Doc.md).
 
 ## Installation
 
 MongoLink is not available on PyPI, can be installed with pip:
 
 ```bash
-pip install git+https://github.com/kovtunov-oleksandr/MongoLink.git
+pip install mongo-link
 ```
 
 ## Quickstart
 
 
 ### Driver
 `Driver` is a class that provides a set of methods for interacting with MongoDB.
```

### Comparing `mongo_link-1.0.0/mongo_link/mongo/indexes/mongo_index.py` & `mongo_link-1.0.1/mongo_link/mongo/indexes/mongo_index.py`

 * *Files identical despite different names*

### Comparing `mongo_link-1.0.0/mongo_link/mongo/model/mongo_model.py` & `mongo_link-1.0.1/mongo_link/mongo/model/mongo_model.py`

 * *Files identical despite different names*

### Comparing `mongo_link-1.0.0/mongo_link/mongo/motor/motor_driver.py` & `mongo_link-1.0.1/mongo_link/mongo/motor/motor_driver.py`

 * *Files identical despite different names*

### Comparing `mongo_link-1.0.0/mongo_link/mongo/motor/motor_repository.py` & `mongo_link-1.0.1/mongo_link/mongo/motor/motor_repository.py`

 * *Files identical despite different names*

### Comparing `mongo_link-1.0.0/mongo_link/mongo/repository/repository.py` & `mongo_link-1.0.1/mongo_link/mongo/repository/repository.py`

 * *Files identical despite different names*

### Comparing `mongo_link-1.0.0/mongo_link/mongo/repository/repository_decorators.py` & `mongo_link-1.0.1/mongo_link/mongo/repository/repository_decorators.py`

 * *Files identical despite different names*

### Comparing `mongo_link-1.0.0/mongo_link/utils/singleton.py` & `mongo_link-1.0.1/mongo_link/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `mongo_link-1.0.0/mongo_link.egg-info/PKG-INFO` & `mongo_link-1.0.1/mongo_link.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongo-link
-Version: 1.0.0
+Version: 1.0.1
 Summary: Mongo link is a orm wrapper for motor and pymongo
 Home-page: https://github.com/kovtunov-oleksandr/MongoLink
 Author: Kovtunov Oleksandr
 Author-email: kovtunov.oleksandr.00@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `mongo_link-1.0.0/setup.py` & `mongo_link-1.0.1/setup.py`

 * *Files identical despite different names*

