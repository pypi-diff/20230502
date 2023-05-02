# Comparing `tmp/pytest_qaseio-1.0.0.tar.gz` & `tmp/pytest_qaseio-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_qaseio-1.0.0.tar", max compression
+gzip compressed data, was "pytest_qaseio-1.0.1.tar", max compression
```

## Comparing `pytest_qaseio-1.0.0.tar` & `pytest_qaseio-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1092 2023-04-06 07:25:14.690639 pytest_qaseio-1.0.0/LICENSE
--rw-r--r--   0        0        0     5444 2023-04-07 04:31:19.166683 pytest_qaseio-1.0.0/README.md
--rw-r--r--   0        0        0     2544 2023-04-07 06:28:49.247424 pytest_qaseio-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-05 13:30:54.606605 pytest_qaseio-1.0.0/pytest_qaseio/__init__.py
--rw-r--r--   0        0        0     2387 2023-04-05 13:30:53.380549 pytest_qaseio-1.0.0/pytest_qaseio/api_client.py
--rw-r--r--   0        0        0      402 2023-04-05 13:30:52.095153 pytest_qaseio-1.0.0/pytest_qaseio/constants.py
--rw-r--r--   0        0        0     8055 2023-04-06 07:51:22.681371 pytest_qaseio-1.0.0/pytest_qaseio/converter.py
--rw-r--r--   0        0        0     3140 2023-04-06 08:04:30.704357 pytest_qaseio-1.0.0/pytest_qaseio/debug_info.py
--rw-r--r--   0        0        0      295 2023-04-05 14:41:26.341327 pytest_qaseio-1.0.0/pytest_qaseio/hooks.py
--rw-r--r--   0        0        0     8448 2023-04-07 06:26:41.054493 pytest_qaseio-1.0.0/pytest_qaseio/plugin.py
--rw-r--r--   0        0        0     1419 2023-04-05 14:02:37.660306 pytest_qaseio-1.0.0/pytest_qaseio/plugin_exceptions.py
--rw-r--r--   0        0        0        0 2023-04-05 13:31:00.616603 pytest_qaseio-1.0.0/pytest_qaseio/py.typed
--rw-r--r--   0        0        0     1156 2023-04-05 13:30:57.987221 pytest_qaseio-1.0.0/pytest_qaseio/storage.py
--rw-r--r--   0        0        0     6369 1970-01-01 00:00:00.000000 pytest_qaseio-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-04-06 07:25:14.690639 pytest_qaseio-1.0.1/LICENSE
+-rw-r--r--   0        0        0     5444 2023-04-07 04:31:19.166683 pytest_qaseio-1.0.1/README.md
+-rw-r--r--   0        0        0     2818 2023-05-02 03:08:38.235157 pytest_qaseio-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-05 13:30:54.606605 pytest_qaseio-1.0.1/pytest_qaseio/__init__.py
+-rw-r--r--   0        0        0     2387 2023-04-05 13:30:53.380549 pytest_qaseio-1.0.1/pytest_qaseio/api_client.py
+-rw-r--r--   0        0        0      402 2023-04-05 13:30:52.095153 pytest_qaseio-1.0.1/pytest_qaseio/constants.py
+-rw-r--r--   0        0        0     8055 2023-04-06 07:51:22.681371 pytest_qaseio-1.0.1/pytest_qaseio/converter.py
+-rw-r--r--   0        0        0     3140 2023-04-06 08:04:30.704357 pytest_qaseio-1.0.1/pytest_qaseio/debug_info.py
+-rw-r--r--   0        0        0      295 2023-04-05 14:41:26.341327 pytest_qaseio-1.0.1/pytest_qaseio/hooks.py
+-rw-r--r--   0        0        0     8448 2023-04-07 06:26:41.054493 pytest_qaseio-1.0.1/pytest_qaseio/plugin.py
+-rw-r--r--   0        0        0     1419 2023-04-05 14:02:37.660306 pytest_qaseio-1.0.1/pytest_qaseio/plugin_exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-05 13:31:00.616603 pytest_qaseio-1.0.1/pytest_qaseio/py.typed
+-rw-r--r--   0        0        0     1156 2023-04-05 13:30:57.987221 pytest_qaseio-1.0.1/pytest_qaseio/storage.py
+-rw-r--r--   0        0        0     6602 1970-01-01 00:00:00.000000 pytest_qaseio-1.0.1/PKG-INFO
```

### Comparing `pytest_qaseio-1.0.0/LICENSE` & `pytest_qaseio-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_qaseio-1.0.0/README.md` & `pytest_qaseio-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pytest_qaseio-1.0.0/pyproject.toml` & `pytest_qaseio-1.0.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,38 @@
 [tool.poetry]
 name = "pytest-qaseio"
 description = "Pytest plugin for Qase.io integration"
