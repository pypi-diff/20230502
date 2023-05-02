# Comparing `tmp/nme-0.1.7.tar.gz` & `tmp/nme-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nme-0.1.7.tar", last modified: Tue May  2 18:27:16 2023, max compression
+gzip compressed data, was "nme-0.1.8.tar", last modified: Tue May  2 20:11:20 2023, max compression
```

## Comparing `nme-0.1.7.tar` & `nme-0.1.8.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 czaki     (1000) grzegorz  (1000)        0 2023-05-02 18:27:16.299731 nme-0.1.7/
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)     3101 2023-05-02 15:28:06.000000 nme-0.1.7/.gitignore
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)     1072 2023-05-02 14:34:16.000000 nme-0.1.7/LICENSE
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)     1040 2023-05-02 18:27:16.299731 nme-0.1.7/PKG-INFO
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)       88 2023-05-02 14:43:09.000000 nme-0.1.7/README.md
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)     1232 2023-05-02 17:22:16.000000 nme-0.1.7/pyproject.toml
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)       38 2023-05-02 18:27:16.299731 nme-0.1.7/setup.cfg
-drwxr-xr-x   0 czaki     (1000) grzegorz  (1000)        0 2023-05-02 18:27:16.299731 nme-0.1.7/src/
-drwxr-xr-x   0 czaki     (1000) grzegorz  (1000)        0 2023-05-02 18:27:16.299731 nme-0.1.7/src/nme.egg-info/
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)     1040 2023-05-02 18:27:16.000000 nme-0.1.7/src/nme.egg-info/PKG-INFO
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)      340 2023-05-02 18:27:16.000000 nme-0.1.7/src/nme.egg-info/SOURCES.txt
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)        1 2023-05-02 18:27:16.000000 nme-0.1.7/src/nme.egg-info/dependency_links.txt
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)       73 2023-05-02 18:27:16.000000 nme-0.1.7/src/nme.egg-info/requires.txt
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)       10 2023-05-02 18:27:16.000000 nme-0.1.7/src/nme.egg-info/top_level.txt
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)      730 2023-05-02 18:22:27.000000 nme-0.1.7/src/nme.py
-drwxr-xr-x   0 czaki     (1000) grzegorz  (1000)        0 2023-05-02 18:27:16.299731 nme-0.1.7/src/tests/
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)       78 2022-09-28 12:57:55.000000 nme-0.1.7/src/tests/class_register_util.py
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)     3644 2023-05-02 15:21:01.000000 nme-0.1.7/src/tests/test_cbor_hooks.py
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)     5104 2023-05-02 15:21:01.000000 nme-0.1.7/src/tests/test_class_register.py
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)     9430 2023-05-02 15:21:55.000000 nme-0.1.7/src/tests/test_json_hooks.py
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)      441 2023-05-02 15:24:32.000000 nme-0.1.7/tox.ini
+drwxr-xr-x   0 czaki     (1000) grzegorz  (1000)        0 2023-05-02 20:11:20.751770 nme-0.1.8/
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)     3101 2023-05-02 15:28:06.000000 nme-0.1.8/.gitignore
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)     1072 2023-05-02 14:34:16.000000 nme-0.1.8/LICENSE
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)     1040 2023-05-02 20:11:20.751770 nme-0.1.8/PKG-INFO
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)       88 2023-05-02 14:43:09.000000 nme-0.1.8/README.md
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)     1483 2023-05-02 20:10:09.000000 nme-0.1.8/pyproject.toml
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)       38 2023-05-02 20:11:20.751770 nme-0.1.8/setup.cfg
+drwxr-xr-x   0 czaki     (1000) grzegorz  (1000)        0 2023-05-02 20:11:20.751770 nme-0.1.8/src/
+drwxr-xr-x   0 czaki     (1000) grzegorz  (1000)        0 2023-05-02 20:11:20.751770 nme-0.1.8/src/nme/
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)      730 2023-05-02 19:29:52.000000 nme-0.1.8/src/nme/__init__.py
+drwxr-xr-x   0 czaki     (1000) grzegorz  (1000)        0 2023-05-02 20:11:20.751770 nme-0.1.8/src/nme.egg-info/
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)     1040 2023-05-02 20:11:20.000000 nme-0.1.8/src/nme.egg-info/PKG-INFO
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)      349 2023-05-02 20:11:20.000000 nme-0.1.8/src/nme.egg-info/SOURCES.txt
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)        1 2023-05-02 20:11:20.000000 nme-0.1.8/src/nme.egg-info/dependency_links.txt
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)       73 2023-05-02 20:11:20.000000 nme-0.1.8/src/nme.egg-info/requires.txt
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)        4 2023-05-02 20:11:20.000000 nme-0.1.8/src/nme.egg-info/top_level.txt
+drwxr-xr-x   0 czaki     (1000) grzegorz  (1000)        0 2023-05-02 20:11:20.751770 nme-0.1.8/src/tests/
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)       78 2022-09-28 12:57:55.000000 nme-0.1.8/src/tests/class_register_util.py
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)     3644 2023-05-02 15:21:01.000000 nme-0.1.8/src/tests/test_cbor_hooks.py
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)     5104 2023-05-02 15:21:01.000000 nme-0.1.8/src/tests/test_class_register.py
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)     9430 2023-05-02 15:21:55.000000 nme-0.1.8/src/tests/test_json_hooks.py
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)      441 2023-05-02 15:24:32.000000 nme-0.1.8/tox.ini
```

### Comparing `nme-0.1.7/.gitignore` & `nme-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `nme-0.1.7/LICENSE` & `nme-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nme-0.1.7/PKG-INFO` & `nme-0.1.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nme
-Version: 0.1.7
+Version: 0.1.8
 Summary: Backward compatybility after change project name to `local_migrator
 Author: Grzegorz Bokota
 Author-email: g.bokota@uw.edu.pl
 License: MIT
 Project-URL: Homepage, https://github.com/Czaki/nme
 Project-URL: Repository, https://github.com/Czaki/nme
 Keywords: migration,persistance
