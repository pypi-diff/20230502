# Comparing `tmp/requests_oidc-0.4.1.tar.gz` & `tmp/requests_oidc-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requests_oidc-0.4.1.tar", max compression
+gzip compressed data, was "requests_oidc-0.4.2.tar", max compression
```

## Comparing `requests_oidc-0.4.1.tar` & `requests_oidc-0.4.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1054 2023-01-12 17:44:30.444663 requests_oidc-0.4.1/LICENSE
--rw-r--r--   0        0        0     3079 2023-01-10 20:21:29.006848 requests_oidc-0.4.1/README.rst
--rw-r--r--   0        0        0      788 2023-03-28 13:38:04.097921 requests_oidc-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      346 2023-03-21 20:20:34.580513 requests_oidc-0.4.1/src/requests_oidc/__init__.py
--rw-r--r--   0        0        0        0 2023-01-10 17:34:02.957460 requests_oidc-0.4.1/src/requests_oidc/__main__.py
--rw-r--r--   0        0        0       41 2023-03-09 21:03:13.808063 requests_oidc-0.4.1/src/requests_oidc/exceptions.py
--rw-r--r--   0        0        0     5071 2023-03-21 20:20:17.836261 requests_oidc-0.4.1/src/requests_oidc/flows/auth_code.py
--rw-r--r--   0        0        0     1063 2023-03-21 20:15:54.248655 requests_oidc-0.4.1/src/requests_oidc/flows/client_credentials.py
--rw-r--r--   0        0        0     3758 2023-03-21 20:15:54.244655 requests_oidc-0.4.1/src/requests_oidc/flows/device_code.py
--rw-r--r--   0        0        0       67 2023-03-09 21:22:29.684713 requests_oidc-0.4.1/src/requests_oidc/types.py
--rw-r--r--   0        0        0      104 2023-03-09 21:21:42.347700 requests_oidc-0.4.1/src/requests_oidc/utils/__init__.py
--rw-r--r--   0        0        0      930 2023-03-21 19:43:12.789884 requests_oidc-0.4.1/src/requests_oidc/utils/catcher.py
--rw-r--r--   0        0        0      637 2023-03-21 20:15:54.236655 requests_oidc-0.4.1/src/requests_oidc/utils/discovery.py
--rw-r--r--   0        0        0      220 2023-03-21 20:15:54.236655 requests_oidc-0.4.1/src/requests_oidc/utils/scope.py
--rw-r--r--   0        0        0     4004 1970-01-01 00:00:00.000000 requests_oidc-0.4.1/setup.py
--rw-r--r--   0        0        0     4060 1970-01-01 00:00:00.000000 requests_oidc-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1054 2023-01-12 17:44:30.444663 requests_oidc-0.4.2/LICENSE
+-rw-r--r--   0        0        0     3079 2023-01-10 20:21:29.006848 requests_oidc-0.4.2/README.rst
+-rw-r--r--   0        0        0      788 2023-05-02 15:05:53.655940 requests_oidc-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      346 2023-03-21 20:20:34.580513 requests_oidc-0.4.2/src/requests_oidc/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-10 17:34:02.957460 requests_oidc-0.4.2/src/requests_oidc/__main__.py
+-rw-r--r--   0        0        0       41 2023-03-09 21:03:13.808063 requests_oidc-0.4.2/src/requests_oidc/exceptions.py
+-rw-r--r--   0        0        0     5071 2023-03-21 20:20:17.836261 requests_oidc-0.4.2/src/requests_oidc/flows/auth_code.py
+-rw-r--r--   0        0        0     1063 2023-03-21 20:15:54.248655 requests_oidc-0.4.2/src/requests_oidc/flows/client_credentials.py
+-rw-r--r--   0        0        0     3760 2023-05-02 15:01:14.317206 requests_oidc-0.4.2/src/requests_oidc/flows/device_code.py
+-rw-r--r--   0        0        0       67 2023-03-09 21:22:29.684713 requests_oidc-0.4.2/src/requests_oidc/types.py
+-rw-r--r--   0        0        0      104 2023-03-09 21:21:42.347700 requests_oidc-0.4.2/src/requests_oidc/utils/__init__.py
+-rw-r--r--   0        0        0      930 2023-03-21 19:43:12.789884 requests_oidc-0.4.2/src/requests_oidc/utils/catcher.py
+-rw-r--r--   0        0        0      637 2023-03-21 20:15:54.236655 requests_oidc-0.4.2/src/requests_oidc/utils/discovery.py
+-rw-r--r--   0        0        0      220 2023-03-21 20:15:54.236655 requests_oidc-0.4.2/src/requests_oidc/utils/scope.py
+-rw-r--r--   0        0        0     4004 1970-01-01 00:00:00.000000 requests_oidc-0.4.2/setup.py
+-rw-r--r--   0        0        0     4060 1970-01-01 00:00:00.000000 requests_oidc-0.4.2/PKG-INFO
```

### Comparing `requests_oidc-0.4.1/LICENSE` & `requests_oidc-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `requests_oidc-0.4.1/README.rst` & `requests_oidc-0.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `requests_oidc-0.4.1/pyproject.toml` & `requests_oidc-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "requests-oidc"
-version = "0.4.1"
+version = "0.4.2"
 description = ""
 authors = ["Tristan Sweeney <tsweeney@dustidentity.com>"]
 readme = "README.rst"
 packages = [{include = "requests_oidc", from = "src"}]
 repository = "https://github.com/tsweeney-dust/requests-oidc"
 documentation = "https://requests-oidc.readthedocs.io/en/latest/"
 license = "MIT"
