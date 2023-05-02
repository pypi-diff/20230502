# Comparing `tmp/resotoclient-1.2.1.tar.gz` & `tmp/resotoclient-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotoclient-1.2.1.tar", max compression
+gzip compressed data, was "resotoclient-1.3.0.tar", max compression
```

## Comparing `resotoclient-1.2.1.tar` & `resotoclient-1.3.0.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0    11357 2022-11-10 13:21:20.119323 resotoclient-1.2.1/LICENSE
--rw-r--r--   0        0        0     1243 2022-11-10 13:21:20.119323 resotoclient-1.2.1/README.md
--rw-r--r--   0        0        0     2080 2022-11-10 13:21:20.123323 resotoclient-1.2.1/pyproject.toml
--rw-r--r--   0        0        0    20232 2022-11-10 13:21:20.123323 resotoclient-1.2.1/resotoclient/__init__.py
--rw-r--r--   0        0        0    22150 2022-11-10 13:21:20.123323 resotoclient-1.2.1/resotoclient/async_client.py
--rw-r--r--   0        0        0     6219 2022-11-10 13:21:20.123323 resotoclient-1.2.1/resotoclient/ca.py
--rw-r--r--   0        0        0     2813 2022-11-10 13:21:20.123323 resotoclient-1.2.1/resotoclient/http_client/__init__.py
--rw-r--r--   0        0        0    10360 2022-11-10 13:21:20.123323 resotoclient-1.2.1/resotoclient/http_client/aiohttp_client.py
--rw-r--r--   0        0        0     1282 2022-11-10 13:21:20.123323 resotoclient-1.2.1/resotoclient/http_client/event_loop_thread.py
--rw-r--r--   0        0        0      693 2022-11-10 13:21:20.123323 resotoclient-1.2.1/resotoclient/json_utils.py
--rw-r--r--   0        0        0     3431 2022-11-10 13:21:20.123323 resotoclient-1.2.1/resotoclient/jwt_utils.py
--rw-r--r--   0        0        0     2283 2022-11-10 13:21:20.123323 resotoclient-1.2.1/resotoclient/models.py
--rw-r--r--   0        0        0     2223 1970-01-01 00:00:00.000000 resotoclient-1.2.1/setup.py
--rw-r--r--   0        0        0     2769 1970-01-01 00:00:00.000000 resotoclient-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-02 07:53:32.413548 resotoclient-1.3.0/LICENSE
+-rw-r--r--   0        0        0     1243 2023-05-02 07:53:32.413548 resotoclient-1.3.0/README.md
+-rw-r--r--   0        0        0     2082 2023-05-02 07:53:32.413548 resotoclient-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0    20448 2023-05-02 07:53:32.413548 resotoclient-1.3.0/resotoclient/__init__.py
+-rw-r--r--   0        0        0    23011 2023-05-02 07:53:32.413548 resotoclient-1.3.0/resotoclient/async_client.py
+-rw-r--r--   0        0        0     6219 2023-05-02 07:53:32.413548 resotoclient-1.3.0/resotoclient/ca.py
+-rw-r--r--   0        0        0     2813 2023-05-02 07:53:32.413548 resotoclient-1.3.0/resotoclient/http_client/__init__.py
+-rw-r--r--   0        0        0    10672 2023-05-02 07:53:32.413548 resotoclient-1.3.0/resotoclient/http_client/aiohttp_client.py
+-rw-r--r--   0        0        0     1282 2023-05-02 07:53:32.413548 resotoclient-1.3.0/resotoclient/http_client/event_loop_thread.py
+-rw-r--r--   0        0        0      693 2023-05-02 07:53:32.413548 resotoclient-1.3.0/resotoclient/json_utils.py
+-rw-r--r--   0        0        0     3431 2023-05-02 07:53:32.413548 resotoclient-1.3.0/resotoclient/jwt_utils.py
+-rw-r--r--   0        0        0     2283 2023-05-02 07:53:32.413548 resotoclient-1.3.0/resotoclient/models.py
+-rw-r--r--   0        0        0     2721 1970-01-01 00:00:00.000000 resotoclient-1.3.0/PKG-INFO
```

### Comparing `resotoclient-1.2.1/LICENSE` & `resotoclient-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `resotoclient-1.2.1/README.md` & `resotoclient-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `resotoclient-1.2.1/pyproject.toml` & `resotoclient-1.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "resotoclient"
-version = "1.2.1"
+version = "1.3.0"
 description = "Resoto Python client library"
 authors = ["Some Engineering Inc."]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/someengineering/resotoclient-python"
 repository = "https://github.com/someengineering/resotoclient-python"
 packages = [
@@ -15,53 +15,53 @@
     "Development Status :: 4 - Beta",
     # Audience
     "Intended Audience :: System Administrators",
     "Intended Audience :: Information Technology",
     # License information
     "License :: OSI Approved :: Apache Software License",
     # Supported python versions
-    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
     # Supported OS's
     "Operating System :: POSIX :: Linux",
     "Operating System :: Unix",
     # Extra metadata
     "Environment :: Console",
     "Natural Language :: English",
     "Topic :: Security",
     "Topic :: Utilities",
 ]
 
 [tool.poetry.urls]
 Changelog = "https://github.com/someengineering/resotoclient-python/releases"
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.9"
 jsons="^1.6.1"
 PyJWT="^2.3.0"
 cryptography=">=36.0.2"
 pandas = { version = "^1.4.2", optional = true }
 graphviz = { version = "^0.20", optional = true }
 aiohttp = "^3.8.1"
 certifi = "^2022.9.24"
 
 
 [tool.poetry.extras]
 extras = ["pandas", "graphviz"]
 
 [tool.poetry.dev-dependencies]
