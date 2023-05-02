# Comparing `tmp/microgue-2.0.1.tar.gz` & `tmp/microgue-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/microgue-2.0.1.tar", last modified: Mon May  1 20:12:31 2023, max compression
+gzip compressed data, was "dist/microgue-2.0.2.tar", last modified: Tue May  2 01:55:19 2023, max compression
```

## Comparing `microgue-2.0.1.tar` & `microgue-2.0.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-01 20:12:31.000000 microgue-2.0.1/
--rw-r--r--   0 mhudelso   (501) staff       (20)     3060 2023-05-01 20:12:31.000000 microgue-2.0.1/PKG-INFO
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-01 20:12:31.000000 microgue-2.0.1/microgue/
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-01 20:12:31.000000 microgue-2.0.1/microgue/storages/
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.1/microgue/storages/__init__.py
--rw-r--r--   0 mhudelso   (501) staff       (20)     3324 2023-04-30 02:26:31.000000 microgue-2.0.1/microgue/storages/abstract_storage.py
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-01 20:12:31.000000 microgue-2.0.1/microgue/loggers/
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.1/microgue/loggers/__init__.py
--rw-r--r--   0 mhudelso   (501) staff       (20)     1369 2023-05-01 20:10:53.000000 microgue-2.0.1/microgue/loggers/logger.py
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-01 20:12:31.000000 microgue-2.0.1/microgue/security/
--rw-r--r--   0 mhudelso   (501) staff       (20)      334 2023-04-30 02:18:57.000000 microgue-2.0.1/microgue/security/generic.py
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.1/microgue/security/__init__.py
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-01 20:12:31.000000 microgue-2.0.1/microgue/secrets/
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.1/microgue/secrets/__init__.py
--rw-r--r--   0 mhudelso   (501) staff       (20)      998 2023-04-30 02:26:31.000000 microgue-2.0.1/microgue/secrets/secrets.py
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-01 20:12:31.000000 microgue-2.0.1/microgue/constants/
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.1/microgue/constants/__init__.py
--rw-r--r--   0 mhudelso   (501) staff       (20)      378 2022-09-21 19:29:50.000000 microgue-2.0.1/microgue/constants/error_constants.py
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.1/microgue/__init__.py
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-01 20:12:31.000000 microgue-2.0.1/microgue/objects/
--rw-r--r--   0 mhudelso   (501) staff       (20)     8626 2023-04-29 23:27:06.000000 microgue-2.0.1/microgue/objects/abstract_model_object.py
--rw-r--r--   0 mhudelso   (501) staff       (20)     2374 2022-09-23 00:54:22.000000 microgue-2.0.1/microgue/objects/object.py
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.1/microgue/objects/__init__.py
--rw-r--r--   0 mhudelso   (501) staff       (20)     1459 2023-04-30 02:26:31.000000 microgue-2.0.1/microgue/objects/abstract_expiring_model_object.py
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-01 20:12:31.000000 microgue-2.0.1/microgue/models/
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.1/microgue/models/__init__.py
--rw-r--r--   0 mhudelso   (501) staff       (20)    10541 2023-04-30 02:26:31.000000 microgue-2.0.1/microgue/models/abstract_model.py
--rw-r--r--   0 mhudelso   (501) staff       (20)     2682 2022-12-09 19:59:12.000000 microgue-2.0.1/microgue/utils.py
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-01 20:12:31.000000 microgue-2.0.1/microgue/queues/
--rw-r--r--   0 mhudelso   (501) staff       (20)     2864 2023-04-30 17:37:32.000000 microgue-2.0.1/microgue/queues/abstract_queue.py
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.1/microgue/queues/__init__.py
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-01 20:12:31.000000 microgue-2.0.1/microgue/events/
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-03-09 20:40:18.000000 microgue-2.0.1/microgue/events/__init__.py
--rw-r--r--   0 mhudelso   (501) staff       (20)     1420 2023-04-30 02:26:31.000000 microgue-2.0.1/microgue/events/abstract_event_bus.py
--rw-r--r--   0 mhudelso   (501) staff       (20)     5204 2023-05-01 13:49:41.000000 microgue-2.0.1/microgue/abstract_app.py
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-01 20:12:31.000000 microgue-2.0.1/microgue/services/
--rw-r--r--   0 mhudelso   (501) staff       (20)     3687 2023-05-01 14:01:58.000000 microgue-2.0.1/microgue/services/service.py
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.1/microgue/services/__init__.py
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-01 20:12:31.000000 microgue-2.0.1/microgue/caches/
--rw-r--r--   0 mhudelso   (501) staff       (20)     3015 2023-04-30 02:26:31.000000 microgue-2.0.1/microgue/caches/abstract_cache.py
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.1/microgue/caches/__init__.py
--rw-r--r--   0 mhudelso   (501) staff       (20)     1907 2022-09-27 19:27:36.000000 microgue-2.0.1/README.md
--rw-r--r--   0 mhudelso   (501) staff       (20)      640 2023-05-01 20:11:57.000000 microgue-2.0.1/setup.py
--rw-r--r--   0 mhudelso   (501) staff       (20)       38 2023-05-01 20:12:31.000000 microgue-2.0.1/setup.cfg
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-01 20:12:31.000000 microgue-2.0.1/microgue.egg-info/
--rw-r--r--   0 mhudelso   (501) staff       (20)     3060 2023-05-01 20:12:31.000000 microgue-2.0.1/microgue.egg-info/PKG-INFO
--rw-r--r--   0 mhudelso   (501) staff       (20)     1010 2023-05-01 20:12:31.000000 microgue-2.0.1/microgue.egg-info/SOURCES.txt
--rw-r--r--   0 mhudelso   (501) staff       (20)       42 2023-05-01 20:12:31.000000 microgue-2.0.1/microgue.egg-info/requires.txt
--rw-r--r--   0 mhudelso   (501) staff       (20)        9 2023-05-01 20:12:31.000000 microgue-2.0.1/microgue.egg-info/top_level.txt
--rw-r--r--   0 mhudelso   (501) staff       (20)        1 2023-05-01 20:12:31.000000 microgue-2.0.1/microgue.egg-info/dependency_links.txt
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-02 01:55:19.000000 microgue-2.0.2/
+-rw-r--r--   0 mhudelso   (501) staff       (20)     3060 2023-05-02 01:55:19.000000 microgue-2.0.2/PKG-INFO
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-02 01:55:19.000000 microgue-2.0.2/microgue/
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-02 01:55:19.000000 microgue-2.0.2/microgue/storages/
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.2/microgue/storages/__init__.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)     3348 2023-05-02 01:36:41.000000 microgue-2.0.2/microgue/storages/abstract_storage.py
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-02 01:55:19.000000 microgue-2.0.2/microgue/loggers/
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.2/microgue/loggers/__init__.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)     1369 2023-05-01 20:10:53.000000 microgue-2.0.2/microgue/loggers/logger.py
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-02 01:55:19.000000 microgue-2.0.2/microgue/security/
+-rw-r--r--   0 mhudelso   (501) staff       (20)      334 2023-04-30 02:18:57.000000 microgue-2.0.2/microgue/security/generic.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.2/microgue/security/__init__.py
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-02 01:55:19.000000 microgue-2.0.2/microgue/secrets/
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.2/microgue/secrets/__init__.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)     1014 2023-05-02 01:36:25.000000 microgue-2.0.2/microgue/secrets/secrets.py
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-02 01:55:19.000000 microgue-2.0.2/microgue/constants/
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.2/microgue/constants/__init__.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)      378 2022-09-21 19:29:50.000000 microgue-2.0.2/microgue/constants/error_constants.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.2/microgue/__init__.py
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-02 01:55:19.000000 microgue-2.0.2/microgue/objects/
+-rw-r--r--   0 mhudelso   (501) staff       (20)     8697 2023-05-02 01:53:58.000000 microgue-2.0.2/microgue/objects/abstract_model_object.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)     2374 2022-09-23 00:54:22.000000 microgue-2.0.2/microgue/objects/object.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.2/microgue/objects/__init__.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)     1483 2023-05-02 01:54:14.000000 microgue-2.0.2/microgue/objects/abstract_expiring_model_object.py
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-02 01:55:19.000000 microgue-2.0.2/microgue/models/
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.2/microgue/models/__init__.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)    10589 2023-05-02 01:36:25.000000 microgue-2.0.2/microgue/models/abstract_model.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)     2670 2023-05-02 01:51:10.000000 microgue-2.0.2/microgue/utils.py
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-02 01:55:19.000000 microgue-2.0.2/microgue/queues/
+-rw-r--r--   0 mhudelso   (501) staff       (20)     2887 2023-05-02 01:49:56.000000 microgue-2.0.2/microgue/queues/abstract_queue.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.2/microgue/queues/__init__.py
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-02 01:55:19.000000 microgue-2.0.2/microgue/events/
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-03-09 20:40:18.000000 microgue-2.0.2/microgue/events/__init__.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)     1420 2023-04-30 02:26:31.000000 microgue-2.0.2/microgue/events/abstract_event_bus.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)     5220 2023-05-02 01:51:02.000000 microgue-2.0.2/microgue/abstract_app.py
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-02 01:55:19.000000 microgue-2.0.2/microgue/services/
+-rw-r--r--   0 mhudelso   (501) staff       (20)     3696 2023-05-02 01:52:15.000000 microgue-2.0.2/microgue/services/service.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.2/microgue/services/__init__.py
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-02 01:55:19.000000 microgue-2.0.2/microgue/caches/
+-rw-r--r--   0 mhudelso   (501) staff       (20)     3039 2023-05-02 01:51:21.000000 microgue-2.0.2/microgue/caches/abstract_cache.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.2/microgue/caches/__init__.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)     1907 2022-09-27 19:27:36.000000 microgue-2.0.2/README.md
+-rw-r--r--   0 mhudelso   (501) staff       (20)      640 2023-05-02 01:55:01.000000 microgue-2.0.2/setup.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)       38 2023-05-02 01:55:19.000000 microgue-2.0.2/setup.cfg
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-02 01:55:19.000000 microgue-2.0.2/microgue.egg-info/
+-rw-r--r--   0 mhudelso   (501) staff       (20)     3060 2023-05-02 01:55:19.000000 microgue-2.0.2/microgue.egg-info/PKG-INFO
+-rw-r--r--   0 mhudelso   (501) staff       (20)     1010 2023-05-02 01:55:19.000000 microgue-2.0.2/microgue.egg-info/SOURCES.txt
+-rw-r--r--   0 mhudelso   (501) staff       (20)       42 2023-05-02 01:55:19.000000 microgue-2.0.2/microgue.egg-info/requires.txt
+-rw-r--r--   0 mhudelso   (501) staff       (20)        9 2023-05-02 01:55:19.000000 microgue-2.0.2/microgue.egg-info/top_level.txt
+-rw-r--r--   0 mhudelso   (501) staff       (20)        1 2023-05-02 01:55:19.000000 microgue-2.0.2/microgue.egg-info/dependency_links.txt
```

### Comparing `microgue-2.0.1/PKG-INFO` & `microgue-2.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microgue
-Version: 2.0.1
+Version: 2.0.2
 Summary: This project contains bootstrap code to speed up the development of AWS based microservices
 Home-page: UNKNOWN
 Author: Michael Hudelson
 Author-email: michaelhudelson@gmail.com
 License: MIT
 Description: # AWS Microservice Bootstrap Code
