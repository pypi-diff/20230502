# Comparing `tmp/core_module_periodic_table_app-2.2.0.tar.gz` & `tmp/core_module_periodic_table_app-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/core_module_periodic_table_app-2.2.0.tar", last modified: Thu Feb 23 20:32:40 2023, max compression
+gzip compressed data, was "core_module_periodic_table_app-2.3.0.tar", last modified: Tue May  2 19:46:20 2023, max compression
```

## Comparing `core_module_periodic_table_app-2.2.0.tar` & `core_module_periodic_table_app-2.3.0.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:40.000000 core_module_periodic_table_app-2.2.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      193 2023-02-23 20:32:38.000000 core_module_periodic_table_app-2.2.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1112 2023-02-23 20:32:40.000000 core_module_periodic_table_app-2.2.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      618 2023-02-23 20:32:38.000000 core_module_periodic_table_app-2.2.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:40.000000 core_module_periodic_table_app-2.2.0/core_module_periodic_table_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:38.000000 core_module_periodic_table_app-2.2.0/core_module_periodic_table_app/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:40.000000 core_module_periodic_table_app-2.2.0/core_module_periodic_table_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:40.000000 core_module_periodic_table_app-2.2.0/core_module_periodic_table_app/static/core_module_periodic_table_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:40.000000 core_module_periodic_table_app-2.2.0/core_module_periodic_table_app/static/core_module_periodic_table_app/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1416 2023-02-23 20:32:38.000000 core_module_periodic_table_app-2.2.0/core_module_periodic_table_app/static/core_module_periodic_table_app/css/periodic.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:40.000000 core_module_periodic_table_app-2.2.0/core_module_periodic_table_app/static/core_module_periodic_table_app/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1075 2023-02-23 20:32:38.000000 core_module_periodic_table_app-2.2.0/core_module_periodic_table_app/static/core_module_periodic_table_app/js/periodic.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:40.000000 core_module_periodic_table_app-2.2.0/core_module_periodic_table_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:40.000000 core_module_periodic_table_app-2.2.0/core_module_periodic_table_app/templates/core_module_periodic_table_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10866 2023-02-23 20:32:38.000000 core_module_periodic_table_app-2.2.0/core_module_periodic_table_app/templates/core_module_periodic_table_app/periodic.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      146 2023-02-23 20:32:38.000000 core_module_periodic_table_app-2.2.0/core_module_periodic_table_app/templates/core_module_periodic_table_app/periodic_simple.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      312 2023-02-23 20:32:38.000000 core_module_periodic_table_app-2.2.0/core_module_periodic_table_app/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1731 2023-02-23 20:32:38.000000 core_module_periodic_table_app-2.2.0/core_module_periodic_table_app/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:40.000000 core_module_periodic_table_app-2.2.0/core_module_periodic_table_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1112 2023-02-23 20:32:39.000000 core_module_periodic_table_app-2.2.0/core_module_periodic_table_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      891 2023-02-23 20:32:39.000000 core_module_periodic_table_app-2.2.0/core_module_periodic_table_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-02-23 20:32:39.000000 core_module_periodic_table_app-2.2.0/core_module_periodic_table_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       30 2023-02-23 20:32:39.000000 core_module_periodic_table_app-2.2.0/core_module_periodic_table_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       37 2023-02-23 20:32:39.000000 core_module_periodic_table_app-2.2.0/core_module_periodic_table_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-02-23 20:32:38.000000 core_module_periodic_table_app-2.2.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       23 2023-02-23 20:32:38.000000 core_module_periodic_table_app-2.2.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        7 2023-02-23 20:32:38.000000 core_module_periodic_table_app-2.2.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-02-23 20:32:40.000000 core_module_periodic_table_app-2.2.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1093 2023-02-23 20:32:38.000000 core_module_periodic_table_app-2.2.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:40.000000 core_module_periodic_table_app-2.2.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:38.000000 core_module_periodic_table_app-2.2.0/tests/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1262 2023-02-23 20:32:38.000000 core_module_periodic_table_app-2.2.0/tests/test_settings.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4065 2023-02-23 20:32:38.000000 core_module_periodic_table_app-2.2.0/tests/test_unit_views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:20.828470 core_module_periodic_table_app-2.3.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:46:19.000000 core_module_periodic_table_app-2.3.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      193 2023-05-02 19:46:19.000000 core_module_periodic_table_app-2.3.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1112 2023-05-02 19:46:20.824554 core_module_periodic_table_app-2.3.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      618 2023-05-02 19:46:19.000000 core_module_periodic_table_app-2.3.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:20.661595 core_module_periodic_table_app-2.3.0/core_module_periodic_table_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:19.000000 core_module_periodic_table_app-2.3.0/core_module_periodic_table_app/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:20.537311 core_module_periodic_table_app-2.3.0/core_module_periodic_table_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:20.550594 core_module_periodic_table_app-2.3.0/core_module_periodic_table_app/static/core_module_periodic_table_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:20.750192 core_module_periodic_table_app-2.3.0/core_module_periodic_table_app/static/core_module_periodic_table_app/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1416 2023-05-02 19:46:19.000000 core_module_periodic_table_app-2.3.0/core_module_periodic_table_app/static/core_module_periodic_table_app/css/periodic.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:20.761102 core_module_periodic_table_app-2.3.0/core_module_periodic_table_app/static/core_module_periodic_table_app/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1075 2023-05-02 19:46:19.000000 core_module_periodic_table_app-2.3.0/core_module_periodic_table_app/static/core_module_periodic_table_app/js/periodic.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:20.556907 core_module_periodic_table_app-2.3.0/core_module_periodic_table_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:20.781537 core_module_periodic_table_app-2.3.0/core_module_periodic_table_app/templates/core_module_periodic_table_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10866 2023-05-02 19:46:19.000000 core_module_periodic_table_app-2.3.0/core_module_periodic_table_app/templates/core_module_periodic_table_app/periodic.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      146 2023-05-02 19:46:19.000000 core_module_periodic_table_app-2.3.0/core_module_periodic_table_app/templates/core_module_periodic_table_app/periodic_simple.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      312 2023-05-02 19:46:19.000000 core_module_periodic_table_app-2.3.0/core_module_periodic_table_app/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1731 2023-05-02 19:46:19.000000 core_module_periodic_table_app-2.3.0/core_module_periodic_table_app/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:20.736823 core_module_periodic_table_app-2.3.0/core_module_periodic_table_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1112 2023-05-02 19:46:20.000000 core_module_periodic_table_app-2.3.0/core_module_periodic_table_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      902 2023-05-02 19:46:20.000000 core_module_periodic_table_app-2.3.0/core_module_periodic_table_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:46:20.000000 core_module_periodic_table_app-2.3.0/core_module_periodic_table_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       30 2023-05-02 19:46:20.000000 core_module_periodic_table_app-2.3.0/core_module_periodic_table_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       37 2023-05-02 19:46:20.000000 core_module_periodic_table_app-2.3.0/core_module_periodic_table_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:46:19.000000 core_module_periodic_table_app-2.3.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       23 2023-05-02 19:46:19.000000 core_module_periodic_table_app-2.3.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        7 2023-05-02 19:46:19.000000 core_module_periodic_table_app-2.3.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:46:20.829897 core_module_periodic_table_app-2.3.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1093 2023-05-02 19:46:19.000000 core_module_periodic_table_app-2.3.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:20.816506 core_module_periodic_table_app-2.3.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:19.000000 core_module_periodic_table_app-2.3.0/tests/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1262 2023-05-02 19:46:19.000000 core_module_periodic_table_app-2.3.0/tests/test_settings.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4065 2023-05-02 19:46:19.000000 core_module_periodic_table_app-2.3.0/tests/test_unit_views.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `core_module_periodic_table_app-2.2.0/PKG-INFO` & `core_module_periodic_table_app-2.3.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_module_periodic_table_app
-Version: 2.2.0
+Version: 2.3.0
 Summary: Periodic table module for the parser core project
 Home-page: https://github.com/usnistgov/core_module_periodic_table_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_module_periodic_table_app
         ==============================
```

