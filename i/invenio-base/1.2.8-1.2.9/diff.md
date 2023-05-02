# Comparing `tmp/invenio-base-1.2.8.tar.gz` & `tmp/invenio-base-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/invenio-base/invenio-base/dist/tmpwul8i8s3/invenio-base-1.2.8.tar", last modified: Mon Feb 21 15:54:22 2022, max compression
+gzip compressed data, was "/home/runner/work/invenio-base/invenio-base/dist/tmpakiwwrle/invenio-base-1.2.9.tar", last modified: Tue Feb 22 17:06:21 2022, max compression
```

## Comparing `invenio-base-1.2.8.tar` & `invenio-base-1.2.9.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-21 15:54:22.000000 invenio-base-1.2.8/
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-02-21 15:54:10.000000 invenio-base-1.2.8/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (121)      832 2022-02-21 15:54:10.000000 invenio-base-1.2.8/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (121)      559 2022-02-21 15:54:10.000000 invenio-base-1.2.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2727 2022-02-21 15:54:10.000000 invenio-base-1.2.8/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3705 2022-02-21 15:54:10.000000 invenio-base-1.2.8/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)      507 2022-02-21 15:54:10.000000 invenio-base-1.2.8/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-02-21 15:54:10.000000 invenio-base-1.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      775 2022-02-21 15:54:10.000000 invenio-base-1.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4160 2022-02-21 15:54:22.000000 invenio-base-1.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1000 2022-02-21 15:54:10.000000 invenio-base-1.2.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-21 15:54:22.000000 invenio-base-1.2.8/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     7433 2022-02-21 15:54:10.000000 invenio-base-1.2.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      484 2022-02-21 15:54:10.000000 invenio-base-1.2.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-02-21 15:54:10.000000 invenio-base-1.2.8/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-02-21 15:54:10.000000 invenio-base-1.2.8/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (121)    10141 2022-02-21 15:54:10.000000 invenio-base-1.2.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      252 2022-02-21 15:54:10.000000 invenio-base-1.2.8/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)      809 2022-02-21 15:54:10.000000 invenio-base-1.2.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-02-21 15:54:10.000000 invenio-base-1.2.8/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)      253 2022-02-21 15:54:10.000000 invenio-base-1.2.8/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6993 2022-02-21 15:54:10.000000 invenio-base-1.2.8/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-02-21 15:54:10.000000 invenio-base-1.2.8/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      261 2022-02-21 15:54:10.000000 invenio-base-1.2.8/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-21 15:54:22.000000 invenio-base-1.2.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     2358 2022-02-21 15:54:10.000000 invenio-base-1.2.8/examples/app.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-21 15:54:22.000000 invenio-base-1.2.8/invenio_base/
--rw-r--r--   0 runner    (1001) docker     (121)     7332 2022-02-21 15:54:10.000000 invenio-base-1.2.8/invenio_base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      384 2022-02-21 15:54:10.000000 invenio-base-1.2.8/invenio_base/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9893 2022-02-21 15:54:10.000000 invenio-base-1.2.8/invenio_base/app.py
--rw-r--r--   0 runner    (1001) docker     (121)     3082 2022-02-21 15:54:10.000000 invenio-base-1.2.8/invenio_base/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)      976 2022-02-21 15:54:10.000000 invenio-base-1.2.8/invenio_base/signals.py
--rw-r--r--   0 runner    (1001) docker     (121)     1196 2022-02-21 15:54:10.000000 invenio-base-1.2.8/invenio_base/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3919 2022-02-21 15:54:10.000000 invenio-base-1.2.8/invenio_base/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-21 15:54:22.000000 invenio-base-1.2.8/invenio_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4160 2022-02-21 15:54:22.000000 invenio-base-1.2.8/invenio_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      911 2022-02-21 15:54:22.000000 invenio-base-1.2.8/invenio_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-21 15:54:22.000000 invenio-base-1.2.8/invenio_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      115 2022-02-21 15:54:22.000000 invenio-base-1.2.8/invenio_base.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-21 15:54:21.000000 invenio-base-1.2.8/invenio_base.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-02-21 15:54:22.000000 invenio-base-1.2.8/invenio_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-02-21 15:54:22.000000 invenio-base-1.2.8/invenio_base.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-02-21 15:54:10.000000 invenio-base-1.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      468 2022-02-21 15:54:10.000000 invenio-base-1.2.8/pytest.ini
--rwxr-xr-x   0 runner    (1001) docker     (121)      458 2022-02-21 15:54:10.000000 invenio-base-1.2.8/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-02-21 15:54:22.000000 invenio-base-1.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      268 2022-02-21 15:54:10.000000 invenio-base-1.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-21 15:54:22.000000 invenio-base-1.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      432 2022-02-21 15:54:10.000000 invenio-base-1.2.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)    11862 2022-02-21 15:54:10.000000 invenio-base-1.2.8/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (121)     5292 2022-02-21 15:54:10.000000 invenio-base-1.2.8/tests/test_cmd.py
--rw-r--r--   0 runner    (1001) docker     (121)     1043 2022-02-21 15:54:10.000000 invenio-base-1.2.8/tests/test_signals.py
--rw-r--r--   0 runner    (1001) docker     (121)     1247 2022-02-21 15:54:10.000000 invenio-base-1.2.8/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3817 2022-02-21 15:54:10.000000 invenio-base-1.2.8/tests/test_wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 17:06:21.000000 invenio-base-1.2.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      124 2022-02-22 17:06:10.000000 invenio-base-1.2.9/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (121)      832 2022-02-22 17:06:10.000000 invenio-base-1.2.9/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (121)      559 2022-02-22 17:06:10.000000 invenio-base-1.2.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2860 2022-02-22 17:06:10.000000 invenio-base-1.2.9/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3705 2022-02-22 17:06:10.000000 invenio-base-1.2.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      507 2022-02-22 17:06:10.000000 invenio-base-1.2.9/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-02-22 17:06:10.000000 invenio-base-1.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      775 2022-02-22 17:06:10.000000 invenio-base-1.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     4293 2022-02-22 17:06:21.000000 invenio-base-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1000 2022-02-22 17:06:10.000000 invenio-base-1.2.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 17:06:21.000000 invenio-base-1.2.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)     7433 2022-02-22 17:06:10.000000 invenio-base-1.2.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)      484 2022-02-22 17:06:10.000000 invenio-base-1.2.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      247 2022-02-22 17:06:10.000000 invenio-base-1.2.9/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      247 2022-02-22 17:06:10.000000 invenio-base-1.2.9/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    10141 2022-02-22 17:06:10.000000 invenio-base-1.2.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      252 2022-02-22 17:06:10.000000 invenio-base-1.2.9/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      809 2022-02-22 17:06:10.000000 invenio-base-1.2.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      247 2022-02-22 17:06:10.000000 invenio-base-1.2.9/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      253 2022-02-22 17:06:10.000000 invenio-base-1.2.9/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     6993 2022-02-22 17:06:10.000000 invenio-base-1.2.9/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2022-02-22 17:06:10.000000 invenio-base-1.2.9/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      261 2022-02-22 17:06:10.000000 invenio-base-1.2.9/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 17:06:21.000000 invenio-base-1.2.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     2358 2022-02-22 17:06:10.000000 invenio-base-1.2.9/examples/app.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 17:06:21.000000 invenio-base-1.2.9/invenio_base/
+-rw-r--r--   0 runner    (1001) docker     (121)     7332 2022-02-22 17:06:10.000000 invenio-base-1.2.9/invenio_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      384 2022-02-22 17:06:10.000000 invenio-base-1.2.9/invenio_base/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9903 2022-02-22 17:06:10.000000 invenio-base-1.2.9/invenio_base/app.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3082 2022-02-22 17:06:10.000000 invenio-base-1.2.9/invenio_base/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)      976 2022-02-22 17:06:10.000000 invenio-base-1.2.9/invenio_base/signals.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1196 2022-02-22 17:06:10.000000 invenio-base-1.2.9/invenio_base/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3919 2022-02-22 17:06:10.000000 invenio-base-1.2.9/invenio_base/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 17:06:21.000000 invenio-base-1.2.9/invenio_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4293 2022-02-22 17:06:20.000000 invenio-base-1.2.9/invenio_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      911 2022-02-22 17:06:21.000000 invenio-base-1.2.9/invenio_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-22 17:06:20.000000 invenio-base-1.2.9/invenio_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      115 2022-02-22 17:06:20.000000 invenio-base-1.2.9/invenio_base.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-22 17:06:19.000000 invenio-base-1.2.9/invenio_base.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      191 2022-02-22 17:06:20.000000 invenio-base-1.2.9/invenio_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2022-02-22 17:06:21.000000 invenio-base-1.2.9/invenio_base.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       90 2022-02-22 17:06:10.000000 invenio-base-1.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      468 2022-02-22 17:06:10.000000 invenio-base-1.2.9/pytest.ini
+-rwxr-xr-x   0 runner    (1001) docker     (121)      458 2022-02-22 17:06:10.000000 invenio-base-1.2.9/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-02-22 17:06:21.000000 invenio-base-1.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      268 2022-02-22 17:06:10.000000 invenio-base-1.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 17:06:21.000000 invenio-base-1.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      432 2022-02-22 17:06:10.000000 invenio-base-1.2.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11862 2022-02-22 17:06:10.000000 invenio-base-1.2.9/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5292 2022-02-22 17:06:10.000000 invenio-base-1.2.9/tests/test_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1043 2022-02-22 17:06:10.000000 invenio-base-1.2.9/tests/test_signals.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1247 2022-02-22 17:06:10.000000 invenio-base-1.2.9/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3817 2022-02-22 17:06:10.000000 invenio-base-1.2.9/tests/test_wsgi.py
```

### Comparing `invenio-base-1.2.8/.editorconfig` & `invenio-base-1.2.9/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-base-1.2.8/AUTHORS.rst` & `invenio-base-1.2.9/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `invenio-base-1.2.8/CHANGES.rst` & `invenio-base-1.2.9/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 
     Invenio is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version 1.2.9 (released 2022-02-22)
+
+- Fixes issue with duplicate entry points during tests due to pytest
+  modifying the sys.path.
+
 Version 1.2.8 (released 2022-02-21)
 
 - Lowered Python requirement to v3.6 to avoid breaking builds.
 
 Version 1.2.7 (released 2022-02-21)
 
 - Fixed minimal test dependencies and limited itsdangerous to <2.1
```

