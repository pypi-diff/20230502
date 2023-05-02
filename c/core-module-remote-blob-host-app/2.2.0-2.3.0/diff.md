# Comparing `tmp/core_module_remote_blob_host_app-2.2.0.tar.gz` & `tmp/core_module_remote_blob_host_app-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/core_module_remote_blob_host_app-2.2.0.tar", last modified: Thu Feb 23 20:32:56 2023, max compression
+gzip compressed data, was "core_module_remote_blob_host_app-2.3.0.tar", last modified: Tue May  2 19:46:34 2023, max compression
```

## Comparing `core_module_remote_blob_host_app-2.2.0.tar` & `core_module_remote_blob_host_app-2.3.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:56.000000 core_module_remote_blob_host_app-2.2.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      197 2023-02-23 20:32:54.000000 core_module_remote_blob_host_app-2.2.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1136 2023-02-23 20:32:56.000000 core_module_remote_blob_host_app-2.2.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      636 2023-02-23 20:32:54.000000 core_module_remote_blob_host_app-2.2.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:56.000000 core_module_remote_blob_host_app-2.2.0/core_module_remote_blob_host_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:54.000000 core_module_remote_blob_host_app-2.2.0/core_module_remote_blob_host_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      435 2023-02-23 20:32:54.000000 core_module_remote_blob_host_app-2.2.0/core_module_remote_blob_host_app/settings.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      328 2023-02-23 20:32:54.000000 core_module_remote_blob_host_app-2.2.0/core_module_remote_blob_host_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:56.000000 core_module_remote_blob_host_app-2.2.0/core_module_remote_blob_host_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:54.000000 core_module_remote_blob_host_app-2.2.0/core_module_remote_blob_host_app/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      157 2023-02-23 20:32:54.000000 core_module_remote_blob_host_app-2.2.0/core_module_remote_blob_host_app/views/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1903 2023-02-23 20:32:54.000000 core_module_remote_blob_host_app-2.2.0/core_module_remote_blob_host_app/views/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:56.000000 core_module_remote_blob_host_app-2.2.0/core_module_remote_blob_host_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1136 2023-02-23 20:32:55.000000 core_module_remote_blob_host_app-2.2.0/core_module_remote_blob_host_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      683 2023-02-23 20:32:56.000000 core_module_remote_blob_host_app-2.2.0/core_module_remote_blob_host_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-02-23 20:32:55.000000 core_module_remote_blob_host_app-2.2.0/core_module_remote_blob_host_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       84 2023-02-23 20:32:55.000000 core_module_remote_blob_host_app-2.2.0/core_module_remote_blob_host_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       39 2023-02-23 20:32:55.000000 core_module_remote_blob_host_app-2.2.0/core_module_remote_blob_host_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-02-23 20:32:54.000000 core_module_remote_blob_host_app-2.2.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-02-23 20:32:54.000000 core_module_remote_blob_host_app-2.2.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        7 2023-02-23 20:32:54.000000 core_module_remote_blob_host_app-2.2.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-02-23 20:32:56.000000 core_module_remote_blob_host_app-2.2.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1101 2023-02-23 20:32:54.000000 core_module_remote_blob_host_app-2.2.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:56.000000 core_module_remote_blob_host_app-2.2.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:54.000000 core_module_remote_blob_host_app-2.2.0/tests/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      119 2023-02-23 20:32:54.000000 core_module_remote_blob_host_app-2.2.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:34.001753 core_module_remote_blob_host_app-2.3.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:46:32.000000 core_module_remote_blob_host_app-2.3.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      197 2023-05-02 19:46:32.000000 core_module_remote_blob_host_app-2.3.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1136 2023-05-02 19:46:33.996939 core_module_remote_blob_host_app-2.3.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      636 2023-05-02 19:46:32.000000 core_module_remote_blob_host_app-2.3.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:33.839465 core_module_remote_blob_host_app-2.3.0/core_module_remote_blob_host_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:32.000000 core_module_remote_blob_host_app-2.3.0/core_module_remote_blob_host_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      435 2023-05-02 19:46:32.000000 core_module_remote_blob_host_app-2.3.0/core_module_remote_blob_host_app/settings.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      328 2023-05-02 19:46:32.000000 core_module_remote_blob_host_app-2.3.0/core_module_remote_blob_host_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:33.948647 core_module_remote_blob_host_app-2.3.0/core_module_remote_blob_host_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:32.000000 core_module_remote_blob_host_app-2.3.0/core_module_remote_blob_host_app/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      157 2023-05-02 19:46:32.000000 core_module_remote_blob_host_app-2.3.0/core_module_remote_blob_host_app/views/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1903 2023-05-02 19:46:32.000000 core_module_remote_blob_host_app-2.3.0/core_module_remote_blob_host_app/views/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:33.904442 core_module_remote_blob_host_app-2.3.0/core_module_remote_blob_host_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1136 2023-05-02 19:46:33.000000 core_module_remote_blob_host_app-2.3.0/core_module_remote_blob_host_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      694 2023-05-02 19:46:33.000000 core_module_remote_blob_host_app-2.3.0/core_module_remote_blob_host_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:46:33.000000 core_module_remote_blob_host_app-2.3.0/core_module_remote_blob_host_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       84 2023-05-02 19:46:33.000000 core_module_remote_blob_host_app-2.3.0/core_module_remote_blob_host_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       39 2023-05-02 19:46:33.000000 core_module_remote_blob_host_app-2.3.0/core_module_remote_blob_host_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:46:32.000000 core_module_remote_blob_host_app-2.3.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:46:32.000000 core_module_remote_blob_host_app-2.3.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        7 2023-05-02 19:46:32.000000 core_module_remote_blob_host_app-2.3.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:46:34.003529 core_module_remote_blob_host_app-2.3.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1101 2023-05-02 19:46:32.000000 core_module_remote_blob_host_app-2.3.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:33.987651 core_module_remote_blob_host_app-2.3.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:32.000000 core_module_remote_blob_host_app-2.3.0/tests/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      119 2023-05-02 19:46:32.000000 core_module_remote_blob_host_app-2.3.0/tests/test_settings.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `core_module_remote_blob_host_app-2.2.0/PKG-INFO` & `core_module_remote_blob_host_app-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_module_remote_blob_host_app
-Version: 2.2.0
+Version: 2.3.0
 Summary: Remote Blob Host module for the parser core project
 Home-page: https://github.com/usnistgov/core_module_remote_blob_host_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_module_remote_blob_host_app
         ================================
```

