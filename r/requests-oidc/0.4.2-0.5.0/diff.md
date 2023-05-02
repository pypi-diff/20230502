# Comparing `tmp/requests_oidc-0.4.2.tar.gz` & `tmp/requests_oidc-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requests_oidc-0.4.2.tar", max compression
+gzip compressed data, was "requests_oidc-0.5.0.tar", max compression
```

## Comparing `requests_oidc-0.4.2.tar` & `requests_oidc-0.5.0.tar`

### file list

```diff
@@ -1,16 +1,20 @@
--rw-r--r--   0        0        0     1054 2023-01-12 17:44:30.444663 requests_oidc-0.4.2/LICENSE
--rw-r--r--   0        0        0     3079 2023-01-10 20:21:29.006848 requests_oidc-0.4.2/README.rst
--rw-r--r--   0        0        0      788 2023-05-02 15:05:53.655940 requests_oidc-0.4.2/pyproject.toml
--rw-r--r--   0        0        0      346 2023-03-21 20:20:34.580513 requests_oidc-0.4.2/src/requests_oidc/__init__.py
--rw-r--r--   0        0        0        0 2023-01-10 17:34:02.957460 requests_oidc-0.4.2/src/requests_oidc/__main__.py
--rw-r--r--   0        0        0       41 2023-03-09 21:03:13.808063 requests_oidc-0.4.2/src/requests_oidc/exceptions.py
--rw-r--r--   0        0        0     5071 2023-03-21 20:20:17.836261 requests_oidc-0.4.2/src/requests_oidc/flows/auth_code.py
--rw-r--r--   0        0        0     1063 2023-03-21 20:15:54.248655 requests_oidc-0.4.2/src/requests_oidc/flows/client_credentials.py
--rw-r--r--   0        0        0     3760 2023-05-02 15:01:14.317206 requests_oidc-0.4.2/src/requests_oidc/flows/device_code.py
--rw-r--r--   0        0        0       67 2023-03-09 21:22:29.684713 requests_oidc-0.4.2/src/requests_oidc/types.py
--rw-r--r--   0        0        0      104 2023-03-09 21:21:42.347700 requests_oidc-0.4.2/src/requests_oidc/utils/__init__.py
--rw-r--r--   0        0        0      930 2023-03-21 19:43:12.789884 requests_oidc-0.4.2/src/requests_oidc/utils/catcher.py
--rw-r--r--   0        0        0      637 2023-03-21 20:15:54.236655 requests_oidc-0.4.2/src/requests_oidc/utils/discovery.py
--rw-r--r--   0        0        0      220 2023-03-21 20:15:54.236655 requests_oidc-0.4.2/src/requests_oidc/utils/scope.py
--rw-r--r--   0        0        0     4004 1970-01-01 00:00:00.000000 requests_oidc-0.4.2/setup.py
--rw-r--r--   0        0        0     4060 1970-01-01 00:00:00.000000 requests_oidc-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1054 2023-01-12 17:44:30.444663 requests_oidc-0.5.0/LICENSE
+-rw-r--r--   0        0        0     3079 2023-01-10 20:21:29.006848 requests_oidc-0.5.0/README.rst
+-rw-r--r--   0        0        0      890 2023-05-02 20:31:44.315480 requests_oidc-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      399 2023-05-02 17:03:33.755813 requests_oidc-0.5.0/src/requests_oidc/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-10 17:34:02.957460 requests_oidc-0.5.0/src/requests_oidc/__main__.py
+-rw-r--r--   0        0        0     3292 2023-05-02 20:09:15.339987 requests_oidc-0.5.0/src/requests_oidc/cli.py
+-rw-r--r--   0        0        0       41 2023-03-09 21:03:13.808063 requests_oidc-0.5.0/src/requests_oidc/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-02 16:29:21.372377 requests_oidc-0.5.0/src/requests_oidc/flows/__init__.py
+-rw-r--r--   0        0        0     3285 2023-05-02 20:05:09.358251 requests_oidc-0.5.0/src/requests_oidc/flows/auth_code.py
+-rw-r--r--   0        0        0     1174 2023-05-02 20:03:58.532599 requests_oidc-0.5.0/src/requests_oidc/flows/client_credentials.py
+-rw-r--r--   0        0        0     4021 2023-05-02 20:04:50.713816 requests_oidc-0.5.0/src/requests_oidc/flows/device_code.py
+-rw-r--r--   0        0        0      558 2023-05-02 20:10:42.870029 requests_oidc-0.5.0/src/requests_oidc/flows/utils.py
+-rw-r--r--   0        0        0     1097 2023-05-02 19:25:42.426856 requests_oidc-0.5.0/src/requests_oidc/plugins.py
+-rw-r--r--   0        0        0      170 2023-05-02 18:00:22.770816 requests_oidc-0.5.0/src/requests_oidc/types.py
+-rw-r--r--   0        0        0      104 2023-03-09 21:21:42.347700 requests_oidc-0.5.0/src/requests_oidc/utils/__init__.py
+-rw-r--r--   0        0        0      930 2023-05-02 16:52:14.156034 requests_oidc-0.5.0/src/requests_oidc/utils/catcher.py
+-rw-r--r--   0        0        0      637 2023-03-21 20:15:54.236655 requests_oidc-0.5.0/src/requests_oidc/utils/discovery.py
+-rw-r--r--   0        0        0      220 2023-03-21 20:15:54.236655 requests_oidc-0.5.0/src/requests_oidc/utils/scope.py
+-rw-r--r--   0        0        0     4148 1970-01-01 00:00:00.000000 requests_oidc-0.5.0/setup.py
+-rw-r--r--   0        0        0     4099 1970-01-01 00:00:00.000000 requests_oidc-0.5.0/PKG-INFO
```

### Comparing `requests_oidc-0.4.2/LICENSE` & `requests_oidc-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `requests_oidc-0.4.2/README.rst` & `requests_oidc-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `requests_oidc-0.4.2/pyproject.toml` & `requests_oidc-0.5.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 [tool.poetry]
 name = "requests-oidc"
