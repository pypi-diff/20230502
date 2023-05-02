# Comparing `tmp/trove-classifiers-2023.4.29.tar.gz` & `tmp/trove-classifiers-2023.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trove-classifiers-2023.4.29.tar", last modified: Sat Apr 29 04:56:44 2023, max compression
+gzip compressed data, was "trove-classifiers-2023.5.2.tar", last modified: Tue May  2 16:32:33 2023, max compression
```

## Comparing `trove-classifiers-2023.4.29.tar` & `trove-classifiers-2023.5.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 04:56:44.143639 trove-classifiers-2023.4.29/
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-29 04:56:12.000000 trove-classifiers-2023.4.29/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-29 04:56:12.000000 trove-classifiers-2023.4.29/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-29 04:56:12.000000 trove-classifiers-2023.4.29/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-29 04:56:12.000000 trove-classifiers-2023.4.29/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-29 04:56:44.143639 trove-classifiers-2023.4.29/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-29 04:56:12.000000 trove-classifiers-2023.4.29/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 04:56:44.143639 trove-classifiers-2023.4.29/bin/
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-29 04:56:12.000000 trove-classifiers-2023.4.29/bin/sort.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-29 04:56:12.000000 trove-classifiers-2023.4.29/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 04:56:44.143639 trove-classifiers-2023.4.29/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-29 04:56:12.000000 trove-classifiers-2023.4.29/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 04:56:44.143639 trove-classifiers-2023.4.29/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-29 04:56:12.000000 trove-classifiers-2023.4.29/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 04:56:44.143639 trove-classifiers-2023.4.29/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 04:56:44.143639 trove-classifiers-2023.4.29/src/trove_classifiers/
--rw-r--r--   0 runner    (1001) docker     (123)    40017 2023-04-29 04:56:12.000000 trove-classifiers-2023.4.29/src/trove_classifiers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-29 04:56:12.000000 trove-classifiers-2023.4.29/src/trove_classifiers/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 04:56:12.000000 trove-classifiers-2023.4.29/src/trove_classifiers/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 04:56:44.143639 trove-classifiers-2023.4.29/src/trove_classifiers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-29 04:56:44.000000 trove-classifiers-2023.4.29/src/trove_classifiers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-29 04:56:44.000000 trove-classifiers-2023.4.29/src/trove_classifiers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 04:56:44.000000 trove-classifiers-2023.4.29/src/trove_classifiers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-29 04:56:44.000000 trove-classifiers-2023.4.29/src/trove_classifiers.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 04:56:44.143639 trove-classifiers-2023.4.29/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 04:56:12.000000 trove-classifiers-2023.4.29/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 04:56:44.143639 trove-classifiers-2023.4.29/tests/lib/
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-04-29 04:56:12.000000 trove-classifiers-2023.4.29/tests/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-29 04:56:12.000000 trove-classifiers-2023.4.29/tests/lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-04-29 04:56:12.000000 trove-classifiers-2023.4.29/tests/test_classifiers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:32:33.434916 trove-classifiers-2023.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-02 16:31:47.000000 trove-classifiers-2023.5.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-02 16:31:47.000000 trove-classifiers-2023.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-02 16:31:47.000000 trove-classifiers-2023.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-02 16:31:47.000000 trove-classifiers-2023.5.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-02 16:32:33.434916 trove-classifiers-2023.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-02 16:31:47.000000 trove-classifiers-2023.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:32:33.434916 trove-classifiers-2023.5.2/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-02 16:31:47.000000 trove-classifiers-2023.5.2/bin/sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-02 16:31:47.000000 trove-classifiers-2023.5.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:32:33.434916 trove-classifiers-2023.5.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-02 16:31:47.000000 trove-classifiers-2023.5.2/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 16:32:33.434916 trove-classifiers-2023.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-02 16:31:47.000000 trove-classifiers-2023.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:32:33.430916 trove-classifiers-2023.5.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:32:33.434916 trove-classifiers-2023.5.2/src/trove_classifiers/
+-rw-r--r--   0 runner    (1001) docker     (123)    40017 2023-05-02 16:31:47.000000 trove-classifiers-2023.5.2/src/trove_classifiers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-02 16:31:47.000000 trove-classifiers-2023.5.2/src/trove_classifiers/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 16:31:47.000000 trove-classifiers-2023.5.2/src/trove_classifiers/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:32:33.434916 trove-classifiers-2023.5.2/src/trove_classifiers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-02 16:32:33.000000 trove-classifiers-2023.5.2/src/trove_classifiers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-02 16:32:33.000000 trove-classifiers-2023.5.2/src/trove_classifiers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 16:32:33.000000 trove-classifiers-2023.5.2/src/trove_classifiers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-02 16:32:33.000000 trove-classifiers-2023.5.2/src/trove_classifiers.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:32:33.434916 trove-classifiers-2023.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 16:31:47.000000 trove-classifiers-2023.5.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:32:33.434916 trove-classifiers-2023.5.2/tests/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-02 16:31:47.000000 trove-classifiers-2023.5.2/tests/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-02 16:31:47.000000 trove-classifiers-2023.5.2/tests/lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-05-02 16:31:47.000000 trove-classifiers-2023.5.2/tests/test_classifiers.py
```

### Comparing `trove-classifiers-2023.4.29/CONTRIBUTING.md` & `trove-classifiers-2023.5.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `trove-classifiers-2023.4.29/LICENSE` & `trove-classifiers-2023.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trove-classifiers-2023.4.29/Makefile` & `trove-classifiers-2023.5.2/Makefile`

 * *Files identical despite different names*

### Comparing `trove-classifiers-2023.4.29/PKG-INFO` & `trove-classifiers-2023.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trove-classifiers
-Version: 2023.4.29
+Version: 2023.5.2
 Summary: Canonical source for classifiers on PyPI (pypi.org).
 Home-page: https://github.com/pypa/trove-classifiers
 Author: The PyPI Admins
 Author-email: admin@pypi.org
 Keywords: classifiers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `trove-classifiers-2023.4.29/README.md` & `trove-classifiers-2023.5.2/README.md`

 * *Files identical despite different names*

### Comparing `trove-classifiers-2023.4.29/bin/sort.py` & `trove-classifiers-2023.5.2/bin/sort.py`

 * *Files identical despite different names*

### Comparing `trove-classifiers-2023.4.29/setup.py` & `trove-classifiers-2023.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `trove-classifiers-2023.4.29/src/trove_classifiers/__init__.py` & `trove-classifiers-2023.5.2/src/trove_classifiers/__init__.py`

 * *Files identical despite different names*

### Comparing `trove-classifiers-2023.4.29/src/trove_classifiers.egg-info/PKG-INFO` & `trove-classifiers-2023.5.2/src/trove_classifiers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trove-classifiers
-Version: 2023.4.29
+Version: 2023.5.2
 Summary: Canonical source for classifiers on PyPI (pypi.org).
 Home-page: https://github.com/pypa/trove-classifiers
 Author: The PyPI Admins
 Author-email: admin@pypi.org
 Keywords: classifiers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `trove-classifiers-2023.4.29/tests/lib/__init__.py` & `trove-classifiers-2023.5.2/tests/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `trove-classifiers-2023.4.29/tests/test_classifiers.py` & `trove-classifiers-2023.5.2/tests/test_classifiers.py`

 * *Files identical despite different names*

