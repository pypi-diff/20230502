# Comparing `tmp/slapdash-1.0.1.tar.gz` & `tmp/slapdash-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slapdash-1.0.1.tar", max compression
+gzip compressed data, was "slapdash-1.0.2.tar", max compression
```

## Comparing `slapdash-1.0.1.tar` & `slapdash-1.0.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1732 2023-03-08 21:35:28.330748 slapdash-1.0.1/README.md
--rw-r--r--   0        0        0      996 2023-03-08 21:54:27.836141 slapdash-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      232 2023-03-08 21:14:25.953456 slapdash-1.0.1/slapdash/__init__.py
--rw-r--r--   0        0        0     6364 2023-03-08 20:45:03.049808 slapdash-1.0.1/slapdash/client.py
--rw-r--r--   0        0        0    21249 2023-03-08 21:15:37.237625 slapdash-1.0.1/slapdash/decorators.py
--rw-r--r--   0        0        0      764 2023-03-08 20:36:48.907348 slapdash-1.0.1/slapdash/examples/async.py
--rw-r--r--   0        0        0       67 2023-03-08 20:36:48.495247 slapdash-1.0.1/slapdash/examples/client_example.py
--rw-r--r--   0        0        0      131 2022-08-23 15:30:06.060760 slapdash-1.0.1/slapdash/examples/custom_css.css
--rw-r--r--   0        0        0      322 2023-03-08 20:36:48.486369 slapdash-1.0.1/slapdash/examples/custom_css.py
--rw-r--r--   0        0        0      278 2023-03-08 20:36:48.906847 slapdash-1.0.1/slapdash/examples/dac_example.py
--rw-r--r--   0        0        0     1056 2023-03-08 21:15:41.005649 slapdash-1.0.1/slapdash/examples/datastream_example.py
--rw-r--r--   0        0        0      589 2023-03-08 20:36:48.906954 slapdash-1.0.1/slapdash/examples/device_example.py
--rw-r--r--   0        0        0      888 2023-03-08 20:36:48.495461 slapdash-1.0.1/slapdash/examples/doc_example.py
--rw-r--r--   0        0        0      988 2023-03-08 21:15:42.602058 slapdash-1.0.1/slapdash/examples/enum_example.py
--rw-r--r--   0        0        0     1202 2023-03-08 20:36:48.906907 slapdash-1.0.1/slapdash/examples/example.py
--rw-r--r--   0        0        0      297 2023-03-08 21:16:05.574366 slapdash-1.0.1/slapdash/examples/hello_world.py
--rw-r--r--   0        0        0     2059 2023-03-08 21:15:43.451462 slapdash-1.0.1/slapdash/examples/metadata_example.py
--rw-r--r--   0        0        0     1684 2023-03-08 21:15:44.650882 slapdash-1.0.1/slapdash/examples/readonly_example.py
--rw-r--r--   0        0        0      515 2023-03-08 20:36:48.906990 slapdash-1.0.1/slapdash/examples/refresh_example.py
--rw-r--r--   0        0        0      876 2023-03-08 21:14:53.457314 slapdash-1.0.1/slapdash/examples/saver_example.py
--rw-r--r--   0        0        0      126 2022-08-23 15:30:06.062411 slapdash-1.0.1/slapdash/examples/settings.json
--rw-r--r--   0        0        0      272 2023-03-08 20:36:50.488583 slapdash-1.0.1/slapdash/examples/simple.py
--rw-r--r--   0        0        0     2908 2023-03-08 21:15:47.749023 slapdash-1.0.1/slapdash/examples/slider_example.py
--rw-r--r--   0        0        0      733 2023-03-08 20:36:48.906973 slapdash-1.0.1/slapdash/examples/subcomponents.py
--rw-r--r--   0        0        0      849 2023-03-08 20:36:48.907040 slapdash-1.0.1/slapdash/examples/trigger_update_example.py
--rw-r--r--   0        0        0      815 2023-03-08 20:36:48.907173 slapdash-1.0.1/slapdash/examples.py
--rw-r--r--   0        0        0        0 2023-03-08 21:29:51.082127 slapdash-1.0.1/slapdash/frontend/custom.css
--rw-r--r--   0        0        0     1093 2023-03-08 21:29:51.105966 slapdash-1.0.1/slapdash/frontend/custom.js
--rw-r--r--   0        0        0     9178 2023-03-08 21:29:51.100802 slapdash-1.0.1/slapdash/frontend/dashboard.css
--rw-r--r--   0        0        0   167882 2023-03-08 21:29:51.105003 slapdash-1.0.1/slapdash/frontend/index.css
--rw-r--r--   0        0        0      472 2023-03-08 21:29:51.100681 slapdash-1.0.1/slapdash/frontend/index.html
--rw-r--r--   0        0        0  1538596 2023-03-08 21:29:51.298413 slapdash-1.0.1/slapdash/frontend/index.js
--rw-r--r--   0        0        0       87 2023-03-08 21:26:57.416425 slapdash-1.0.1/slapdash/frontend/package-lock.json
--rw-r--r--   0        0        0     6415 2023-03-08 21:15:38.722514 slapdash-1.0.1/slapdash/main.py
--rw-r--r--   0        0        0     5680 2023-03-08 21:15:40.029174 slapdash-1.0.1/slapdash/metadata.py
--rw-r--r--   0        0        0    21215 2023-03-08 20:32:05.230243 slapdash-1.0.1/slapdash/model.py
--rw-r--r--   0        0        0     1008 2023-03-08 20:32:00.464892 slapdash-1.0.1/slapdash/testing.py
--rw-r--r--   0        0        0      253 2022-08-23 15:30:06.086214 slapdash-1.0.1/slapdash/types.py
--rw-r--r--   0        0        0       45 2023-03-08 21:54:40.851486 slapdash-1.0.1/slapdash/version.json
--rw-r--r--   0        0        0      874 2022-08-23 15:30:06.086760 slapdash-1.0.1/slapdash/version.py
--rw-r--r--   0        0        0    13560 2023-03-08 21:14:28.487128 slapdash-1.0.1/slapdash/web.py
--rw-r--r--   0        0        0     2728 1970-01-01 00:00:00.000000 slapdash-1.0.1/setup.py
--rw-r--r--   0        0        0     2603 1970-01-01 00:00:00.000000 slapdash-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1732 2023-03-08 21:35:28.330748 slapdash-1.0.2/README.md
+-rw-r--r--   0        0        0      996 2023-05-01 22:20:12.590670 slapdash-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      232 2023-03-08 21:14:25.953456 slapdash-1.0.2/slapdash/__init__.py
+-rw-r--r--   0        0        0     8027 2023-05-01 22:19:32.667441 slapdash-1.0.2/slapdash/client.py
+-rw-r--r--   0        0        0    21249 2023-03-08 21:15:37.237625 slapdash-1.0.2/slapdash/decorators.py
+-rw-r--r--   0        0        0      764 2023-03-08 20:36:48.907348 slapdash-1.0.2/slapdash/examples/async.py
+-rw-r--r--   0        0        0       67 2023-03-08 20:36:48.495247 slapdash-1.0.2/slapdash/examples/client_example.py
+-rw-r--r--   0        0        0      131 2022-08-23 15:30:06.060760 slapdash-1.0.2/slapdash/examples/custom_css.css
+-rw-r--r--   0        0        0      322 2023-03-08 20:36:48.486369 slapdash-1.0.2/slapdash/examples/custom_css.py
+-rw-r--r--   0        0        0      278 2023-03-08 20:36:48.906847 slapdash-1.0.2/slapdash/examples/dac_example.py
+-rw-r--r--   0        0        0     1056 2023-03-08 21:15:41.005649 slapdash-1.0.2/slapdash/examples/datastream_example.py
+-rw-r--r--   0        0        0      589 2023-03-08 20:36:48.906954 slapdash-1.0.2/slapdash/examples/device_example.py
+-rw-r--r--   0        0        0      888 2023-03-08 20:36:48.495461 slapdash-1.0.2/slapdash/examples/doc_example.py
+-rw-r--r--   0        0        0      988 2023-03-08 21:15:42.602058 slapdash-1.0.2/slapdash/examples/enum_example.py
+-rw-r--r--   0        0        0     1202 2023-03-08 20:36:48.906907 slapdash-1.0.2/slapdash/examples/example.py
+-rw-r--r--   0        0        0      297 2023-03-08 21:16:05.574366 slapdash-1.0.2/slapdash/examples/hello_world.py
+-rw-r--r--   0        0        0     2059 2023-03-08 21:15:43.451462 slapdash-1.0.2/slapdash/examples/metadata_example.py
+-rw-r--r--   0        0        0     1684 2023-03-08 21:15:44.650882 slapdash-1.0.2/slapdash/examples/readonly_example.py
+-rw-r--r--   0        0        0      515 2023-03-08 20:36:48.906990 slapdash-1.0.2/slapdash/examples/refresh_example.py
+-rw-r--r--   0        0        0      876 2023-03-08 21:14:53.457314 slapdash-1.0.2/slapdash/examples/saver_example.py
+-rw-r--r--   0        0        0      126 2022-08-23 15:30:06.062411 slapdash-1.0.2/slapdash/examples/settings.json
+-rw-r--r--   0        0        0      272 2023-03-08 20:36:50.488583 slapdash-1.0.2/slapdash/examples/simple.py
+-rw-r--r--   0        0        0     2908 2023-03-08 21:15:47.749023 slapdash-1.0.2/slapdash/examples/slider_example.py
+-rw-r--r--   0        0        0      733 2023-03-08 20:36:48.906973 slapdash-1.0.2/slapdash/examples/subcomponents.py
+-rw-r--r--   0        0        0      849 2023-03-08 20:36:48.907040 slapdash-1.0.2/slapdash/examples/trigger_update_example.py
+-rw-r--r--   0        0        0      815 2023-03-08 20:36:48.907173 slapdash-1.0.2/slapdash/examples.py
+-rw-r--r--   0        0        0        0 2023-03-08 21:29:51.082127 slapdash-1.0.2/slapdash/frontend/custom.css
+-rw-r--r--   0        0        0     1093 2023-03-08 21:29:51.105966 slapdash-1.0.2/slapdash/frontend/custom.js
+-rw-r--r--   0        0        0     9178 2023-03-08 21:29:51.100802 slapdash-1.0.2/slapdash/frontend/dashboard.css
+-rw-r--r--   0        0        0   167882 2023-03-08 21:29:51.105003 slapdash-1.0.2/slapdash/frontend/index.css
+-rw-r--r--   0        0        0      472 2023-03-08 21:29:51.100681 slapdash-1.0.2/slapdash/frontend/index.html
+-rw-r--r--   0        0        0  1538596 2023-03-08 21:29:51.298413 slapdash-1.0.2/slapdash/frontend/index.js
+-rw-r--r--   0        0        0       87 2023-03-08 21:26:57.416425 slapdash-1.0.2/slapdash/frontend/package-lock.json
+-rw-r--r--   0        0        0     6415 2023-03-08 21:15:38.722514 slapdash-1.0.2/slapdash/main.py
+-rw-r--r--   0        0        0     5680 2023-03-08 21:15:40.029174 slapdash-1.0.2/slapdash/metadata.py
+-rw-r--r--   0        0        0    21215 2023-03-08 20:32:05.230243 slapdash-1.0.2/slapdash/model.py
+-rw-r--r--   0        0        0     1008 2023-03-08 20:32:00.464892 slapdash-1.0.2/slapdash/testing.py
+-rw-r--r--   0        0        0      253 2022-08-23 15:30:06.086214 slapdash-1.0.2/slapdash/types.py
+-rw-r--r--   0        0        0       45 2023-05-01 22:19:45.824872 slapdash-1.0.2/slapdash/version.json
+-rw-r--r--   0        0        0      874 2022-08-23 15:30:06.086760 slapdash-1.0.2/slapdash/version.py
+-rw-r--r--   0        0        0    13560 2023-03-08 21:14:28.487128 slapdash-1.0.2/slapdash/web.py
+-rw-r--r--   0        0        0     2728 1970-01-01 00:00:00.000000 slapdash-1.0.2/setup.py
+-rw-r--r--   0        0        0     2603 1970-01-01 00:00:00.000000 slapdash-1.0.2/PKG-INFO
```

### Comparing `slapdash-1.0.1/README.md` & `slapdash-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `slapdash-1.0.1/pyproject.toml` & `slapdash-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "slapdash"
-version = "1.0.1"
+version = "1.0.2"
 description = "Create device and application control dashboards instantly"
 authors = ["Matt Grau <graum@phys.ethz.ch>", "Chris Axline <chris@axlines.org>", "Carmelo Mordini <cmordini@phys.ethz.ch>"]
 readme = "README.md"
 packages = [{include = "slapdash"}]
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `slapdash-1.0.1/slapdash/client.py` & `slapdash-1.0.2/slapdash/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import requests
 import re
 import json
 import inspect
 import urllib
 from .model import BASE_TYPES
 from .version import __version__, __major__, __minor__
