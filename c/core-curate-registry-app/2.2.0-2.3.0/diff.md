# Comparing `tmp/core_curate_registry_app-2.2.0.tar.gz` & `tmp/core_curate_registry_app-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/core_curate_registry_app-2.2.0.tar", last modified: Thu Feb 23 20:26:58 2023, max compression
+gzip compressed data, was "core_curate_registry_app-2.3.0.tar", last modified: Tue May  2 19:35:57 2023, max compression
```

## Comparing `core_curate_registry_app-2.2.0.tar` & `core_curate_registry_app-2.3.0.tar`

### file list

```diff
@@ -1,76 +1,77 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:58.000000 core_curate_registry_app-2.2.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      156 2023-02-23 20:26:55.000000 core_curate_registry_app-2.2.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1180 2023-02-23 20:26:58.000000 core_curate_registry_app-2.2.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      644 2023-02-23 20:26:55.000000 core_curate_registry_app-2.2.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:57.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:55.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:58.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:55.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:58.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/components/curate_data_structure/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:55.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/components/curate_data_structure/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      620 2023-02-23 20:26:55.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/components/curate_data_structure/api.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:58.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:55.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/rest/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      332 2023-02-23 20:26:55.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/rest/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      666 2023-02-23 20:26:55.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:57.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:57.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/static/core_curate_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:57.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/static/core_curate_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:58.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/static/core_curate_app/user/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       75 2023-02-23 20:26:55.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/static/core_curate_app/user/js/select_template.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2059 2023-02-23 20:26:55.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/static/core_curate_app/user/js/view_data_registry.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      181 2023-02-23 20:26:55.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/static/core_curate_app/user/js/view_data_registry.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:57.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/static/core_curate_registry_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:57.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/static/core_curate_registry_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:58.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/static/core_curate_registry_app/user/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       61 2023-02-23 20:26:55.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/static/core_curate_registry_app/user/css/index.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:58.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/static/core_curate_registry_app/user/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      348 2023-02-23 20:26:55.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/static/core_curate_registry_app/user/js/banner.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1076 2023-02-23 20:26:55.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/static/core_curate_registry_app/user/js/enter_data_registry.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       86 2023-02-23 20:26:55.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/static/core_curate_registry_app/user/js/enter_data_registry.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      945 2023-02-23 20:26:55.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/static/core_curate_registry_app/user/js/role.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      871 2023-02-23 20:26:55.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/static/core_curate_registry_app/user/js/start_curate.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1158 2023-02-23 20:26:55.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/static/core_curate_registry_app/user/js/title.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       45 2023-02-23 20:26:55.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/static/core_curate_registry_app/user/js/title.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:57.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:57.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/templates/core_curate_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:58.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/templates/core_curate_app/user/
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     1286 2023-02-23 20:26:56.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/templates/core_curate_app/user/curate.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      547 2023-02-23 20:26:56.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/templates/core_curate_app/user/curate_start.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:58.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/templates/core_curate_app/user/data-entry/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1704 2023-02-23 20:26:56.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/templates/core_curate_app/user/data-entry/enter_data.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:58.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/templates/core_curate_app/user/data-entry/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      740 2023-02-23 20:26:56.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/templates/core_curate_app/user/data-entry/modals/xml-valid-registry.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:58.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/templates/core_curate_app/user/data-review/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:58.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/templates/core_curate_app/user/data-review/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1218 2023-02-23 20:26:56.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/templates/core_curate_app/user/data-review/modals/save-form-registry.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1047 2023-02-23 20:26:56.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/templates/core_curate_app/user/data-review/view_data.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:57.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/templates/core_curate_registry_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:58.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/templates/core_curate_registry_app/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      509 2023-02-23 20:26:56.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/templates/core_curate_registry_app/user/index.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3797 2023-02-23 20:26:56.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:58.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:56.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/utils/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      472 2023-02-23 20:26:56.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/utils/jquery.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:58.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:56.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:58.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:56.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1463 2023-02-23 20:26:56.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/views/user/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8133 2023-02-23 20:26:56.000000 core_curate_registry_app-2.2.0/core_curate_registry_app/views/user/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:58.000000 core_curate_registry_app-2.2.0/core_curate_registry_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1180 2023-02-23 20:26:57.000000 core_curate_registry_app-2.2.0/core_curate_registry_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2489 2023-02-23 20:26:57.000000 core_curate_registry_app-2.2.0/core_curate_registry_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-02-23 20:26:57.000000 core_curate_registry_app-2.2.0/core_curate_registry_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       60 2023-02-23 20:26:57.000000 core_curate_registry_app-2.2.0/core_curate_registry_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       31 2023-02-23 20:26:57.000000 core_curate_registry_app-2.2.0/core_curate_registry_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-02-23 20:26:56.000000 core_curate_registry_app-2.2.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       53 2023-02-23 20:26:56.000000 core_curate_registry_app-2.2.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-02-23 20:26:58.000000 core_curate_registry_app-2.2.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1480 2023-02-23 20:26:56.000000 core_curate_registry_app-2.2.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:58.000000 core_curate_registry_app-2.2.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:56.000000 core_curate_registry_app-2.2.0/tests/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1105 2023-02-23 20:26:56.000000 core_curate_registry_app-2.2.0/tests/test_settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:58.000000 core_curate_registry_app-2.2.0/tests/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:56.000000 core_curate_registry_app-2.2.0/tests/utils/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1749 2023-02-23 20:26:56.000000 core_curate_registry_app-2.2.0/tests/utils/test_units.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:57.863752 core_curate_registry_app-2.3.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:35:54.000000 core_curate_registry_app-2.3.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      156 2023-05-02 19:35:54.000000 core_curate_registry_app-2.3.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1180 2023-05-02 19:35:57.858855 core_curate_registry_app-2.3.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      644 2023-05-02 19:35:54.000000 core_curate_registry_app-2.3.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:57.227145 core_curate_registry_app-2.3.0/core_curate_registry_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:54.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:57.347119 core_curate_registry_app-2.3.0/core_curate_registry_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:54.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:57.383341 core_curate_registry_app-2.3.0/core_curate_registry_app/components/curate_data_structure/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:54.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/components/curate_data_structure/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      620 2023-05-02 19:35:54.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/components/curate_data_structure/api.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:57.409603 core_curate_registry_app-2.3.0/core_curate_registry_app/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:54.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/rest/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      332 2023-05-02 19:35:54.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/rest/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      666 2023-05-02 19:35:54.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:56.951219 core_curate_registry_app-2.3.0/core_curate_registry_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:56.941708 core_curate_registry_app-2.3.0/core_curate_registry_app/static/core_curate_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:56.944615 core_curate_registry_app-2.3.0/core_curate_registry_app/static/core_curate_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:57.460381 core_curate_registry_app-2.3.0/core_curate_registry_app/static/core_curate_app/user/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       75 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/static/core_curate_app/user/js/select_template.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2059 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/static/core_curate_app/user/js/view_data_registry.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      181 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/static/core_curate_app/user/js/view_data_registry.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:56.954510 core_curate_registry_app-2.3.0/core_curate_registry_app/static/core_curate_registry_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:56.971533 core_curate_registry_app-2.3.0/core_curate_registry_app/static/core_curate_registry_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:57.478550 core_curate_registry_app-2.3.0/core_curate_registry_app/static/core_curate_registry_app/user/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       61 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/static/core_curate_registry_app/user/css/index.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:57.563991 core_curate_registry_app-2.3.0/core_curate_registry_app/static/core_curate_registry_app/user/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      348 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/static/core_curate_registry_app/user/js/banner.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1076 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/static/core_curate_registry_app/user/js/enter_data_registry.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       86 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/static/core_curate_registry_app/user/js/enter_data_registry.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      945 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/static/core_curate_registry_app/user/js/role.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      871 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/static/core_curate_registry_app/user/js/start_curate.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1158 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/static/core_curate_registry_app/user/js/title.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       45 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/static/core_curate_registry_app/user/js/title.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:57.024314 core_curate_registry_app-2.3.0/core_curate_registry_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:56.984846 core_curate_registry_app-2.3.0/core_curate_registry_app/templates/core_curate_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:57.599974 core_curate_registry_app-2.3.0/core_curate_registry_app/templates/core_curate_app/user/
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     1286 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/templates/core_curate_app/user/curate.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      547 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/templates/core_curate_app/user/curate_start.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:57.613671 core_curate_registry_app-2.3.0/core_curate_registry_app/templates/core_curate_app/user/data-entry/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1704 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/templates/core_curate_app/user/data-entry/enter_data.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:57.629148 core_curate_registry_app-2.3.0/core_curate_registry_app/templates/core_curate_app/user/data-entry/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      740 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/templates/core_curate_app/user/data-entry/modals/xml-valid-registry.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:57.641960 core_curate_registry_app-2.3.0/core_curate_registry_app/templates/core_curate_app/user/data-review/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:57.656349 core_curate_registry_app-2.3.0/core_curate_registry_app/templates/core_curate_app/user/data-review/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1218 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/templates/core_curate_app/user/data-review/modals/save-form-registry.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1047 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/templates/core_curate_app/user/data-review/view_data.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:57.034659 core_curate_registry_app-2.3.0/core_curate_registry_app/templates/core_curate_registry_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:57.668982 core_curate_registry_app-2.3.0/core_curate_registry_app/templates/core_curate_registry_app/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      509 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/templates/core_curate_registry_app/user/index.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3665 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:57.700707 core_curate_registry_app-2.3.0/core_curate_registry_app/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/utils/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      472 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/utils/jquery.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:57.715953 core_curate_registry_app-2.3.0/core_curate_registry_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:57.768465 core_curate_registry_app-2.3.0/core_curate_registry_app/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1463 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/views/user/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7985 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/views/user/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:57.332546 core_curate_registry_app-2.3.0/core_curate_registry_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1180 2023-05-02 19:35:56.000000 core_curate_registry_app-2.3.0/core_curate_registry_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2500 2023-05-02 19:35:56.000000 core_curate_registry_app-2.3.0/core_curate_registry_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:35:56.000000 core_curate_registry_app-2.3.0/core_curate_registry_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       60 2023-05-02 19:35:56.000000 core_curate_registry_app-2.3.0/core_curate_registry_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       31 2023-05-02 19:35:56.000000 core_curate_registry_app-2.3.0/core_curate_registry_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       53 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:35:57.865853 core_curate_registry_app-2.3.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1480 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:57.804615 core_curate_registry_app-2.3.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/tests/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1105 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:57.846053 core_curate_registry_app-2.3.0/tests/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/tests/utils/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1749 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/tests/utils/test_units.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `core_curate_registry_app-2.2.0/PKG-INFO` & `core_curate_registry_app-2.3.0/core_curate_registry_app.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
-Name: core_curate_registry_app
-Version: 2.2.0
+Name: core-curate-registry-app
+Version: 2.3.0
 Summary: Curation functionalities specific to Registry applications for the curator core project
 Home-page: https://github.com/usnistgov/core_curate_registry_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: Core Curate Registry App
         ========================
```