```

### Comparing `microgue-2.0.1/microgue/storages/abstract_storage.py` & `microgue-2.0.2/microgue/storages/abstract_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import uuid
 from pathlib import Path
 from ..loggers.logger import Logger
 
 logger = Logger()
 
 
-class DownloadFailed(Exception): pass
-class UploadFailed(Exception): pass
-class DeleteFailed(Exception): pass
+class DownloadFailed(Exception): pass  # noqa
+class UploadFailed(Exception): pass  # noqa
+class DeleteFailed(Exception): pass  # noqa
 
 
 class AbstractStorage:
     class File:
         def __init__(self, remote_path=None, local_path=None, url=None):
             self.remote_path = remote_path
             self.local_path = local_path
```

### Comparing `microgue-2.0.1/microgue/loggers/logger.py` & `microgue-2.0.2/microgue/loggers/logger.py`

 * *Files identical despite different names*

### Comparing `microgue-2.0.1/microgue/secrets/secrets.py` & `microgue-2.0.2/microgue/secrets/secrets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import boto3
 import json
 from ..loggers.logger import Logger
 
 logger = Logger()
 
 
-class GetSecretFailed(Exception): pass
-class SecretsConnectionFailed(Exception): pass
+class GetSecretFailed(Exception): pass  # noqa
+class SecretsConnectionFailed(Exception): pass  # noqa
 
 
 class Secrets:
     secrets = None
     __instance = None
 
     def __new__(cls, *args, **kwargs):
