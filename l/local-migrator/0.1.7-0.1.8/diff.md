# Comparing `tmp/local_migrator-0.1.7.tar.gz` & `tmp/local_migrator-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "local_migrator-0.1.7.tar", last modified: Tue May  2 18:49:57 2023, max compression
+gzip compressed data, was "local_migrator-0.1.8.tar", last modified: Tue May  2 19:49:48 2023, max compression
```

## Comparing `local_migrator-0.1.7.tar` & `local_migrator-0.1.8.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 czaki     (1000) grzegorz  (1000)        0 2023-05-02 18:49:57.479931 local_migrator-0.1.7/
-drwxr-xr-x   0 czaki     (1000) grzegorz  (1000)        0 2023-05-02 18:49:57.475932 local_migrator-0.1.7/.github/
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)      277 2022-09-28 15:55:58.000000 local_migrator-0.1.7/.github/dependabot.yml
-drwxr-xr-x   0 czaki     (1000) grzegorz  (1000)        0 2023-05-02 18:49:57.475932 local_migrator-0.1.7/.github/workflows/
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)     2964 2023-05-02 18:34:23.000000 local_migrator-0.1.7/.github/workflows/tests.yml
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)     5307 2023-05-02 13:22:35.000000 local_migrator-0.1.7/.gitignore
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)      847 2023-05-02 10:23:59.000000 local_migrator-0.1.7/.pre-commit-config.yaml
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)      536 2022-04-01 13:54:50.000000 local_migrator-0.1.7/.readthedocs.yml
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)     1072 2022-04-01 10:45:36.000000 local_migrator-0.1.7/LICENSE.txt
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)     6197 2023-05-02 18:49:57.479931 local_migrator-0.1.7/PKG-INFO
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)     5148 2023-05-02 15:03:59.000000 local_migrator-0.1.7/README.rst
-drwxr-xr-x   0 czaki     (1000) grzegorz  (1000)        0 2023-05-02 18:49:57.475932 local_migrator-0.1.7/docs/
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)      634 2022-03-31 22:32:04.000000 local_migrator-0.1.7/docs/Makefile
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)      162 2022-04-04 08:31:02.000000 local_migrator-0.1.7/docs/api.rst
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)     2346 2023-05-02 13:22:35.000000 local_migrator-0.1.7/docs/conf.py
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)     3660 2022-04-04 09:58:06.000000 local_migrator-0.1.7/docs/examples.rst
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)     1103 2022-04-04 08:49:26.000000 local_migrator-0.1.7/docs/index.rst
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)      800 2022-03-31 22:32:04.000000 local_migrator-0.1.7/docs/make.bat
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)       91 2022-03-31 23:43:40.000000 local_migrator-0.1.7/docs/requirements.txt
-drwxr-xr-x   0 czaki     (1000) grzegorz  (1000)        0 2023-05-02 18:49:57.475932 local_migrator-0.1.7/examples/
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)      414 2023-05-02 13:54:29.000000 local_migrator-0.1.7/examples/base_cbor_example.py
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)      387 2023-05-02 13:49:58.000000 local_migrator-0.1.7/examples/base_example.py
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)     3302 2023-05-02 13:29:07.000000 local_migrator-0.1.7/pyproject.toml
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)       38 2023-05-02 18:49:57.479931 local_migrator-0.1.7/setup.cfg
-drwxr-xr-x   0 czaki     (1000) grzegorz  (1000)        0 2023-05-02 18:49:57.471931 local_migrator-0.1.7/src/
-drwxr-xr-x   0 czaki     (1000) grzegorz  (1000)        0 2023-05-02 18:49:57.475932 local_migrator-0.1.7/src/local_migrator/
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)     1929 2023-05-02 15:03:59.000000 local_migrator-0.1.7/src/local_migrator/__init__.py
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)    13789 2023-05-02 13:42:28.000000 local_migrator-0.1.7/src/local_migrator/_class_register.py
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)     5509 2023-05-02 13:51:08.000000 local_migrator-0.1.7/src/local_migrator/_serialize_hooks.py
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)      260 2023-05-02 13:22:35.000000 local_migrator-0.1.7/src/local_migrator/_testsupport.py
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)      160 2023-05-02 18:49:57.000000 local_migrator-0.1.7/src/local_migrator/version.py
-drwxr-xr-x   0 czaki     (1000) grzegorz  (1000)        0 2023-05-02 18:49:57.475932 local_migrator-0.1.7/src/local_migrator.egg-info/
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)     6197 2023-05-02 18:49:57.000000 local_migrator-0.1.7/src/local_migrator.egg-info/PKG-INFO
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)      895 2023-05-02 18:49:57.000000 local_migrator-0.1.7/src/local_migrator.egg-info/SOURCES.txt
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)        1 2023-05-02 18:49:57.000000 local_migrator-0.1.7/src/local_migrator.egg-info/dependency_links.txt
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)       56 2023-05-02 18:49:57.000000 local_migrator-0.1.7/src/local_migrator.egg-info/entry_points.txt
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)       99 2023-05-02 18:49:57.000000 local_migrator-0.1.7/src/local_migrator.egg-info/requires.txt
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)       21 2023-05-02 18:49:57.000000 local_migrator-0.1.7/src/local_migrator.egg-info/top_level.txt
-drwxr-xr-x   0 czaki     (1000) grzegorz  (1000)        0 2023-05-02 18:49:57.475932 local_migrator-0.1.7/src/tests/
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)       89 2023-05-02 13:22:35.000000 local_migrator-0.1.7/src/tests/class_register_util.py
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)      284 2023-05-02 15:03:59.000000 local_migrator-0.1.7/src/tests/nme_fail.py
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)     3578 2023-05-02 18:34:23.000000 local_migrator-0.1.7/src/tests/test_cbor_hooks.py
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)     5163 2023-05-02 18:34:23.000000 local_migrator-0.1.7/src/tests/test_class_register.py
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)    10214 2023-05-02 18:34:23.000000 local_migrator-0.1.7/src/tests/test_json_hooks.py
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)      467 2023-05-02 15:03:59.000000 local_migrator-0.1.7/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:49:48.273054 local_migrator-0.1.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:49:48.269054 local_migrator-0.1.8/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-02 19:49:25.000000 local_migrator-0.1.8/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:49:48.269054 local_migrator-0.1.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-05-02 19:49:25.000000 local_migrator-0.1.8/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-05-02 19:49:25.000000 local_migrator-0.1.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-02 19:49:25.000000 local_migrator-0.1.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-02 19:49:25.000000 local_migrator-0.1.8/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-02 19:49:25.000000 local_migrator-0.1.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-05-02 19:49:48.273054 local_migrator-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-05-02 19:49:25.000000 local_migrator-0.1.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:49:48.269054 local_migrator-0.1.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-02 19:49:25.000000 local_migrator-0.1.8/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-02 19:49:25.000000 local_migrator-0.1.8/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-05-02 19:49:25.000000 local_migrator-0.1.8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-05-02 19:49:25.000000 local_migrator-0.1.8/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-02 19:49:25.000000 local_migrator-0.1.8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-02 19:49:25.000000 local_migrator-0.1.8/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-02 19:49:25.000000 local_migrator-0.1.8/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:49:48.273054 local_migrator-0.1.8/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-02 19:49:25.000000 local_migrator-0.1.8/examples/base_cbor_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-02 19:49:25.000000 local_migrator-0.1.8/examples/base_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-05-02 19:49:25.000000 local_migrator-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 19:49:48.273054 local_migrator-0.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:49:48.269054 local_migrator-0.1.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:49:48.273054 local_migrator-0.1.8/src/local_migrator/
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-02 19:49:25.000000 local_migrator-0.1.8/src/local_migrator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13789 2023-05-02 19:49:25.000000 local_migrator-0.1.8/src/local_migrator/_class_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-05-02 19:49:25.000000 local_migrator-0.1.8/src/local_migrator/_serialize_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-02 19:49:25.000000 local_migrator-0.1.8/src/local_migrator/_testsupport.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-02 19:49:48.000000 local_migrator-0.1.8/src/local_migrator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:49:48.273054 local_migrator-0.1.8/src/local_migrator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-05-02 19:49:48.000000 local_migrator-0.1.8/src/local_migrator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-02 19:49:48.000000 local_migrator-0.1.8/src/local_migrator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 19:49:48.000000 local_migrator-0.1.8/src/local_migrator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-02 19:49:48.000000 local_migrator-0.1.8/src/local_migrator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-02 19:49:48.000000 local_migrator-0.1.8/src/local_migrator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-02 19:49:48.000000 local_migrator-0.1.8/src/local_migrator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:49:48.273054 local_migrator-0.1.8/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-02 19:49:25.000000 local_migrator-0.1.8/src/tests/class_register_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-02 19:49:25.000000 local_migrator-0.1.8/src/tests/nme_fail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-05-02 19:49:25.000000 local_migrator-0.1.8/src/tests/test_cbor_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-05-02 19:49:25.000000 local_migrator-0.1.8/src/tests/test_class_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10214 2023-05-02 19:49:25.000000 local_migrator-0.1.8/src/tests/test_json_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-02 19:49:25.000000 local_migrator-0.1.8/tox.ini
```

### Comparing `local_migrator-0.1.7/.github/workflows/tests.yml` & `local_migrator-0.1.8/.github/workflows/tests.yml`

 * *Files 10% similar despite different names*

```diff
@@ -84,25 +84,25 @@
   deploy:
     # this will run when you have tagged a commit, starting with "v*"
     # and requires that you have put your twine API key in your
     # github secrets (see readme for details)
     needs: [test]
     runs-on: ubuntu-latest
     if: contains(github.ref, 'tags')
