# Comparing `tmp/xapi-python-0.1.0.tar.gz` & `tmp/xapi-python-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xapi-python-0.1.0.tar", last modified: Sat Apr 29 11:42:03 2023, max compression
+gzip compressed data, was "xapi-python-0.1.1.tar", last modified: Tue May  2 15:09:58 2023, max compression
```

## Comparing `xapi-python-0.1.0.tar` & `xapi-python-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-04-29 11:42:03.464872 xapi-python-0.1.0/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1071 2023-04-25 04:51:26.000000 xapi-python-0.1.0/LICENSE
--rw-r--r--   0 pawel     (1000) pawel     (1000)     8099 2023-04-29 11:42:03.464872 xapi-python-0.1.0/PKG-INFO
--rw-r--r--   0 pawel     (1000) pawel     (1000)     5794 2023-04-29 11:41:41.000000 xapi-python-0.1.0/README.md
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1105 2023-04-29 11:41:41.000000 xapi-python-0.1.0/pyproject.toml
--rw-r--r--   0 pawel     (1000) pawel     (1000)       38 2023-04-29 11:42:03.464872 xapi-python-0.1.0/setup.cfg
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1027 2023-04-29 11:41:41.000000 xapi-python-0.1.0/setup.py
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-04-29 11:42:03.454872 xapi-python-0.1.0/tests/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     4687 2023-04-29 11:41:41.000000 xapi-python-0.1.0/tests/test_connect.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     7958 2023-04-26 11:15:10.000000 xapi-python-0.1.0/tests/test_socket.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     4014 2023-04-27 05:35:22.000000 xapi-python-0.1.0/tests/test_stream.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1566 2023-04-29 10:20:03.000000 xapi-python-0.1.0/tests/test_xapi.py
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-04-29 11:42:03.464872 xapi-python-0.1.0/xapi/
--rw-r--r--   0 pawel     (1000) pawel     (1000)      338 2023-04-29 11:41:41.000000 xapi-python-0.1.0/xapi/__init__.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     2114 2023-04-29 11:41:41.000000 xapi-python-0.1.0/xapi/connection.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1464 2023-04-24 14:52:49.000000 xapi-python-0.1.0/xapi/enums.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      205 2023-04-29 11:41:41.000000 xapi-python-0.1.0/xapi/exceptions.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     6640 2023-04-29 11:38:37.000000 xapi-python-0.1.0/xapi/socket.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     2947 2023-04-29 11:39:31.000000 xapi-python-0.1.0/xapi/stream.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     2207 2023-04-29 11:41:41.000000 xapi-python-0.1.0/xapi/xapi.py
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-04-29 11:42:03.464872 xapi-python-0.1.0/xapi_python.egg-info/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     8099 2023-04-29 11:42:03.000000 xapi-python-0.1.0/xapi_python.egg-info/PKG-INFO
--rw-r--r--   0 pawel     (1000) pawel     (1000)      376 2023-04-29 11:42:03.000000 xapi-python-0.1.0/xapi_python.egg-info/SOURCES.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)        1 2023-04-29 11:42:03.000000 xapi-python-0.1.0/xapi_python.egg-info/dependency_links.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)        5 2023-04-29 11:42:03.000000 xapi-python-0.1.0/xapi_python.egg-info/top_level.txt
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-05-02 15:09:58.197023 xapi-python-0.1.1/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1071 2023-04-25 04:51:26.000000 xapi-python-0.1.1/LICENSE
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     8167 2023-05-02 15:09:58.197023 xapi-python-0.1.1/PKG-INFO
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     5862 2023-05-02 15:06:07.000000 xapi-python-0.1.1/README.md
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1234 2023-05-02 15:09:32.000000 xapi-python-0.1.1/pyproject.toml
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       38 2023-05-02 15:09:58.197023 xapi-python-0.1.1/setup.cfg
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1027 2023-05-02 15:09:32.000000 xapi-python-0.1.1/setup.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-05-02 15:09:58.197023 xapi-python-0.1.1/tests/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     5121 2023-05-02 15:09:32.000000 xapi-python-0.1.1/tests/test_connect.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     7958 2023-04-26 11:15:10.000000 xapi-python-0.1.1/tests/test_socket.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     4014 2023-04-27 05:35:22.000000 xapi-python-0.1.1/tests/test_stream.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1566 2023-04-29 10:20:03.000000 xapi-python-0.1.1/tests/test_xapi.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-05-02 15:09:58.197023 xapi-python-0.1.1/xapi/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      338 2023-05-02 15:09:32.000000 xapi-python-0.1.1/xapi/__init__.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     2227 2023-05-02 15:09:32.000000 xapi-python-0.1.1/xapi/connection.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1464 2023-04-24 14:52:49.000000 xapi-python-0.1.1/xapi/enums.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      205 2023-04-29 11:41:41.000000 xapi-python-0.1.1/xapi/exceptions.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     6640 2023-04-29 11:38:37.000000 xapi-python-0.1.1/xapi/socket.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     2947 2023-04-29 11:39:31.000000 xapi-python-0.1.1/xapi/stream.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     2207 2023-04-29 11:41:41.000000 xapi-python-0.1.1/xapi/xapi.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-05-02 15:09:58.197023 xapi-python-0.1.1/xapi_python.egg-info/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     8167 2023-05-02 15:09:58.000000 xapi-python-0.1.1/xapi_python.egg-info/PKG-INFO
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      376 2023-05-02 15:09:58.000000 xapi-python-0.1.1/xapi_python.egg-info/SOURCES.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)        1 2023-05-02 15:09:58.000000 xapi-python-0.1.1/xapi_python.egg-info/dependency_links.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)        5 2023-05-02 15:09:58.000000 xapi-python-0.1.1/xapi_python.egg-info/top_level.txt
```

### Comparing `xapi-python-0.1.0/LICENSE` & `xapi-python-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xapi-python-0.1.0/PKG-INFO` & `xapi-python-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xapi-python
-Version: 0.1.0
+Version: 0.1.1
 Summary: The xStation5 API Python library
 Home-page: https://github.com/pawelkn/xapi-python
 Author: Paweł Knioła
 Author-email: Paweł Knioła <pawel.kn@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Paweł Knioła
