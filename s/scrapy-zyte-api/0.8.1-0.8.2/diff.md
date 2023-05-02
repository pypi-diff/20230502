# Comparing `tmp/scrapy-zyte-api-0.8.1.tar.gz` & `tmp/scrapy-zyte-api-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapy-zyte-api-0.8.1.tar", last modified: Thu Apr 13 06:30:08 2023, max compression
+gzip compressed data, was "scrapy-zyte-api-0.8.2.tar", last modified: Tue May  2 12:02:49 2023, max compression
```

## Comparing `scrapy-zyte-api-0.8.1.tar` & `scrapy-zyte-api-0.8.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 06:30:08.621831 scrapy-zyte-api-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-04-13 06:29:59.000000 scrapy-zyte-api-0.8.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    29333 2023-04-13 06:30:08.621831 scrapy-zyte-api-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    28567 2023-04-13 06:29:59.000000 scrapy-zyte-api-0.8.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 06:30:08.621831 scrapy-zyte-api-0.8.1/scrapy_zyte_api/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-13 06:29:59.000000 scrapy-zyte-api-0.8.1/scrapy_zyte_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-13 06:29:59.000000 scrapy-zyte-api-0.8.1/scrapy_zyte_api/_cookies.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-13 06:29:59.000000 scrapy-zyte-api-0.8.1/scrapy_zyte_api/_downloader_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)    20886 2023-04-13 06:29:59.000000 scrapy-zyte-api-0.8.1/scrapy_zyte_api/_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-04-13 06:29:59.000000 scrapy-zyte-api-0.8.1/scrapy_zyte_api/_request_fingerprinter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9226 2023-04-13 06:29:59.000000 scrapy-zyte-api-0.8.1/scrapy_zyte_api/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7500 2023-04-13 06:29:59.000000 scrapy-zyte-api-0.8.1/scrapy_zyte_api/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-13 06:29:59.000000 scrapy-zyte-api-0.8.1/scrapy_zyte_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 06:30:08.621831 scrapy-zyte-api-0.8.1/scrapy_zyte_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    29333 2023-04-13 06:30:08.000000 scrapy-zyte-api-0.8.1/scrapy_zyte_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-13 06:30:08.000000 scrapy-zyte-api-0.8.1/scrapy_zyte_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 06:30:08.000000 scrapy-zyte-api-0.8.1/scrapy_zyte_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-13 06:30:08.000000 scrapy-zyte-api-0.8.1/scrapy_zyte_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-13 06:30:08.000000 scrapy-zyte-api-0.8.1/scrapy_zyte_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-13 06:30:08.621831 scrapy-zyte-api-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-13 06:29:59.000000 scrapy-zyte-api-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:02:49.762856 scrapy-zyte-api-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-02 12:02:39.000000 scrapy-zyte-api-0.8.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    29333 2023-05-02 12:02:49.762856 scrapy-zyte-api-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    28567 2023-05-02 12:02:39.000000 scrapy-zyte-api-0.8.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:02:49.762856 scrapy-zyte-api-0.8.2/scrapy_zyte_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-02 12:02:39.000000 scrapy-zyte-api-0.8.2/scrapy_zyte_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-05-02 12:02:39.000000 scrapy-zyte-api-0.8.2/scrapy_zyte_api/_cookies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-02 12:02:39.000000 scrapy-zyte-api-0.8.2/scrapy_zyte_api/_downloader_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20886 2023-05-02 12:02:39.000000 scrapy-zyte-api-0.8.2/scrapy_zyte_api/_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-02 12:02:39.000000 scrapy-zyte-api-0.8.2/scrapy_zyte_api/_request_fingerprinter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9226 2023-05-02 12:02:39.000000 scrapy-zyte-api-0.8.2/scrapy_zyte_api/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-05-02 12:02:39.000000 scrapy-zyte-api-0.8.2/scrapy_zyte_api/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-02 12:02:39.000000 scrapy-zyte-api-0.8.2/scrapy_zyte_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:02:49.762856 scrapy-zyte-api-0.8.2/scrapy_zyte_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    29333 2023-05-02 12:02:49.000000 scrapy-zyte-api-0.8.2/scrapy_zyte_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-02 12:02:49.000000 scrapy-zyte-api-0.8.2/scrapy_zyte_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 12:02:49.000000 scrapy-zyte-api-0.8.2/scrapy_zyte_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-02 12:02:49.000000 scrapy-zyte-api-0.8.2/scrapy_zyte_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-02 12:02:49.000000 scrapy-zyte-api-0.8.2/scrapy_zyte_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-02 12:02:49.762856 scrapy-zyte-api-0.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-02 12:02:39.000000 scrapy-zyte-api-0.8.2/setup.py
```

### Comparing `scrapy-zyte-api-0.8.1/LICENSE.txt` & `scrapy-zyte-api-0.8.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scrapy-zyte-api-0.8.1/PKG-INFO` & `scrapy-zyte-api-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapy-zyte-api
-Version: 0.8.1
+Version: 0.8.2
 Summary: Client library to process URLs through Zyte API
 Home-page: https://github.com/scrapy-plugins/scrapy-zyte-api
 Author: Zyte Group Ltd
 Author-email: info@zyte.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `scrapy-zyte-api-0.8.1/README.rst` & `scrapy-zyte-api-0.8.2/README.rst`

 * *Files identical despite different names*