-pytest = "^6.2.5"
-safety = "^2.3.1"
-pyright = "^1.1.238"
-flake8 = "^4.0.1"
-black = ">=21.10b0"
-flake8-bandit = "^2.1.2"
-flake8-bugbear = "^21.9.2"
-pep8-naming = "^0.12.1"
+pytest = "^7.3.1"
+safety = "^2.3.5"
+pyright = "^1.1.304"
+flake8 = "^6.0.0"
+black = ">=22.12.0"
+flake8-bandit = "^4.1.1"
+flake8-bugbear = "^23.3.23"
+pep8-naming = "^0.13.3"
 networkx = "^2.8"
-six = "^1.2.0"
+six = "^1.16.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest-asyncio = "^0.19.0"
 
 [tool.pyright]
 include = ["resotoclient", "tests"]
 exclude = ["**/node_modules",
```

### Comparing `resotoclient-1.2.1/resotoclient/__init__.py` & `resotoclient-1.3.0/resotoclient/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     Sequence,
     Mapping,
     Type,
     AsyncIterator,
     TypeVar,
     Awaitable,
     Callable,
+    cast,
 )
 from types import TracebackType
 from resotoclient.models import (
     Subscriber,
     Subscription,
     ParsedCommands,
     GraphUpdate,
@@ -105,21 +106,24 @@
     """
     The ApiClient interacts with a running core instance via the REST interface.
     """
 
     def __init__(
         self,
         url: str,
+        *,
         psk: Optional[str],
+        additional_headers: Optional[Dict[str, str]] = None,
         custom_ca_cert_path: Optional[str] = None,
         verify: bool = True,
         renew_before: timedelta = timedelta(days=1),
     ):
         self.resotocore_url = url
         self.psk = psk
+        self.additional_headers = additional_headers
         self.custom_ca_cert_path = custom_ca_cert_path
         self.verify = verify
         self.renew_before = renew_before
         self.event_loop_thread = EventLoopThread()
         self.event_loop_thread.daemon = True
         atexit.register(self.shutdown)
 
@@ -137,28 +141,28 @@
         exc_type: Optional[Type[BaseException]],
         exc_val: Optional[BaseException],
         exc_tb: Optional[TracebackType],
     ) -> None:
         self.shutdown()
 
     def start(self) -> None:
