# Comparing `tmp/core_module_blob_host_app-2.2.0.tar.gz` & `tmp/core_module_blob_host_app-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/core_module_blob_host_app-2.2.0.tar", last modified: Thu Feb 23 20:31:53 2023, max compression
+gzip compressed data, was "core_module_blob_host_app-2.3.0.tar", last modified: Tue May  2 19:44:47 2023, max compression
```

## Comparing `core_module_blob_host_app-2.2.0.tar` & `core_module_blob_host_app-2.3.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:53.000000 core_module_blob_host_app-2.2.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      183 2023-02-23 20:31:51.000000 core_module_blob_host_app-2.2.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1052 2023-02-23 20:31:53.000000 core_module_blob_host_app-2.2.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      573 2023-02-23 20:31:51.000000 core_module_blob_host_app-2.2.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:53.000000 core_module_blob_host_app-2.2.0/core_module_blob_host_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:51.000000 core_module_blob_host_app-2.2.0/core_module_blob_host_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      716 2023-02-23 20:31:51.000000 core_module_blob_host_app-2.2.0/core_module_blob_host_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:53.000000 core_module_blob_host_app-2.2.0/core_module_blob_host_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:53.000000 core_module_blob_host_app-2.2.0/core_module_blob_host_app/static/core_module_blob_host_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:53.000000 core_module_blob_host_app-2.2.0/core_module_blob_host_app/static/core_module_blob_host_app/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      347 2023-02-23 20:31:51.000000 core_module_blob_host_app-2.2.0/core_module_blob_host_app/static/core_module_blob_host_app/js/blob_host.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:53.000000 core_module_blob_host_app-2.2.0/core_module_blob_host_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:53.000000 core_module_blob_host_app-2.2.0/core_module_blob_host_app/templates/core_module_blob_host_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      156 2023-02-23 20:31:51.000000 core_module_blob_host_app-2.2.0/core_module_blob_host_app/templates/core_module_blob_host_app/blob_host.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      507 2023-02-23 20:31:51.000000 core_module_blob_host_app-2.2.0/core_module_blob_host_app/templates/core_module_blob_host_app/blob_host_display.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      288 2023-02-23 20:31:51.000000 core_module_blob_host_app-2.2.0/core_module_blob_host_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:53.000000 core_module_blob_host_app-2.2.0/core_module_blob_host_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:51.000000 core_module_blob_host_app-2.2.0/core_module_blob_host_app/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      152 2023-02-23 20:31:51.000000 core_module_blob_host_app-2.2.0/core_module_blob_host_app/views/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5661 2023-02-23 20:31:51.000000 core_module_blob_host_app-2.2.0/core_module_blob_host_app/views/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:53.000000 core_module_blob_host_app-2.2.0/core_module_blob_host_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1052 2023-02-23 20:31:52.000000 core_module_blob_host_app-2.2.0/core_module_blob_host_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      843 2023-02-23 20:31:53.000000 core_module_blob_host_app-2.2.0/core_module_blob_host_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-02-23 20:31:52.000000 core_module_blob_host_app-2.2.0/core_module_blob_host_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       51 2023-02-23 20:31:52.000000 core_module_blob_host_app-2.2.0/core_module_blob_host_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       32 2023-02-23 20:31:52.000000 core_module_blob_host_app-2.2.0/core_module_blob_host_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-02-23 20:31:51.000000 core_module_blob_host_app-2.2.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       44 2023-02-23 20:31:51.000000 core_module_blob_host_app-2.2.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        7 2023-02-23 20:31:51.000000 core_module_blob_host_app-2.2.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-02-23 20:31:53.000000 core_module_blob_host_app-2.2.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1073 2023-02-23 20:31:51.000000 core_module_blob_host_app-2.2.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:53.000000 core_module_blob_host_app-2.2.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:51.000000 core_module_blob_host_app-2.2.0/tests/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      119 2023-02-23 20:31:51.000000 core_module_blob_host_app-2.2.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:44:47.026694 core_module_blob_host_app-2.3.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:44:45.000000 core_module_blob_host_app-2.3.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      183 2023-05-02 19:44:45.000000 core_module_blob_host_app-2.3.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1052 2023-05-02 19:44:47.022309 core_module_blob_host_app-2.3.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      573 2023-05-02 19:44:45.000000 core_module_blob_host_app-2.3.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:44:46.817067 core_module_blob_host_app-2.3.0/core_module_blob_host_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:44:45.000000 core_module_blob_host_app-2.3.0/core_module_blob_host_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      716 2023-05-02 19:44:45.000000 core_module_blob_host_app-2.3.0/core_module_blob_host_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:44:46.648777 core_module_blob_host_app-2.3.0/core_module_blob_host_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:44:46.652531 core_module_blob_host_app-2.3.0/core_module_blob_host_app/static/core_module_blob_host_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:44:46.907011 core_module_blob_host_app-2.3.0/core_module_blob_host_app/static/core_module_blob_host_app/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      347 2023-05-02 19:44:45.000000 core_module_blob_host_app-2.3.0/core_module_blob_host_app/static/core_module_blob_host_app/js/blob_host.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:44:46.662747 core_module_blob_host_app-2.3.0/core_module_blob_host_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:44:46.931410 core_module_blob_host_app-2.3.0/core_module_blob_host_app/templates/core_module_blob_host_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      156 2023-05-02 19:44:45.000000 core_module_blob_host_app-2.3.0/core_module_blob_host_app/templates/core_module_blob_host_app/blob_host.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      507 2023-05-02 19:44:45.000000 core_module_blob_host_app-2.3.0/core_module_blob_host_app/templates/core_module_blob_host_app/blob_host_display.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      288 2023-05-02 19:44:45.000000 core_module_blob_host_app-2.3.0/core_module_blob_host_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:44:46.974514 core_module_blob_host_app-2.3.0/core_module_blob_host_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:44:45.000000 core_module_blob_host_app-2.3.0/core_module_blob_host_app/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      152 2023-05-02 19:44:45.000000 core_module_blob_host_app-2.3.0/core_module_blob_host_app/views/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5661 2023-05-02 19:44:45.000000 core_module_blob_host_app-2.3.0/core_module_blob_host_app/views/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:44:46.893554 core_module_blob_host_app-2.3.0/core_module_blob_host_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1052 2023-05-02 19:44:46.000000 core_module_blob_host_app-2.3.0/core_module_blob_host_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      854 2023-05-02 19:44:46.000000 core_module_blob_host_app-2.3.0/core_module_blob_host_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:44:46.000000 core_module_blob_host_app-2.3.0/core_module_blob_host_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       51 2023-05-02 19:44:46.000000 core_module_blob_host_app-2.3.0/core_module_blob_host_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       32 2023-05-02 19:44:46.000000 core_module_blob_host_app-2.3.0/core_module_blob_host_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:44:45.000000 core_module_blob_host_app-2.3.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       44 2023-05-02 19:44:45.000000 core_module_blob_host_app-2.3.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        7 2023-05-02 19:44:45.000000 core_module_blob_host_app-2.3.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:44:47.028282 core_module_blob_host_app-2.3.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1073 2023-05-02 19:44:45.000000 core_module_blob_host_app-2.3.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:44:47.000390 core_module_blob_host_app-2.3.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:44:45.000000 core_module_blob_host_app-2.3.0/tests/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      119 2023-05-02 19:44:45.000000 core_module_blob_host_app-2.3.0/tests/test_settings.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `core_module_blob_host_app-2.2.0/PKG-INFO` & `core_module_blob_host_app-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_module_blob_host_app
-Version: 2.2.0
+Version: 2.3.0
 Summary: Blob Host module for the parser core project
 Home-page: https://github.com/usnistgov/core_module_blob_host_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_module_blob_host_app
         =========================
```