+    permissions:
+      id-token: write
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: "3.x"
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install -U setuptools setuptools_scm wheel twine build
-      - name: Build and publish
-        env:
-          TWINE_USERNAME: __token__
-          TWINE_PASSWORD: ${{ secrets.TWINE_API_KEY }}
+      - name: Build
         run: |
           git tag
           python -m build .
-          twine upload dist/*
+      - name: Publish package distributions to PyPI
+        uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `local_migrator-0.1.7/.gitignore` & `local_migrator-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `local_migrator-0.1.7/.pre-commit-config.yaml` & `local_migrator-0.1.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `local_migrator-0.1.7/.readthedocs.yml` & `local_migrator-0.1.8/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `local_migrator-0.1.7/LICENSE.txt` & `local_migrator-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `local_migrator-0.1.7/PKG-INFO` & `local_migrator-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: local_migrator
-Version: 0.1.7
+Version: 0.1.8
 Summary: Package for simplify data structures migrations
 Author: Grzegorz Bokota
 Author-email: g.bokota@uw.edu.pl
 License: MIT
 Project-URL: Homepage, https://github.com/Czaki/local_migrator
 Project-URL: Documentation, https://local_migrator.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/Czaki/local_migrator
```

### Comparing `local_migrator-0.1.7/README.rst` & `local_migrator-0.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `local_migrator-0.1.7/docs/Makefile` & `local_migrator-0.1.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `local_migrator-0.1.7/docs/conf.py` & `local_migrator-0.1.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `local_migrator-0.1.7/docs/examples.rst` & `local_migrator-0.1.8/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `local_migrator-0.1.7/docs/index.rst` & `local_migrator-0.1.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `local_migrator-0.1.7/docs/make.bat` & `local_migrator-0.1.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `local_migrator-0.1.7/pyproject.toml` & `local_migrator-0.1.8/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -58,14 +58,19 @@
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = ""
 testpaths = [
     "src/tests",
 ]
 
+[tool.setuptools.packages.find]
+where = ["src"]  # list of folders that contain the packages (["."] by default)
+exclude = ["tests"]  # exclude packages matching these glob patterns (empty by default)
+namespaces = false  # to disable scanning PEP 420 namespaces (true by default)
+
 [tool.setuptools_scm]
 write_to = "src/local_migrator/version.py"
 
 [tool.black]
 line-length = 120
 target-version = ['py36']
 include = '\.pyi?$'
```

### Comparing `local_migrator-0.1.7/src/local_migrator/__init__.py` & `local_migrator-0.1.8/src/local_migrator/__init__.py`

 * *Files identical despite different names*

### Comparing `local_migrator-0.1.7/src/local_migrator/_class_register.py` & `local_migrator-0.1.8/src/local_migrator/_class_register.py`

 * *Files identical despite different names*

### Comparing `local_migrator-0.1.7/src/local_migrator/_serialize_hooks.py` & `local_migrator-0.1.8/src/local_migrator/_serialize_hooks.py`

 * *Files identical despite different names*

### Comparing `local_migrator-0.1.7/src/local_migrator.egg-info/PKG-INFO` & `local_migrator-0.1.8/src/local_migrator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: local-migrator
-Version: 0.1.7
+Version: 0.1.8
 Summary: Package for simplify data structures migrations
 Author: Grzegorz Bokota
 Author-email: g.bokota@uw.edu.pl
 License: MIT
 Project-URL: Homepage, https://github.com/Czaki/local_migrator
 Project-URL: Documentation, https://local_migrator.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/Czaki/local_migrator
```

### Comparing `local_migrator-0.1.7/src/local_migrator.egg-info/SOURCES.txt` & `local_migrator-0.1.8/src/local_migrator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `local_migrator-0.1.7/src/tests/test_cbor_hooks.py` & `local_migrator-0.1.8/src/tests/test_cbor_hooks.py`

 * *Files identical despite different names*

### Comparing `local_migrator-0.1.7/src/tests/test_class_register.py` & `local_migrator-0.1.8/src/tests/test_class_register.py`

 * *Files identical despite different names*

### Comparing `local_migrator-0.1.7/src/tests/test_json_hooks.py` & `local_migrator-0.1.8/src/tests/test_json_hooks.py`

 * *Files identical despite different names*