-
+from typing import Any
 
 class ComClient:
     pass
 
 
 class RequestClient(ComClient):
 
@@ -185,7 +185,54 @@
             elif minor != __minor__:
                 print(
                     f'version mismatch: server is using slapdash version `{version}`, but client is using version `{__version__}`')
         name = client('name')
         props = client('get_props')
 
         return make_class(client, name, props)
+
+
+class SimpleRequestClient:
+    '''Allows direct communication without error-checking or convenience attributes,
+    through `set(name, value)` and `get(name)` methods.'''
+
+    _url: str
+    _timeout: int
+
+    def __init__(self, hostname: str = 'localhost', port: int = 8000, timeout: int = 1):
+        if not (hostname.startswith('http://') or hostname.startswith('https://')):
+            hostname = 'http://' + hostname
+        o = urllib.parse.urlparse(hostname)
+        if o.port is not None:
+            port = o.port
+        self._url = f'{o.scheme}://{o.hostname}:{port}/'
+        self._timeout = timeout
+
+    def get(self, obj):
+        url = self._url
+        timeout = self._timeout
+        return object.__getattribute__(self, '__call__')(url+'get_param?name='+obj, timeout)
+    
+    def set(self, name: str, value: Any) -> None:
+        params = {'value': value}
+        endpoint = re.sub('\]', '', re.sub('\.|\[', '/', name))  # noqa
+        requests.post(self._url + endpoint,
+                      timeout=self._timeout, params=params)
+
+    def __call__(self, method_name: str, timeout=1., **kwargs):
+        req = requests.get(method_name,
+                           timeout=timeout, params=kwargs)
+        try:
+            return req.json()
+        except json.decoder.JSONDecodeError:
+            raise Exception('Server Error: {}'.format(req.text))
+
+class SimpleClient:
+    def __new__(cls,
+                 hostname: str = 'localhost',
+                 port: int = 8000,
+                 timeout: float = 1.):
+
+        client = SimpleRequestClient(hostname=hostname, port=port, timeout=timeout)
+
+        return client
+
```

### Comparing `slapdash-1.0.1/slapdash/decorators.py` & `slapdash-1.0.2/slapdash/decorators.py`

 * *Files identical despite different names*

### Comparing `slapdash-1.0.1/slapdash/examples/async.py` & `slapdash-1.0.2/slapdash/examples/async.py`

 * *Files identical despite different names*

### Comparing `slapdash-1.0.1/slapdash/examples/datastream_example.py` & `slapdash-1.0.2/slapdash/examples/datastream_example.py`

 * *Files identical despite different names*

### Comparing `slapdash-1.0.1/slapdash/examples/device_example.py` & `slapdash-1.0.2/slapdash/examples/device_example.py`

 * *Files identical despite different names*

### Comparing `slapdash-1.0.1/slapdash/examples/doc_example.py` & `slapdash-1.0.2/slapdash/examples/doc_example.py`

 * *Files identical despite different names*

### Comparing `slapdash-1.0.1/slapdash/examples/enum_example.py` & `slapdash-1.0.2/slapdash/examples/enum_example.py`

 * *Files identical despite different names*

### Comparing `slapdash-1.0.1/slapdash/examples/example.py` & `slapdash-1.0.2/slapdash/examples/example.py`

 * *Files identical despite different names*

### Comparing `slapdash-1.0.1/slapdash/examples/metadata_example.py` & `slapdash-1.0.2/slapdash/examples/metadata_example.py`

 * *Files identical despite different names*

### Comparing `slapdash-1.0.1/slapdash/examples/readonly_example.py` & `slapdash-1.0.2/slapdash/examples/readonly_example.py`

 * *Files identical despite different names*

### Comparing `slapdash-1.0.1/slapdash/examples/refresh_example.py` & `slapdash-1.0.2/slapdash/examples/refresh_example.py`

 * *Files identical despite different names*

### Comparing `slapdash-1.0.1/slapdash/examples/saver_example.py` & `slapdash-1.0.2/slapdash/examples/saver_example.py`

 * *Files identical despite different names*

### Comparing `slapdash-1.0.1/slapdash/examples/slider_example.py` & `slapdash-1.0.2/slapdash/examples/slider_example.py`

 * *Files identical despite different names*

### Comparing `slapdash-1.0.1/slapdash/examples/subcomponents.py` & `slapdash-1.0.2/slapdash/examples/subcomponents.py`

 * *Files identical despite different names*

### Comparing `slapdash-1.0.1/slapdash/examples/trigger_update_example.py` & `slapdash-1.0.2/slapdash/examples/trigger_update_example.py`

 * *Files identical despite different names*

### Comparing `slapdash-1.0.1/slapdash/examples.py` & `slapdash-1.0.2/slapdash/examples.py`

 * *Files identical despite different names*

### Comparing `slapdash-1.0.1/slapdash/frontend/custom.js` & `slapdash-1.0.2/slapdash/frontend/custom.js`

 * *Files identical despite different names*

### Comparing `slapdash-1.0.1/slapdash/frontend/dashboard.css` & `slapdash-1.0.2/slapdash/frontend/dashboard.css`

 * *Files identical despite different names*

### Comparing `slapdash-1.0.1/slapdash/frontend/index.css` & `slapdash-1.0.2/slapdash/frontend/index.css`

 * *Files identical despite different names*

### Comparing `slapdash-1.0.1/slapdash/frontend/index.js` & `slapdash-1.0.2/slapdash/frontend/index.js`

 * *Files identical despite different names*

### Comparing `slapdash-1.0.1/slapdash/main.py` & `slapdash-1.0.2/slapdash/main.py`

 * *Files identical despite different names*

### Comparing `slapdash-1.0.1/slapdash/metadata.py` & `slapdash-1.0.2/slapdash/metadata.py`

 * *Files identical despite different names*

### Comparing `slapdash-1.0.1/slapdash/model.py` & `slapdash-1.0.2/slapdash/model.py`

 * *Files identical despite different names*

### Comparing `slapdash-1.0.1/slapdash/testing.py` & `slapdash-1.0.2/slapdash/testing.py`

 * *Files identical despite different names*

### Comparing `slapdash-1.0.1/slapdash/version.py` & `slapdash-1.0.2/slapdash/version.py`

 * *Files identical despite different names*

### Comparing `slapdash-1.0.1/slapdash/web.py` & `slapdash-1.0.2/slapdash/web.py`

 * *Files identical despite different names*

### Comparing `slapdash-1.0.1/setup.py` & `slapdash-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'websockets>=10.4,<11.0']
 
 extras_require = \
 {'examples': ['matplotlib']}
 
 setup_kwargs = {
     'name': 'slapdash',
-    'version': '1.0.1',
+    'version': '1.0.2',
     'description': 'Create device and application control dashboards instantly',
     'long_description': "# Slapdash\n\n**<https://github.com/cathaychris/slapdash/>**\n\nThe Slapdash library lets you create a control dashboard with ease. It takes device driver classes written in simple python and automatically generates\n\n- A web server exposing the class via a RESTful API, that can be accessed with HTTP requests or using the provided clients;\n- An automatically generated fronted rendered in a web page that directly connects to the web server for immediate access;\n- and modularly permits the bootstrapping of other interfaces such as RPC. Bring-Your-Own-Interface.\n\nFor example, it will turn this:\n\n```python\nclass Device:\n\n    _current = 0.0\n    _voltage = 0.0\n    _power = False\n\n    @property\n    def current(self):\n        # run code to get current\n        return self._current\n\n    @current.setter\n    def current(self, value):\n        # run code to set current\n        self._current = value\n\n    @property\n    def voltage(self):\n        # run code to get voltage\n        return self._voltage\n\n    @voltage.setter\n    def voltage(self, value):\n        # run code to set voltage\n        self._voltage = value\n\n    @property\n    def power(self):\n        # run code to get power state\n        return self._power\n\n    @power.setter\n    def power(self, value):\n        # run code to set power state\n        self._power = value\n\n    def reset(self):\n        self.current = 0.0\n        self.voltage = 0.0\n```\n\ninto this:\n\n![](./docs/images/fast-api-example.png)\n\nTry running this example with\n\n```python\nfrom slapdash.examples import run_example\nrun_example('doc_example')\n```\n\n# Credits\n\nSlapdash was developed in the [TIQI group](https://tiqi.ethz.ch/) at ETH Zürich, primarily by [Matt Grau](https://www.odu.edu/directory/matt-grau).\n",
     'author': 'Matt Grau',
     'author_email': 'graum@phys.ethz.ch',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `slapdash-1.0.1/PKG-INFO` & `slapdash-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slapdash
-Version: 1.0.1
+Version: 1.0.2
 Summary: Create device and application control dashboards instantly
 Author: Matt Grau
 Author-email: graum@phys.ethz.ch
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