```

### Comparing `microgue-2.0.1/microgue/objects/abstract_model_object.py` & `microgue-2.0.2/microgue/objects/abstract_model_object.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import uuid
-from ..models.abstract_model import *
-from .object import *
+from ..models.abstract_model import *  # noqa
+from .object import *  # noqa
 
 
-class RequiredAttributes(Exception): pass
-class UniqueAttributes(Exception): pass
+class RequiredAttributes(Exception): pass  # noqa
+class UniqueAttributes(Exception): pass  # noqa
 
 
-class AbstractModelObject(Object):
+class AbstractModelObject(Object):  # noqa
     """
     attributes: defined on Object
 
     hidden_attributes: defined on Object
 
     default_attributes: defines the default values to use when inserting a new object in the database
 
@@ -52,15 +52,15 @@
 
     @property
     def _sk(self):
         return self._model.sk
 
     @property
     def _sk_value(self):
-        return  self.__dict__.get(self._sk)
+        return self.__dict__.get(self._sk)
 
     @classmethod
     def get_by_unique_attribute(cls, attribute, value):
         unique_key = f"{attribute.upper()}#{value}"
         reference = cls._model.get(unique_key, "#UNIQUE")
 
         model_object = cls()
@@ -144,15 +144,15 @@
             raise e
         else:
             # remove previous unique attribute values
             if previous_state:
                 for old_attribute in insert_unique_attributes:
                     try:
                         self._model.delete(f"{old_attribute.upper()}#{previous_state.get(old_attribute)}", "#UNIQUE")
-                    except:
+                    except:  # noqa
                         pass
 
     def save(self):
         # check if the record exists
         if self._pk_value:
             try:
                 record_exists = bool(self._model.get(self._pk_value, self._sk_value))
@@ -168,15 +168,15 @@
     def delete(self):
         # check if the object has unique attributes
         if self.unique_attributes:
             try:
                 # undo all unique attributes before deleting the object
                 user = self.__class__(self._pk_value, self._sk_value)
                 user._undo_insert_unique_attributes(self.unique_attributes)
-            except:
+            except:  # noqa
                 pass
 
         # delete the object
         return self._model.delete(self._pk_value, self._sk_value)
 
     def _get_missing_required_attributes(self):
         missing_required_attributes = []
@@ -199,15 +199,15 @@
                 self._pk_value,
                 self._sk_value
             )
 
             try:
                 # attempt to insert
                 self._model.insert(unique_entry)
-            except ItemAlreadyExists:
+            except ItemAlreadyExists:  # noqa
                 # track failures
                 failures.append(attribute)
             else:
                 # track successes
                 successes.append(attribute)
 
         # undo all success if any failures occurred
@@ -226,9 +226,9 @@
 
     def _undo_insert_unique_attributes(self, unique_attributes):
         for attribute in unique_attributes:
             try:
                 delete_pk = f"{attribute.upper()}#{self.__dict__.get(attribute)}"
                 delete_sk = "#UNIQUE"
                 self._model.delete(delete_pk, delete_sk)
-            except:
+            except:  # noqa
                 pass
```

### Comparing `microgue-2.0.1/microgue/objects/object.py` & `microgue-2.0.2/microgue/objects/object.py`

 * *Files identical despite different names*

### Comparing `microgue-2.0.1/microgue/objects/abstract_expiring_model_object.py` & `microgue-2.0.2/microgue/objects/abstract_expiring_model_object.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import datetime
 import time
-from .abstract_model_object import *
+from .abstract_model_object import *  # noqa
 from ..loggers.logger import Logger
 
 logger = Logger()
 
 
-class AbstractExpiringModelObject(AbstractModelObject):
+class AbstractExpiringModelObject(AbstractModelObject):  # noqa
     expiration_seconds = 0
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         if self.expires_in and self.expires_in < int(time.mktime(datetime.datetime.utcnow().timetuple())):
             logger.debug(f"{self.__class__.__name__}.__init__ - expired", priority=2)
-            raise GetFailed("item expired")
+            raise GetFailed("item expired")  # noqa
 
     def insert(self):
         # add expires_in
         expires_in = datetime.datetime.utcnow() + datetime.timedelta(seconds=self.expiration_seconds)
         self.expires_in = int((expires_in - datetime.datetime(1970, 1, 1)).total_seconds())
         super().insert()
```

### Comparing `microgue-2.0.1/microgue/models/abstract_model.py` & `microgue-2.0.2/microgue/models/abstract_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 from boto3.dynamodb.types import Decimal
 from ..utils import mask_fields_in_data
 from ..loggers.logger import Logger
 
 logger = Logger()
 
 
-class DatabaseConnectionFailed(Exception): pass
-class DeleteFailed(Exception): pass
-class GetFailed(Exception): pass
-class ItemAlreadyExists(Exception): pass
-class MissingKey(Exception): pass
-class UpdateFailed(Exception): pass
+class DatabaseConnectionFailed(Exception): pass  # noqa
+class DeleteFailed(Exception): pass  # noqa
+class GetFailed(Exception): pass  # noqa
+class ItemAlreadyExists(Exception): pass  # noqa
+class MissingKey(Exception): pass  # noqa
+class UpdateFailed(Exception): pass  # noqa
 
 
 class AbstractModel:
     """
     database: the connection to dynamodb
     table_name: name of table in dynamodb
     pk: partion key of the table - defaulted to id
