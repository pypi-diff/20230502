# Comparing `tmp/core_module_chemical_composition_app-2.2.0.tar.gz` & `tmp/core_module_chemical_composition_app-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/core_module_chemical_composition_app-2.2.0.tar", last modified: Thu Feb 23 20:32:01 2023, max compression
+gzip compressed data, was "core_module_chemical_composition_app-2.3.0.tar", last modified: Tue May  2 20:20:22 2023, max compression
```

## Comparing `core_module_chemical_composition_app-2.2.0.tar` & `core_module_chemical_composition_app-2.3.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:01.000000 core_module_chemical_composition_app-2.2.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      175 2023-02-23 20:31:59.000000 core_module_chemical_composition_app-2.2.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1184 2023-02-23 20:32:01.000000 core_module_chemical_composition_app-2.2.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      672 2023-02-23 20:31:59.000000 core_module_chemical_composition_app-2.2.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:01.000000 core_module_chemical_composition_app-2.2.0/core_module_chemical_composition_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:59.000000 core_module_chemical_composition_app-2.2.0/core_module_chemical_composition_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3537 2023-02-23 20:31:59.000000 core_module_chemical_composition_app-2.2.0/core_module_chemical_composition_app/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      435 2023-02-23 20:31:59.000000 core_module_chemical_composition_app-2.2.0/core_module_chemical_composition_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:01.000000 core_module_chemical_composition_app-2.2.0/core_module_chemical_composition_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:01.000000 core_module_chemical_composition_app-2.2.0/core_module_chemical_composition_app/static/core_module_chemical_composition_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:01.000000 core_module_chemical_composition_app-2.2.0/core_module_chemical_composition_app/static/core_module_chemical_composition_app/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      372 2023-02-23 20:31:59.000000 core_module_chemical_composition_app-2.2.0/core_module_chemical_composition_app/static/core_module_chemical_composition_app/css/chemical_element_composition.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:01.000000 core_module_chemical_composition_app-2.2.0/core_module_chemical_composition_app/static/core_module_chemical_composition_app/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1492 2023-02-23 20:31:59.000000 core_module_chemical_composition_app-2.2.0/core_module_chemical_composition_app/static/core_module_chemical_composition_app/js/chemical_element_composition.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1389 2023-02-23 20:31:59.000000 core_module_chemical_composition_app-2.2.0/core_module_chemical_composition_app/static/core_module_chemical_composition_app/js/events.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:01.000000 core_module_chemical_composition_app-2.2.0/core_module_chemical_composition_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:01.000000 core_module_chemical_composition_app-2.2.0/core_module_chemical_composition_app/templates/core_module_chemical_composition_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      113 2023-02-23 20:31:59.000000 core_module_chemical_composition_app-2.2.0/core_module_chemical_composition_app/templates/core_module_chemical_composition_app/chemical_composition.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2061 2023-02-23 20:31:59.000000 core_module_chemical_composition_app-2.2.0/core_module_chemical_composition_app/templates/core_module_chemical_composition_app/edit_data.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      832 2023-02-23 20:31:59.000000 core_module_chemical_composition_app-2.2.0/core_module_chemical_composition_app/templates/core_module_chemical_composition_app/render_data.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      352 2023-02-23 20:31:59.000000 core_module_chemical_composition_app-2.2.0/core_module_chemical_composition_app/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4217 2023-02-23 20:31:59.000000 core_module_chemical_composition_app-2.2.0/core_module_chemical_composition_app/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:01.000000 core_module_chemical_composition_app-2.2.0/core_module_chemical_composition_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1184 2023-02-23 20:32:00.000000 core_module_chemical_composition_app-2.2.0/core_module_chemical_composition_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1274 2023-02-23 20:32:01.000000 core_module_chemical_composition_app-2.2.0/core_module_chemical_composition_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-02-23 20:32:00.000000 core_module_chemical_composition_app-2.2.0/core_module_chemical_composition_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        7 2023-02-23 20:32:01.000000 core_module_chemical_composition_app-2.2.0/core_module_chemical_composition_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       43 2023-02-23 20:32:01.000000 core_module_chemical_composition_app-2.2.0/core_module_chemical_composition_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-02-23 20:31:59.000000 core_module_chemical_composition_app-2.2.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        7 2023-02-23 20:31:59.000000 core_module_chemical_composition_app-2.2.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-02-23 20:32:01.000000 core_module_chemical_composition_app-2.2.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      960 2023-02-23 20:32:00.000000 core_module_chemical_composition_app-2.2.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:01.000000 core_module_chemical_composition_app-2.2.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:00.000000 core_module_chemical_composition_app-2.2.0/tests/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      120 2023-02-23 20:32:00.000000 core_module_chemical_composition_app-2.2.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 20:20:22.134686 core_module_chemical_composition_app-2.3.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 20:20:20.000000 core_module_chemical_composition_app-2.3.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      175 2023-05-02 20:20:20.000000 core_module_chemical_composition_app-2.3.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1184 2023-05-02 20:20:22.129234 core_module_chemical_composition_app-2.3.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      672 2023-05-02 20:20:20.000000 core_module_chemical_composition_app-2.3.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 20:20:21.938504 core_module_chemical_composition_app-2.3.0/core_module_chemical_composition_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 20:20:20.000000 core_module_chemical_composition_app-2.3.0/core_module_chemical_composition_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3537 2023-05-02 20:20:20.000000 core_module_chemical_composition_app-2.3.0/core_module_chemical_composition_app/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      435 2023-05-02 20:20:20.000000 core_module_chemical_composition_app-2.3.0/core_module_chemical_composition_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 20:20:21.754585 core_module_chemical_composition_app-2.3.0/core_module_chemical_composition_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 20:20:21.763005 core_module_chemical_composition_app-2.3.0/core_module_chemical_composition_app/static/core_module_chemical_composition_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 20:20:22.018486 core_module_chemical_composition_app-2.3.0/core_module_chemical_composition_app/static/core_module_chemical_composition_app/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      372 2023-05-02 20:20:20.000000 core_module_chemical_composition_app-2.3.0/core_module_chemical_composition_app/static/core_module_chemical_composition_app/css/chemical_element_composition.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 20:20:22.041596 core_module_chemical_composition_app-2.3.0/core_module_chemical_composition_app/static/core_module_chemical_composition_app/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1492 2023-05-02 20:20:20.000000 core_module_chemical_composition_app-2.3.0/core_module_chemical_composition_app/static/core_module_chemical_composition_app/js/chemical_element_composition.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1389 2023-05-02 20:20:20.000000 core_module_chemical_composition_app-2.3.0/core_module_chemical_composition_app/static/core_module_chemical_composition_app/js/events.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 20:20:21.785017 core_module_chemical_composition_app-2.3.0/core_module_chemical_composition_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 20:20:22.083020 core_module_chemical_composition_app-2.3.0/core_module_chemical_composition_app/templates/core_module_chemical_composition_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      113 2023-05-02 20:20:20.000000 core_module_chemical_composition_app-2.3.0/core_module_chemical_composition_app/templates/core_module_chemical_composition_app/chemical_composition.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2061 2023-05-02 20:20:20.000000 core_module_chemical_composition_app-2.3.0/core_module_chemical_composition_app/templates/core_module_chemical_composition_app/edit_data.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      832 2023-05-02 20:20:20.000000 core_module_chemical_composition_app-2.3.0/core_module_chemical_composition_app/templates/core_module_chemical_composition_app/render_data.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      352 2023-05-02 20:20:20.000000 core_module_chemical_composition_app-2.3.0/core_module_chemical_composition_app/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4217 2023-05-02 20:20:20.000000 core_module_chemical_composition_app-2.3.0/core_module_chemical_composition_app/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 20:20:22.002752 core_module_chemical_composition_app-2.3.0/core_module_chemical_composition_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1184 2023-05-02 20:20:21.000000 core_module_chemical_composition_app-2.3.0/core_module_chemical_composition_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1285 2023-05-02 20:20:21.000000 core_module_chemical_composition_app-2.3.0/core_module_chemical_composition_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 20:20:21.000000 core_module_chemical_composition_app-2.3.0/core_module_chemical_composition_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        7 2023-05-02 20:20:21.000000 core_module_chemical_composition_app-2.3.0/core_module_chemical_composition_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       43 2023-05-02 20:20:21.000000 core_module_chemical_composition_app-2.3.0/core_module_chemical_composition_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 20:20:20.000000 core_module_chemical_composition_app-2.3.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        7 2023-05-02 20:20:20.000000 core_module_chemical_composition_app-2.3.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 20:20:22.136372 core_module_chemical_composition_app-2.3.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      960 2023-05-02 20:20:20.000000 core_module_chemical_composition_app-2.3.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 20:20:22.119866 core_module_chemical_composition_app-2.3.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 20:20:20.000000 core_module_chemical_composition_app-2.3.0/tests/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      120 2023-05-02 20:20:20.000000 core_module_chemical_composition_app-2.3.0/tests/test_settings.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `core_module_chemical_composition_app-2.2.0/PKG-INFO` & `core_module_chemical_composition_app-2.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_module_chemical_composition_app
-Version: 2.2.0
+Version: 2.3.0
 Summary: Chemical composition module for the parser core project
 Home-page: https://github.com/usnistgov/core_module_chemical_composition_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_module_chemical_composition_app
         ====================================
```