### Comparing `scrapy-zyte-api-0.8.1/scrapy_zyte_api/_cookies.py` & `scrapy-zyte-api-0.8.2/scrapy_zyte_api/_cookies.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,32 @@
 from http.cookiejar import Cookie
 from typing import Any, Dict, List, Optional
+from urllib.parse import urlparse
 
 from scrapy.http import Request
 from scrapy.http.cookies import CookieJar
 
 
 def _get_cookie_jar(request: Request, cookie_jars: Dict[Any, CookieJar]) -> CookieJar:
     jar_id = request.meta.get("cookiejar")
     return cookie_jars[jar_id]
 
 
+def _get_cookie_domain(cookie, url):
+    domain = cookie.get("domain")
+    if domain:
+        return domain
+    domain = urlparse(url).hostname
+    if domain:
+        return domain
+    raise ValueError(
+        f"Got a cookie without a domain from URL {url} which has no domain either."
+    )
+
+
 def _process_cookies(
     api_response: Dict[str, Any],
     request: Request,
     cookie_jars: Optional[Dict[Any, CookieJar]],
 ):
     if not cookie_jars:
         return
@@ -31,17 +44,17 @@
             rest["sameSite"] = same_site
         cookie = Cookie(
             version=1,
             name=response_cookie["name"],
             value=response_cookie["value"],
             port=None,
             port_specified=False,
-            domain=response_cookie["domain"],
-            domain_specified=True,
-            domain_initial_dot=response_cookie["domain"].startswith("."),
+            domain=_get_cookie_domain(response_cookie, api_response["url"]),
+            domain_specified="domain" in response_cookie,
+            domain_initial_dot=response_cookie.get("domain", "").startswith("."),
             path=response_cookie.get("path", "/"),
             path_specified="path" in response_cookie,
             secure=response_cookie.get("secure", False),
             expires=response_cookie.get("expires", None),
             discard=False,
             comment=None,
             comment_url=None,
```

### Comparing `scrapy-zyte-api-0.8.1/scrapy_zyte_api/_downloader_middleware.py` & `scrapy-zyte-api-0.8.2/scrapy_zyte_api/_downloader_middleware.py`

 * *Files identical despite different names*

### Comparing `scrapy-zyte-api-0.8.1/scrapy_zyte_api/_params.py` & `scrapy-zyte-api-0.8.2/scrapy_zyte_api/_params.py`

 * *Files identical despite different names*

### Comparing `scrapy-zyte-api-0.8.1/scrapy_zyte_api/_request_fingerprinter.py` & `scrapy-zyte-api-0.8.2/scrapy_zyte_api/_request_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `scrapy-zyte-api-0.8.1/scrapy_zyte_api/handler.py` & `scrapy-zyte-api-0.8.2/scrapy_zyte_api/handler.py`

 * *Files identical despite different names*

### Comparing `scrapy-zyte-api-0.8.1/scrapy_zyte_api/responses.py` & `scrapy-zyte-api-0.8.2/scrapy_zyte_api/responses.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,18 @@
         To see the full list of parameters and their description, kindly refer to the
         `Zyte API Specification <https://docs.zyte.com/zyte-api/openapi.html#zyte-openapi-spec>`_.
         """
         return self._raw_api_response
 
     @staticmethod
     def _response_cookie_to_header_value(cookie):
-        result = f"{cookie['name']}={cookie['value']}; Domain={cookie['domain']}"
+        result = f"{cookie['name']}={cookie['value']}"
+        domain = cookie.get("domain")
+        if domain:
+            result += f"; Domain={cookie['domain']}"
         path = cookie.get("path")
         if path is not None:
             result += f"; Path={path}"
         expires = cookie.get("expires")
         if expires is not None:
             expires_date = datetime.utcfromtimestamp(expires)
             expires_date_string = expires_date.strftime("%a, %d %b %Y %H:%M:%S GMT")
```

### Comparing `scrapy-zyte-api-0.8.1/scrapy_zyte_api/utils.py` & `scrapy-zyte-api-0.8.2/scrapy_zyte_api/utils.py`

 * *Files identical despite different names*

### Comparing `scrapy-zyte-api-0.8.1/scrapy_zyte_api.egg-info/PKG-INFO` & `scrapy-zyte-api-0.8.2/scrapy_zyte_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapy-zyte-api
-Version: 0.8.1
+Version: 0.8.2
 Summary: Client library to process URLs through Zyte API
 Home-page: https://github.com/scrapy-plugins/scrapy-zyte-api
 Author: Zyte Group Ltd
 Author-email: info@zyte.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `scrapy-zyte-api-0.8.1/setup.py` & `scrapy-zyte-api-0.8.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="scrapy-zyte-api",
-    version="0.8.1",
+    version="0.8.2",
     description="Client library to process URLs through Zyte API",
     long_description=open("README.rst").read(),
     long_description_content_type="text/x-rst",
     author="Zyte Group Ltd",
     author_email="info@zyte.com",
     url="https://github.com/scrapy-plugins/scrapy-zyte-api",
     packages=["scrapy_zyte_api"],
```

