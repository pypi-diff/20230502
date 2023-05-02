# Comparing `tmp/core_module_advanced_blob_host_app-2.2.0.tar.gz` & `tmp/core_module_advanced_blob_host_app-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/core_module_advanced_blob_host_app-2.2.0.tar", last modified: Thu Feb 23 20:31:40 2023, max compression
+gzip compressed data, was "core_module_advanced_blob_host_app-2.3.0.tar", last modified: Tue May  2 19:43:13 2023, max compression
```

## Comparing `core_module_advanced_blob_host_app-2.2.0.tar` & `core_module_advanced_blob_host_app-2.3.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:40.000000 core_module_advanced_blob_host_app-2.2.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      201 2023-02-23 20:31:38.000000 core_module_advanced_blob_host_app-2.2.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1160 2023-02-23 20:31:40.000000 core_module_advanced_blob_host_app-2.2.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      654 2023-02-23 20:31:38.000000 core_module_advanced_blob_host_app-2.2.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:40.000000 core_module_advanced_blob_host_app-2.2.0/core_module_advanced_blob_host_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:38.000000 core_module_advanced_blob_host_app-2.2.0/core_module_advanced_blob_host_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      437 2023-02-23 20:31:38.000000 core_module_advanced_blob_host_app-2.2.0/core_module_advanced_blob_host_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:40.000000 core_module_advanced_blob_host_app-2.2.0/core_module_advanced_blob_host_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:40.000000 core_module_advanced_blob_host_app-2.2.0/core_module_advanced_blob_host_app/static/core_module_advanced_blob_host_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:40.000000 core_module_advanced_blob_host_app-2.2.0/core_module_advanced_blob_host_app/static/core_module_advanced_blob_host_app/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      616 2023-02-23 20:31:38.000000 core_module_advanced_blob_host_app-2.2.0/core_module_advanced_blob_host_app/static/core_module_advanced_blob_host_app/css/advanced_blob_host.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:40.000000 core_module_advanced_blob_host_app-2.2.0/core_module_advanced_blob_host_app/static/core_module_advanced_blob_host_app/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      387 2023-02-23 20:31:38.000000 core_module_advanced_blob_host_app-2.2.0/core_module_advanced_blob_host_app/static/core_module_advanced_blob_host_app/js/advanced_blob_host.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:40.000000 core_module_advanced_blob_host_app-2.2.0/core_module_advanced_blob_host_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:40.000000 core_module_advanced_blob_host_app-2.2.0/core_module_advanced_blob_host_app/templates/core_module_advanced_blob_host_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      807 2023-02-23 20:31:38.000000 core_module_advanced_blob_host_app-2.2.0/core_module_advanced_blob_host_app/templates/core_module_advanced_blob_host_app/advanced_blob_host.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      349 2023-02-23 20:31:38.000000 core_module_advanced_blob_host_app-2.2.0/core_module_advanced_blob_host_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:40.000000 core_module_advanced_blob_host_app-2.2.0/core_module_advanced_blob_host_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:38.000000 core_module_advanced_blob_host_app-2.2.0/core_module_advanced_blob_host_app/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3032 2023-02-23 20:31:38.000000 core_module_advanced_blob_host_app-2.2.0/core_module_advanced_blob_host_app/views/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:40.000000 core_module_advanced_blob_host_app-2.2.0/core_module_advanced_blob_host_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1160 2023-02-23 20:31:39.000000 core_module_advanced_blob_host_app-2.2.0/core_module_advanced_blob_host_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      965 2023-02-23 20:31:40.000000 core_module_advanced_blob_host_app-2.2.0/core_module_advanced_blob_host_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-02-23 20:31:39.000000 core_module_advanced_blob_host_app-2.2.0/core_module_advanced_blob_host_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      124 2023-02-23 20:31:39.000000 core_module_advanced_blob_host_app-2.2.0/core_module_advanced_blob_host_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       41 2023-02-23 20:31:39.000000 core_module_advanced_blob_host_app-2.2.0/core_module_advanced_blob_host_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-02-23 20:31:38.000000 core_module_advanced_blob_host_app-2.2.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      117 2023-02-23 20:31:38.000000 core_module_advanced_blob_host_app-2.2.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        7 2023-02-23 20:31:38.000000 core_module_advanced_blob_host_app-2.2.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-02-23 20:31:40.000000 core_module_advanced_blob_host_app-2.2.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1104 2023-02-23 20:31:38.000000 core_module_advanced_blob_host_app-2.2.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:40.000000 core_module_advanced_blob_host_app-2.2.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:38.000000 core_module_advanced_blob_host_app-2.2.0/tests/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      119 2023-02-23 20:31:38.000000 core_module_advanced_blob_host_app-2.2.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:43:13.726481 core_module_advanced_blob_host_app-2.3.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:43:11.000000 core_module_advanced_blob_host_app-2.3.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      201 2023-05-02 19:43:11.000000 core_module_advanced_blob_host_app-2.3.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1160 2023-05-02 19:43:13.721741 core_module_advanced_blob_host_app-2.3.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      654 2023-05-02 19:43:11.000000 core_module_advanced_blob_host_app-2.3.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:43:13.528554 core_module_advanced_blob_host_app-2.3.0/core_module_advanced_blob_host_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:43:11.000000 core_module_advanced_blob_host_app-2.3.0/core_module_advanced_blob_host_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      437 2023-05-02 19:43:11.000000 core_module_advanced_blob_host_app-2.3.0/core_module_advanced_blob_host_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:43:13.311473 core_module_advanced_blob_host_app-2.3.0/core_module_advanced_blob_host_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:43:13.321088 core_module_advanced_blob_host_app-2.3.0/core_module_advanced_blob_host_app/static/core_module_advanced_blob_host_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:43:13.623019 core_module_advanced_blob_host_app-2.3.0/core_module_advanced_blob_host_app/static/core_module_advanced_blob_host_app/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      616 2023-05-02 19:43:11.000000 core_module_advanced_blob_host_app-2.3.0/core_module_advanced_blob_host_app/static/core_module_advanced_blob_host_app/css/advanced_blob_host.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:43:13.637998 core_module_advanced_blob_host_app-2.3.0/core_module_advanced_blob_host_app/static/core_module_advanced_blob_host_app/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      387 2023-05-02 19:43:11.000000 core_module_advanced_blob_host_app-2.3.0/core_module_advanced_blob_host_app/static/core_module_advanced_blob_host_app/js/advanced_blob_host.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:43:13.331322 core_module_advanced_blob_host_app-2.3.0/core_module_advanced_blob_host_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:43:13.652217 core_module_advanced_blob_host_app-2.3.0/core_module_advanced_blob_host_app/templates/core_module_advanced_blob_host_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      807 2023-05-02 19:43:11.000000 core_module_advanced_blob_host_app-2.3.0/core_module_advanced_blob_host_app/templates/core_module_advanced_blob_host_app/advanced_blob_host.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      349 2023-05-02 19:43:11.000000 core_module_advanced_blob_host_app-2.3.0/core_module_advanced_blob_host_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:43:13.683076 core_module_advanced_blob_host_app-2.3.0/core_module_advanced_blob_host_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:43:11.000000 core_module_advanced_blob_host_app-2.3.0/core_module_advanced_blob_host_app/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3032 2023-05-02 19:43:11.000000 core_module_advanced_blob_host_app-2.3.0/core_module_advanced_blob_host_app/views/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:43:13.607415 core_module_advanced_blob_host_app-2.3.0/core_module_advanced_blob_host_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1160 2023-05-02 19:43:13.000000 core_module_advanced_blob_host_app-2.3.0/core_module_advanced_blob_host_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      976 2023-05-02 19:43:13.000000 core_module_advanced_blob_host_app-2.3.0/core_module_advanced_blob_host_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:43:13.000000 core_module_advanced_blob_host_app-2.3.0/core_module_advanced_blob_host_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      124 2023-05-02 19:43:13.000000 core_module_advanced_blob_host_app-2.3.0/core_module_advanced_blob_host_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       41 2023-05-02 19:43:13.000000 core_module_advanced_blob_host_app-2.3.0/core_module_advanced_blob_host_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:43:11.000000 core_module_advanced_blob_host_app-2.3.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      117 2023-05-02 19:43:11.000000 core_module_advanced_blob_host_app-2.3.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        7 2023-05-02 19:43:11.000000 core_module_advanced_blob_host_app-2.3.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:43:13.728166 core_module_advanced_blob_host_app-2.3.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1104 2023-05-02 19:43:12.000000 core_module_advanced_blob_host_app-2.3.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:43:13.712761 core_module_advanced_blob_host_app-2.3.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:43:12.000000 core_module_advanced_blob_host_app-2.3.0/tests/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      119 2023-05-02 19:43:12.000000 core_module_advanced_blob_host_app-2.3.0/tests/test_settings.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `core_module_advanced_blob_host_app-2.2.0/PKG-INFO` & `core_module_advanced_blob_host_app-2.3.0/core_module_advanced_blob_host_app.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
-Name: core_module_advanced_blob_host_app
-Version: 2.2.0
+Name: core-module-advanced-blob-host-app
+Version: 2.3.0
 Summary: Advanced Blob Host module for the parser core project
 Home-page: https://github.com/usnistgov/core_module_advanced_blob_host_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_module_advanced_blob_host_app
         ==================================
```