-version = "1.0.0"
+version = "1.0.1"
 license = "MIT"
 
-authors = []
+authors = [
+  "Saritasa <pypi@saritasa.com>",
+]
 
 readme = "README.md"
 
+homepage = "https://pypi.org/project/pytest-qaseio/"
 repository = "https://github.com/saritasa-nest/pytest-qaseio"
 
-keywords = []
+keywords = [
+  "pytest",
+  "qase",
+  "qaseio",
+  "selenium",
+  "autotests",
+]
 
 classifiers = [
   "Development Status :: 4 - Beta",
   "Intended Audience :: Developers",
   "Operating System :: OS Independent",
+  "Framework :: Pytest",
   "Topic :: Software Development :: Libraries :: Python Modules",
+  "Topic :: Software Development :: Bug Tracking",
+  "Topic :: Software Development :: Testing",
 ]
 
 [tool.poetry.plugins."pytest11"]
 pytest_qaseio = "pytest_qaseio.plugin"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `pytest_qaseio-1.0.0/pytest_qaseio/api_client.py` & `pytest_qaseio-1.0.1/pytest_qaseio/api_client.py`

 * *Files identical despite different names*

### Comparing `pytest_qaseio-1.0.0/pytest_qaseio/converter.py` & `pytest_qaseio-1.0.1/pytest_qaseio/converter.py`

 * *Files identical despite different names*

### Comparing `pytest_qaseio-1.0.0/pytest_qaseio/debug_info.py` & `pytest_qaseio-1.0.1/pytest_qaseio/debug_info.py`

 * *Files identical despite different names*

### Comparing `pytest_qaseio-1.0.0/pytest_qaseio/plugin.py` & `pytest_qaseio-1.0.1/pytest_qaseio/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_qaseio-1.0.0/pytest_qaseio/plugin_exceptions.py` & `pytest_qaseio-1.0.1/pytest_qaseio/plugin_exceptions.py`

 * *Files identical despite different names*

### Comparing `pytest_qaseio-1.0.0/pytest_qaseio/storage.py` & `pytest_qaseio-1.0.1/pytest_qaseio/storage.py`

 * *Files identical despite different names*

### Comparing `pytest_qaseio-1.0.0/PKG-INFO` & `pytest_qaseio-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 Metadata-Version: 2.1
 Name: pytest-qaseio
-Version: 1.0.0
+Version: 1.0.1
 Summary: Pytest plugin for Qase.io integration
-Home-page: https://github.com/saritasa-nest/pytest-qaseio
+Home-page: https://pypi.org/project/pytest-qaseio/
 License: MIT
+Keywords: pytest,qase,qaseio,selenium,autotests
+Author: Saritasa
+Author-email: pypi@saritasa.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
+Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Bug Tracking
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: Testing
 Requires-Dist: arrow (>=1.2.3,<2.0.0)
 Requires-Dist: filelock (>=3.10.7,<4.0.0)
 Requires-Dist: pytest (>=7.2.2,<8.0.0)
 Requires-Dist: qaseio (>=3.2.1,<4.0.0)
 Requires-Dist: selenium (>=4.8.3,<5.0.0)
 Project-URL: Repository, https://github.com/saritasa-nest/pytest-qaseio
 Description-Content-Type: text/markdown
```

