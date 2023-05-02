# Comparing `tmp/core_module_excel_uploader_app-2.2.0.tar.gz` & `tmp/core_module_excel_uploader_app-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/core_module_excel_uploader_app-2.2.0.tar", last modified: Thu Feb 23 20:32:15 2023, max compression
+gzip compressed data, was "core_module_excel_uploader_app-2.3.0.tar", last modified: Tue May  2 19:45:53 2023, max compression
```

## Comparing `core_module_excel_uploader_app-2.2.0.tar` & `core_module_excel_uploader_app-2.3.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:15.000000 core_module_excel_uploader_app-2.2.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      193 2023-02-23 20:32:13.000000 core_module_excel_uploader_app-2.2.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1112 2023-02-23 20:32:15.000000 core_module_excel_uploader_app-2.2.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      618 2023-02-23 20:32:13.000000 core_module_excel_uploader_app-2.2.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:15.000000 core_module_excel_uploader_app-2.2.0/core_module_excel_uploader_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:13.000000 core_module_excel_uploader_app-2.2.0/core_module_excel_uploader_app/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:15.000000 core_module_excel_uploader_app-2.2.0/core_module_excel_uploader_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:15.000000 core_module_excel_uploader_app-2.2.0/core_module_excel_uploader_app/static/core_module_excel_uploader_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:15.000000 core_module_excel_uploader_app-2.2.0/core_module_excel_uploader_app/static/core_module_excel_uploader_app/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      426 2023-02-23 20:32:13.000000 core_module_excel_uploader_app-2.2.0/core_module_excel_uploader_app/static/core_module_excel_uploader_app/css/excel_uploader.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:15.000000 core_module_excel_uploader_app-2.2.0/core_module_excel_uploader_app/static/core_module_excel_uploader_app/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      310 2023-02-23 20:32:13.000000 core_module_excel_uploader_app-2.2.0/core_module_excel_uploader_app/static/core_module_excel_uploader_app/js/excel_uploader.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:15.000000 core_module_excel_uploader_app-2.2.0/core_module_excel_uploader_app/static/core_module_excel_uploader_app/xslx/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    22415 2023-02-23 20:32:13.000000 core_module_excel_uploader_app-2.2.0/core_module_excel_uploader_app/static/core_module_excel_uploader_app/xslx/data.xlsx
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:15.000000 core_module_excel_uploader_app-2.2.0/core_module_excel_uploader_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:15.000000 core_module_excel_uploader_app-2.2.0/core_module_excel_uploader_app/templates/core_module_excel_uploader_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      161 2023-02-23 20:32:13.000000 core_module_excel_uploader_app-2.2.0/core_module_excel_uploader_app/templates/core_module_excel_uploader_app/excel_uploader.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      318 2023-02-23 20:32:13.000000 core_module_excel_uploader_app-2.2.0/core_module_excel_uploader_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:15.000000 core_module_excel_uploader_app-2.2.0/core_module_excel_uploader_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:13.000000 core_module_excel_uploader_app-2.2.0/core_module_excel_uploader_app/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      178 2023-02-23 20:32:13.000000 core_module_excel_uploader_app-2.2.0/core_module_excel_uploader_app/views/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7529 2023-02-23 20:32:13.000000 core_module_excel_uploader_app-2.2.0/core_module_excel_uploader_app/views/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:15.000000 core_module_excel_uploader_app-2.2.0/core_module_excel_uploader_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1112 2023-02-23 20:32:14.000000 core_module_excel_uploader_app-2.2.0/core_module_excel_uploader_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      976 2023-02-23 20:32:15.000000 core_module_excel_uploader_app-2.2.0/core_module_excel_uploader_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-02-23 20:32:14.000000 core_module_excel_uploader_app-2.2.0/core_module_excel_uploader_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       60 2023-02-23 20:32:14.000000 core_module_excel_uploader_app-2.2.0/core_module_excel_uploader_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       37 2023-02-23 20:32:14.000000 core_module_excel_uploader_app-2.2.0/core_module_excel_uploader_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-02-23 20:32:13.000000 core_module_excel_uploader_app-2.2.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       41 2023-02-23 20:32:13.000000 core_module_excel_uploader_app-2.2.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       19 2023-02-23 20:32:13.000000 core_module_excel_uploader_app-2.2.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-02-23 20:32:15.000000 core_module_excel_uploader_app-2.2.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1093 2023-02-23 20:32:13.000000 core_module_excel_uploader_app-2.2.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:15.000000 core_module_excel_uploader_app-2.2.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:32:13.000000 core_module_excel_uploader_app-2.2.0/tests/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      120 2023-02-23 20:32:13.000000 core_module_excel_uploader_app-2.2.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:45:53.004203 core_module_excel_uploader_app-2.3.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:45:51.000000 core_module_excel_uploader_app-2.3.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      193 2023-05-02 19:45:51.000000 core_module_excel_uploader_app-2.3.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1160 2023-05-02 19:45:52.999256 core_module_excel_uploader_app-2.3.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      666 2023-05-02 19:45:51.000000 core_module_excel_uploader_app-2.3.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:45:52.782479 core_module_excel_uploader_app-2.3.0/core_module_excel_uploader_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:45:51.000000 core_module_excel_uploader_app-2.3.0/core_module_excel_uploader_app/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:45:52.631703 core_module_excel_uploader_app-2.3.0/core_module_excel_uploader_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:45:52.644435 core_module_excel_uploader_app-2.3.0/core_module_excel_uploader_app/static/core_module_excel_uploader_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:45:52.872592 core_module_excel_uploader_app-2.3.0/core_module_excel_uploader_app/static/core_module_excel_uploader_app/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      426 2023-05-02 19:45:51.000000 core_module_excel_uploader_app-2.3.0/core_module_excel_uploader_app/static/core_module_excel_uploader_app/css/excel_uploader.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:45:52.884409 core_module_excel_uploader_app-2.3.0/core_module_excel_uploader_app/static/core_module_excel_uploader_app/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      310 2023-05-02 19:45:51.000000 core_module_excel_uploader_app-2.3.0/core_module_excel_uploader_app/static/core_module_excel_uploader_app/js/excel_uploader.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:45:52.896551 core_module_excel_uploader_app-2.3.0/core_module_excel_uploader_app/static/core_module_excel_uploader_app/xls/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    25600 2023-05-02 19:45:51.000000 core_module_excel_uploader_app-2.3.0/core_module_excel_uploader_app/static/core_module_excel_uploader_app/xls/data.xls
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:45:52.653899 core_module_excel_uploader_app-2.3.0/core_module_excel_uploader_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:45:52.909402 core_module_excel_uploader_app-2.3.0/core_module_excel_uploader_app/templates/core_module_excel_uploader_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      161 2023-05-02 19:45:51.000000 core_module_excel_uploader_app-2.3.0/core_module_excel_uploader_app/templates/core_module_excel_uploader_app/excel_uploader.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      318 2023-05-02 19:45:51.000000 core_module_excel_uploader_app-2.3.0/core_module_excel_uploader_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:45:52.951185 core_module_excel_uploader_app-2.3.0/core_module_excel_uploader_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:45:51.000000 core_module_excel_uploader_app-2.3.0/core_module_excel_uploader_app/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      178 2023-05-02 19:45:51.000000 core_module_excel_uploader_app-2.3.0/core_module_excel_uploader_app/views/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7529 2023-05-02 19:45:51.000000 core_module_excel_uploader_app-2.3.0/core_module_excel_uploader_app/views/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:45:52.858525 core_module_excel_uploader_app-2.3.0/core_module_excel_uploader_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1160 2023-05-02 19:45:52.000000 core_module_excel_uploader_app-2.3.0/core_module_excel_uploader_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      985 2023-05-02 19:45:52.000000 core_module_excel_uploader_app-2.3.0/core_module_excel_uploader_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:45:52.000000 core_module_excel_uploader_app-2.3.0/core_module_excel_uploader_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       60 2023-05-02 19:45:52.000000 core_module_excel_uploader_app-2.3.0/core_module_excel_uploader_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       37 2023-05-02 19:45:52.000000 core_module_excel_uploader_app-2.3.0/core_module_excel_uploader_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:45:51.000000 core_module_excel_uploader_app-2.3.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       41 2023-05-02 19:45:51.000000 core_module_excel_uploader_app-2.3.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       19 2023-05-02 19:45:51.000000 core_module_excel_uploader_app-2.3.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:45:53.006231 core_module_excel_uploader_app-2.3.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1093 2023-05-02 19:45:51.000000 core_module_excel_uploader_app-2.3.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:45:52.989626 core_module_excel_uploader_app-2.3.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:45:51.000000 core_module_excel_uploader_app-2.3.0/tests/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      120 2023-05-02 19:45:51.000000 core_module_excel_uploader_app-2.3.0/tests/test_settings.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `core_module_excel_uploader_app-2.2.0/PKG-INFO` & `core_module_excel_uploader_app-2.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 1.0
 Name: core_module_excel_uploader_app
-Version: 2.2.0
+Version: 2.3.0
 Summary: Excel Uploader module for the parser core project
 Home-page: https://github.com/usnistgov/core_module_excel_uploader_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_module_excel_uploader_app
         ==============================
         
-        Excel Uploader module for the parser core project.
+        Excel Uploader module for the parser core project. A sample file is provided in the static folder.
         
         Quick start
         ===========
         
         1. Add "core_module_excel_uploader_app" to your INSTALLED_APPS setting
         ----------------------------------------------------------------------
```

