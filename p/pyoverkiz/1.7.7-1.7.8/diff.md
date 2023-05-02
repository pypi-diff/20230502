# Comparing `tmp/pyoverkiz-1.7.7.tar.gz` & `tmp/pyoverkiz-1.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyoverkiz-1.7.7.tar", max compression
+gzip compressed data, was "pyoverkiz-1.7.8.tar", max compression
```

## Comparing `pyoverkiz-1.7.7.tar` & `pyoverkiz-1.7.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1073 2023-03-04 20:42:39.680526 pyoverkiz-1.7.7/LICENSE
--rw-r--r--   0        0        0     3319 2023-03-04 20:42:39.680526 pyoverkiz-1.7.7/README.md
--rw-r--r--   0        0        0        0 2023-03-04 20:42:39.696526 pyoverkiz-1.7.7/pyoverkiz/__init__.py
--rw-r--r--   0        0        0    30963 2023-03-04 20:42:39.696526 pyoverkiz-1.7.7/pyoverkiz/client.py
--rw-r--r--   0        0        0     3917 2023-03-04 20:42:39.696526 pyoverkiz-1.7.7/pyoverkiz/const.py
--rw-r--r--   0        0        0      220 2023-03-04 20:42:39.696526 pyoverkiz-1.7.7/pyoverkiz/enums/__init__.py
--rw-r--r--   0        0        0     8866 2023-03-04 20:42:39.696526 pyoverkiz-1.7.7/pyoverkiz/enums/command.py
--rw-r--r--   0        0        0     1888 2023-03-04 20:42:39.696526 pyoverkiz-1.7.7/pyoverkiz/enums/execution.py
--rw-r--r--   0        0        0     2945 2023-03-04 20:42:39.696526 pyoverkiz-1.7.7/pyoverkiz/enums/gateway.py
--rw-r--r--   0        0        0    17217 2023-03-04 20:42:39.696526 pyoverkiz-1.7.7/pyoverkiz/enums/general.py
--rw-r--r--   0        0        0     2141 2023-03-04 20:42:39.696526 pyoverkiz-1.7.7/pyoverkiz/enums/measured_value_type.py
--rw-r--r--   0        0        0     1052 2023-03-04 20:42:39.696526 pyoverkiz-1.7.7/pyoverkiz/enums/protocol.py
--rw-r--r--   0        0        0    14019 2023-03-04 20:42:39.696526 pyoverkiz-1.7.7/pyoverkiz/enums/state.py
--rw-r--r--   0        0        0    18302 2023-03-04 20:42:39.696526 pyoverkiz-1.7.7/pyoverkiz/enums/ui.py
--rw-r--r--   0        0        0     1642 2023-03-04 20:42:39.696526 pyoverkiz-1.7.7/pyoverkiz/exceptions.py
--rw-r--r--   0        0        0    24495 2023-03-04 20:42:39.696526 pyoverkiz-1.7.7/pyoverkiz/models.py
--rw-r--r--   0        0        0     1727 2023-03-04 20:42:39.696526 pyoverkiz-1.7.7/pyoverkiz/obfuscate.py
--rw-r--r--   0        0        0        0 2023-03-04 20:42:39.696526 pyoverkiz-1.7.7/pyoverkiz/py.typed
--rw-r--r--   0        0        0      518 2023-03-04 20:42:39.696526 pyoverkiz-1.7.7/pyoverkiz/types.py
--rw-r--r--   0        0        0      987 2023-03-04 20:43:13.197157 pyoverkiz-1.7.7/pyproject.toml
--rw-r--r--   0        0        0     4303 1970-01-01 00:00:00.000000 pyoverkiz-1.7.7/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-02 21:47:25.634441 pyoverkiz-1.7.8/LICENSE
+-rw-r--r--   0        0        0     3319 2023-05-02 21:47:25.634441 pyoverkiz-1.7.8/README.md
+-rw-r--r--   0        0        0        0 2023-05-02 21:47:25.646441 pyoverkiz-1.7.8/pyoverkiz/__init__.py
+-rw-r--r--   0        0        0    30963 2023-05-02 21:47:25.646441 pyoverkiz-1.7.8/pyoverkiz/client.py
+-rw-r--r--   0        0        0     3917 2023-05-02 21:47:25.646441 pyoverkiz-1.7.8/pyoverkiz/const.py
+-rw-r--r--   0        0        0      220 2023-05-02 21:47:25.646441 pyoverkiz-1.7.8/pyoverkiz/enums/__init__.py
+-rw-r--r--   0        0        0     8866 2023-05-02 21:47:25.646441 pyoverkiz-1.7.8/pyoverkiz/enums/command.py
+-rw-r--r--   0        0        0     1888 2023-05-02 21:47:25.646441 pyoverkiz-1.7.8/pyoverkiz/enums/execution.py
+-rw-r--r--   0        0        0     2945 2023-05-02 21:47:25.646441 pyoverkiz-1.7.8/pyoverkiz/enums/gateway.py
+-rw-r--r--   0        0        0    17241 2023-05-02 21:47:25.646441 pyoverkiz-1.7.8/pyoverkiz/enums/general.py
+-rw-r--r--   0        0        0     2141 2023-05-02 21:47:25.646441 pyoverkiz-1.7.8/pyoverkiz/enums/measured_value_type.py
+-rw-r--r--   0        0        0     1052 2023-05-02 21:47:25.646441 pyoverkiz-1.7.8/pyoverkiz/enums/protocol.py
+-rw-r--r--   0        0        0    14019 2023-05-02 21:47:25.646441 pyoverkiz-1.7.8/pyoverkiz/enums/state.py
+-rw-r--r--   0        0        0    18302 2023-05-02 21:47:25.646441 pyoverkiz-1.7.8/pyoverkiz/enums/ui.py
+-rw-r--r--   0        0        0     1642 2023-05-02 21:47:25.646441 pyoverkiz-1.7.8/pyoverkiz/exceptions.py
+-rw-r--r--   0        0        0    24495 2023-05-02 21:47:25.646441 pyoverkiz-1.7.8/pyoverkiz/models.py
+-rw-r--r--   0        0        0     1727 2023-05-02 21:47:25.646441 pyoverkiz-1.7.8/pyoverkiz/obfuscate.py
+-rw-r--r--   0        0        0        0 2023-05-02 21:47:25.646441 pyoverkiz-1.7.8/pyoverkiz/py.typed
+-rw-r--r--   0        0        0      518 2023-05-02 21:47:25.646441 pyoverkiz-1.7.8/pyoverkiz/types.py
+-rw-r--r--   0        0        0      987 2023-05-02 21:47:47.250689 pyoverkiz-1.7.8/pyproject.toml
+-rw-r--r--   0        0        0     4303 1970-01-01 00:00:00.000000 pyoverkiz-1.7.8/PKG-INFO
```

### Comparing `pyoverkiz-1.7.7/LICENSE` & `pyoverkiz-1.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.7.7/README.md` & `pyoverkiz-1.7.8/README.md`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.7.7/pyoverkiz/client.py` & `pyoverkiz-1.7.8/pyoverkiz/client.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.7.7/pyoverkiz/const.py` & `pyoverkiz-1.7.8/pyoverkiz/const.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.7.7/pyoverkiz/enums/command.py` & `pyoverkiz-1.7.8/pyoverkiz/enums/command.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.7.7/pyoverkiz/enums/execution.py` & `pyoverkiz-1.7.8/pyoverkiz/enums/execution.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.7.7/pyoverkiz/enums/gateway.py` & `pyoverkiz-1.7.8/pyoverkiz/enums/gateway.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.7.7/pyoverkiz/enums/general.py` & `pyoverkiz-1.7.8/pyoverkiz/enums/general.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,14 +122,15 @@
     DISCOVER_NO_REMOTE_CONTROLLER_ERROR = 184
     COMMAND_INTERRUPTED = 185
     PRIORITY_LOCK__WIND_FORCING_AVAILABLE = 190
     PRIORITY_LOCK__WIND_FORCING_UNAVAILABLE = 191
     PRIORITY_LOCK__NO_SECURITY_DEVICE = 192
     PRIORITY_LOCK__DEAD_SENSOR = 193
     PRIORITY_LOCK__UNKNOWN_ERROR = 194
+    CMDDEPRECATED = 197
     DBUS_ERROR = 200
     DBUS_NO_MEMORY = 201
     DBUS_SERVICE_UNKNOWN = 202
     DBUS_NAME_HAS_NO_OWNER = 203
     DBUS_NO_REPLY = 204
     DBUS_IO_ERROR = 205
     DBUS_BAD_ADDRESS = 206
```