```

### Comparing `requests_oidc-0.4.1/src/requests_oidc/flows/auth_code.py` & `requests_oidc-0.4.2/src/requests_oidc/flows/auth_code.py`

 * *Files identical despite different names*

### Comparing `requests_oidc-0.4.1/src/requests_oidc/flows/client_credentials.py` & `requests_oidc-0.4.2/src/requests_oidc/flows/client_credentials.py`

 * *Files identical despite different names*

### Comparing `requests_oidc-0.4.1/src/requests_oidc/flows/device_code.py` & `requests_oidc-0.4.2/src/requests_oidc/flows/device_code.py`

 * *Files 5% similar despite different names*

```diff
@@ -100,15 +100,15 @@
     _prompt_user(
         data["verification_uri"], data["user_code"], data["verification_uri_complete"]
     )
 
     token = _poll_for_token(
         data["expires_in"],
         data["interval"],
-        data["user_code"],
+        data["device_code"],
         client_id,
         urls.token_url,
     )
 
     if token["expires_in"]:
         token["expires_at"] = time.time() + token["expires_in"]
```

### Comparing `requests_oidc-0.4.1/src/requests_oidc/utils/catcher.py` & `requests_oidc-0.4.2/src/requests_oidc/utils/catcher.py`

 * *Files identical despite different names*

### Comparing `requests_oidc-0.4.1/src/requests_oidc/utils/discovery.py` & `requests_oidc-0.4.2/src/requests_oidc/utils/discovery.py`

 * *Files identical despite different names*

### Comparing `requests_oidc-0.4.1/setup.py` & `requests_oidc-0.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ['appdirs>=1.4.4,<2.0.0',
  'qrcode>=7.4.2,<8.0.0',
  'requests-oauthlib>=1.3.1,<2.0.0',
  'requests>=2.28.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'requests-oidc',
-    'version': '0.4.1',
+    'version': '0.4.2',
     'description': '',
     'long_description': 'Requests-OIDC\n=================\n\n.. inclusion-marker-do-not-remove\n\nImplements a simple single-function API for creating a requests ``Session`` that\nmanages your OIDC-discovered OAuth2 session for you.\n\n::\n\n   pip install requests-oidc\n\n\n.. list-table::\n\n   * - Package\n     - |pypi| |license| |py status| |formats| |python| |py impls| |downloads|\n   * - build\n     - |checks| |rtd build| |coverage|\n   * - Git\n     - |last commit| |commit activity| |commits since| |issues| |prs|\n\n.. |pypi| image:: https://img.shields.io/pypi/v/requests-oidc\n   :target: https://pypi.org/project/requests-oidc/\n   :alt: PyPI\n   \n.. |downloads| image:: https://img.shields.io/pypi/dm/requests-oidc\n   :target: https://pypistats.org/packages/requests-oidc\n   :alt: PyPI - Downloads\n\n.. |formats| image:: https://img.shields.io/pypi/format/requests-oidc\n   :target: https://pypi.org/project/requests-oidc/\n   :alt: PyPI - Format\n\n.. |py status| image:: https://img.shields.io/pypi/status/requests-oidc\n   :target: https://pypi.org/project/requests-oidc/\n   :alt: PyPI - Status\n\n.. |py impls| image:: https://img.shields.io/pypi/implementation/requests-oidc\n   :target: https://pypi.org/project/requests-oidc/\n   :alt: PyPI - Implementation\n\n.. |python| image:: https://img.shields.io/pypi/pyversions/requests-oidc\n   :target: https://pypi.org/project/requests-oidc/\n   :alt: PyPI - Python Version\n\n.. |license| image:: https://img.shields.io/github/license/tsweeney-dust/requests-oidc\n   :target: https://github.com/tsweeney-dust/requests-oidc\n   :alt: GitHub\n\n.. |checks| image:: https://img.shields.io/github/checks-status/tsweeney-dust/requests-oidc/main?logo=github\n   :target: https://github.com/tsweeney-dust/requests-oidc\n   :alt: GitHub branch checks state\n\n.. |rtd build| image:: https://img.shields.io/readthedocs/requests-oidc\n   :target: https://requests-oidc.readthedocs.io/en/latest/?badge=latest\n   :alt: Read the Docs\n\n.. |coverage| image:: https://coveralls.io/repos/github/tsweeney-dust/requests-oidc/badge.svg?branch=main\n   :target: https://coveralls.io/github/tsweeney-dust/requests-oidc?branch=main\n   :alt: Coverage\n\n.. |last commit| image:: https://img.shields.io/github/last-commit/tsweeney-dust/requests-oidc\n   :target: https://github.com/tsweeney-dust/requests-oidc\n   :alt: GitHub last commit\n\n.. |commit activity| image:: https://img.shields.io/github/commit-activity/m/tsweeney-dust/requests-oidc\n   :target: https://github.com/tsweeney-dust/requests-oidc\n   :alt: GitHub commit activity\n\n.. |commits since| image:: https://img.shields.io/github/commits-since/tsweeney-dust/requests-oidc/latest\n   :target: https://github.com/tsweeney-dust/requests-oidc\n   :alt: GitHub commits since latest release (by SemVer)\n\n.. |issues| image:: https://img.shields.io/github/issues/tsweeney-dust/requests-oidc\n   :target: https://github.com/tsweeney-dust/requests-oidc/issues\n   :alt: GitHub issues\n\n.. |prs| image:: https://img.shields.io/github/issues-pr/tsweeney-dust/requests-oidc\n   :target: https://github.com/tsweeney-dust/requests-oidc/pulls\n   :alt: GitHub pull requests',
     'author': 'Tristan Sweeney',
     'author_email': 'tsweeney@dustidentity.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/tsweeney-dust/requests-oidc',
```

### Comparing `requests_oidc-0.4.1/PKG-INFO` & `requests_oidc-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requests-oidc
-Version: 0.4.1
+Version: 0.4.2
 Summary: 
 Home-page: https://github.com/tsweeney-dust/requests-oidc
 License: MIT
 Author: Tristan Sweeney
 Author-email: tsweeney@dustidentity.com
 Requires-Python: >=3.7,<4
 Classifier: Development Status :: 3 - Alpha
```

