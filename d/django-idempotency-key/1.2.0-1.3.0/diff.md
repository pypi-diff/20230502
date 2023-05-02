# Comparing `tmp/django-idempotency-key-1.2.0.tar.gz` & `tmp/django_idempotency_key-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-idempotency-key-1.2.0.tar", max compression
+gzip compressed data, was "django_idempotency_key-1.3.0.tar", max compression
```

## Comparing `django-idempotency-key-1.2.0.tar` & `django_idempotency_key-1.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1068 2022-07-19 10:48:21.661345 django-idempotency-key-1.2.0/LICENSE
--rw-r--r--   0        0        0        0 2022-07-19 10:48:21.661345 django-idempotency-key-1.2.0/idempotency_key/__init__.py
--rwxr-xr-x   0        0        0     2294 2022-07-19 10:48:21.661345 django-idempotency-key-1.2.0/idempotency_key/decorators.py
--rw-r--r--   0        0        0      670 2022-07-19 10:48:21.661345 django-idempotency-key-1.2.0/idempotency_key/encoders.py
--rw-r--r--   0        0        0      831 2022-07-19 10:48:21.661345 django-idempotency-key-1.2.0/idempotency_key/exceptions.py
--rw-r--r--   0        0        0        0 2022-07-19 10:48:21.661345 django-idempotency-key-1.2.0/idempotency_key/locks/__init__.py
--rw-r--r--   0        0        0      766 2022-07-19 10:48:21.661345 django-idempotency-key-1.2.0/idempotency_key/locks/basic.py
--rw-r--r--   0        0        0      978 2022-07-19 10:48:21.661345 django-idempotency-key-1.2.0/idempotency_key/locks/redis.py
--rw-r--r--   0        0        0    10467 2022-07-19 10:48:21.661345 django-idempotency-key-1.2.0/idempotency_key/middleware.py
--rw-r--r--   0        0        0     1626 2022-07-19 10:48:21.661345 django-idempotency-key-1.2.0/idempotency_key/status.py
--rw-r--r--   0        0        0     3031 2022-07-19 10:48:21.661345 django-idempotency-key-1.2.0/idempotency_key/storage.py
--rw-r--r--   0        0        0     2366 2022-07-19 10:48:21.661345 django-idempotency-key-1.2.0/idempotency_key/utils.py
--rw-r--r--   0        0        0      836 2022-07-19 10:48:23.921326 django-idempotency-key-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      719 2022-07-19 10:48:25.326146 django-idempotency-key-1.2.0/setup.py
--rw-r--r--   0        0        0      614 2022-07-19 10:48:25.326425 django-idempotency-key-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-05-02 12:00:03.444022 django_idempotency_key-1.3.0/LICENSE
+-rw-r--r--   0        0        0     7642 2023-05-02 12:00:03.444022 django_idempotency_key-1.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-02 12:00:03.444022 django_idempotency_key-1.3.0/idempotency_key/__init__.py
+-rwxr-xr-x   0        0        0     2346 2023-05-02 12:00:03.444022 django_idempotency_key-1.3.0/idempotency_key/decorators.py
+-rw-r--r--   0        0        0      857 2023-05-02 12:00:03.444022 django_idempotency_key-1.3.0/idempotency_key/encoders.py
+-rw-r--r--   0        0        0      831 2023-05-02 12:00:03.444022 django_idempotency_key-1.3.0/idempotency_key/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-02 12:00:03.444022 django_idempotency_key-1.3.0/idempotency_key/locks/__init__.py
+-rw-r--r--   0        0        0      766 2023-05-02 12:00:03.444022 django_idempotency_key-1.3.0/idempotency_key/locks/basic.py
+-rw-r--r--   0        0        0      978 2023-05-02 12:00:03.444022 django_idempotency_key-1.3.0/idempotency_key/locks/redis.py
+-rw-r--r--   0        0        0    10467 2023-05-02 12:00:03.444022 django_idempotency_key-1.3.0/idempotency_key/middleware.py
+-rw-r--r--   0        0        0     1626 2023-05-02 12:00:03.444022 django_idempotency_key-1.3.0/idempotency_key/status.py
+-rw-r--r--   0        0        0     3051 2023-05-02 12:00:03.444022 django_idempotency_key-1.3.0/idempotency_key/storage.py
+-rw-r--r--   0        0        0     2366 2023-05-02 12:00:03.444022 django_idempotency_key-1.3.0/idempotency_key/utils.py
+-rw-r--r--   0        0        0      868 2023-05-02 12:00:03.448022 django_idempotency_key-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     8482 1970-01-01 00:00:00.000000 django_idempotency_key-1.3.0/PKG-INFO
```

### Comparing `django-idempotency-key-1.2.0/LICENSE` & `django_idempotency_key-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-idempotency-key-1.2.0/idempotency_key/decorators.py` & `django_idempotency_key-1.3.0/idempotency_key/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 from functools import wraps
 
 from idempotency_key import utils
 
 # NOTE:
-# The following decorators must be specified BEFORE the @api_view decorator or the function will not be marked
-# correctly.
+# The following decorators must be specified BEFORE the @api_view decorator or the
+# function will not be marked correctly.
 #
 # i.e:
 #
 # @idempotency_key
 # @api_view(['POST'])
 # def my_view_func()
 #   ...
 
 
 def idempotency_key(*args, optional=False, cache_name=None):
     """
-    Allows an optional cache name to be specified so that different cache settings can be used on a per-view function
-    basis.
-    :param args: optional arguments. This can contain the view function object if cache_name is not specified
+    Allows an optional cache name to be specified so that different cache settings can
+    be used on a per-view function basis.
+    :param args: optional arguments. This can contain the view function object if
+                 cache_name is not specified
     :param optional: Mark idempotency key header as optional
-    :param cache_name: The name of the cache to use from the settings file under CACHES={...}
+    :param cache_name: The name of the cache to use from the settings file under
+                       CACHES={...}
     :return: wrapped function
     """
 
     def _idempotency_key(view_func):
         """
-        Mark a view function as requiring idempotency key protection but the view should control the response.
+        Mark a view function as requiring idempotency key protection but the view
+        should control the response.
         """
 
         @wraps(view_func)
         def wrapped_view(*args, **kwargs):
             return view_func(*args, **kwargs)
 
         wrapped_view.idempotency_key = True
@@ -38,16 +41,16 @@
 
         if cache_name:
             wrapped_view.idempotency_key_cache_name = cache_name
             utils.get_storage_class().validate_storage(cache_name)
 
         return wrapped_view
 
-    # if there is an argument passed and it is a callable then this will be the view function object so pass it to
-    # the wrapper
+    # if there is an argument passed and it is a callable then this will be the view
+    # function object so pass it to the wrapper
     if len(args) > 0 and callable(args[0]):
         return _idempotency_key(args[0])
 
     # otherwise just return the wrapper object
     return _idempotency_key
 
 
@@ -61,15 +64,16 @@
 
     wrapped_view.idempotency_key_exempt = True
     return wraps(view_func)(wrapped_view)
 
 
 def idempotency_key_manual(view_func):
     """
-    Mark a view function as requiring idempotency key protection but the view should control the response.
+    Mark a view function as requiring idempotency key protection but the view should
+    control the response.
     """
 
     def wrapped_view(*args, **kwargs):
         return view_func(*args, **kwargs)
 
     wrapped_view.idempotency_key_manual = True
     return wraps(view_func)(wrapped_view)
```

### Comparing `django-idempotency-key-1.2.0/idempotency_key/encoders.py` & `django_idempotency_key-1.3.0/idempotency_key/encoders.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 import abc
 import hashlib
 
