# Comparing `tmp/herre-0.3.8.tar.gz` & `tmp/herre-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "herre-0.3.8.tar", max compression
+gzip compressed data, was "herre-0.3.9.tar", max compression
```

## Comparing `herre-0.3.8.tar` & `herre-0.3.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     3343 2022-11-21 11:26:28.582243 herre-0.3.8/README.md
--rw-r--r--   0        0        0       40 2022-03-04 14:40:22.918938 herre-0.3.8/herre/__init__.py
--rw-r--r--   0        0        0      179 2022-06-20 09:03:10.357626 herre-0.3.8/herre/errors.py
--rw-r--r--   0        0        0      182 2022-11-21 11:28:53.254514 herre-0.3.8/herre/grants/__init__.py
--rw-r--r--   0        0        0      550 2022-11-28 16:27:03.394681 herre-0.3.8/herre/grants/base.py
--rw-r--r--   0        0        0      248 2022-11-20 16:10:45.259109 herre-0.3.8/herre/grants/errors.py
--rw-r--r--   0        0        0       88 2022-11-20 16:09:22.899003 herre-0.3.8/herre/grants/fakts/__init__.py
--rw-r--r--   0        0        0     1810 2023-01-18 16:05:51.171823 herre-0.3.8/herre/grants/fakts/fakts_login_screen.py
--rw-r--r--   0        0        0     2171 2023-02-14 16:49:45.064708 herre-0.3.8/herre/grants/fakts/grant.py
--rw-r--r--   0        0        0     1582 2022-11-28 16:10:22.203048 herre-0.3.8/herre/grants/fakts/registry.py
--rw-r--r--   0        0        0       56 2022-11-20 16:09:14.874992 herre-0.3.8/herre/grants/meta/__init__.py
--rw-r--r--   0        0        0     2062 2022-11-28 16:02:14.422771 herre-0.3.8/herre/grants/meta/cache.py
--rw-r--r--   0        0        0      248 2022-11-20 15:08:16.580669 herre-0.3.8/herre/grants/mock.py
--rw-r--r--   0        0        0      243 2022-11-20 16:10:08.871062 herre-0.3.8/herre/grants/oauth2/__init__.py
--rw-r--r--   0        0        0     2794 2022-11-28 16:34:37.159008 herre-0.3.8/herre/grants/oauth2/authorization_code_qt.py
--rw-r--r--   0        0        0     2249 2022-11-28 16:13:52.446718 herre-0.3.8/herre/grants/oauth2/authorization_code_server.py
--rw-r--r--   0        0        0      714 2022-11-20 15:25:33.995881 herre-0.3.8/herre/grants/oauth2/base.py
--rw-r--r--   0        0        0     1279 2022-11-28 16:26:07.786650 herre-0.3.8/herre/grants/oauth2/client_credentials.py
--rw-r--r--   0        0        0      244 2022-11-20 16:11:04.903135 herre-0.3.8/herre/grants/oauth2/errors.py
--rw-r--r--   0        0        0     3366 2022-11-28 16:07:01.875209 herre-0.3.8/herre/grants/oauth2/refresh.py
--rw-r--r--   0        0        0    22125 2022-11-28 16:15:25.006635 herre-0.3.8/herre/grants/oauth2/session.py
--rw-r--r--   0        0        0     2362 2022-11-28 16:32:20.810898 herre-0.3.8/herre/grants/oauth2/utils.py
--rw-r--r--   0        0        0      159 2023-01-16 09:49:33.766216 herre-0.3.8/herre/grants/qt/errors.py
--rw-r--r--   0        0        0     7383 2023-01-18 15:53:59.502693 herre-0.3.8/herre/grants/qt/login_screen.py
--rw-r--r--   0        0        0      216 2022-11-28 16:27:13.862687 herre-0.3.8/herre/grants/static.py
--rw-r--r--   0        0        0     6523 2023-01-19 09:10:32.249672 herre-0.3.8/herre/herre.py
--rw-r--r--   0        0        0      560 2022-11-28 16:06:43.427181 herre-0.3.8/herre/types.py
--rw-r--r--   0        0        0     1376 2023-02-15 09:34:47.287404 herre-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     4399 1970-01-01 00:00:00.000000 herre-0.3.8/setup.py
--rw-r--r--   0        0        0     4251 1970-01-01 00:00:00.000000 herre-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     3343 2022-11-21 11:26:28.582243 herre-0.3.9/README.md
+-rw-r--r--   0        0        0       40 2022-03-04 14:40:22.918938 herre-0.3.9/herre/__init__.py
+-rw-r--r--   0        0        0      179 2022-06-20 09:03:10.357626 herre-0.3.9/herre/errors.py
+-rw-r--r--   0        0        0      182 2022-11-21 11:28:53.254514 herre-0.3.9/herre/grants/__init__.py
+-rw-r--r--   0        0        0      550 2022-11-28 16:27:03.394681 herre-0.3.9/herre/grants/base.py
+-rw-r--r--   0        0        0      248 2022-11-20 16:10:45.259109 herre-0.3.9/herre/grants/errors.py
+-rw-r--r--   0        0        0       88 2022-11-20 16:09:22.899003 herre-0.3.9/herre/grants/fakts/__init__.py
+-rw-r--r--   0        0        0     1808 2023-02-15 17:00:57.718428 herre-0.3.9/herre/grants/fakts/fakts_login_screen.py
+-rw-r--r--   0        0        0     2171 2023-02-14 16:49:45.064708 herre-0.3.9/herre/grants/fakts/grant.py
+-rw-r--r--   0        0        0     1582 2022-11-28 16:10:22.203048 herre-0.3.9/herre/grants/fakts/registry.py
+-rw-r--r--   0        0        0       56 2022-11-20 16:09:14.874992 herre-0.3.9/herre/grants/meta/__init__.py
+-rw-r--r--   0        0        0     2062 2022-11-28 16:02:14.422771 herre-0.3.9/herre/grants/meta/cache.py
+-rw-r--r--   0        0        0      248 2022-11-20 15:08:16.580669 herre-0.3.9/herre/grants/mock.py
+-rw-r--r--   0        0        0      243 2022-11-20 16:10:08.871062 herre-0.3.9/herre/grants/oauth2/__init__.py
+-rw-r--r--   0        0        0     2794 2022-11-28 16:34:37.159008 herre-0.3.9/herre/grants/oauth2/authorization_code_qt.py
+-rw-r--r--   0        0        0     2249 2022-11-28 16:13:52.446718 herre-0.3.9/herre/grants/oauth2/authorization_code_server.py
+-rw-r--r--   0        0        0      714 2022-11-20 15:25:33.995881 herre-0.3.9/herre/grants/oauth2/base.py
+-rw-r--r--   0        0        0     1279 2022-11-28 16:26:07.786650 herre-0.3.9/herre/grants/oauth2/client_credentials.py
+-rw-r--r--   0        0        0      244 2022-11-20 16:11:04.903135 herre-0.3.9/herre/grants/oauth2/errors.py
+-rw-r--r--   0        0        0     3366 2022-11-28 16:07:01.875209 herre-0.3.9/herre/grants/oauth2/refresh.py
+-rw-r--r--   0        0        0    22125 2022-11-28 16:15:25.006635 herre-0.3.9/herre/grants/oauth2/session.py
+-rw-r--r--   0        0        0     2362 2022-11-28 16:32:20.810898 herre-0.3.9/herre/grants/oauth2/utils.py
+-rw-r--r--   0        0        0      159 2023-01-16 09:49:33.766216 herre-0.3.9/herre/grants/qt/errors.py
+-rw-r--r--   0        0        0     7383 2023-01-18 15:53:59.502693 herre-0.3.9/herre/grants/qt/login_screen.py
+-rw-r--r--   0        0        0      216 2022-11-28 16:27:13.862687 herre-0.3.9/herre/grants/static.py
+-rw-r--r--   0        0        0     6523 2023-02-15 17:46:03.002517 herre-0.3.9/herre/herre.py
+-rw-r--r--   0        0        0      560 2022-11-28 16:06:43.427181 herre-0.3.9/herre/types.py
+-rw-r--r--   0        0        0     1376 2023-02-24 17:43:36.325270 herre-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     4399 1970-01-01 00:00:00.000000 herre-0.3.9/setup.py
+-rw-r--r--   0        0        0     4251 1970-01-01 00:00:00.000000 herre-0.3.9/PKG-INFO
```

### Comparing `herre-0.3.8/README.md` & `herre-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `herre-0.3.8/herre/grants/base.py` & `herre-0.3.9/herre/grants/base.py`

 * *Files identical despite different names*

