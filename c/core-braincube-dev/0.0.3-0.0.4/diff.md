# Comparing `tmp/core-braincube-dev-0.0.3.tar.gz` & `tmp/core-braincube-dev-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core-braincube-dev-0.0.3.tar", last modified: Tue May  2 11:34:58 2023, max compression
+gzip compressed data, was "core-braincube-dev-0.0.4.tar", last modified: Tue May  2 11:40:37 2023, max compression
```

## Comparing `core-braincube-dev-0.0.3.tar` & `core-braincube-dev-0.0.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:34:58.080685 core-braincube-dev-0.0.3/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1066 2023-05-02 09:45:18.000000 core-braincube-dev-0.0.3/LICENSE
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      903 2023-05-02 11:34:58.080900 core-braincube-dev-0.0.3/PKG-INFO
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     4275 2023-05-02 09:47:16.000000 core-braincube-dev-0.0.3/README.rst
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:34:58.072860 core-braincube-dev-0.0.3/core/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.3/core/__init__.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:34:58.074420 core-braincube-dev-0.0.3/core/dal/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.3/core/dal/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1289 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.3/core/dal/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      281 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.3/core/dal/database_errors.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1497 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.3/core/dal/postgres_connection.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)    20547 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.3/core/dal/postgres_repository.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:34:58.075515 core-braincube-dev-0.0.3/core/di/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.3/core/di/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      623 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.3/core/di/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     3472 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.3/core/di/injector.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:34:58.076799 core-braincube-dev-0.0.3/core/rest/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.3/core/rest/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1112 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.3/core/rest/app_controller.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     3026 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.3/core/rest/app_module.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     3631 2023-05-02 11:05:30.000000 core-braincube-dev-0.0.3/core/rest/data.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:34:58.077901 core-braincube-dev-0.0.3/core/utils/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.3/core/utils/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      580 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.3/core/utils/convert.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1111 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.3/core/utils/data.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:34:58.080176 core-braincube-dev-0.0.3/core_braincube_dev.egg-info/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      903 2023-05-02 11:34:58.000000 core-braincube-dev-0.0.3/core_braincube_dev.egg-info/PKG-INFO
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      605 2023-05-02 11:34:58.000000 core-braincube-dev-0.0.3/core_braincube_dev.egg-info/SOURCES.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        1 2023-05-02 11:34:58.000000 core-braincube-dev-0.0.3/core_braincube_dev.egg-info/dependency_links.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)       48 2023-05-02 11:34:58.000000 core-braincube-dev-0.0.3/core_braincube_dev.egg-info/requires.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        5 2023-05-02 11:34:58.000000 core-braincube-dev-0.0.3/core_braincube_dev.egg-info/top_level.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      940 2023-05-02 11:34:58.081805 core-braincube-dev-0.0.3/setup.cfg
--rw-r--r--   0 evangelosboudis   (501) staff       (20)       38 2023-05-02 11:28:19.000000 core-braincube-dev-0.0.3/setup.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:40:37.606597 core-braincube-dev-0.0.4/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1066 2023-05-02 09:45:18.000000 core-braincube-dev-0.0.4/LICENSE
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      903 2023-05-02 11:40:37.606817 core-braincube-dev-0.0.4/PKG-INFO
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     4291 2023-05-02 11:38:16.000000 core-braincube-dev-0.0.4/README.md
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:40:37.595172 core-braincube-dev-0.0.4/core/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.4/core/__init__.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:40:37.598300 core-braincube-dev-0.0.4/core/dal/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.4/core/dal/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1289 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.4/core/dal/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      281 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.4/core/dal/database_errors.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1497 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.4/core/dal/postgres_connection.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)    20547 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.4/core/dal/postgres_repository.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:40:37.600300 core-braincube-dev-0.0.4/core/di/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.4/core/di/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      623 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.4/core/di/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     3472 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.4/core/di/injector.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:40:37.602472 core-braincube-dev-0.0.4/core/rest/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.4/core/rest/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1112 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.4/core/rest/app_controller.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     3026 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.4/core/rest/app_module.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     3631 2023-05-02 11:05:30.000000 core-braincube-dev-0.0.4/core/rest/data.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:40:37.603910 core-braincube-dev-0.0.4/core/utils/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.4/core/utils/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      580 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.4/core/utils/convert.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1111 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.4/core/utils/data.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:40:37.606230 core-braincube-dev-0.0.4/core_braincube_dev.egg-info/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      903 2023-05-02 11:40:37.000000 core-braincube-dev-0.0.4/core_braincube_dev.egg-info/PKG-INFO
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      604 2023-05-02 11:40:37.000000 core-braincube-dev-0.0.4/core_braincube_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        1 2023-05-02 11:40:37.000000 core-braincube-dev-0.0.4/core_braincube_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)       48 2023-05-02 11:40:37.000000 core-braincube-dev-0.0.4/core_braincube_dev.egg-info/requires.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        5 2023-05-02 11:40:37.000000 core-braincube-dev-0.0.4/core_braincube_dev.egg-info/top_level.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      940 2023-05-02 11:40:37.607685 core-braincube-dev-0.0.4/setup.cfg
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)       38 2023-05-02 11:28:19.000000 core-braincube-dev-0.0.4/setup.py
```

### Comparing `core-braincube-dev-0.0.3/LICENSE` & `core-braincube-dev-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.3/PKG-INFO` & `core-braincube-dev-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: core-braincube-dev
-Version: 0.0.3
+Version: 0.0.4
 Summary: Microframework for python aws lambdas
 Home-page: https://bitbucket.org/braincube-common/core-aws.git
 Author: Braincube
 Author-email: spresvias@braincube.gr
 License: MIT
 Keywords: python,amazon,aws,lambda,routing,dal,injection
 Classifier: Intended Audience :: Developers