### Comparing `core_module_blob_host_app-2.2.0/README.rst` & `core_module_blob_host_app-2.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_module_blob_host_app-2.2.0/core_module_blob_host_app/settings.py` & `core_module_blob_host_app-2.3.0/core_module_blob_host_app/settings.py`

 * *Files identical despite different names*

### Comparing `core_module_blob_host_app-2.2.0/core_module_blob_host_app/views/views.py` & `core_module_blob_host_app-2.3.0/core_module_blob_host_app/views/views.py`

 * *Files identical despite different names*

### Comparing `core_module_blob_host_app-2.2.0/core_module_blob_host_app.egg-info/PKG-INFO` & `core_module_blob_host_app-2.3.0/core_module_blob_host_app.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-module-blob-host-app
-Version: 2.2.0
+Version: 2.3.0
 Summary: Blob Host module for the parser core project
 Home-page: https://github.com/usnistgov/core_module_blob_host_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_module_blob_host_app
         =========================
```

### Comparing `core_module_blob_host_app-2.2.0/core_module_blob_host_app.egg-info/SOURCES.txt` & `core_module_blob_host_app-2.3.0/core_module_blob_host_app.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.md
 MANIFEST.in
 README.rst
 pyproject.toml
 requirements.core.txt
 requirements.txt
 setup.py
 core_module_blob_host_app/__init__.py
```

### Comparing `core_module_blob_host_app-2.2.0/setup.py` & `core_module_blob_host_app-2.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_module_blob_host_app",
-    version="2.2.0",
+    version="2.3.0",
     description="Blob Host module for the parser core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_module_blob_host_app",
     packages=find_packages(),
     include_package_data=True,
```