```

### Comparing `nme-0.1.7/pyproject.toml` & `nme-0.1.8/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 # Minimum requirements for the build system to execute.
-requires = ["setuptools>=61.0.0", "wheel>=0.37.0", "setuptools_scm[toml]>=6.4"]  # PEP 508 specifications.
+requires = ["setuptools>=61.0.0", "wheel>=0.37.0"]  # PEP 508 specifications.
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nme"
 description = "Backward compatybility after change project name to `local_migrator"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
 keywords = ["migration", "persistance"]
-version = "0.1.7"
+version = "0.1.8"
 authors = [
   {email = "g.bokota@uw.edu.pl"},
   {name = "Grzegorz Bokota"}
 ]
 maintainers = []
 classifiers = [
   "Development Status :: 3 - Alpha",
@@ -34,11 +34,16 @@
 test = [
   "local_migrator[test]",
 ]
 cbor = [
   "local_migrator[cbor]",
 ]
 
+[tool.setuptools.packages.find]
+where = ["src"]  # list of folders that contain the packages (["."] by default)
+exclude = ["tests"]  # exclude packages matching these glob patterns (empty by default)
+namespaces = false  # to disable scanning PEP 420 namespaces (true by default)
+
 
 [project.urls]
 Homepage = "https://github.com/Czaki/nme"
 Repository = "https://github.com/Czaki/nme"
```

### Comparing `nme-0.1.7/src/nme.egg-info/PKG-INFO` & `nme-0.1.8/src/nme.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nme
-Version: 0.1.7
+Version: 0.1.8
 Summary: Backward compatybility after change project name to `local_migrator
 Author: Grzegorz Bokota
 Author-email: g.bokota@uw.edu.pl
 License: MIT
 Project-URL: Homepage, https://github.com/Czaki/nme
 Project-URL: Repository, https://github.com/Czaki/nme
 Keywords: migration,persistance
```

### Comparing `nme-0.1.7/src/nme.py` & `nme-0.1.8/src/nme/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     nme_cbor_decoder,
 )
 
 warnings.warn("nme is deprecated, use local_migrator instead", DeprecationWarning)
 
 del warnings
 
-__version__ = "0.1.7"
+__version__ = "0.1.8"
 
 __all__ = (
     "class_to_str",
     "check_for_errors_in_dkt_values",
     "register_class",
     "nme_object_hook",
     "rename_key",
```

### Comparing `nme-0.1.7/src/tests/test_cbor_hooks.py` & `nme-0.1.8/src/tests/test_cbor_hooks.py`

 * *Files identical despite different names*

### Comparing `nme-0.1.7/src/tests/test_class_register.py` & `nme-0.1.8/src/tests/test_class_register.py`

 * *Files identical despite different names*

### Comparing `nme-0.1.7/src/tests/test_json_hooks.py` & `nme-0.1.8/src/tests/test_json_hooks.py`

 * *Files identical despite different names*