### Comparing `core_curate_registry_app-2.2.0/README.rst` & `core_curate_registry_app-2.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_curate_registry_app-2.2.0/core_curate_registry_app/components/curate_data_structure/api.py` & `core_curate_registry_app-2.3.0/core_curate_registry_app/components/curate_data_structure/api.py`

 * *Files identical despite different names*

### Comparing `core_curate_registry_app-2.2.0/core_curate_registry_app/settings.py` & `core_curate_registry_app-2.3.0/core_curate_registry_app/settings.py`

 * *Files identical despite different names*

### Comparing `core_curate_registry_app-2.2.0/core_curate_registry_app/static/core_curate_app/user/js/view_data_registry.js` & `core_curate_registry_app-2.3.0/core_curate_registry_app/static/core_curate_app/user/js/view_data_registry.js`

 * *Files identical despite different names*

### Comparing `core_curate_registry_app-2.2.0/core_curate_registry_app/static/core_curate_registry_app/user/js/enter_data_registry.js` & `core_curate_registry_app-2.3.0/core_curate_registry_app/static/core_curate_registry_app/user/js/enter_data_registry.js`

 * *Files identical despite different names*

### Comparing `core_curate_registry_app-2.2.0/core_curate_registry_app/static/core_curate_registry_app/user/js/role.js` & `core_curate_registry_app-2.3.0/core_curate_registry_app/static/core_curate_registry_app/user/js/role.js`

 * *Files identical despite different names*