### Comparing `core_module_advanced_blob_host_app-2.2.0/README.rst` & `core_module_advanced_blob_host_app-2.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_module_advanced_blob_host_app-2.2.0/core_module_advanced_blob_host_app/static/core_module_advanced_blob_host_app/css/advanced_blob_host.css` & `core_module_advanced_blob_host_app-2.3.0/core_module_advanced_blob_host_app/static/core_module_advanced_blob_host_app/css/advanced_blob_host.css`

 * *Files identical despite different names*

### Comparing `core_module_advanced_blob_host_app-2.2.0/core_module_advanced_blob_host_app/templates/core_module_advanced_blob_host_app/advanced_blob_host.html` & `core_module_advanced_blob_host_app-2.3.0/core_module_advanced_blob_host_app/templates/core_module_advanced_blob_host_app/advanced_blob_host.html`

 * *Files identical despite different names*

### Comparing `core_module_advanced_blob_host_app-2.2.0/core_module_advanced_blob_host_app/views/views.py` & `core_module_advanced_blob_host_app-2.3.0/core_module_advanced_blob_host_app/views/views.py`

 * *Files identical despite different names*

### Comparing `core_module_advanced_blob_host_app-2.2.0/core_module_advanced_blob_host_app.egg-info/PKG-INFO` & `core_module_advanced_blob_host_app-2.3.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
-Name: core-module-advanced-blob-host-app
-Version: 2.2.0
+Name: core_module_advanced_blob_host_app
+Version: 2.3.0
 Summary: Advanced Blob Host module for the parser core project
 Home-page: https://github.com/usnistgov/core_module_advanced_blob_host_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_module_advanced_blob_host_app
         ==================================
```

### Comparing `core_module_advanced_blob_host_app-2.2.0/core_module_advanced_blob_host_app.egg-info/SOURCES.txt` & `core_module_advanced_blob_host_app-2.3.0/core_module_advanced_blob_host_app.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.md
 MANIFEST.in
 README.rst
 pyproject.toml
 requirements.core.txt
 requirements.txt
 setup.py
 core_module_advanced_blob_host_app/__init__.py
```

### Comparing `core_module_advanced_blob_host_app-2.2.0/setup.py` & `core_module_advanced_blob_host_app-2.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_module_advanced_blob_host_app",
-    version="2.2.0",
+    version="2.3.0",
     description="Advanced Blob Host module for the parser core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_module_advanced_blob_host_app",
     packages=find_packages(),
     include_package_data=True,
```