### Comparing `core_module_chemical_composition_app-2.2.0/README.rst` & `core_module_chemical_composition_app-2.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_module_chemical_composition_app-2.2.0/core_module_chemical_composition_app/api.py` & `core_module_chemical_composition_app-2.3.0/core_module_chemical_composition_app/api.py`

 * *Files identical despite different names*

### Comparing `core_module_chemical_composition_app-2.2.0/core_module_chemical_composition_app/static/core_module_chemical_composition_app/js/chemical_element_composition.js` & `core_module_chemical_composition_app-2.3.0/core_module_chemical_composition_app/static/core_module_chemical_composition_app/js/chemical_element_composition.js`

 * *Files identical despite different names*

### Comparing `core_module_chemical_composition_app-2.2.0/core_module_chemical_composition_app/static/core_module_chemical_composition_app/js/events.js` & `core_module_chemical_composition_app-2.3.0/core_module_chemical_composition_app/static/core_module_chemical_composition_app/js/events.js`

 * *Files identical despite different names*

### Comparing `core_module_chemical_composition_app-2.2.0/core_module_chemical_composition_app/templates/core_module_chemical_composition_app/edit_data.html` & `core_module_chemical_composition_app-2.3.0/core_module_chemical_composition_app/templates/core_module_chemical_composition_app/edit_data.html`

 * *Files identical despite different names*