### Comparing `core_module_remote_blob_host_app-2.2.0/README.rst` & `core_module_remote_blob_host_app-2.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_module_remote_blob_host_app-2.2.0/core_module_remote_blob_host_app/views/views.py` & `core_module_remote_blob_host_app-2.3.0/core_module_remote_blob_host_app/views/views.py`

 * *Files identical despite different names*

### Comparing `core_module_remote_blob_host_app-2.2.0/core_module_remote_blob_host_app.egg-info/PKG-INFO` & `core_module_remote_blob_host_app-2.3.0/core_module_remote_blob_host_app.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-module-remote-blob-host-app
-Version: 2.2.0
+Version: 2.3.0
 Summary: Remote Blob Host module for the parser core project
 Home-page: https://github.com/usnistgov/core_module_remote_blob_host_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_module_remote_blob_host_app
         ================================
```

### Comparing `core_module_remote_blob_host_app-2.2.0/core_module_remote_blob_host_app.egg-info/SOURCES.txt` & `core_module_remote_blob_host_app-2.3.0/core_module_remote_blob_host_app.egg-info/SOURCES.txt`

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
 core_module_remote_blob_host_app/__init__.py
```

### Comparing `core_module_remote_blob_host_app-2.2.0/setup.py` & `core_module_remote_blob_host_app-2.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_module_remote_blob_host_app",
-    version="2.2.0",
+    version="2.3.0",
     description="Remote Blob Host module for the parser core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_module_remote_blob_host_app",
     packages=find_packages(),
     include_package_data=True,
```

