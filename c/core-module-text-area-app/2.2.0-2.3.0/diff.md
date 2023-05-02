# Comparing `tmp/core_module_text_area_app-2.2.0.tar.gz` & `tmp/core_module_text_area_app-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/core_module_text_area_app-2.2.0.tar", last modified: Thu Feb 23 20:33:09 2023, max compression
+gzip compressed data, was "core_module_text_area_app-2.3.0.tar", last modified: Tue May  2 19:46:49 2023, max compression
```

## Comparing `core_module_text_area_app-2.2.0.tar` & `core_module_text_area_app-2.3.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:09.000000 core_module_text_area_app-2.2.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      183 2023-02-23 20:33:08.000000 core_module_text_area_app-2.2.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1052 2023-02-23 20:33:09.000000 core_module_text_area_app-2.2.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      573 2023-02-23 20:33:08.000000 core_module_text_area_app-2.2.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:09.000000 core_module_text_area_app-2.2.0/core_module_text_area_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:08.000000 core_module_text_area_app-2.2.0/core_module_text_area_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      587 2023-02-23 20:33:08.000000 core_module_text_area_app-2.2.0/core_module_text_area_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:09.000000 core_module_text_area_app-2.2.0/core_module_text_area_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:09.000000 core_module_text_area_app-2.2.0/core_module_text_area_app/templates/core_module_text_area_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      159 2023-02-23 20:33:08.000000 core_module_text_area_app-2.2.0/core_module_text_area_app/templates/core_module_text_area_app/predefined_entities_warning.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      288 2023-02-23 20:33:08.000000 core_module_text_area_app-2.2.0/core_module_text_area_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:09.000000 core_module_text_area_app-2.2.0/core_module_text_area_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:08.000000 core_module_text_area_app-2.2.0/core_module_text_area_app/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1851 2023-02-23 20:33:08.000000 core_module_text_area_app-2.2.0/core_module_text_area_app/views/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:09.000000 core_module_text_area_app-2.2.0/core_module_text_area_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1052 2023-02-23 20:33:09.000000 core_module_text_area_app-2.2.0/core_module_text_area_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      685 2023-02-23 20:33:09.000000 core_module_text_area_app-2.2.0/core_module_text_area_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-02-23 20:33:09.000000 core_module_text_area_app-2.2.0/core_module_text_area_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       48 2023-02-23 20:33:09.000000 core_module_text_area_app-2.2.0/core_module_text_area_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       32 2023-02-23 20:33:09.000000 core_module_text_area_app-2.2.0/core_module_text_area_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-02-23 20:33:08.000000 core_module_text_area_app-2.2.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       41 2023-02-23 20:33:08.000000 core_module_text_area_app-2.2.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        7 2023-02-23 20:33:08.000000 core_module_text_area_app-2.2.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-02-23 20:33:09.000000 core_module_text_area_app-2.2.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1073 2023-02-23 20:33:08.000000 core_module_text_area_app-2.2.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:09.000000 core_module_text_area_app-2.2.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:08.000000 core_module_text_area_app-2.2.0/tests/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1312 2023-02-23 20:33:08.000000 core_module_text_area_app-2.2.0/tests/test_settings.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2836 2023-02-23 20:33:08.000000 core_module_text_area_app-2.2.0/tests/test_unit_views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:49.964343 core_module_text_area_app-2.3.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:46:48.000000 core_module_text_area_app-2.3.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      183 2023-05-02 19:46:48.000000 core_module_text_area_app-2.3.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1052 2023-05-02 19:46:49.960195 core_module_text_area_app-2.3.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      573 2023-05-02 19:46:48.000000 core_module_text_area_app-2.3.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:49.819577 core_module_text_area_app-2.3.0/core_module_text_area_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:48.000000 core_module_text_area_app-2.3.0/core_module_text_area_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      587 2023-05-02 19:46:48.000000 core_module_text_area_app-2.3.0/core_module_text_area_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:49.697050 core_module_text_area_app-2.3.0/core_module_text_area_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:49.894989 core_module_text_area_app-2.3.0/core_module_text_area_app/templates/core_module_text_area_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      159 2023-05-02 19:46:48.000000 core_module_text_area_app-2.3.0/core_module_text_area_app/templates/core_module_text_area_app/predefined_entities_warning.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      288 2023-05-02 19:46:48.000000 core_module_text_area_app-2.3.0/core_module_text_area_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:49.918215 core_module_text_area_app-2.3.0/core_module_text_area_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:48.000000 core_module_text_area_app-2.3.0/core_module_text_area_app/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1851 2023-05-02 19:46:48.000000 core_module_text_area_app-2.3.0/core_module_text_area_app/views/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:49.880791 core_module_text_area_app-2.3.0/core_module_text_area_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1052 2023-05-02 19:46:49.000000 core_module_text_area_app-2.3.0/core_module_text_area_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      696 2023-05-02 19:46:49.000000 core_module_text_area_app-2.3.0/core_module_text_area_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:46:49.000000 core_module_text_area_app-2.3.0/core_module_text_area_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       48 2023-05-02 19:46:49.000000 core_module_text_area_app-2.3.0/core_module_text_area_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       32 2023-05-02 19:46:49.000000 core_module_text_area_app-2.3.0/core_module_text_area_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:46:48.000000 core_module_text_area_app-2.3.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       41 2023-05-02 19:46:48.000000 core_module_text_area_app-2.3.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        7 2023-05-02 19:46:48.000000 core_module_text_area_app-2.3.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:46:49.968556 core_module_text_area_app-2.3.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1073 2023-05-02 19:46:48.000000 core_module_text_area_app-2.3.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:49.951981 core_module_text_area_app-2.3.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:48.000000 core_module_text_area_app-2.3.0/tests/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1312 2023-05-02 19:46:48.000000 core_module_text_area_app-2.3.0/tests/test_settings.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2836 2023-05-02 19:46:48.000000 core_module_text_area_app-2.3.0/tests/test_unit_views.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `core_module_text_area_app-2.2.0/PKG-INFO` & `core_module_text_area_app-2.3.0/core_module_text_area_app.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
-Name: core_module_text_area_app
-Version: 2.2.0
+Name: core-module-text-area-app
+Version: 2.3.0
 Summary: Text Area module for the parser core project
 Home-page: https://github.com/usnistgov/core_module_text_area_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_module_text_area_app
         =========================
```