### Comparing `pyoverkiz-1.7.7/pyoverkiz/enums/measured_value_type.py` & `pyoverkiz-1.7.8/pyoverkiz/enums/measured_value_type.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.7.7/pyoverkiz/enums/protocol.py` & `pyoverkiz-1.7.8/pyoverkiz/enums/protocol.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.7.7/pyoverkiz/enums/state.py` & `pyoverkiz-1.7.8/pyoverkiz/enums/state.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.7.7/pyoverkiz/enums/ui.py` & `pyoverkiz-1.7.8/pyoverkiz/enums/ui.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.7.7/pyoverkiz/exceptions.py` & `pyoverkiz-1.7.8/pyoverkiz/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.7.7/pyoverkiz/models.py` & `pyoverkiz-1.7.8/pyoverkiz/models.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.7.7/pyoverkiz/obfuscate.py` & `pyoverkiz-1.7.8/pyoverkiz/obfuscate.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.7.7/pyoverkiz/types.py` & `pyoverkiz-1.7.8/pyoverkiz/types.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.7.7/pyproject.toml` & `pyoverkiz-1.7.8/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyoverkiz"
-version = "1.7.7"
+version = "1.7.8"
 description = "Async Python client to interact with internal OverKiz API (e.g. used by Somfy TaHoma)."
 authors = ["Mick Vleeshouwer", "Vincent Le Bourlot", "Thibaut Etienne"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/iMicknl/python-overkiz-api"
 repository = "https://github.com/iMicknl/python-overkiz-api"
 packages = [
@@ -13,28 +13,28 @@
 
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4.0"
 aiohttp = "^3.6.1"
 pyhumps = "^3.0.2,!=3.7.3"
 backoff = ">=1.10.0,<3.0"
-attrs = ">=21.2,<23.0"
+attrs = ">=21.2,<24.0"
 boto3 = "^1.18.59"
 warrant-lite = "^1.0.4"
 
 [tool.poetry.dev-dependencies]
 tox = "^3.28"
-pytest = "^7.2"
+pytest = "^7.3"
 pytest-cov = "^4.0.0"
 pre-commit = "^2.21"
 black = {version = "^22.12", allow-prereleases = true}
 pylint = "^2.13.9"
 isort = "^5.11.5"
-mypy = "^1.0"
+mypy = "^1.2"
 flake8 = "^5.0.4"
-pyupgrade = "^3.3.1"
-pytest-asyncio = "^0.20.3"
+pyupgrade = "^3.3.2"
+pytest-asyncio = "^0.21.0"
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pyoverkiz-1.7.7/PKG-INFO` & `pyoverkiz-1.7.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pyoverkiz
-Version: 1.7.7
+Version: 1.7.8
 Summary: Async Python client to interact with internal OverKiz API (e.g. used by Somfy TaHoma).
 Home-page: https://github.com/iMicknl/python-overkiz-api
 License: MIT
 Author: Mick Vleeshouwer
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.6.1,<4.0.0)
-Requires-Dist: attrs (>=21.2,<23.0)
+Requires-Dist: attrs (>=21.2,<24.0)
 Requires-Dist: backoff (>=1.10.0,<3.0)
 Requires-Dist: boto3 (>=1.18.59,<2.0.0)
 Requires-Dist: pyhumps (>=3.0.2,<4.0.0,!=3.7.3)
 Requires-Dist: warrant-lite (>=1.0.4,<2.0.0)
 Project-URL: Repository, https://github.com/iMicknl/python-overkiz-api
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: pyoverkiz Version: 1.7.7 Summary: Async Python
+Metadata-Version: 2.1 Name: pyoverkiz Version: 1.7.8 Summary: Async Python
 client to interact with internal OverKiz API (e.g. used by Somfy TaHoma). Home-
 page: https://github.com/iMicknl/python-overkiz-api License: MIT Author: Mick
 Vleeshouwer Requires-Python: >=3.7,<4.0 Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Dist: aiohttp (>=3.6.1,<4.0.0) Requires-Dist: attrs
-(>=21.2,<23.0) Requires-Dist: backoff (>=1.10.0,<3.0) Requires-Dist: boto3
+(>=21.2,<24.0) Requires-Dist: backoff (>=1.10.0,<3.0) Requires-Dist: boto3
 (>=1.18.59,<2.0.0) Requires-Dist: pyhumps (>=3.0.2,<4.0.0,!=3.7.3) Requires-
 Dist: warrant-lite (>=1.0.4,<2.0.0) Project-URL: Repository, https://
 github.com/iMicknl/python-overkiz-api Description-Content-Type: text/markdown #
 Python client for OverKiz API
 [https://github.com/iMicknl/python-overkiz-api/workflows/CI/badge.svg] [https:/
              /img.shields.io/badge/code%20style-black-000000.svg]
 A fully async and easy to use API client for the (internal) OverKiz API. You
```