### Comparing `core_module_chemical_composition_app-2.2.0/core_module_chemical_composition_app/templates/core_module_chemical_composition_app/render_data.html` & `core_module_chemical_composition_app-2.3.0/core_module_chemical_composition_app/templates/core_module_chemical_composition_app/render_data.html`

 * *Files identical despite different names*

### Comparing `core_module_chemical_composition_app-2.2.0/core_module_chemical_composition_app/views.py` & `core_module_chemical_composition_app-2.3.0/core_module_chemical_composition_app/views.py`

 * *Files identical despite different names*

### Comparing `core_module_chemical_composition_app-2.2.0/core_module_chemical_composition_app.egg-info/PKG-INFO` & `core_module_chemical_composition_app-2.3.0/core_module_chemical_composition_app.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-module-chemical-composition-app
-Version: 2.2.0
+Version: 2.3.0
 Summary: Chemical composition module for the parser core project
 Home-page: https://github.com/usnistgov/core_module_chemical_composition_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_module_chemical_composition_app
         ====================================
```

### Comparing `core_module_chemical_composition_app-2.2.0/core_module_chemical_composition_app.egg-info/SOURCES.txt` & `core_module_chemical_composition_app-2.3.0/core_module_chemical_composition_app.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.md
 MANIFEST.in
 README.rst
 pyproject.toml
 requirements.txt
 setup.py
 core_module_chemical_composition_app/__init__.py
 core_module_chemical_composition_app/api.py
```

### Comparing `core_module_chemical_composition_app-2.2.0/setup.py` & `core_module_chemical_composition_app-2.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_module_chemical_composition_app",
-    version="2.2.0",
+    version="2.3.0",
     description="Chemical composition module for the parser core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_module_chemical_composition_app",
     packages=find_packages(),
     include_package_data=True,
```