@@ -212,13 +212,15 @@
 ```
 
 ## Unit Tests
 
 This will run all of the unit tests in the tests directory:
 
 ```shell
+git clone https://github.com/pawelkn/xapi-python.git
+cd xapi-python
 python3 -m unittest discover tests
 ```
 
 ## Buy Me A Coffee! ☕
 
 If you find the project beneficial and would like to support me, please consider showing your appreciation by buying me a coffee on [BuyMeACoffee](https://www.buymeacoffee.com/pawelkn)
```

### Comparing `xapi-python-0.1.0/README.md` & `xapi-python-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -168,13 +168,15 @@
 ```
 
 ## Unit Tests
 
 This will run all of the unit tests in the tests directory:
 
 ```shell
+git clone https://github.com/pawelkn/xapi-python.git
+cd xapi-python
 python3 -m unittest discover tests
 ```
 
 ## Buy Me A Coffee! ☕
 
 If you find the project beneficial and would like to support me, please consider showing your appreciation by buying me a coffee on [BuyMeACoffee](https://www.buymeacoffee.com/pawelkn)
```

### Comparing `xapi-python-0.1.0/pyproject.toml` & `xapi-python-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "xapi-python"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Paweł Knioła", email="pawel.kn@gmail.com" },
 ]
 description = "The xStation5 API Python library"
 keywords = [
   "python", "python3", "bitcoin", "trading", "websocket", "trading-api", "forex", "xapi", "forex-trading",
   "exchange-api", "forex-data", "xstation", "xstation5", "xtb", "xopenhub", "forex-api", "xopenhub-api",
@@ -20,10 +20,18 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12"
 ]
 
+[build-system]
+build-backend = "setuptools.build_meta"
+requires = [
+    "wheel",
+    "setuptools",
+    "websockets >= 11.0.2"
+]
+
 [project.urls]
 "Homepage" = "https://github.com/pawelkn/xapi-python"
 "Bug Tracker" = "https://github.com/pawelkn/xapi-python/issues"
```

### Comparing `xapi-python-0.1.0/setup.py` & `xapi-python-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,10 +16,10 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12"
     ],
     python_requires='>=3.7',