### Comparing `invenio-base-1.2.8/CONTRIBUTING.rst` & `invenio-base-1.2.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-base-1.2.8/LICENSE` & `invenio-base-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-base-1.2.8/MANIFEST.in` & `invenio-base-1.2.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-base-1.2.8/PKG-INFO` & `invenio-base-1.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-base
-Version: 1.2.8
+Version: 1.2.9
 Summary: "Base package for building Invenio application factories."
 Home-page: https://github.com/inveniosoftware/invenio-base
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Keywords: invenio
 Platform: any
@@ -48,14 +48,19 @@
 
     Invenio is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version 1.2.9 (released 2022-02-22)
+
+- Fixes issue with duplicate entry points during tests due to pytest
+  modifying the sys.path.
+
 Version 1.2.8 (released 2022-02-21)
 
 - Lowered Python requirement to v3.6 to avoid breaking builds.
 
 Version 1.2.7 (released 2022-02-21)
 
 - Fixed minimal test dependencies and limited itsdangerous to <2.1
```

### Comparing `invenio-base-1.2.8/README.rst` & `invenio-base-1.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-base-1.2.8/docs/Makefile` & `invenio-base-1.2.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-base-1.2.8/docs/conf.py` & `invenio-base-1.2.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-base-1.2.8/docs/index.rst` & `invenio-base-1.2.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-base-1.2.8/docs/make.bat` & `invenio-base-1.2.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-base-1.2.8/examples/app.py` & `invenio-base-1.2.9/examples/app.py`

 * *Files identical despite different names*

### Comparing `invenio-base-1.2.8/invenio_base/__init__.py` & `invenio-base-1.2.9/invenio_base/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -233,15 +233,15 @@
    $ inveniomanage instance migrate_secret_key --help
    ...
 """
 
 from .app import create_app_factory, create_cli
 from .wsgi import create_wsgi_factory
 
-__version__ = '1.2.8'
+__version__ = '1.2.9'
 
 __all__ = (
     '__version__',
     'create_app_factory',
     'create_cli',
     'create_wsgi_factory',
 )
```

### Comparing `invenio-base-1.2.8/invenio_base/app.py` & `invenio-base-1.2.9/invenio_base/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,15 +201,15 @@
     :param entry_points: List of entry points providing to Blue.
     :param modules: Map of coverters.
 
     .. versionadded: 1.0.0
     """
     if entry_points:
         for entry_point in entry_points:
-            for ep in iter_entry_points(group=entry_point):
+            for ep in set(iter_entry_points(group=entry_point)):
                 try:
                     app.url_map.converters[ep.name] = ep.load()
                 except Exception:
                     app.logger.error(
                         f'Failed to initialize entry point: {ep}')
                     raise
 
@@ -223,15 +223,15 @@
     Used to load and initialize entry points and modules using an custom
     initialization function.
 
     .. versionadded: 1.0.0
     """
     if entry_points:
         for entry_point in entry_points:
-            for ep in iter_entry_points(group=entry_point):
+            for ep in set(iter_entry_points(group=entry_point)):
                 try:
                     init_func(ep.load())
                 except Exception:
                     app.logger.error(
                         f'Failed to initialize entry point: {ep}')
                     raise
     if modules:
```

### Comparing `invenio-base-1.2.8/invenio_base/cli.py` & `invenio-base-1.2.9/invenio_base/cli.py`

 * *Files identical despite different names*

### Comparing `invenio-base-1.2.8/invenio_base/signals.py` & `invenio-base-1.2.9/invenio_base/signals.py`

 * *Files identical despite different names*

### Comparing `invenio-base-1.2.8/invenio_base/utils.py` & `invenio-base-1.2.9/invenio_base/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-base-1.2.8/invenio_base/wsgi.py` & `invenio-base-1.2.9/invenio_base/wsgi.py`

 * *Files identical despite different names*

### Comparing `invenio-base-1.2.8/invenio_base.egg-info/PKG-INFO` & `invenio-base-1.2.9/invenio_base.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-base
-Version: 1.2.8
+Version: 1.2.9
 Summary: "Base package for building Invenio application factories."
 Home-page: https://github.com/inveniosoftware/invenio-base
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Keywords: invenio
 Platform: any
@@ -48,14 +48,19 @@
 
     Invenio is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version 1.2.9 (released 2022-02-22)
+
+- Fixes issue with duplicate entry points during tests due to pytest
+  modifying the sys.path.
+
 Version 1.2.8 (released 2022-02-21)
 
 - Lowered Python requirement to v3.6 to avoid breaking builds.
 
 Version 1.2.7 (released 2022-02-21)
 
 - Fixed minimal test dependencies and limited itsdangerous to <2.1
```

### Comparing `invenio-base-1.2.8/invenio_base.egg-info/SOURCES.txt` & `invenio-base-1.2.9/invenio_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-base-1.2.8/setup.cfg` & `invenio-base-1.2.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-base-1.2.8/tests/test_app.py` & `invenio-base-1.2.9/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `invenio-base-1.2.8/tests/test_cmd.py` & `invenio-base-1.2.9/tests/test_cmd.py`

 * *Files identical despite different names*

### Comparing `invenio-base-1.2.8/tests/test_signals.py` & `invenio-base-1.2.9/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `invenio-base-1.2.8/tests/test_utils.py` & `invenio-base-1.2.9/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `invenio-base-1.2.8/tests/test_wsgi.py` & `invenio-base-1.2.9/tests/test_wsgi.py`

 * *Files identical despite different names*