### Comparing `core_module_text_area_app-2.2.0/README.rst` & `core_module_text_area_app-2.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_module_text_area_app-2.2.0/core_module_text_area_app/settings.py` & `core_module_text_area_app-2.3.0/core_module_text_area_app/settings.py`

 * *Files identical despite different names*

### Comparing `core_module_text_area_app-2.2.0/core_module_text_area_app/views/views.py` & `core_module_text_area_app-2.3.0/core_module_text_area_app/views/views.py`

 * *Files identical despite different names*

### Comparing `core_module_text_area_app-2.2.0/core_module_text_area_app.egg-info/PKG-INFO` & `core_module_text_area_app-2.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
-Name: core-module-text-area-app
-Version: 2.2.0
+Name: core_module_text_area_app
+Version: 2.3.0
 Summary: Text Area module for the parser core project
 Home-page: https://github.com/usnistgov/core_module_text_area_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_module_text_area_app
         =========================
```

### Comparing `core_module_text_area_app-2.2.0/core_module_text_area_app.egg-info/SOURCES.txt` & `core_module_text_area_app-2.3.0/core_module_text_area_app.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.md
 MANIFEST.in
 README.rst
 pyproject.toml
 requirements.core.txt
 requirements.txt
 setup.py
 core_module_text_area_app/__init__.py
```

### Comparing `core_module_text_area_app-2.2.0/setup.py` & `core_module_text_area_app-2.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_module_text_area_app",
-    version="2.2.0",
+    version="2.3.0",
     description="Text Area module for the parser core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_module_text_area_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_module_text_area_app-2.2.0/tests/test_settings.py` & `core_module_text_area_app-2.3.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `core_module_text_area_app-2.2.0/tests/test_unit_views.py` & `core_module_text_area_app-2.3.0/tests/test_unit_views.py`

 * *Files identical despite different names*

