# Comparing `tmp/core_module_fancy_tree_registry_app-2.2.0.tar.gz` & `tmp/core_module_fancy_tree_registry_app-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/core_module_fancy_tree_registry_app-2.2.0.tar", last modified: Thu Feb 23 20:32:24 2023, max compression
+gzip compressed data, was "core_module_fancy_tree_registry_app-2.3.0.tar", last modified: Tue May  2 19:46:03 2023, max compression
```

## Comparing `core_module_fancy_tree_registry_app-2.2.0.tar` & `core_module_fancy_tree_registry_app-2.3.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:24.000000 core_module_fancy_tree_registry_app-2.2.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      203 2023-02-23 20:32:21.000000 core_module_fancy_tree_registry_app-2.2.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1154 2023-02-23 20:32:24.000000 core_module_fancy_tree_registry_app-2.2.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      654 2023-02-23 20:32:21.000000 core_module_fancy_tree_registry_app-2.2.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:24.000000 core_module_fancy_tree_registry_app-2.2.0/core_module_fancy_tree_registry_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:21.000000 core_module_fancy_tree_registry_app-2.2.0/core_module_fancy_tree_registry_app/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:24.000000 core_module_fancy_tree_registry_app-2.2.0/core_module_fancy_tree_registry_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:24.000000 core_module_fancy_tree_registry_app-2.2.0/core_module_fancy_tree_registry_app/static/core_module_fancy_tree_registry_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:24.000000 core_module_fancy_tree_registry_app-2.2.0/core_module_fancy_tree_registry_app/static/core_module_fancy_tree_registry_app/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      605 2023-02-23 20:32:21.000000 core_module_fancy_tree_registry_app-2.2.0/core_module_fancy_tree_registry_app/static/core_module_fancy_tree_registry_app/js/fancy_tree.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:24.000000 core_module_fancy_tree_registry_app-2.2.0/core_module_fancy_tree_registry_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:24.000000 core_module_fancy_tree_registry_app-2.2.0/core_module_fancy_tree_registry_app/templates/core_module_fancy_tree_registry_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       89 2023-02-23 20:32:21.000000 core_module_fancy_tree_registry_app-2.2.0/core_module_fancy_tree_registry_app/templates/core_module_fancy_tree_registry_app/fancy_tree.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      316 2023-02-23 20:32:21.000000 core_module_fancy_tree_registry_app-2.2.0/core_module_fancy_tree_registry_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:24.000000 core_module_fancy_tree_registry_app-2.2.0/core_module_fancy_tree_registry_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:22.000000 core_module_fancy_tree_registry_app-2.2.0/core_module_fancy_tree_registry_app/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1087 2023-02-23 20:32:22.000000 core_module_fancy_tree_registry_app-2.2.0/core_module_fancy_tree_registry_app/views/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6987 2023-02-23 20:32:22.000000 core_module_fancy_tree_registry_app-2.2.0/core_module_fancy_tree_registry_app/views/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:24.000000 core_module_fancy_tree_registry_app-2.2.0/core_module_fancy_tree_registry_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1154 2023-02-23 20:32:24.000000 core_module_fancy_tree_registry_app-2.2.0/core_module_fancy_tree_registry_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      862 2023-02-23 20:32:24.000000 core_module_fancy_tree_registry_app-2.2.0/core_module_fancy_tree_registry_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-02-23 20:32:24.000000 core_module_fancy_tree_registry_app-2.2.0/core_module_fancy_tree_registry_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       60 2023-02-23 20:32:24.000000 core_module_fancy_tree_registry_app-2.2.0/core_module_fancy_tree_registry_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       42 2023-02-23 20:32:24.000000 core_module_fancy_tree_registry_app-2.2.0/core_module_fancy_tree_registry_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-02-23 20:32:22.000000 core_module_fancy_tree_registry_app-2.2.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       53 2023-02-23 20:32:22.000000 core_module_fancy_tree_registry_app-2.2.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        7 2023-02-23 20:32:22.000000 core_module_fancy_tree_registry_app-2.2.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-02-23 20:32:24.000000 core_module_fancy_tree_registry_app-2.2.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1104 2023-02-23 20:32:22.000000 core_module_fancy_tree_registry_app-2.2.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:24.000000 core_module_fancy_tree_registry_app-2.2.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:22.000000 core_module_fancy_tree_registry_app-2.2.0/tests/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      119 2023-02-23 20:32:23.000000 core_module_fancy_tree_registry_app-2.2.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:03.372286 core_module_fancy_tree_registry_app-2.3.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:46:01.000000 core_module_fancy_tree_registry_app-2.3.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      203 2023-05-02 19:46:01.000000 core_module_fancy_tree_registry_app-2.3.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1154 2023-05-02 19:46:03.367563 core_module_fancy_tree_registry_app-2.3.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      654 2023-05-02 19:46:01.000000 core_module_fancy_tree_registry_app-2.3.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:03.179972 core_module_fancy_tree_registry_app-2.3.0/core_module_fancy_tree_registry_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:01.000000 core_module_fancy_tree_registry_app-2.3.0/core_module_fancy_tree_registry_app/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:03.040377 core_module_fancy_tree_registry_app-2.3.0/core_module_fancy_tree_registry_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:03.043907 core_module_fancy_tree_registry_app-2.3.0/core_module_fancy_tree_registry_app/static/core_module_fancy_tree_registry_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:03.271141 core_module_fancy_tree_registry_app-2.3.0/core_module_fancy_tree_registry_app/static/core_module_fancy_tree_registry_app/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      605 2023-05-02 19:46:01.000000 core_module_fancy_tree_registry_app-2.3.0/core_module_fancy_tree_registry_app/static/core_module_fancy_tree_registry_app/js/fancy_tree.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:03.054706 core_module_fancy_tree_registry_app-2.3.0/core_module_fancy_tree_registry_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:03.284482 core_module_fancy_tree_registry_app-2.3.0/core_module_fancy_tree_registry_app/templates/core_module_fancy_tree_registry_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       89 2023-05-02 19:46:01.000000 core_module_fancy_tree_registry_app-2.3.0/core_module_fancy_tree_registry_app/templates/core_module_fancy_tree_registry_app/fancy_tree.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      316 2023-05-02 19:46:01.000000 core_module_fancy_tree_registry_app-2.3.0/core_module_fancy_tree_registry_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:03.324577 core_module_fancy_tree_registry_app-2.3.0/core_module_fancy_tree_registry_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:01.000000 core_module_fancy_tree_registry_app-2.3.0/core_module_fancy_tree_registry_app/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1087 2023-05-02 19:46:01.000000 core_module_fancy_tree_registry_app-2.3.0/core_module_fancy_tree_registry_app/views/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6987 2023-05-02 19:46:01.000000 core_module_fancy_tree_registry_app-2.3.0/core_module_fancy_tree_registry_app/views/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:03.248910 core_module_fancy_tree_registry_app-2.3.0/core_module_fancy_tree_registry_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1154 2023-05-02 19:46:02.000000 core_module_fancy_tree_registry_app-2.3.0/core_module_fancy_tree_registry_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      873 2023-05-02 19:46:02.000000 core_module_fancy_tree_registry_app-2.3.0/core_module_fancy_tree_registry_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:46:02.000000 core_module_fancy_tree_registry_app-2.3.0/core_module_fancy_tree_registry_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       60 2023-05-02 19:46:02.000000 core_module_fancy_tree_registry_app-2.3.0/core_module_fancy_tree_registry_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       42 2023-05-02 19:46:02.000000 core_module_fancy_tree_registry_app-2.3.0/core_module_fancy_tree_registry_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:46:01.000000 core_module_fancy_tree_registry_app-2.3.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       53 2023-05-02 19:46:01.000000 core_module_fancy_tree_registry_app-2.3.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        7 2023-05-02 19:46:01.000000 core_module_fancy_tree_registry_app-2.3.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:46:03.375342 core_module_fancy_tree_registry_app-2.3.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1104 2023-05-02 19:46:01.000000 core_module_fancy_tree_registry_app-2.3.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:03.358334 core_module_fancy_tree_registry_app-2.3.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:01.000000 core_module_fancy_tree_registry_app-2.3.0/tests/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      119 2023-05-02 19:46:01.000000 core_module_fancy_tree_registry_app-2.3.0/tests/test_settings.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `core_module_fancy_tree_registry_app-2.2.0/PKG-INFO` & `core_module_fancy_tree_registry_app-2.3.0/core_module_fancy_tree_registry_app.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
-Name: core_module_fancy_tree_registry_app
-Version: 2.2.0
+Name: core-module-fancy-tree-registry-app
+Version: 2.3.0
 Summary: Fancy Tree module for the parser core project
 Home-page: https://github.com/usnistgov/core_module_fancy_tree_registry_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_module_fancy_tree_registry_app
         ===================================
```