-version = "0.4.2"
+version = "0.5.0"
 description = ""
 authors = ["Tristan Sweeney <tsweeney@dustidentity.com>"]
 readme = "README.rst"
 packages = [{include = "requests_oidc", from = "src"}]
 repository = "https://github.com/tsweeney-dust/requests-oidc"
 documentation = "https://requests-oidc.readthedocs.io/en/latest/"
 license = "MIT"
 classifiers = [
     "Development Status :: 3 - Alpha"
 ]
 
+[tool.poetry.scripts]
+requests-oidc-cli = "requests_oidc.cli:app"
+
 [tool.poetry.dependencies]
 python = ">=3.7, <4"
 requests = "^2.28.1"
 requests-oauthlib = "^1.3.1"
 appdirs = "^1.4.4"
 qrcode = "^7.4.2"
+typer = "^0.9.0"
 
 
 [tool.poetry.group.dev.dependencies]
 sphinx = ">=5.0.0"
 sphinx-toolbox = "^3.2.0"
 sphinx-copybutton = "^0.5.1"
 types-requests = "^2.28.11.15"
 mypy = "^1.1.1"
+black = "^23.3.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `requests_oidc-0.4.2/src/requests_oidc/flows/client_credentials.py` & `requests_oidc-0.5.0/src/requests_oidc/flows/client_credentials.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 from typing import List, Optional
 
 from oauthlib.oauth2 import BackendApplicationClient
 from requests_oauthlib import OAuth2Session  # type: ignore
 
-from ..types import TokenUpdater
+from ..types import Plugin
 from ..utils import ServerDetails, make_scope
 
 
 def make_client_credentials_session(
     oidc_url: str,
     client_id: str,
     client_secret: str,
-    updater: Optional[TokenUpdater] = None,
     scope: Optional[List[str]] = None,
     *,
     klass=OAuth2Session,
+    plugin: Optional[Plugin] = None,
     **kwargs,
 ) -> OAuth2Session:
     auth_server = ServerDetails.discover(oidc_url)
     client = BackendApplicationClient(client_id=client_id)
+    scope = make_scope(scope)
+
+    def updater(token: dict) -> None:
+        if plugin:
+            plugin.update(token)
+
     session = klass(
         client=client,
         auto_refresh_url=auth_server.token_url,
-        token_updater=updater or (lambda token: None),
-        scope=make_scope(scope),
+        token_updater=updater,
+        scope=scope,
         **kwargs,
     )
 
     def refresh_token(url, *args, **kwargs) -> dict:
         return session.fetch_token(
             url, client_id=client_id, client_secret=client_secret
         )
 
     session.refresh_token = refresh_token
-    refresh_token(auth_server.token_url)
+    token = session.refresh_token(session.auto_refresh_url)
+    updater(token)
 
     return session