### Comparing `core_module_periodic_table_app-2.2.0/README.rst` & `core_module_periodic_table_app-2.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_module_periodic_table_app-2.2.0/core_module_periodic_table_app/static/core_module_periodic_table_app/css/periodic.css` & `core_module_periodic_table_app-2.3.0/core_module_periodic_table_app/static/core_module_periodic_table_app/css/periodic.css`

 * *Files identical despite different names*

### Comparing `core_module_periodic_table_app-2.2.0/core_module_periodic_table_app/static/core_module_periodic_table_app/js/periodic.js` & `core_module_periodic_table_app-2.3.0/core_module_periodic_table_app/static/core_module_periodic_table_app/js/periodic.js`

 * *Files identical despite different names*

### Comparing `core_module_periodic_table_app-2.2.0/core_module_periodic_table_app/templates/core_module_periodic_table_app/periodic.html` & `core_module_periodic_table_app-2.3.0/core_module_periodic_table_app/templates/core_module_periodic_table_app/periodic.html`

 * *Files identical despite different names*

### Comparing `core_module_periodic_table_app-2.2.0/core_module_periodic_table_app/views.py` & `core_module_periodic_table_app-2.3.0/core_module_periodic_table_app/views.py`

 * *Files identical despite different names*

### Comparing `core_module_periodic_table_app-2.2.0/core_module_periodic_table_app.egg-info/PKG-INFO` & `core_module_periodic_table_app-2.3.0/core_module_periodic_table_app.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-module-periodic-table-app
-Version: 2.2.0
+Version: 2.3.0
 Summary: Periodic table module for the parser core project
 Home-page: https://github.com/usnistgov/core_module_periodic_table_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_module_periodic_table_app
         ==============================
```

### Comparing `core_module_periodic_table_app-2.2.0/core_module_periodic_table_app.egg-info/SOURCES.txt` & `core_module_periodic_table_app-2.3.0/core_module_periodic_table_app.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.md
 MANIFEST.in
 README.rst
 pyproject.toml
 requirements.core.txt
 requirements.txt
 setup.py
 core_module_periodic_table_app/__init__.py
```

### Comparing `core_module_periodic_table_app-2.2.0/setup.py` & `core_module_periodic_table_app-2.3.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_module_periodic_table_app",
-    version="2.2.0",
+    version="2.3.0",
     description="Periodic table module for the parser core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_module_periodic_table_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_module_periodic_table_app-2.2.0/tests/test_settings.py` & `core_module_periodic_table_app-2.3.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `core_module_periodic_table_app-2.2.0/tests/test_unit_views.py` & `core_module_periodic_table_app-2.3.0/tests/test_unit_views.py`

 * *Files identical despite different names*