```

### Comparing `core-braincube-dev-0.0.3/README.rst` & `core-braincube-dev-0.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -30,20 +30,20 @@
 
 ### PostgresRepository usage
 
 ```python
 from core.rest.data import HTTPRequest
 from core.dal.data import Key
 from core.dal.postgres_connection import get_pool
-from repository.equities_repo import EquitiesRepo
+from core.dal.postgres_repository import PostgresRepository
 
 request = HTTPRequest()
 
 pool = await get_pool()
-repo = EquitiesRepo(pool)
+repo = PostgresRepository(pool)
 
 await repo.find_by_id(key=Key(request.path_parameters["id"]), aliases=request.query_parameters.fields)
 
 await repo.exists_by_id(key=Key("9448a57b-f686-4935-b152-566baab712db"))
 
 await repo.find_one(
     aliases=request.query_parameters.fields,
```

### Comparing `core-braincube-dev-0.0.3/core/dal/data.py` & `core-braincube-dev-0.0.4/core/dal/data.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.3/core/dal/postgres_connection.py` & `core-braincube-dev-0.0.4/core/dal/postgres_connection.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.3/core/dal/postgres_repository.py` & `core-braincube-dev-0.0.4/core/dal/postgres_repository.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.3/core/di/data.py` & `core-braincube-dev-0.0.4/core/di/data.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.3/core/di/injector.py` & `core-braincube-dev-0.0.4/core/di/injector.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.3/core/rest/app_controller.py` & `core-braincube-dev-0.0.4/core/rest/app_controller.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.3/core/rest/app_module.py` & `core-braincube-dev-0.0.4/core/rest/app_module.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.3/core/rest/data.py` & `core-braincube-dev-0.0.4/core/rest/data.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.3/core/utils/convert.py` & `core-braincube-dev-0.0.4/core/utils/convert.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.3/core/utils/data.py` & `core-braincube-dev-0.0.4/core/utils/data.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.3/core_braincube_dev.egg-info/PKG-INFO` & `core-braincube-dev-0.0.4/core_braincube_dev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: core-braincube-dev
-Version: 0.0.3
+Version: 0.0.4
 Summary: Microframework for python aws lambdas
 Home-page: https://bitbucket.org/braincube-common/core-aws.git
 Author: Braincube
 Author-email: spresvias@braincube.gr
 License: MIT
 Keywords: python,amazon,aws,lambda,routing,dal,injection
 Classifier: Intended Audience :: Developers
```

### Comparing `core-braincube-dev-0.0.3/core_braincube_dev.egg-info/SOURCES.txt` & `core-braincube-dev-0.0.4/core_braincube_dev.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 LICENSE
-README.rst
+README.md
 setup.cfg
 setup.py
 core/__init__.py
 core/dal/__init__.py
 core/dal/data.py
 core/dal/database_errors.py
 core/dal/postgres_connection.py
```

### Comparing `core-braincube-dev-0.0.3/setup.cfg` & `core-braincube-dev-0.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = core-braincube-dev
-version = 0.0.3
+version = 0.0.4
 url = https://bitbucket.org/braincube-common/core-aws.git
 author = Braincube
 author_email = spresvias@braincube.gr
 license = MIT
 license_files = LICENSE
 description = Microframework for python aws lambdas
 classifiers =
```