### Comparing `core_curate_registry_app-2.2.0/core_curate_registry_app/static/core_curate_registry_app/user/js/start_curate.js` & `core_curate_registry_app-2.3.0/core_curate_registry_app/static/core_curate_registry_app/user/js/start_curate.js`

 * *Files identical despite different names*

### Comparing `core_curate_registry_app-2.2.0/core_curate_registry_app/static/core_curate_registry_app/user/js/title.js` & `core_curate_registry_app-2.3.0/core_curate_registry_app/static/core_curate_registry_app/user/js/title.js`

 * *Files identical despite different names*

### Comparing `core_curate_registry_app-2.2.0/core_curate_registry_app/templates/core_curate_app/user/curate.html` & `core_curate_registry_app-2.3.0/core_curate_registry_app/templates/core_curate_app/user/curate.html`

 * *Files identical despite different names*

### Comparing `core_curate_registry_app-2.2.0/core_curate_registry_app/templates/core_curate_app/user/curate_start.html` & `core_curate_registry_app-2.3.0/core_curate_registry_app/templates/core_curate_app/user/curate_start.html`

 * *Files identical despite different names*

### Comparing `core_curate_registry_app-2.2.0/core_curate_registry_app/templates/core_curate_app/user/data-entry/enter_data.html` & `core_curate_registry_app-2.3.0/core_curate_registry_app/templates/core_curate_app/user/data-entry/enter_data.html`

 * *Files identical despite different names*

