# Comparing `tmp/core_module_local_id_registry_app-2.2.0.tar.gz` & `tmp/core_module_local_id_registry_app-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/core_module_local_id_registry_app-2.2.0.tar", last modified: Thu Feb 23 20:32:32 2023, max compression
+gzip compressed data, was "core_module_local_id_registry_app-2.3.0.tar", last modified: Tue May  2 19:46:12 2023, max compression
```

## Comparing `core_module_local_id_registry_app-2.2.0.tar` & `core_module_local_id_registry_app-2.3.0.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:32.000000 core_module_local_id_registry_app-2.2.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      199 2023-02-23 20:32:30.000000 core_module_local_id_registry_app-2.2.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1091 2023-02-23 20:32:32.000000 core_module_local_id_registry_app-2.2.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      616 2023-02-23 20:32:30.000000 core_module_local_id_registry_app-2.2.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:32.000000 core_module_local_id_registry_app-2.2.0/core_module_local_id_registry_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:30.000000 core_module_local_id_registry_app-2.2.0/core_module_local_id_registry_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      600 2023-02-23 20:32:30.000000 core_module_local_id_registry_app-2.2.0/core_module_local_id_registry_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:32.000000 core_module_local_id_registry_app-2.2.0/core_module_local_id_registry_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:32.000000 core_module_local_id_registry_app-2.2.0/core_module_local_id_registry_app/static/core_module_local_id_registry_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:32.000000 core_module_local_id_registry_app-2.2.0/core_module_local_id_registry_app/static/core_module_local_id_registry_app/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      234 2023-02-23 20:32:30.000000 core_module_local_id_registry_app-2.2.0/core_module_local_id_registry_app/static/core_module_local_id_registry_app/css/module_local_id.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:32.000000 core_module_local_id_registry_app-2.2.0/core_module_local_id_registry_app/static/core_module_local_id_registry_app/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      974 2023-02-23 20:32:30.000000 core_module_local_id_registry_app-2.2.0/core_module_local_id_registry_app/static/core_module_local_id_registry_app/js/module_local_id.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:32.000000 core_module_local_id_registry_app-2.2.0/core_module_local_id_registry_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:32.000000 core_module_local_id_registry_app-2.2.0/core_module_local_id_registry_app/templates/core_module_local_id_registry_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       89 2023-02-23 20:32:30.000000 core_module_local_id_registry_app-2.2.0/core_module_local_id_registry_app/templates/core_module_local_id_registry_app/pid_display_box.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      408 2023-02-23 20:32:30.000000 core_module_local_id_registry_app-2.2.0/core_module_local_id_registry_app/templates/core_module_local_id_registry_app/pid_edit_input.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      334 2023-02-23 20:32:30.000000 core_module_local_id_registry_app-2.2.0/core_module_local_id_registry_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:32.000000 core_module_local_id_registry_app-2.2.0/core_module_local_id_registry_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:30.000000 core_module_local_id_registry_app-2.2.0/core_module_local_id_registry_app/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9379 2023-02-23 20:32:30.000000 core_module_local_id_registry_app-2.2.0/core_module_local_id_registry_app/views/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:32.000000 core_module_local_id_registry_app-2.2.0/core_module_local_id_registry_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1091 2023-02-23 20:32:31.000000 core_module_local_id_registry_app-2.2.0/core_module_local_id_registry_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1201 2023-02-23 20:32:32.000000 core_module_local_id_registry_app-2.2.0/core_module_local_id_registry_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-02-23 20:32:31.000000 core_module_local_id_registry_app-2.2.0/core_module_local_id_registry_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      104 2023-02-23 20:32:31.000000 core_module_local_id_registry_app-2.2.0/core_module_local_id_registry_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       40 2023-02-23 20:32:31.000000 core_module_local_id_registry_app-2.2.0/core_module_local_id_registry_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-02-23 20:32:30.000000 core_module_local_id_registry_app-2.2.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       97 2023-02-23 20:32:30.000000 core_module_local_id_registry_app-2.2.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        7 2023-02-23 20:32:30.000000 core_module_local_id_registry_app-2.2.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-02-23 20:32:32.000000 core_module_local_id_registry_app-2.2.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1081 2023-02-23 20:32:30.000000 core_module_local_id_registry_app-2.2.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:32.000000 core_module_local_id_registry_app-2.2.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:30.000000 core_module_local_id_registry_app-2.2.0/tests/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      971 2023-02-23 20:32:30.000000 core_module_local_id_registry_app-2.2.0/tests/test_settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:32.000000 core_module_local_id_registry_app-2.2.0/tests/views/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:32.000000 core_module_local_id_registry_app-2.2.0/tests/views/LocalIdRegistryModule/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:30.000000 core_module_local_id_registry_app-2.2.0/tests/views/LocalIdRegistryModule/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1918 2023-02-23 20:32:30.000000 core_module_local_id_registry_app-2.2.0/tests/views/LocalIdRegistryModule/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    38376 2023-02-23 20:32:30.000000 core_module_local_id_registry_app-2.2.0/tests/views/LocalIdRegistryModule/test_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:30.000000 core_module_local_id_registry_app-2.2.0/tests/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:12.641677 core_module_local_id_registry_app-2.3.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:46:10.000000 core_module_local_id_registry_app-2.3.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      199 2023-05-02 19:46:10.000000 core_module_local_id_registry_app-2.3.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1091 2023-05-02 19:46:12.637067 core_module_local_id_registry_app-2.3.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      616 2023-05-02 19:46:10.000000 core_module_local_id_registry_app-2.3.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:12.283016 core_module_local_id_registry_app-2.3.0/core_module_local_id_registry_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:10.000000 core_module_local_id_registry_app-2.3.0/core_module_local_id_registry_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      600 2023-05-02 19:46:10.000000 core_module_local_id_registry_app-2.3.0/core_module_local_id_registry_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:12.104740 core_module_local_id_registry_app-2.3.0/core_module_local_id_registry_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:12.111240 core_module_local_id_registry_app-2.3.0/core_module_local_id_registry_app/static/core_module_local_id_registry_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:12.362726 core_module_local_id_registry_app-2.3.0/core_module_local_id_registry_app/static/core_module_local_id_registry_app/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      537 2023-05-02 19:46:10.000000 core_module_local_id_registry_app-2.3.0/core_module_local_id_registry_app/static/core_module_local_id_registry_app/css/module_local_id.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:12.372084 core_module_local_id_registry_app-2.3.0/core_module_local_id_registry_app/static/core_module_local_id_registry_app/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      778 2023-05-02 19:46:10.000000 core_module_local_id_registry_app-2.3.0/core_module_local_id_registry_app/static/core_module_local_id_registry_app/js/module_local_id.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:12.118885 core_module_local_id_registry_app-2.3.0/core_module_local_id_registry_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:12.404573 core_module_local_id_registry_app-2.3.0/core_module_local_id_registry_app/templates/core_module_local_id_registry_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       89 2023-05-02 19:46:10.000000 core_module_local_id_registry_app-2.3.0/core_module_local_id_registry_app/templates/core_module_local_id_registry_app/pid_display_box.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      384 2023-05-02 19:46:10.000000 core_module_local_id_registry_app-2.3.0/core_module_local_id_registry_app/templates/core_module_local_id_registry_app/pid_edit_input.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      334 2023-05-02 19:46:10.000000 core_module_local_id_registry_app-2.3.0/core_module_local_id_registry_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:12.439470 core_module_local_id_registry_app-2.3.0/core_module_local_id_registry_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:10.000000 core_module_local_id_registry_app-2.3.0/core_module_local_id_registry_app/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9379 2023-05-02 19:46:10.000000 core_module_local_id_registry_app-2.3.0/core_module_local_id_registry_app/views/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:12.349438 core_module_local_id_registry_app-2.3.0/core_module_local_id_registry_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1091 2023-05-02 19:46:11.000000 core_module_local_id_registry_app-2.3.0/core_module_local_id_registry_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1212 2023-05-02 19:46:12.000000 core_module_local_id_registry_app-2.3.0/core_module_local_id_registry_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:46:11.000000 core_module_local_id_registry_app-2.3.0/core_module_local_id_registry_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      104 2023-05-02 19:46:11.000000 core_module_local_id_registry_app-2.3.0/core_module_local_id_registry_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       40 2023-05-02 19:46:11.000000 core_module_local_id_registry_app-2.3.0/core_module_local_id_registry_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:46:10.000000 core_module_local_id_registry_app-2.3.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       97 2023-05-02 19:46:10.000000 core_module_local_id_registry_app-2.3.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        7 2023-05-02 19:46:10.000000 core_module_local_id_registry_app-2.3.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:46:12.643361 core_module_local_id_registry_app-2.3.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1081 2023-05-02 19:46:10.000000 core_module_local_id_registry_app-2.3.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:12.538696 core_module_local_id_registry_app-2.3.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:10.000000 core_module_local_id_registry_app-2.3.0/tests/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      971 2023-05-02 19:46:10.000000 core_module_local_id_registry_app-2.3.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:12.551644 core_module_local_id_registry_app-2.3.0/tests/views/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:12.626986 core_module_local_id_registry_app-2.3.0/tests/views/LocalIdRegistryModule/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:10.000000 core_module_local_id_registry_app-2.3.0/tests/views/LocalIdRegistryModule/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1918 2023-05-02 19:46:10.000000 core_module_local_id_registry_app-2.3.0/tests/views/LocalIdRegistryModule/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    38376 2023-05-02 19:46:10.000000 core_module_local_id_registry_app-2.3.0/tests/views/LocalIdRegistryModule/test_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:10.000000 core_module_local_id_registry_app-2.3.0/tests/views/__init__.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `core_module_local_id_registry_app-2.2.0/PKG-INFO` & `core_module_local_id_registry_app-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_module_local_id_registry_app
-Version: 2.2.0
+Version: 2.3.0
 Summary: Local id registry module
 Home-page: https://github.com/usnistgov/core_module_local_id_registry_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_module_local_id_registry_app
         =================================
```

