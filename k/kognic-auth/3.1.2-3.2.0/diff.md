# Comparing `tmp/kognic-auth-3.1.2.tar.gz` & `tmp/kognic-auth-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kognic-auth-3.1.2.tar", last modified: Tue Apr 25 14:01:21 2023, max compression
+gzip compressed data, was "kognic-auth-3.2.0.tar", last modified: Tue May  2 12:22:14 2023, max compression
```

## Comparing `kognic-auth-3.1.2.tar` & `kognic-auth-3.2.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:01:21.001928 kognic-auth-3.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:01:20.997928 kognic-auth-3.1.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-25 14:01:06.000000 kognic-auth-3.1.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:01:20.997928 kognic-auth-3.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-25 14:01:06.000000 kognic-auth-3.1.2/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-25 14:01:06.000000 kognic-auth-3.1.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-25 14:01:06.000000 kognic-auth-3.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-25 14:01:06.000000 kognic-auth-3.1.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-04-25 14:01:21.001928 kognic-auth-3.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-25 14:01:06.000000 kognic-auth-3.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-25 14:01:06.000000 kognic-auth-3.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 14:01:21.001928 kognic-auth-3.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:01:20.997928 kognic-auth-3.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:01:20.997928 kognic-auth-3.1.2/src/kognic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:01:20.997928 kognic-auth-3.1.2/src/kognic/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-25 14:01:06.000000 kognic-auth-3.1.2/src/kognic/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-25 14:01:20.000000 kognic-auth-3.1.2/src/kognic/auth/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:01:21.001928 kognic-auth-3.1.2/src/kognic/auth/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:01:06.000000 kognic-auth-3.1.2/src/kognic/auth/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-25 14:01:06.000000 kognic-auth-3.1.2/src/kognic/auth/base/auth_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-04-25 14:01:06.000000 kognic-auth-3.1.2/src/kognic/auth/credentials_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:01:21.001928 kognic-auth-3.1.2/src/kognic/auth/httpx/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:01:06.000000 kognic-auth-3.1.2/src/kognic/auth/httpx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-04-25 14:01:06.000000 kognic-auth-3.1.2/src/kognic/auth/httpx/async_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:01:21.001928 kognic-auth-3.1.2/src/kognic/auth/requests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:01:06.000000 kognic-auth-3.1.2/src/kognic/auth/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-25 14:01:06.000000 kognic-auth-3.1.2/src/kognic/auth/requests/auth_session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:01:21.001928 kognic-auth-3.1.2/src/kognic_auth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-04-25 14:01:20.000000 kognic-auth-3.1.2/src/kognic_auth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-25 14:01:20.000000 kognic-auth-3.1.2/src/kognic_auth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 14:01:20.000000 kognic-auth-3.1.2/src/kognic_auth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-25 14:01:20.000000 kognic-auth-3.1.2/src/kognic_auth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-25 14:01:20.000000 kognic-auth-3.1.2/src/kognic_auth.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:01:21.001928 kognic-auth-3.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-25 14:01:06.000000 kognic-auth-3.1.2/tests/credentials_parser_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:22:14.636991 kognic-auth-3.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:22:14.636991 kognic-auth-3.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-02 12:21:57.000000 kognic-auth-3.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:22:14.636991 kognic-auth-3.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-02 12:21:57.000000 kognic-auth-3.2.0/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-02 12:21:57.000000 kognic-auth-3.2.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-02 12:21:57.000000 kognic-auth-3.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-02 12:21:57.000000 kognic-auth-3.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-02 12:22:14.636991 kognic-auth-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-02 12:21:57.000000 kognic-auth-3.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-02 12:21:57.000000 kognic-auth-3.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 12:22:14.636991 kognic-auth-3.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:22:14.632991 kognic-auth-3.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:22:14.632991 kognic-auth-3.2.0/src/kognic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:22:14.636991 kognic-auth-3.2.0/src/kognic/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-02 12:21:57.000000 kognic-auth-3.2.0/src/kognic/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-02 12:22:14.000000 kognic-auth-3.2.0/src/kognic/auth/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:22:14.636991 kognic-auth-3.2.0/src/kognic/auth/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 12:21:57.000000 kognic-auth-3.2.0/src/kognic/auth/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-02 12:21:57.000000 kognic-auth-3.2.0/src/kognic/auth/base/auth_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-02 12:21:57.000000 kognic-auth-3.2.0/src/kognic/auth/credentials_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:22:14.636991 kognic-auth-3.2.0/src/kognic/auth/httpx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 12:21:57.000000 kognic-auth-3.2.0/src/kognic/auth/httpx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-02 12:21:57.000000 kognic-auth-3.2.0/src/kognic/auth/httpx/async_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:22:14.636991 kognic-auth-3.2.0/src/kognic/auth/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 12:21:57.000000 kognic-auth-3.2.0/src/kognic/auth/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-02 12:21:57.000000 kognic-auth-3.2.0/src/kognic/auth/requests/auth_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:22:14.636991 kognic-auth-3.2.0/src/kognic_auth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-02 12:22:14.000000 kognic-auth-3.2.0/src/kognic_auth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-02 12:22:14.000000 kognic-auth-3.2.0/src/kognic_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 12:22:14.000000 kognic-auth-3.2.0/src/kognic_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-02 12:22:14.000000 kognic-auth-3.2.0/src/kognic_auth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-02 12:22:14.000000 kognic-auth-3.2.0/src/kognic_auth.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:22:14.636991 kognic-auth-3.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-02 12:21:57.000000 kognic-auth-3.2.0/tests/credentials_parser_tests.py
```

### Comparing `kognic-auth-3.1.2/.github/workflows/python-package.yml` & `kognic-auth-3.2.0/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `kognic-auth-3.1.2/.github/workflows/python-publish.yml` & `kognic-auth-3.2.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `kognic-auth-3.1.2/CHANGELOG.md` & `kognic-auth-3.2.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `kognic-auth-3.1.2/PKG-INFO` & `kognic-auth-3.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kognic-auth
-Version: 3.1.2
+Version: 3.2.0
 Summary: Kognic Authentication
 Author-email: Kognic <michel.edkrantz@kognic.com>
 License: MIT
 Project-URL: homepage, https://github.com/annotell/kognic-auth-python
 Keywords: Kognic,API
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `kognic-auth-3.1.2/README.md` & `kognic-auth-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `kognic-auth-3.1.2/pyproject.toml` & `kognic-auth-3.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 name = "kognic-auth"
 dynamic = ["version"]
 authors = [
     { name = "Kognic", email = "michel.edkrantz@kognic.com" },
 ]
 description = "Kognic Authentication"
 dependencies = [
-    "authlib>=0.14.1,<1.1"
+    "authlib>=0.14.1,<1.3"
 ]
 requires-python=">=3.6"
 readme = "README.md"
 keywords = ["Kognic", "API"]
 license = {text = "MIT"}
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `kognic-auth-3.1.2/src/kognic/auth/base/auth_client.py` & `kognic-auth-3.2.0/src/kognic/auth/base/auth_client.py`

 * *Files identical despite different names*

### Comparing `kognic-auth-3.1.2/src/kognic/auth/credentials_parser.py` & `kognic-auth-3.2.0/src/kognic/auth/credentials_parser.py`

 * *Files identical despite different names*

### Comparing `kognic-auth-3.1.2/src/kognic/auth/httpx/async_client.py` & `kognic-auth-3.2.0/src/kognic/auth/httpx/async_client.py`

 * *Files identical despite different names*

### Comparing `kognic-auth-3.1.2/src/kognic/auth/requests/auth_session.py` & `kognic-auth-3.2.0/src/kognic/auth/requests/auth_session.py`

 * *Files identical despite different names*

### Comparing `kognic-auth-3.1.2/src/kognic_auth.egg-info/PKG-INFO` & `kognic-auth-3.2.0/src/kognic_auth.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kognic-auth
-Version: 3.1.2
+Version: 3.2.0
 Summary: Kognic Authentication
 Author-email: Kognic <michel.edkrantz@kognic.com>
 License: MIT
 Project-URL: homepage, https://github.com/annotell/kognic-auth-python
 Keywords: Kognic,API
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `kognic-auth-3.1.2/src/kognic_auth.egg-info/SOURCES.txt` & `kognic-auth-3.2.0/src/kognic_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kognic-auth-3.1.2/tests/credentials_parser_tests.py` & `kognic-auth-3.2.0/tests/credentials_parser_tests.py`

 * *Files identical despite different names*