### Comparing `core_curate_registry_app-2.2.0/core_curate_registry_app/templates/core_curate_app/user/data-entry/modals/xml-valid-registry.html` & `core_curate_registry_app-2.3.0/core_curate_registry_app/templates/core_curate_app/user/data-entry/modals/xml-valid-registry.html`

 * *Files identical despite different names*

### Comparing `core_curate_registry_app-2.2.0/core_curate_registry_app/templates/core_curate_app/user/data-review/modals/save-form-registry.html` & `core_curate_registry_app-2.3.0/core_curate_registry_app/templates/core_curate_app/user/data-review/modals/save-form-registry.html`

 * *Files identical despite different names*

### Comparing `core_curate_registry_app-2.2.0/core_curate_registry_app/templates/core_curate_app/user/data-review/view_data.html` & `core_curate_registry_app-2.3.0/core_curate_registry_app/templates/core_curate_app/user/data-review/view_data.html`

 * *Files identical despite different names*

### Comparing `core_curate_registry_app-2.2.0/core_curate_registry_app/urls.py` & `core_curate_registry_app-2.3.0/core_curate_registry_app/urls.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """ Url router for the curate application
 """
 from django.conf.urls import include
-from django.urls import re_path, reverse_lazy
+from django.urls import re_path
 
-from core_curate_app.permissions import rights
 import core_curate_app.views.user.ajax as user_ajax
 import core_curate_app.views.user.views as user_views
+import core_curate_registry_app.views.user.ajax as user_registry_ajax
+import core_curate_registry_app.views.user.views as user_registry_views
+from core_curate_app.permissions import rights
 from core_curate_app.views.common import views as common_views
 from core_main_app.utils.decorators import permission_required
-import core_curate_registry_app.views.user.views as user_registry_views
-import core_curate_registry_app.views.user.ajax as user_registry_ajax
 
 urlpatterns = [
     re_path(r"^$", user_registry_views.index, name="core_curate_index"),
     re_path(
         r"^start_curate$",
         user_registry_ajax.StartCurate.as_view(),
         name="core_curate_start",
@@ -86,22 +86,20 @@
         name="core_curate_validate_form",
     ),
     re_path(
         r"^view-form/(?P<curate_data_structure_id>\w+)$",
         permission_required(
             content_type=rights.CURATE_CONTENT_TYPE,
             permission=rights.CURATE_ACCESS,
-            login_url=reverse_lazy("core_main_app_login"),
         )(common_views.FormView.as_view()),
         name="core_curate_view_form",
     ),
     re_path(
         r"^xml-editor/form",
         permission_required(
             content_type=rights.CURATE_CONTENT_TYPE,
             permission=rights.CURATE_DATA_STRUCTURE_ACCESS,
-            login_url=reverse_lazy("core_main_app_login"),
         )(common_views.DraftContentEditor.as_view()),
         name="core_curate_app_xml_text_editor_view",
     ),
     re_path(r"^rest/", include("core_curate_registry_app.rest.urls")),
 ]
```

### Comparing `core_curate_registry_app-2.2.0/core_curate_registry_app/views/user/ajax.py` & `core_curate_registry_app-2.3.0/core_curate_registry_app/views/user/ajax.py`

 * *Files identical despite different names*

### Comparing `core_curate_registry_app-2.2.0/core_curate_registry_app/views/user/views.py` & `core_curate_registry_app-2.3.0/core_curate_registry_app/views/user/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,37 @@
 """Curate registry app user views
 """
-from django.urls import reverse_lazy
 from django.utils.decorators import method_decorator
 from django.views import View
 
-from core_main_app.utils import decorators
-from core_main_app.utils.rendering import render
+from core_curate_app.permissions import rights
+from core_curate_app.views.user.views import EnterDataView, ViewDataView
+from core_curate_registry_app.settings import (
+    REGISTRY_XSD_FILENAME,
+    XPATH_TITLE,
+)
+from core_curate_registry_app.utils import jquery as jquery_utils
 from core_main_app.commons import exceptions
 from core_main_app.components.template_version_manager import (
     api as template_version_manager_api,
 )
-from core_curate_app.permissions import rights
-from core_curate_app.views.user.views import EnterDataView, ViewDataView
-from core_parser_app.components.data_structure_element import (
-    api as data_structure_element_api,
-)
-
+from core_main_app.utils import decorators
+from core_main_app.utils.rendering import render
 from core_main_registry_app.components.custom_resource import (
     api as custom_resource_api,
 )
 from core_main_registry_app.constants import CUSTOM_RESOURCE_TYPE
-from core_curate_registry_app.settings import (
-    REGISTRY_XSD_FILENAME,
-    XPATH_TITLE,
+from core_parser_app.components.data_structure_element import (
+    api as data_structure_element_api,
 )
-from core_curate_registry_app.utils import jquery as jquery_utils
 
 
 @decorators.permission_required(
     content_type=rights.CURATE_CONTENT_TYPE,
     permission=rights.CURATE_ACCESS,
-    login_url=reverse_lazy("core_main_app_login"),
 )
 def index(request):
     """Curate homepage for the registry.
 
     Args:
         request:
 