### Comparing `core_module_local_id_registry_app-2.2.0/README.rst` & `core_module_local_id_registry_app-2.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_module_local_id_registry_app-2.2.0/core_module_local_id_registry_app/settings.py` & `core_module_local_id_registry_app-2.3.0/core_module_local_id_registry_app/settings.py`

 * *Files identical despite different names*

### Comparing `core_module_local_id_registry_app-2.2.0/core_module_local_id_registry_app/views/views.py` & `core_module_local_id_registry_app-2.3.0/core_module_local_id_registry_app/views/views.py`

 * *Files identical despite different names*

### Comparing `core_module_local_id_registry_app-2.2.0/core_module_local_id_registry_app.egg-info/PKG-INFO` & `core_module_local_id_registry_app-2.3.0/core_module_local_id_registry_app.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-module-local-id-registry-app
-Version: 2.2.0
+Version: 2.3.0
 Summary: Local id registry module
 Home-page: https://github.com/usnistgov/core_module_local_id_registry_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_module_local_id_registry_app
         =================================
```

### Comparing `core_module_local_id_registry_app-2.2.0/core_module_local_id_registry_app.egg-info/SOURCES.txt` & `core_module_local_id_registry_app-2.3.0/core_module_local_id_registry_app.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.md
 MANIFEST.in
 README.rst
 pyproject.toml
 requirements.core.txt
 requirements.txt
 setup.py
 core_module_local_id_registry_app/__init__.py
```

### Comparing `core_module_local_id_registry_app-2.2.0/setup.py` & `core_module_local_id_registry_app-2.3.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_module_local_id_registry_app",
-    version="2.2.0",
+    version="2.3.0",
     description="Local id registry module",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_module_local_id_registry_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_module_local_id_registry_app-2.2.0/tests/test_settings.py` & `core_module_local_id_registry_app-2.3.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `core_module_local_id_registry_app-2.2.0/tests/views/LocalIdRegistryModule/fixtures.py` & `core_module_local_id_registry_app-2.3.0/tests/views/LocalIdRegistryModule/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_module_local_id_registry_app-2.2.0/tests/views/LocalIdRegistryModule/test_unit.py` & `core_module_local_id_registry_app-2.3.0/tests/views/LocalIdRegistryModule/test_unit.py`

 * *Files identical despite different names*