-
         with self.state_lock:
             if self.client_state != ClientState.INITIALIZED:
                 return
 
             self.event_loop_thread.start()
             import time
 
             while not self.event_loop_thread.running:
                 time.sleep(0.05)
 
             self.async_client = AsyncResotoClient(
                 url=self.resotocore_url,
                 psk=self.psk,
+                additional_headers=self.additional_headers,
                 custom_ca_cert_path=self.custom_ca_cert_path,
                 verify=self.verify,
                 renew_before=self.renew_before,
                 loop=self.event_loop_thread.loop,
             )
 
             self.event_loop_thread.run_coroutine(self.async_client.start())
@@ -405,15 +409,15 @@
                     del node_data["group"]
                     for k, v in group.items():
                         node_data[k] = v
             else:
                 if flatten:
                     if not "reported" in node or not isinstance(node["reported"], dict):
                         return None
-                    node_data = node["reported"]
+                    node_data = cast(Dict[str, Any], node["reported"])
                     for k, v in node.items():
                         if isinstance(v, dict) and k != "reported":
                             node_data[k] = v
                     node_data["cloud_id"] = js_find(
                         node,
                         ["ancestors", "cloud", "reported", "id"],
                     )
```

### Comparing `resotoclient-1.2.1/resotoclient/async_client.py` & `resotoclient-1.3.0/resotoclient/async_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,20 +44,32 @@
     """
     The ApiClient interacts with a running core instance via the REST interface.
     """
 
     def __init__(
         self,
         url: str,
+        *,
         psk: Optional[str],
+        additional_headers: Optional[Dict[str, str]] = None,
         custom_ca_cert_path: Optional[str] = None,
         verify: bool = True,
         renew_before: timedelta = timedelta(days=1),
         loop: Optional[AbstractEventLoop] = None,
     ):
+        """
+        Create a new resoto client instance.
+        :param url: the url of the resotocore instance.
+        :param psk: the optional pre-shared key to use for authentication. The PSK is used to authenticate the client. If you do not have access to the PSK, you can use the auth_header parameter to authenticate with a JWT token.
+        :param additional_headers: additional headers to send with each request.
+        :param custom_ca_cert_path: path to a custom CA certificate to use for verifying the server certificate.
+        :param verify: whether to verify the server certificate.
+        :param renew_before: how long before the certificate expires to renew it.
+        :param loop: the event loop to use.
+        """
         self.resotocore_url = url
         self.psk = psk
         self.verify = verify
         self.session_id = rnd_str()
         self.holder = CertificatesHolder(
             resotocore_url=url,
             psk=psk,
@@ -65,14 +77,15 @@
             renew_before=renew_before,
         )
         self.http_client = AioHttpClient(
             url=url,
             psk=psk,
             session_id=self.session_id,
             get_ssl_context=self.holder.ssl_context if verify else None,
+            additional_headers=additional_headers,
             loop=loop,
         )
 
     async def __aenter__(self) -> "ResotoClient":
         await self.start()
         return self
 
@@ -88,15 +101,14 @@
         await self.holder.start()
 
     async def shutdown(self) -> None:
         await self.http_client.close()
         self.holder.shutdown()
 
     def _headers(self) -> Dict[str, str]:
-
         headers = {"Content-type": "application/json", "Accept": "application/json"}
 
         if self.psk:
             encode_jwt_to_headers(headers, {}, self.psk)
 
         return headers