@@ -93,15 +90,14 @@
         }
         self.modals = []
 
     @method_decorator(
         decorators.permission_required(
             content_type=rights.CURATE_CONTENT_TYPE,
             permission=rights.CURATE_ACCESS,
-            login_url=reverse_lazy("core_main_app_login"),
         )
     )
     def get(self, request, role):
         """Start curate with role parameter.
         Args:
             request:
             role:
```

### Comparing `core_curate_registry_app-2.2.0/core_curate_registry_app.egg-info/PKG-INFO` & `core_curate_registry_app-2.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
-Name: core-curate-registry-app
-Version: 2.2.0
+Name: core_curate_registry_app
+Version: 2.3.0
 Summary: Curation functionalities specific to Registry applications for the curator core project
 Home-page: https://github.com/usnistgov/core_curate_registry_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: Core Curate Registry App
         ========================
```

### Comparing `core_curate_registry_app-2.2.0/core_curate_registry_app.egg-info/SOURCES.txt` & `core_curate_registry_app-2.3.0/core_curate_registry_app.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.md
 MANIFEST.in
 README.rst
 pyproject.toml
 requirements.core.txt
 setup.py
 core_curate_registry_app/__init__.py
 core_curate_registry_app/settings.py
```

### Comparing `core_curate_registry_app-2.2.0/setup.py` & `core_curate_registry_app-2.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 chdir(normpath(join(abspath(__file__), pardir)))
 
 dep_links = [r for r in required if r.startswith("https://")]
 required = [req_link(r) if r.startswith("https://") else r for r in required]
 
 setup(
     name="core_curate_registry_app",
-    version="2.2.0",
+    version="2.3.0",
     description="Curation functionalities specific to Registry applications for the curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_curate_registry_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_curate_registry_app-2.2.0/tests/test_settings.py` & `core_curate_registry_app-2.3.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `core_curate_registry_app-2.2.0/tests/utils/test_units.py` & `core_curate_registry_app-2.3.0/tests/utils/test_units.py`

 * *Files identical despite different names*