### Comparing `core_module_excel_uploader_app-2.2.0/README.rst` & `core_module_excel_uploader_app-2.3.0/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 00000000: 636f 7265 5f6d 6f64 756c 655f 6578 6365  core_module_exce
 00000010: 6c5f 7570 6c6f 6164 6572 5f61 7070 0a3d  l_uploader_app.=
 00000020: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00000030: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 0a45  =============..E
 00000040: 7863 656c 2055 706c 6f61 6465 7220 6d6f  xcel Uploader mo
 00000050: 6475 6c65 2066 6f72 2074 6865 2070 6172  dule for the par
 00000060: 7365 7220 636f 7265 2070 726f 6a65 6374  ser core project
-00000070: 2e0a 0a51 7569 636b 2073 7461 7274 0a3d  ...Quick start.=
-00000080: 3d3d 3d3d 3d3d 3d3d 3d3d 0a0a 312e 2041  ==========..1. A
-00000090: 6464 2022 636f 7265 5f6d 6f64 756c 655f  dd "core_module_
-000000a0: 6578 6365 6c5f 7570 6c6f 6164 6572 5f61  excel_uploader_a
-000000b0: 7070 2220 746f 2079 6f75 7220 494e 5354  pp" to your INST
-000000c0: 414c 4c45 445f 4150 5053 2073 6574 7469  ALLED_APPS setti
-000000d0: 6e67 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ng.-------------
-000000e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000000f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000100: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000110: 2d2d 2d2d 2d2d 2d2d 2d0a 0a2e 2e20 636f  ---------.... co
-00000120: 6465 3a3a 2070 7974 686f 6e0a 0a20 2020  de:: python..   
-00000130: 2049 4e53 5441 4c4c 4544 5f41 5050 5320   INSTALLED_APPS 
-00000140: 3d20 5b0a 2020 2020 2020 2e2e 2e0a 2020  = [.      ....  
-00000150: 2020 2020 2763 6f72 655f 6d6f 6475 6c65      'core_module
-00000160: 5f65 7863 656c 5f75 706c 6f61 6465 725f  _excel_uploader_
-00000170: 6170 7027 2c0a 2020 2020 5d0a 0a32 2e20  app',.    ]..2. 
-00000180: 496e 636c 7564 6520 7468 6520 636f 7265  Include the core
-00000190: 5f6d 6f64 756c 655f 6578 6365 6c5f 7570  _module_excel_up
-000001a0: 6c6f 6164 6572 5f61 7070 2055 524c 636f  loader_app URLco
-000001b0: 6e66 2069 6e20 796f 7572 2070 726f 6a65  nf in your proje
-000001c0: 6374 2075 726c 732e 7079 0a2d 2d2d 2d2d  ct urls.py.-----
-000001d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000001e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000001f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000070: 2e20 4120 7361 6d70 6c65 2066 696c 6520  . A sample file 
+00000080: 6973 2070 726f 7669 6465 6420 696e 2074  is provided in t
+00000090: 6865 2073 7461 7469 6320 666f 6c64 6572  he static folder
+000000a0: 2e0a 0a51 7569 636b 2073 7461 7274 0a3d  ...Quick start.=
+000000b0: 3d3d 3d3d 3d3d 3d3d 3d3d 0a0a 312e 2041  ==========..1. A
+000000c0: 6464 2022 636f 7265 5f6d 6f64 756c 655f  dd "core_module_
+000000d0: 6578 6365 6c5f 7570 6c6f 6164 6572 5f61  excel_uploader_a
+000000e0: 7070 2220 746f 2079 6f75 7220 494e 5354  pp" to your INST
+000000f0: 414c 4c45 445f 4150 5053 2073 6574 7469  ALLED_APPS setti
+00000100: 6e67 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ng.-------------
+00000110: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000120: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000130: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000140: 2d2d 2d2d 2d2d 2d2d 2d0a 0a2e 2e20 636f  ---------.... co
+00000150: 6465 3a3a 2070 7974 686f 6e0a 0a20 2020  de:: python..   
+00000160: 2049 4e53 5441 4c4c 4544 5f41 5050 5320   INSTALLED_APPS 
+00000170: 3d20 5b0a 2020 2020 2020 2e2e 2e0a 2020  = [.      ....  
+00000180: 2020 2020 2763 6f72 655f 6d6f 6475 6c65      'core_module
+00000190: 5f65 7863 656c 5f75 706c 6f61 6465 725f  _excel_uploader_
+000001a0: 6170 7027 2c0a 2020 2020 5d0a 0a32 2e20  app',.    ]..2. 
+000001b0: 496e 636c 7564 6520 7468 6520 636f 7265  Include the core
+000001c0: 5f6d 6f64 756c 655f 6578 6365 6c5f 7570  _module_excel_up
+000001d0: 6c6f 6164 6572 5f61 7070 2055 524c 636f  loader_app URLco
+000001e0: 6e66 2069 6e20 796f 7572 2070 726f 6a65  nf in your proje
+000001f0: 6374 2075 726c 732e 7079 0a2d 2d2d 2d2d  ct urls.py.-----
 00000200: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000210: 2d2d 2d2d 2d2d 2d2d 0a0a 2e2e 2063 6f64  --------.... cod
-00000220: 653a 3a20 7079 7468 6f6e 0a0a 2020 2020  e:: python..    
-00000230: 7572 6c28 7227 5e27 2c20 696e 636c 7564  url(r'^', includ
-00000240: 6528 2763 6f72 655f 6d6f 6475 6c65 5f65  e('core_module_e
-00000250: 7863 656c 5f75 706c 6f61 6465 725f 6170  xcel_uploader_ap
-00000260: 702e 7572 6c73 2729 292c                 p.urls')),
+00000210: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000220: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000230: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000240: 2d2d 2d2d 2d2d 2d2d 0a0a 2e2e 2063 6f64  --------.... cod
+00000250: 653a 3a20 7079 7468 6f6e 0a0a 2020 2020  e:: python..    
+00000260: 7572 6c28 7227 5e27 2c20 696e 636c 7564  url(r'^', includ
+00000270: 6528 2763 6f72 655f 6d6f 6475 6c65 5f65  e('core_module_e
+00000280: 7863 656c 5f75 706c 6f61 6465 725f 6170  xcel_uploader_ap
+00000290: 702e 7572 6c73 2729 292c                 p.urls')),
```

### Comparing `core_module_excel_uploader_app-2.2.0/core_module_excel_uploader_app/views/views.py` & `core_module_excel_uploader_app-2.3.0/core_module_excel_uploader_app/views/views.py`

 * *Files identical despite different names*

### Comparing `core_module_excel_uploader_app-2.2.0/core_module_excel_uploader_app.egg-info/PKG-INFO` & `core_module_excel_uploader_app-2.3.0/core_module_excel_uploader_app.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 1.0
 Name: core-module-excel-uploader-app
-Version: 2.2.0
+Version: 2.3.0
 Summary: Excel Uploader module for the parser core project
 Home-page: https://github.com/usnistgov/core_module_excel_uploader_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_module_excel_uploader_app
         ==============================
         
-        Excel Uploader module for the parser core project.
+        Excel Uploader module for the parser core project. A sample file is provided in the static folder.
         
         Quick start
         ===========
         
         1. Add "core_module_excel_uploader_app" to your INSTALLED_APPS setting
         ----------------------------------------------------------------------
```

### Comparing `core_module_excel_uploader_app-2.2.0/core_module_excel_uploader_app.egg-info/SOURCES.txt` & `core_module_excel_uploader_app-2.3.0/core_module_excel_uploader_app.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.md
 MANIFEST.in
 README.rst
 pyproject.toml
 requirements.core.txt
 requirements.txt
 setup.py
 core_module_excel_uploader_app/__init__.py
@@ -9,14 +10,14 @@
 core_module_excel_uploader_app.egg-info/PKG-INFO
 core_module_excel_uploader_app.egg-info/SOURCES.txt
 core_module_excel_uploader_app.egg-info/dependency_links.txt
 core_module_excel_uploader_app.egg-info/requires.txt
 core_module_excel_uploader_app.egg-info/top_level.txt
 core_module_excel_uploader_app/static/core_module_excel_uploader_app/css/excel_uploader.css
 core_module_excel_uploader_app/static/core_module_excel_uploader_app/js/excel_uploader.js
-core_module_excel_uploader_app/static/core_module_excel_uploader_app/xslx/data.xlsx
+core_module_excel_uploader_app/static/core_module_excel_uploader_app/xls/data.xls
 core_module_excel_uploader_app/templates/core_module_excel_uploader_app/excel_uploader.html
 core_module_excel_uploader_app/views/__init__.py
 core_module_excel_uploader_app/views/forms.py
 core_module_excel_uploader_app/views/views.py
 tests/__init__.py
 tests/test_settings.py
```

### Comparing `core_module_excel_uploader_app-2.2.0/setup.py` & `core_module_excel_uploader_app-2.3.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_module_excel_uploader_app",
-    version="2.2.0",
+    version="2.3.0",
     description="Excel Uploader module for the parser core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_module_excel_uploader_app",
     packages=find_packages(),
     include_package_data=True,
```