-    version="0.1.0",
+    version="0.1.1",
     packages=['xapi'],
 )
```

### Comparing `xapi-python-0.1.0/tests/test_connect.py` & `xapi-python-0.1.1/tests/test_connect.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,28 @@
 import unittest
 from unittest.mock import AsyncMock, patch
 
 import websockets.client
 import websockets.exceptions
+import socket
 import json
 import asyncio
 
 from xapi import Connection, ConnectionClosed
 
 class TestConnection(unittest.IsolatedAsyncioTestCase):
 
+    async def test_connect_socket_gaierror(self):
+        c = Connection()
+        with patch("websockets.client.connect", new_callable=AsyncMock) as mocked_connect:
+            mocked_connect.side_effect = socket.gaierror()
+            with self.assertRaises(ConnectionClosed) as cm:
+                await c.connect("ws://127.0.0.1:9000")
+            self.assertEqual(str(cm.exception), "Hostname cannot be resolved")
+
     async def test_connect_timeout_error(self):
         c = Connection()
         with patch("websockets.client.connect", new_callable=AsyncMock) as mocked_connect:
             mocked_connect.side_effect = asyncio.exceptions.TimeoutError()
             with self.assertRaises(ConnectionClosed) as cm:
                 await c.connect("ws://127.0.0.1:9000")
             self.assertEqual(str(cm.exception), "Connection timed out")
```

### Comparing `xapi-python-0.1.0/tests/test_socket.py` & `xapi-python-0.1.1/tests/test_socket.py`

 * *Files identical despite different names*

### Comparing `xapi-python-0.1.0/tests/test_stream.py` & `xapi-python-0.1.1/tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `xapi-python-0.1.0/tests/test_xapi.py` & `xapi-python-0.1.1/tests/test_xapi.py`

 * *Files identical despite different names*

### Comparing `xapi-python-0.1.0/xapi/connection.py` & `xapi-python-0.1.1/xapi/connection.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 from .exceptions import ConnectionClosed
 
 import websockets.client
 import websockets.exceptions
+import socket
 import asyncio
 import json
 
 class Connection():
     def __init__(self):
         self.safe = True
         self._conn = None
         self._lock = asyncio.Lock()
 
     async def connect(self, url):
         try:
             self._conn = await websockets.client.connect(url, close_timeout=0, max_size=None)
 
+        except socket.gaierror:
+            raise ConnectionClosed("Hostname cannot be resolved")
+
         except asyncio.exceptions.TimeoutError:
             raise ConnectionClosed("Connection timed out")
 
         except ConnectionRefusedError:
             raise ConnectionClosed("Connection refused")
 
     async def disconnect(self):
```

### Comparing `xapi-python-0.1.0/xapi/enums.py` & `xapi-python-0.1.1/xapi/enums.py`

 * *Files identical despite different names*

### Comparing `xapi-python-0.1.0/xapi/socket.py` & `xapi-python-0.1.1/xapi/socket.py`

 * *Files identical despite different names*

### Comparing `xapi-python-0.1.0/xapi/stream.py` & `xapi-python-0.1.1/xapi/stream.py`

 * *Files identical despite different names*

### Comparing `xapi-python-0.1.0/xapi/xapi.py` & `xapi-python-0.1.1/xapi/xapi.py`

 * *Files identical despite different names*

### Comparing `xapi-python-0.1.0/xapi_python.egg-info/PKG-INFO` & `xapi-python-0.1.1/xapi_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xapi-python
-Version: 0.1.0
+Version: 0.1.1
 Summary: The xStation5 API Python library
 Home-page: https://github.com/pawelkn/xapi-python
 Author: Paweł Knioła
 Author-email: Paweł Knioła <pawel.kn@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Paweł Knioła
@@ -212,13 +212,15 @@
 ```
 
 ## Unit Tests
 
 This will run all of the unit tests in the tests directory:
 
 ```shell
+git clone https://github.com/pawelkn/xapi-python.git
+cd xapi-python
 python3 -m unittest discover tests
 ```
 
 ## Buy Me A Coffee! ☕
 
 If you find the project beneficial and would like to support me, please consider showing your appreciation by buying me a coffee on [BuyMeACoffee](https://www.buymeacoffee.com/pawelkn)
```