### Comparing `herre-0.3.8/herre/grants/fakts/fakts_login_screen.py` & `herre-0.3.9/herre/grants/fakts/fakts_login_screen.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,25 +8,25 @@
 logger = logging.getLogger(__name__)
 
 
 
 
 class FaktsQtLoginScreen(QtLoginScreen):
     userinfo_endpoint: Optional[str]
-    fakts_group: str = "herre"
+    fakts_group: str = "lok"
     fakts: Optional[Fakts] = None
 
     _userinfo_endpoint = None
 
     """ An ssl context to use for the connection to the endpoint"""
 
     async def aget_userinfo_endpoint(self) -> str:
         fakts = get_current_fakts()
         unserialized = await fakts.aget(self.fakts_group)
-        self.userinfo_endpoint = unserialized["userinfo_endpoint"]
+        self.userinfo_endpoint = unserialized["base_url"] + "/me/"
 
 
 
     async def afetch_user(self, token: Token) -> User:
 
         if not self._userinfo_endpoint:
             self._userinfo_endpoint = await self.aget_userinfo_endpoint()
```

### Comparing `herre-0.3.8/herre/grants/fakts/grant.py` & `herre-0.3.9/herre/grants/fakts/grant.py`

 * *Files identical despite different names*

### Comparing `herre-0.3.8/herre/grants/fakts/registry.py` & `herre-0.3.9/herre/grants/fakts/registry.py`

 * *Files identical despite different names*

### Comparing `herre-0.3.8/herre/grants/meta/cache.py` & `herre-0.3.9/herre/grants/meta/cache.py`

 * *Files identical despite different names*

### Comparing `herre-0.3.8/herre/grants/oauth2/authorization_code_qt.py` & `herre-0.3.9/herre/grants/oauth2/authorization_code_qt.py`

 * *Files identical despite different names*

### Comparing `herre-0.3.8/herre/grants/oauth2/authorization_code_server.py` & `herre-0.3.9/herre/grants/oauth2/authorization_code_server.py`

 * *Files identical despite different names*

### Comparing `herre-0.3.8/herre/grants/oauth2/base.py` & `herre-0.3.9/herre/grants/oauth2/base.py`

 * *Files identical despite different names*

### Comparing `herre-0.3.8/herre/grants/oauth2/client_credentials.py` & `herre-0.3.9/herre/grants/oauth2/client_credentials.py`

 * *Files identical despite different names*

### Comparing `herre-0.3.8/herre/grants/oauth2/refresh.py` & `herre-0.3.9/herre/grants/oauth2/refresh.py`

 * *Files identical despite different names*

### Comparing `herre-0.3.8/herre/grants/oauth2/session.py` & `herre-0.3.9/herre/grants/oauth2/session.py`

 * *Files identical despite different names*

### Comparing `herre-0.3.8/herre/grants/oauth2/utils.py` & `herre-0.3.9/herre/grants/oauth2/utils.py`

 * *Files identical despite different names*

### Comparing `herre-0.3.8/herre/grants/qt/login_screen.py` & `herre-0.3.9/herre/grants/qt/login_screen.py`

 * *Files identical despite different names*

### Comparing `herre-0.3.8/herre/herre.py` & `herre-0.3.9/herre/herre.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 logger = logging.getLogger(__name__)
 
 
 class Herre(KoiledModel):
     """Herre is a client for Token authentication.
 
-    It provides a unified, compsoable interface for token based authentication based on grant.
+    It provides a unified, composable interface for token based authentication based on grant.
     A grant is a class that is able to retrieve a token. Importantly grants do not have to
     directly call the token endpoint. They can also use a cache or other means to retrieve the
     token.
 
     Herre is a context manager. This allows it both to provide itself as a singleton and handle
     the asynchronous interface of the grant. As well as providing a lock to ensure that only one
     request is happening at a time.
```

### Comparing `herre-0.3.8/herre/types.py` & `herre-0.3.9/herre/types.py`

 * *Files identical despite different names*

### Comparing `herre-0.3.8/pyproject.toml` & `herre-0.3.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "herre"
-version = "0.3.8"
+version = "0.3.9"
 readme = "README.md"
 description = "oauth2/openid client tailored to pyqt and async environments"
 authors = ["jhnnsrs <jhnnsrs@gmail.com>"]
 license = "CC BY-NC 3.0"
 packages = [{ include = "herre" }]
 
 [tool.poetry.dependencies]
```

### Comparing `herre-0.3.8/setup.py` & `herre-0.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'pydantic>=1.9.0,<2.0.0']
 
 extras_require = \
 {'fakts': ['fakts>=0.2.13,<0.3.0'], 'qt': ['QtPy>=2.0.1,<3.0.0']}
 
 setup_kwargs = {
     'name': 'herre',
-    'version': '0.3.8',
+    'version': '0.3.9',
     'description': 'oauth2/openid client tailored to pyqt and async environments',
     'long_description': '# herre\n\n[![codecov](https://codecov.io/gh/jhnnsrs/herre/branch/master/graph/badge.svg?token=UGXEA2THBV)](https://codecov.io/gh/jhnnsrs/herre)\n[![PyPI version](https://badge.fury.io/py/herre.svg)](https://pypi.org/project/herre/)\n![Maintainer](https://img.shields.io/badge/maintainer-jhnnsrs-blue)\n[![PyPI pyversions](https://img.shields.io/pypi/pyversions/herre.svg)](https://pypi.python.org/pypi/herre/)\n[![PyPI status](https://img.shields.io/pypi/status/herre.svg)](https://pypi.python.org/pypi/herre/)\n[![PyPI download month](https://img.shields.io/pypi/dm/herre.svg)](https://pypi.python.org/pypi/herre/)\n\n#### DEVELOPMENT\n\n## Idea\n\nherre is an (asynchronous) client for token authentication through oauth2 (and potentially other protocols).\n\n## Prerequisites\n\nherre needs a oauth2/opendid server to connect to\n\n## Supports\n\n- Authorization Code Flow (PKCE)\n  - Within a Qt app through a QtWebengine View\n  - With a Redirect Server\n- Client-Credentials Flow\n\n## Usage\n\nIn order to initialize the Client you need to specify a specific grant to retrieve the code. A grant constitutes\na way of retrieving a Token in an asynchronous manner.\n\n```python\nfrom herre import Herre\nfrom herre.grants.oauth2.authorization_code_server import AuthorizationCodeServer\n\nclient = Herre(\n    grant=AuthorizationCodeServerGrant(base_url="https://your_server/oauth_path",\n    client_id="$YOUR_CLIENT_ID",\n    client_secret="$YOUR_CLIENT_SECRET",)\n)\n\nwith client:\n  client.login()\n\n```\n\nAsync usage\n\n```python\n\nclient = Herre(\n    grant=AuthorizationCodeServerGrant(base_url="https://your_server/oauth_path",\n    client_id="$YOUR_CLIENT_ID",\n    client_secret="$YOUR_CLIENT_SECRET",\n    redirect_uri="http://localhost:6767)\n)\n\nasync with client as c:\n  await c.login()\n\n```\n\n## Composability\n\nHerre grants provide a simple interface to be composable and enable caching, or support for refresh tokens:\n\n```python\nclient = Herre(\n    grant=CacheGrant(\n      grant=AuthorizationCodeServerGrant(base_url="https://your_server/oauth_path",\n          client_id="$YOUR_CLIENT_ID",\n          client_secret="$YOUR_CLIENT_SECRET",\n          redirect_uri="http://localhost:6767")\n))\n\nasync with client:\n  await client.login()\n```\n\nPlease check out the documentation for the meta grants to see how to enable custom logic.\n\n## Intergration with Qt\n\nherre fully supports qt-based applications (both PySide2 and PyQt5) as well as a a redirect_flow for authentication in a webengine powered qt window Authoriation Code Flow (needs pyqtwebengine as additional dependency) ( you can still use the authorization code server if so desired)\n\n```python\nclass MainWindow(QtWidget)\n\n    def __init__(self, *args, **kwargs):\n        self.herre = Herre(\n          grant=AuthorizationCodeQtGrant(\n            base_url="https://your_server/oauth_path",\n            client_id="$YOUR_CLIENT_ID",\n            client_secret="$YOUR_CLIENT_SECRET",\n            redirect_uri="about:blank,)\n        )\n\n        self.herre.enter() #programmatically enter context (make sure to call exit)\n\n\n    def login()\n        self.herre.login()\n```\n\n## Build with\n\n- [koil](https://github.com/jhnnsrs/koil) - for pyqt event loop handling\n- [oauthlib](https://github.com/oauthlib/oauthlib) - for oauth2 compliance\n- [aiohttp](https://github.com/aio-libs/aiohttp) - transport layer (especially redirect server)\n',
     'author': 'jhnnsrs',
     'author_email': 'jhnnsrs@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `herre-0.3.8/PKG-INFO` & `herre-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: herre
-Version: 0.3.8
+Version: 0.3.9
 Summary: oauth2/openid client tailored to pyqt and async environments
 License: CC BY-NC 3.0
 Author: jhnnsrs
 Author-email: jhnnsrs@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

