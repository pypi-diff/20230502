# Comparing `tmp/merqube_client_lib-0.2.1.tar.gz` & `tmp/merqube_client_lib-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "merqube_client_lib-0.2.1.tar", max compression
+gzip compressed data, was "merqube_client_lib-0.2.2.tar", max compression
```

## Comparing `merqube_client_lib-0.2.1.tar` & `merqube_client_lib-0.2.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2023-05-02 19:34:55.877713 merqube_client_lib-0.2.1/LICENSE
--rw-r--r--   0        0        0        0 2023-05-02 19:34:55.877713 merqube_client_lib-0.2.1/merqube_client_lib/__init__.py
--rw-r--r--   0        0        0      207 2023-05-02 19:34:55.877713 merqube_client_lib-0.2.1/merqube_client_lib/constants.py
--rw-r--r--   0        0        0      482 2023-05-02 19:34:55.877713 merqube_client_lib-0.2.1/merqube_client_lib/exceptions.py
--rw-r--r--   0        0        0    10949 2023-05-02 19:34:55.877713 merqube_client_lib-0.2.1/merqube_client_lib/session.py
--rw-r--r--   0        0        0      351 2023-05-02 19:34:55.877713 merqube_client_lib-0.2.1/merqube_client_lib/types.py
--rw-r--r--   0        0        0     1567 2023-05-02 19:34:55.877713 merqube_client_lib-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      541 1970-01-01 00:00:00.000000 merqube_client_lib-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-02 19:46:00.759556 merqube_client_lib-0.2.2/LICENSE
+-rw-r--r--   0        0        0        0 2023-05-02 19:46:00.759556 merqube_client_lib-0.2.2/merqube_client_lib/__init__.py
+-rw-r--r--   0        0        0      207 2023-05-02 19:46:00.759556 merqube_client_lib-0.2.2/merqube_client_lib/constants.py
+-rw-r--r--   0        0        0      482 2023-05-02 19:46:00.759556 merqube_client_lib-0.2.2/merqube_client_lib/exceptions.py
+-rw-r--r--   0        0        0    10941 2023-05-02 19:46:00.759556 merqube_client_lib-0.2.2/merqube_client_lib/session.py
+-rw-r--r--   0        0        0      351 2023-05-02 19:46:00.759556 merqube_client_lib-0.2.2/merqube_client_lib/types.py
+-rw-r--r--   0        0        0     1545 2023-05-02 19:46:00.759556 merqube_client_lib-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      520 1970-01-01 00:00:00.000000 merqube_client_lib-0.2.2/PKG-INFO
```

### Comparing `merqube_client_lib-0.2.1/LICENSE` & `merqube_client_lib-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.2.1/merqube_client_lib/session.py` & `merqube_client_lib-0.2.2/merqube_client_lib/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,15 +198,15 @@
     def delete(self, url: str, **kwargs: Any) -> Response:
         """
         requests.Session like http DELETE method
         """
         return self.request(httpm.DELETE, url, **kwargs)
 
 
-# Public methods
+# Public
 
 
 class MerqubeAPISession(_BaseAPISession):
     """
     API Session tailored to MerQube's API indexapi and its errors
     The session is initialized with an API Key, and that API Key is passed in the Authorization header for all requests
     """
```

### Comparing `merqube_client_lib-0.2.1/pyproject.toml` & `merqube_client_lib-0.2.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 [tool.poetry]
 name = "merqube-client-lib"
-version = "0.2.1"
+version = "0.2.2"
 description = "MerQube IndexAPI + SecAPI client library"
 authors = ["Merqube"]
 
 [tool.poetry.dependencies]
 python = "^3.10,<4.0"
 requests = "*"
 pydantic = {"version" = "^1.10.5"}
-numpy = "1.24.1"
-pandas = "1.5.2"
-Flask = "2.2.2"
-Flask-Cors = "3.0.10"
-cachetools = "5.2.1"
+pandas = "^1.3.0"
+Flask = "~2"
+Flask-Cors = "~3"
+cachetools = "^5.2.0"
 
 [tool.poetry.dev-dependencies]
 coverage =  {version="*"}
 pdbpp = {version="*"}
 pytest = {version="*"}
 pytest-cov =  {version="*"}
 pytest-timeout =  {version="*"}
```

### Comparing `merqube_client_lib-0.2.1/PKG-INFO` & `merqube_client_lib-0.2.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: merqube-client-lib
-Version: 0.2.1
+Version: 0.2.2
 Summary: MerQube IndexAPI + SecAPI client library
 Author: Merqube
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: Flask (==2.2.2)
-Requires-Dist: Flask-Cors (==3.0.10)
-Requires-Dist: cachetools (==5.2.1)
-Requires-Dist: numpy (==1.24.1)
-Requires-Dist: pandas (==1.5.2)
+Requires-Dist: Flask (>=2,<3)
+Requires-Dist: Flask-Cors (>=3,<4)
+Requires-Dist: cachetools (>=5.2.0,<6.0.0)
+Requires-Dist: pandas (>=1.3.0,<2.0.0)
 Requires-Dist: pydantic (>=1.10.5,<2.0.0)
 Requires-Dist: requests
```

