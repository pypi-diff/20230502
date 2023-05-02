# Comparing `tmp/core_module_raw_xml_app-2.2.0.tar.gz` & `tmp/core_module_raw_xml_app-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/core_module_raw_xml_app-2.2.0.tar", last modified: Thu Feb 23 20:32:47 2023, max compression
+gzip compressed data, was "core_module_raw_xml_app-2.3.0.tar", last modified: Tue May  2 19:46:27 2023, max compression
```

## Comparing `core_module_raw_xml_app-2.2.0.tar` & `core_module_raw_xml_app-2.3.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:47.000000 core_module_raw_xml_app-2.2.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      179 2023-02-23 20:32:45.000000 core_module_raw_xml_app-2.2.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1028 2023-02-23 20:32:47.000000 core_module_raw_xml_app-2.2.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      555 2023-02-23 20:32:45.000000 core_module_raw_xml_app-2.2.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:47.000000 core_module_raw_xml_app-2.2.0/core_module_raw_xml_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:45.000000 core_module_raw_xml_app-2.2.0/core_module_raw_xml_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      276 2023-02-23 20:32:45.000000 core_module_raw_xml_app-2.2.0/core_module_raw_xml_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:47.000000 core_module_raw_xml_app-2.2.0/core_module_raw_xml_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:45.000000 core_module_raw_xml_app-2.2.0/core_module_raw_xml_app/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2686 2023-02-23 20:32:45.000000 core_module_raw_xml_app-2.2.0/core_module_raw_xml_app/views/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:47.000000 core_module_raw_xml_app-2.2.0/core_module_raw_xml_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1028 2023-02-23 20:32:46.000000 core_module_raw_xml_app-2.2.0/core_module_raw_xml_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      534 2023-02-23 20:32:47.000000 core_module_raw_xml_app-2.2.0/core_module_raw_xml_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-02-23 20:32:46.000000 core_module_raw_xml_app-2.2.0/core_module_raw_xml_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       58 2023-02-23 20:32:46.000000 core_module_raw_xml_app-2.2.0/core_module_raw_xml_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       30 2023-02-23 20:32:46.000000 core_module_raw_xml_app-2.2.0/core_module_raw_xml_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-02-23 20:32:45.000000 core_module_raw_xml_app-2.2.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       51 2023-02-23 20:32:45.000000 core_module_raw_xml_app-2.2.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        7 2023-02-23 20:32:45.000000 core_module_raw_xml_app-2.2.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-02-23 20:32:47.000000 core_module_raw_xml_app-2.2.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1065 2023-02-23 20:32:45.000000 core_module_raw_xml_app-2.2.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:47.000000 core_module_raw_xml_app-2.2.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:45.000000 core_module_raw_xml_app-2.2.0/tests/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      120 2023-02-23 20:32:45.000000 core_module_raw_xml_app-2.2.0/tests/test_settings.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       33 2023-02-23 20:32:45.000000 core_module_raw_xml_app-2.2.0/tests/test_unit_views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:27.279566 core_module_raw_xml_app-2.3.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:46:25.000000 core_module_raw_xml_app-2.3.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      179 2023-05-02 19:46:25.000000 core_module_raw_xml_app-2.3.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1028 2023-05-02 19:46:27.273971 core_module_raw_xml_app-2.3.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      555 2023-05-02 19:46:25.000000 core_module_raw_xml_app-2.3.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:27.098338 core_module_raw_xml_app-2.3.0/core_module_raw_xml_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:25.000000 core_module_raw_xml_app-2.3.0/core_module_raw_xml_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      276 2023-05-02 19:46:25.000000 core_module_raw_xml_app-2.3.0/core_module_raw_xml_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:27.205685 core_module_raw_xml_app-2.3.0/core_module_raw_xml_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:25.000000 core_module_raw_xml_app-2.3.0/core_module_raw_xml_app/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2686 2023-05-02 19:46:25.000000 core_module_raw_xml_app-2.3.0/core_module_raw_xml_app/views/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:27.171906 core_module_raw_xml_app-2.3.0/core_module_raw_xml_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1028 2023-05-02 19:46:26.000000 core_module_raw_xml_app-2.3.0/core_module_raw_xml_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      545 2023-05-02 19:46:26.000000 core_module_raw_xml_app-2.3.0/core_module_raw_xml_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:46:26.000000 core_module_raw_xml_app-2.3.0/core_module_raw_xml_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       58 2023-05-02 19:46:26.000000 core_module_raw_xml_app-2.3.0/core_module_raw_xml_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       30 2023-05-02 19:46:26.000000 core_module_raw_xml_app-2.3.0/core_module_raw_xml_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:46:25.000000 core_module_raw_xml_app-2.3.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       51 2023-05-02 19:46:25.000000 core_module_raw_xml_app-2.3.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        7 2023-05-02 19:46:25.000000 core_module_raw_xml_app-2.3.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:46:27.281816 core_module_raw_xml_app-2.3.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1065 2023-05-02 19:46:25.000000 core_module_raw_xml_app-2.3.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:27.244884 core_module_raw_xml_app-2.3.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:25.000000 core_module_raw_xml_app-2.3.0/tests/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      120 2023-05-02 19:46:25.000000 core_module_raw_xml_app-2.3.0/tests/test_settings.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       33 2023-05-02 19:46:25.000000 core_module_raw_xml_app-2.3.0/tests/test_unit_views.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `core_module_raw_xml_app-2.2.0/PKG-INFO` & `core_module_raw_xml_app-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_module_raw_xml_app
-Version: 2.2.0
+Version: 2.3.0
 Summary: Raw xml module for the parser core project
 Home-page: https://github.com/usnistgov/core_module_raw_xml_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_module_raw_xml_app
         =======================
```

### Comparing `core_module_raw_xml_app-2.2.0/README.rst` & `core_module_raw_xml_app-2.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_module_raw_xml_app-2.2.0/core_module_raw_xml_app/views/views.py` & `core_module_raw_xml_app-2.3.0/core_module_raw_xml_app/views/views.py`

 * *Files identical despite different names*

### Comparing `core_module_raw_xml_app-2.2.0/core_module_raw_xml_app.egg-info/PKG-INFO` & `core_module_raw_xml_app-2.3.0/core_module_raw_xml_app.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-module-raw-xml-app
-Version: 2.2.0
+Version: 2.3.0
 Summary: Raw xml module for the parser core project
 Home-page: https://github.com/usnistgov/core_module_raw_xml_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_module_raw_xml_app
         =======================
```

### Comparing `core_module_raw_xml_app-2.2.0/core_module_raw_xml_app.egg-info/SOURCES.txt` & `core_module_raw_xml_app-2.3.0/core_module_raw_xml_app.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.md
 MANIFEST.in
 README.rst
 pyproject.toml
 requirements.core.txt
 requirements.txt
 setup.py
 core_module_raw_xml_app/__init__.py
```

### Comparing `core_module_raw_xml_app-2.2.0/setup.py` & `core_module_raw_xml_app-2.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_module_raw_xml_app",
-    version="2.2.0",
+    version="2.3.0",
     description="Raw xml module for the parser core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_module_raw_xml_app",
     packages=find_packages(),
     include_package_data=True,
```