### Comparing `core_module_fancy_tree_registry_app-2.2.0/README.rst` & `core_module_fancy_tree_registry_app-2.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_module_fancy_tree_registry_app-2.2.0/core_module_fancy_tree_registry_app/static/core_module_fancy_tree_registry_app/js/fancy_tree.js` & `core_module_fancy_tree_registry_app-2.3.0/core_module_fancy_tree_registry_app/static/core_module_fancy_tree_registry_app/js/fancy_tree.js`

 * *Files identical despite different names*

### Comparing `core_module_fancy_tree_registry_app-2.2.0/core_module_fancy_tree_registry_app/views/forms.py` & `core_module_fancy_tree_registry_app-2.3.0/core_module_fancy_tree_registry_app/views/forms.py`

 * *Files identical despite different names*

### Comparing `core_module_fancy_tree_registry_app-2.2.0/core_module_fancy_tree_registry_app/views/views.py` & `core_module_fancy_tree_registry_app-2.3.0/core_module_fancy_tree_registry_app/views/views.py`

 * *Files identical despite different names*

### Comparing `core_module_fancy_tree_registry_app-2.2.0/core_module_fancy_tree_registry_app.egg-info/PKG-INFO` & `core_module_fancy_tree_registry_app-2.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
-Name: core-module-fancy-tree-registry-app
-Version: 2.2.0
+Name: core_module_fancy_tree_registry_app
+Version: 2.3.0
 Summary: Fancy Tree module for the parser core project
 Home-page: https://github.com/usnistgov/core_module_fancy_tree_registry_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_module_fancy_tree_registry_app
         ===================================
```

### Comparing `core_module_fancy_tree_registry_app-2.2.0/core_module_fancy_tree_registry_app.egg-info/SOURCES.txt` & `core_module_fancy_tree_registry_app-2.3.0/core_module_fancy_tree_registry_app.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.md
 MANIFEST.in
 README.rst
 pyproject.toml
 requirements.core.txt
 requirements.txt
 setup.py
 core_module_fancy_tree_registry_app/__init__.py
```

### Comparing `core_module_fancy_tree_registry_app-2.2.0/setup.py` & `core_module_fancy_tree_registry_app-2.3.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_module_fancy_tree_registry_app",
-    version="2.2.0",
+    version="2.3.0",
     description="Fancy Tree module for the parser core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_module_fancy_tree_registry_app",
     packages=find_packages(),
     include_package_data=True,
```

