# Comparing `tmp/resotoclient-1.3.0.tar.gz` & `tmp/resotoclient-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotoclient-1.3.0.tar", max compression
+gzip compressed data, was "resotoclient-1.3.1.tar", max compression
```

## Comparing `resotoclient-1.3.0.tar` & `resotoclient-1.3.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11357 2023-05-02 07:53:32.413548 resotoclient-1.3.0/LICENSE
--rw-r--r--   0        0        0     1243 2023-05-02 07:53:32.413548 resotoclient-1.3.0/README.md
--rw-r--r--   0        0        0     2082 2023-05-02 07:53:32.413548 resotoclient-1.3.0/pyproject.toml
--rw-r--r--   0        0        0    20448 2023-05-02 07:53:32.413548 resotoclient-1.3.0/resotoclient/__init__.py
--rw-r--r--   0        0        0    23011 2023-05-02 07:53:32.413548 resotoclient-1.3.0/resotoclient/async_client.py
--rw-r--r--   0        0        0     6219 2023-05-02 07:53:32.413548 resotoclient-1.3.0/resotoclient/ca.py
--rw-r--r--   0        0        0     2813 2023-05-02 07:53:32.413548 resotoclient-1.3.0/resotoclient/http_client/__init__.py
--rw-r--r--   0        0        0    10672 2023-05-02 07:53:32.413548 resotoclient-1.3.0/resotoclient/http_client/aiohttp_client.py
--rw-r--r--   0        0        0     1282 2023-05-02 07:53:32.413548 resotoclient-1.3.0/resotoclient/http_client/event_loop_thread.py
--rw-r--r--   0        0        0      693 2023-05-02 07:53:32.413548 resotoclient-1.3.0/resotoclient/json_utils.py
--rw-r--r--   0        0        0     3431 2023-05-02 07:53:32.413548 resotoclient-1.3.0/resotoclient/jwt_utils.py
--rw-r--r--   0        0        0     2283 2023-05-02 07:53:32.413548 resotoclient-1.3.0/resotoclient/models.py
--rw-r--r--   0        0        0     2721 1970-01-01 00:00:00.000000 resotoclient-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-02 12:40:14.056864 resotoclient-1.3.1/LICENSE
+-rw-r--r--   0        0        0     1243 2023-05-02 12:40:14.056864 resotoclient-1.3.1/README.md
+-rw-r--r--   0        0        0     2082 2023-05-02 12:40:14.056864 resotoclient-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0    20455 2023-05-02 12:40:14.056864 resotoclient-1.3.1/resotoclient/__init__.py
+-rw-r--r--   0        0        0    23018 2023-05-02 12:40:14.056864 resotoclient-1.3.1/resotoclient/async_client.py
+-rw-r--r--   0        0        0     6219 2023-05-02 12:40:14.056864 resotoclient-1.3.1/resotoclient/ca.py
+-rw-r--r--   0        0        0     2813 2023-05-02 12:40:14.056864 resotoclient-1.3.1/resotoclient/http_client/__init__.py
+-rw-r--r--   0        0        0    10672 2023-05-02 12:40:14.056864 resotoclient-1.3.1/resotoclient/http_client/aiohttp_client.py
+-rw-r--r--   0        0        0     1282 2023-05-02 12:40:14.056864 resotoclient-1.3.1/resotoclient/http_client/event_loop_thread.py
+-rw-r--r--   0        0        0      693 2023-05-02 12:40:14.056864 resotoclient-1.3.1/resotoclient/json_utils.py
+-rw-r--r--   0        0        0     3431 2023-05-02 12:40:14.056864 resotoclient-1.3.1/resotoclient/jwt_utils.py
+-rw-r--r--   0        0        0     2283 2023-05-02 12:40:14.056864 resotoclient-1.3.1/resotoclient/models.py
+-rw-r--r--   0        0        0     2721 1970-01-01 00:00:00.000000 resotoclient-1.3.1/PKG-INFO
```

### Comparing `resotoclient-1.3.0/LICENSE` & `resotoclient-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `resotoclient-1.3.0/README.md` & `resotoclient-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `resotoclient-1.3.0/pyproject.toml` & `resotoclient-1.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "resotoclient"
-version = "1.3.0"
+version = "1.3.1"
 description = "Resoto Python client library"
 authors = ["Some Engineering Inc."]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/someengineering/resotoclient-python"
 repository = "https://github.com/someengineering/resotoclient-python"
 packages = [
```

### Comparing `resotoclient-1.3.0/resotoclient/__init__.py` & `resotoclient-1.3.1/resotoclient/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
     The ApiClient interacts with a running core instance via the REST interface.
     """
 
     def __init__(
         self,
         url: str,
         *,
-        psk: Optional[str],
+        psk: Optional[str] = None,
         additional_headers: Optional[Dict[str, str]] = None,
         custom_ca_cert_path: Optional[str] = None,
         verify: bool = True,
         renew_before: timedelta = timedelta(days=1),
     ):
         self.resotocore_url = url
         self.psk = psk
```

### Comparing `resotoclient-1.3.0/resotoclient/async_client.py` & `resotoclient-1.3.1/resotoclient/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     The ApiClient interacts with a running core instance via the REST interface.
     """
 
     def __init__(
         self,
         url: str,
         *,
-        psk: Optional[str],
+        psk: Optional[str] = None,
         additional_headers: Optional[Dict[str, str]] = None,
         custom_ca_cert_path: Optional[str] = None,
         verify: bool = True,
         renew_before: timedelta = timedelta(days=1),
         loop: Optional[AbstractEventLoop] = None,
     ):
         """
```

### Comparing `resotoclient-1.3.0/resotoclient/ca.py` & `resotoclient-1.3.1/resotoclient/ca.py`

 * *Files identical despite different names*

### Comparing `resotoclient-1.3.0/resotoclient/http_client/__init__.py` & `resotoclient-1.3.1/resotoclient/http_client/__init__.py`

 * *Files identical despite different names*

### Comparing `resotoclient-1.3.0/resotoclient/http_client/aiohttp_client.py` & `resotoclient-1.3.1/resotoclient/http_client/aiohttp_client.py`

 * *Files identical despite different names*

### Comparing `resotoclient-1.3.0/resotoclient/http_client/event_loop_thread.py` & `resotoclient-1.3.1/resotoclient/http_client/event_loop_thread.py`

 * *Files identical despite different names*

### Comparing `resotoclient-1.3.0/resotoclient/json_utils.py` & `resotoclient-1.3.1/resotoclient/json_utils.py`

 * *Files identical despite different names*

### Comparing `resotoclient-1.3.0/resotoclient/jwt_utils.py` & `resotoclient-1.3.1/resotoclient/jwt_utils.py`

 * *Files identical despite different names*

### Comparing `resotoclient-1.3.0/resotoclient/models.py` & `resotoclient-1.3.1/resotoclient/models.py`

 * *Files identical despite different names*

### Comparing `resotoclient-1.3.0/PKG-INFO` & `resotoclient-1.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotoclient
-Version: 1.3.0
+Version: 1.3.1
 Summary: Resoto Python client library
 Home-page: https://github.com/someengineering/resotoclient-python
 License: Apache-2.0
 Author: Some Engineering Inc.
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