+from django.http.request import HttpRequest
+
 from idempotency_key.exceptions import MissingIdempotencyKeyError
 
 
 class IdempotencyKeyEncoder(object):
     @abc.abstractmethod
     def encode_key(self, request, key):
         raise NotImplementedError
 
 
 class BasicKeyEncoder(IdempotencyKeyEncoder):
-    def encode_key(self, request, key):
+    def encode_key(self, request: HttpRequest, key):
         if key is None:
             raise MissingIdempotencyKeyError()
         # Basic method for generating an encoded key
         m = hashlib.sha256()
         m.update(key.encode("UTF-8"))
         m.update(request.path_info.encode("UTF-8"))
         m.update(request.method.encode("UTF-8"))
         m.update(request.body)
+        if request.META.get("HTTP_AUTHORIZATION"):
+            m.update(request.META.get("HTTP_AUTHORIZATION").encode("UTF-8"))
+
         return m.hexdigest()
```

### Comparing `django-idempotency-key-1.2.0/idempotency_key/exceptions.py` & `django_idempotency_key-1.3.0/idempotency_key/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-idempotency-key-1.2.0/idempotency_key/locks/basic.py` & `django_idempotency_key-1.3.0/idempotency_key/locks/basic.py`

 * *Files identical despite different names*

### Comparing `django-idempotency-key-1.2.0/idempotency_key/locks/redis.py` & `django_idempotency_key-1.3.0/idempotency_key/locks/redis.py`

 * *Files identical despite different names*

### Comparing `django-idempotency-key-1.2.0/idempotency_key/middleware.py` & `django_idempotency_key-1.3.0/idempotency_key/middleware.py`

 * *Files identical despite different names*

### Comparing `django-idempotency-key-1.2.0/idempotency_key/status.py` & `django_idempotency_key-1.3.0/idempotency_key/status.py`

 * *Files identical despite different names*

### Comparing `django-idempotency-key-1.2.0/idempotency_key/storage.py` & `django_idempotency_key-1.3.0/idempotency_key/storage.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,16 +28,17 @@
         """
         raise NotImplementedError
 
     @staticmethod
     @abc.abstractmethod
     def validate_storage(name: str):
         """
-        Validate that the storage name exists. If the class is using django `CACHES` setting then this function ensures
-        that the cache is setup correctly in the settings file and will cause a failure at startup if it is not.
+        Validate that the storage name exists. If the class is using django `CACHES`
+        setting then this function ensures that the cache is setup correctly in the
+        settings file and will cause a failure at startup if it is not.
         This function should raise an exception if the storage name cannot be validated.
         :param name: The name of the storage.
         """
         raise NotImplementedError
 
 
 class MemoryKeyStorage(IdempotencyKeyStorage):
@@ -69,10 +70,11 @@
             str_response = caches[cache_name].get(encoded_key)
             return True, pickle.loads(str_response)
 
         return False, None
 
     @staticmethod
     def validate_storage(name: str):
-        # Check that the cache exists. If the cache is not found then an InvalidCacheBackendError is raised.
-        # Not that there is no get function on the caches object so we cannot perform a normal check.
+        # Check that the cache exists. If the cache is not found then an
+        # InvalidCacheBackendError is raised. Note that there is no get function on the
+        # caches object, so we cannot perform a normal check.
         caches[name]
```

### Comparing `django-idempotency-key-1.2.0/idempotency_key/utils.py` & `django_idempotency_key-1.3.0/idempotency_key/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 def get_lock_class():
     return module_loading.import_string(
         get_lock_settings().get("CLASS", "idempotency_key.locks.basic.ThreadLock")
     )
 
 
 def get_lock_location():
-    return get_lock_settings().get("LOCATION", "Redis://localhost:6379/1")
+    return get_lock_settings().get("LOCATION", "redis://localhost:6379/1")
 
 
 def get_lock_timeout():
     return get_lock_settings().get("TIMEOUT", 0.1)  # default to 100ms
 
 
 def get_lock_enable():
```