```

### Comparing `requests_oidc-0.4.2/src/requests_oidc/flows/device_code.py` & `requests_oidc-0.5.0/src/requests_oidc/flows/device_code.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 from typing import List, Optional
 
 import qrcode  # type: ignore
 import requests
 from requests_oauthlib import OAuth2Session  # type: ignore
 
 from ..exceptions import AuthFlowError
-from ..types import TokenUpdater
+from ..types import Plugin
 from ..utils import ServerDetails, make_scope
+from .utils import refresh_expired, scope_mismatch
 
 
 def _make_qr(msg: str) -> str:
     qr = qrcode.QRCode()
     qr.add_data(msg)
     f = io.StringIO()
     qr.print_ascii(out=f)
@@ -22,16 +23,18 @@
 
 
 def _prompt_user(partial_url: str, user_code: str, full_url: str) -> None:
     webbrowser.open(full_url)
 
     # Stole this prompt from AWS SSO
     print(
-        f"""Attempting to automatically open the SSO authorization page in your default browser.
-If the browser does not open or you wish to use a different device to authorize this request, open the following URL:
+        f"""\
+Attempting to automatically open the SSO authorization page in your default browser.
+If the browser does not open or you wish to use a different device to authorize this
+request, open the following URL:
 
 {partial_url}
 
 Then enter the code:
 
 {user_code}"""
     )
@@ -83,15 +86,15 @@
             res.raise_for_status()
             continue
 
     res.raise_for_status()
     return res.json()
 
 
-def auth_code_flow(
+def device_code_flow(
     urls: ServerDetails, client_id: str, scope: List[str], aud: str
 ) -> dict:
     res = requests.post(
         urls.device_url,
         data={"client_id": client_id, "scope": make_scope(scope), "audience": aud},
     )
     res.raise_for_status()
@@ -116,29 +119,34 @@
 
 
 def make_device_code_session(
     oidc_url: str,
     client_id: str,
     audience: str,
     token: Optional[dict] = None,
-    updater: Optional[TokenUpdater] = None,
     scope: Optional[List[str]] = None,
     *,
     klass=OAuth2Session,
+    plugin: Optional[Plugin] = None,
     **kwargs,
 ):
     auth_server = ServerDetails.discover(oidc_url)
+    scope = make_scope(scope)
 
-    token = auth_code_flow(auth_server, client_id, make_scope(scope), audience)
+    def updater(token: dict) -> None:
+        if plugin:
+            plugin.update(token)
+
+    token = None if plugin is None else plugin.load()
+    if token is None or refresh_expired(token, margin=15) or scope_mismatch(token, scope):
+        token = device_code_flow(auth_server, client_id, scope, audience)
+        updater(token)
 
     session = klass(
         auto_refresh_url=auth_server.token_url,
         auto_refresh_kwargs={"client_id": client_id},
         token=token,
-        token_updater=updater or (lambda token: None),
+        token_updater=updater,
         **kwargs,
     )
 
-    if updater:
-        updater(token)
-
     return session
```

### Comparing `requests_oidc-0.4.2/src/requests_oidc/utils/catcher.py` & `requests_oidc-0.5.0/src/requests_oidc/utils/catcher.py`

 * *Files identical despite different names*

### Comparing `requests_oidc-0.4.2/src/requests_oidc/utils/discovery.py` & `requests_oidc-0.5.0/src/requests_oidc/utils/discovery.py`

 * *Files identical despite different names*

### Comparing `requests_oidc-0.4.2/setup.py` & `requests_oidc-0.5.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,28 +10,33 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['appdirs>=1.4.4,<2.0.0',
  'qrcode>=7.4.2,<8.0.0',
  'requests-oauthlib>=1.3.1,<2.0.0',
- 'requests>=2.28.1,<3.0.0']
+ 'requests>=2.28.1,<3.0.0',
+ 'typer>=0.9.0,<0.10.0']
+
+entry_points = \
+{'console_scripts': ['requests-oidc-cli = requests_oidc.cli:app']}
 
 setup_kwargs = {
     'name': 'requests-oidc',
-    'version': '0.4.2',
+    'version': '0.5.0',
     'description': '',
     'long_description': 'Requests-OIDC\n=================\n\n.. inclusion-marker-do-not-remove\n\nImplements a simple single-function API for creating a requests ``Session`` that\nmanages your OIDC-discovered OAuth2 session for you.\n\n::\n\n   pip install requests-oidc\n\n\n.. list-table::\n\n   * - Package\n     - |pypi| |license| |py status| |formats| |python| |py impls| |downloads|\n   * - build\n     - |checks| |rtd build| |coverage|\n   * - Git\n     - |last commit| |commit activity| |commits since| |issues| |prs|\n\n.. |pypi| image:: https://img.shields.io/pypi/v/requests-oidc\n   :target: https://pypi.org/project/requests-oidc/\n   :alt: PyPI\n   \n.. |downloads| image:: https://img.shields.io/pypi/dm/requests-oidc\n   :target: https://pypistats.org/packages/requests-oidc\n   :alt: PyPI - Downloads\n\n.. |formats| image:: https://img.shields.io/pypi/format/requests-oidc\n   :target: https://pypi.org/project/requests-oidc/\n   :alt: PyPI - Format\n\n.. |py status| image:: https://img.shields.io/pypi/status/requests-oidc\n   :target: https://pypi.org/project/requests-oidc/\n   :alt: PyPI - Status\n\n.. |py impls| image:: https://img.shields.io/pypi/implementation/requests-oidc\n   :target: https://pypi.org/project/requests-oidc/\n   :alt: PyPI - Implementation\n\n.. |python| image:: https://img.shields.io/pypi/pyversions/requests-oidc\n   :target: https://pypi.org/project/requests-oidc/\n   :alt: PyPI - Python Version\n\n.. |license| image:: https://img.shields.io/github/license/tsweeney-dust/requests-oidc\n   :target: https://github.com/tsweeney-dust/requests-oidc\n   :alt: GitHub\n\n.. |checks| image:: https://img.shields.io/github/checks-status/tsweeney-dust/requests-oidc/main?logo=github\n   :target: https://github.com/tsweeney-dust/requests-oidc\n   :alt: GitHub branch checks state\n\n.. |rtd build| image:: https://img.shields.io/readthedocs/requests-oidc\n   :target: https://requests-oidc.readthedocs.io/en/latest/?badge=latest\n   :alt: Read the Docs\n\n.. |coverage| image:: https://coveralls.io/repos/github/tsweeney-dust/requests-oidc/badge.svg?branch=main\n   :target: https://coveralls.io/github/tsweeney-dust/requests-oidc?branch=main\n   :alt: Coverage\n\n.. |last commit| image:: https://img.shields.io/github/last-commit/tsweeney-dust/requests-oidc\n   :target: https://github.com/tsweeney-dust/requests-oidc\n   :alt: GitHub last commit\n\n.. |commit activity| image:: https://img.shields.io/github/commit-activity/m/tsweeney-dust/requests-oidc\n   :target: https://github.com/tsweeney-dust/requests-oidc\n   :alt: GitHub commit activity\n\n.. |commits since| image:: https://img.shields.io/github/commits-since/tsweeney-dust/requests-oidc/latest\n   :target: https://github.com/tsweeney-dust/requests-oidc\n   :alt: GitHub commits since latest release (by SemVer)\n\n.. |issues| image:: https://img.shields.io/github/issues/tsweeney-dust/requests-oidc\n   :target: https://github.com/tsweeney-dust/requests-oidc/issues\n   :alt: GitHub issues\n\n.. |prs| image:: https://img.shields.io/github/issues-pr/tsweeney-dust/requests-oidc\n   :target: https://github.com/tsweeney-dust/requests-oidc/pulls\n   :alt: GitHub pull requests',
     'author': 'Tristan Sweeney',
     'author_email': 'tsweeney@dustidentity.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/tsweeney-dust/requests-oidc',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
+    'entry_points': entry_points,
     'python_requires': '>=3.7,<4',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `requests_oidc-0.4.2/PKG-INFO` & `requests_oidc-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requests-oidc
-Version: 0.4.2
+Version: 0.5.0
 Summary: 
 Home-page: https://github.com/tsweeney-dust/requests-oidc
 License: MIT
 Author: Tristan Sweeney
 Author-email: tsweeney@dustidentity.com
 Requires-Python: >=3.7,<4
 Classifier: Development Status :: 3 - Alpha
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: qrcode (>=7.4.2,<8.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: requests-oauthlib (>=1.3.1,<2.0.0)
+Requires-Dist: typer (>=0.9.0,<0.10.0)
 Project-URL: Documentation, https://requests-oidc.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/tsweeney-dust/requests-oidc
 Description-Content-Type: text/x-rst
 
 Requests-OIDC
 =================
```