```

### Comparing `resotoclient-1.2.1/resotoclient/ca.py` & `resotoclient-1.3.0/resotoclient/ca.py`

 * *Files identical despite different names*

### Comparing `resotoclient-1.2.1/resotoclient/http_client/__init__.py` & `resotoclient-1.3.0/resotoclient/http_client/__init__.py`

 * *Files identical despite different names*

### Comparing `resotoclient-1.2.1/resotoclient/http_client/aiohttp_client.py` & `resotoclient-1.3.0/resotoclient/http_client/aiohttp_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,47 +24,51 @@
     pass
 
 
 class AioHttpClient(AsyncHttpClient):
     def __init__(
         self,
         url: str,
+        *,
         psk: Optional[str],
+        additional_headers: Optional[Dict[str, str]] = None,
         session_id: str,
         get_ssl_context: Optional[Callable[[], Awaitable[ssl.SSLContext]]] = None,
         loop: Optional[AbstractEventLoop] = None,
     ):
-
         self.session = aiohttp.ClientSession(loop=loop)
         self.url = url
         self.psk = psk
         self.get_ssl_context = get_ssl_context
         self.session_id = session_id
+        self.additional_headers = additional_headers or {}
 
     async def _ssl_context(self) -> Union[ssl.SSLContext, bool]:
         if self.get_ssl_context:
             return await self.get_ssl_context()
         else:
             return False
 
     async def close(self) -> None:
         await self.session.close()
 
     def _default_query_params(self) -> Dict[str, str]:
         return {"session_id": self.session_id}
 
     def _default_headers(self) -> CIMultiDict[str]:
+        # default headers sent for every request
         default_headers = {
             "Content-type": "application/json",
             "Accept": "application/json",
         }
-
+        # add auth header if psk is set
         if self.psk:
             encode_jwt_to_headers(default_headers, {}, self.psk)
-
+        # set all user defined headers
+        default_headers.update(self.additional_headers)
         return CIMultiDict(default_headers)
 
     async def lines(self, response: aiohttp.ClientResponse) -> AsyncIterator[bytes]:
         async for line in response.content:
             # aiohttp keeps the newline separator when iterating over the content
             # we should strip the newline as it was done in the old http client
             yield line.rstrip(b"\n")
```

### Comparing `resotoclient-1.2.1/resotoclient/http_client/event_loop_thread.py` & `resotoclient-1.3.0/resotoclient/http_client/event_loop_thread.py`

 * *Files identical despite different names*

### Comparing `resotoclient-1.2.1/resotoclient/json_utils.py` & `resotoclient-1.3.0/resotoclient/json_utils.py`

 * *Files identical despite different names*

### Comparing `resotoclient-1.2.1/resotoclient/jwt_utils.py` & `resotoclient-1.3.0/resotoclient/jwt_utils.py`

 * *Files identical despite different names*

### Comparing `resotoclient-1.2.1/resotoclient/models.py` & `resotoclient-1.3.0/resotoclient/models.py`

 * *Files identical despite different names*

### Comparing `resotoclient-1.2.1/PKG-INFO` & `resotoclient-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 Metadata-Version: 2.1
 Name: resotoclient
-Version: 1.2.1
+Version: 1.3.0
 Summary: Resoto Python client library
 Home-page: https://github.com/someengineering/resotoclient-python
 License: Apache-2.0
 Author: Some Engineering Inc.
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Provides-Extra: extras
 Requires-Dist: PyJWT (>=2.3.0,<3.0.0)
 Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
 Requires-Dist: certifi (>=2022.9.24,<2023.0.0)
 Requires-Dist: cryptography (>=36.0.2)
-Requires-Dist: graphviz (>=0.20,<0.21); extra == "extras"
+Requires-Dist: graphviz (>=0.20,<0.21) ; extra == "extras"
 Requires-Dist: jsons (>=1.6.1,<2.0.0)
-Requires-Dist: pandas (>=1.4.2,<2.0.0); extra == "extras"
+Requires-Dist: pandas (>=1.4.2,<2.0.0) ; extra == "extras"
 Project-URL: Changelog, https://github.com/someengineering/resotoclient-python/releases
 Project-URL: Repository, https://github.com/someengineering/resotoclient-python
 Description-Content-Type: text/markdown
 
 # resotoclient-python
 Python client for Resoto
```