```

### Comparing `microgue-2.0.1/microgue/utils.py` & `microgue-2.0.2/microgue/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import json
-import time
 from flask import Response, request, g
 
 
 def set_authenticated(authenticated=True):
     g.authenticated = authenticated
```

### Comparing `microgue-2.0.1/microgue/queues/abstract_queue.py` & `microgue-2.0.2/microgue/queues/abstract_queue.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import boto3
 import json
 from ..loggers.logger import Logger
 
 logger = Logger()
 
 
-class QueueConnectionFailed(Exception): pass
-class DeleteFailed(Exception): pass
+class QueueConnectionFailed(Exception): pass  # noqa
+class DeleteFailed(Exception): pass  # noqa
 
 
 class AbstractQueue:
     queue = None
     queue_url = ""
 
     def __init__(self, *args, **kwargs):
@@ -57,15 +57,15 @@
         for i in range(len(response_messages)):
             try:
                 message = {
                     "id": response_messages[i]["ReceiptHandle"],
                     "message": json.loads(response_messages[i]["Body"])
                 }
                 messages.append(message)
-            except:
+            except: # noqa
                 pass
         return messages
 
     def delete(self, message):
         logger.debug(f"{self.__class__.__name__}.delete", priority=2)
         logger.debug(f"message: {message}")
