# Comparing `tmp/start_github-0.0.1.tar.gz` & `tmp/start_github-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "start_github-0.0.1.tar", max compression
+gzip compressed data, was "start_github-0.0.2.tar", max compression
```

## Comparing `start_github-0.0.1.tar` & `start_github-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      250 2023-05-01 03:47:30.094454 start_github-0.0.1/README.md
--rw-r--r--   0        0        0     1510 2023-05-01 03:13:10.160668 start_github-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       90 2023-05-01 04:18:33.402119 start_github-0.0.1/start_github/__init__.py
--rw-r--r--   0        0        0     3621 2023-05-01 03:28:29.631605 start_github-0.0.1/start_github/main.py
--rw-r--r--   0        0        0     1370 2023-05-01 03:41:38.920891 start_github-0.0.1/start_github/repository.py
--rw-r--r--   0        0        0     1057 1970-01-01 00:00:00.000000 start_github-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      250 2023-05-01 03:47:30.094454 start_github-0.0.2/README.md
+-rw-r--r--   0        0        0     1508 2023-05-02 05:04:29.478303 start_github-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       90 2023-05-02 05:04:32.439000 start_github-0.0.2/start_github/__init__.py
+-rw-r--r--   0        0        0     3621 2023-05-01 03:28:29.631605 start_github-0.0.2/start_github/main.py
+-rw-r--r--   0        0        0     2046 2023-05-02 05:10:40.522844 start_github-0.0.2/start_github/repository.py
+-rw-r--r--   0        0        0     1002 1970-01-01 00:00:00.000000 start_github-0.0.2/PKG-INFO
```

### Comparing `start_github-0.0.1/pyproject.toml` & `start_github-0.0.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "start-github"
 description = "Use Github Token to Access API"
-version = "0.0.1"
+version = "0.0.2"
 authors = ["Marcelino G. Veloso III <mars@veloso.one>"]
 readme = "README.md"
 homepage = "https://mv3.dev"
 repository = "https://github.com/justmars/start-github"
 documentation = "https://mv3.dev/start-github"
 classifiers = [
   "Programming Language :: Python :: 3.11",
   "Typing :: Typed",
   "Development Status :: 4 - Beta",
   "Framework :: Pytest",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.11"
 python-dotenv = "^1.0"
-httpx = "^0.24.0"
+httpx = "^0.24"
 pydantic = "^1.10.7"
 
 [tool.poetry.group.dev.dependencies]
 rich = "^13.3"
 pytest = "^7.2"
 pytest-datadir = "^1.4"
 pytest-cov = "^2.12"
```

### Comparing `start_github-0.0.1/start_github/main.py` & `start_github-0.0.2/start_github/main.py`

 * *Files identical despite different names*

### Comparing `start_github-0.0.1/PKG-INFO` & `start_github-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: start-github
-Version: 0.0.1
+Version: 0.0.2
 Summary: Use Github Token to Access API
 Home-page: https://mv3.dev
 Author: Marcelino G. Veloso III
 Author-email: mars@veloso.one
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
-Requires-Dist: httpx (>=0.24.0,<0.25.0)
+Requires-Dist: httpx (>=0.24,<0.25)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0,<2.0)
 Project-URL: Documentation, https://mv3.dev/start-github
 Project-URL: Repository, https://github.com/justmars/start-github
 Description-Content-Type: text/markdown
 
 # start-github
```