```

### Comparing `microgue-2.0.1/microgue/events/abstract_event_bus.py` & `microgue-2.0.2/microgue/events/abstract_event_bus.py`

 * *Files identical despite different names*

### Comparing `microgue-2.0.1/microgue/abstract_app.py` & `microgue-2.0.2/microgue/abstract_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,24 +51,24 @@
     def before_request_handler(cls):
         # mask request header fields
         try:
             request_headers = dict(request.headers)
             for mask_request_header_field in cls.mask_request_headers_fields:
                 if mask_request_header_field in request_headers:
                     request_headers[mask_request_header_field] = "*****"
-        except:
+        except:  # noqa
             request_headers = {}
 
         # mask request data fields
         try:
             request_data = json.loads(request.data.decode("utf-8"))
             for mask_request_data_field in cls.mask_request_data_fields:
                 if mask_request_data_field in request_data:
                     request_data[mask_request_data_field] = "*****"
-        except:
+        except:  # noqa
             request_data = {}
 
         logger.debug("Request Received", priority=1)
         logger.debug(f"method: {request.method}")
         logger.debug(f"url: {request.url}")
         logger.debug(f"headers: {request_headers}")
         logger.debug(f"body: {request_data}")
```

### Comparing `microgue-2.0.1/microgue/services/service.py` & `microgue-2.0.2/microgue/services/service.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-import json
 import requests
 import traceback
 from collections import OrderedDict
 from ..constants.error_constants import ErrorConstants
 from ..utils import mask_fields_in_data
 from ..loggers.logger import Logger
 
 logger = Logger()
 
 
 class Service:
     class Request:
-        def __init__(self,
+        def __init__(
+            self,
             url="",
             parameters={},
             method="GET",
             headers={},
             cookies={},
             data={},
             files={},
@@ -72,15 +72,15 @@
 
             response_status_code = requests_response.status_code
             response_headers = dict(requests_response.headers)
             response_cookies = dict(requests_response.cookies)
 
             try:
                 response_data = requests_response.json()
-            except:
+            except:  # noqa
                 response_data = requests_response.text
 
             logger.debug(f"{self.__class__.__name__}.invoke - Response", priority=3)
             logger.debug(f"response status code: {response_status_code}")
             logger.debug(f"response headers: {response_headers}")
             logger.debug(f"response cookies: {response_cookies}")
             logger.debug(f"response data: {response_data}")
```

### Comparing `microgue-2.0.1/microgue/caches/abstract_cache.py` & `microgue-2.0.2/microgue/caches/abstract_cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import json
 import redis
 from ..loggers.logger import Logger
 
 logger = Logger()
 
 
-class CacheConnectionFailed(Exception): pass
+class CacheConnectionFailed(Exception): pass  # noqa
 
 
 class AbstractCache:
     cache = None
     host = ""
     port = ""
     prefix = ""
@@ -47,19 +47,19 @@
             prefixed_key = self._prefix_key(key)
             value = self.cache.get(prefixed_key)
             logger.debug(f"{self.__class__.__name__}.get", priority=2)
             logger.debug(f"Key: {prefixed_key}")
             logger.debug(f"Value: {value}")
             try:
                 return json.loads(value)
-            except:
+            except:  # noqa
                 pass
             try:
                 return value.decode("ascii")
-            except:
+            except:  # noqa
                 pass
             return value
 
     def set(self, key, value, ttl=None):
         if self.cache:
             value = value if type(value) is str else json.dumps(value)
             prefixed_key = self._prefix_key(key)
```

### Comparing `microgue-2.0.1/README.md` & `microgue-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `microgue-2.0.1/setup.py` & `microgue-2.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="microgue",
-    version="2.0.1",
+    version="2.0.2",
     author="Michael Hudelson",
     author_email="michaelhudelson@gmail.com",
     description="This project contains bootstrap code to speed up the development of AWS based microservices",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     packages=find_packages(),
```

### Comparing `microgue-2.0.1/microgue.egg-info/PKG-INFO` & `microgue-2.0.2/microgue.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microgue
-Version: 2.0.1
+Version: 2.0.2
 Summary: This project contains bootstrap code to speed up the development of AWS based microservices
 Home-page: UNKNOWN
 Author: Michael Hudelson
 Author-email: michaelhudelson@gmail.com
 License: MIT
 Description: # AWS Microservice Bootstrap Code
```

### Comparing `microgue-2.0.1/microgue.egg-info/SOURCES.txt` & `microgue-2.0.2/microgue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

