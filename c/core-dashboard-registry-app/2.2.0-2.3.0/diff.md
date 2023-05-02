# Comparing `tmp/core_dashboard_registry_app-2.2.0.tar.gz` & `tmp/core_dashboard_registry_app-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/core_dashboard_registry_app-2.2.0.tar", last modified: Thu Feb 23 20:27:31 2023, max compression
+gzip compressed data, was "core_dashboard_registry_app-2.3.0.tar", last modified: Tue May  2 19:36:38 2023, max compression
```

## Comparing `core_dashboard_registry_app-2.2.0.tar` & `core_dashboard_registry_app-2.3.0.tar`

### file list

```diff
@@ -1,81 +1,82 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:31.000000 core_dashboard_registry_app-2.2.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      162 2023-02-23 20:27:28.000000 core_dashboard_registry_app-2.2.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1145 2023-02-23 20:27:31.000000 core_dashboard_registry_app-2.2.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      633 2023-02-23 20:27:28.000000 core_dashboard_registry_app-2.2.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:30.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:28.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3446 2023-02-23 20:27:28.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/admin.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      661 2023-02-23 20:27:28.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/constants.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2803 2023-02-23 20:27:28.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/menus.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      415 2023-02-23 20:27:28.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:30.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:30.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/static/core_dashboard_registry_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:30.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:30.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       98 2023-02-23 20:27:28.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/css/home.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:30.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/css/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1672 2023-02-23 20:27:28.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/css/list/records.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:30.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1056 2023-02-23 20:27:28.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/get_url.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      107 2023-02-23 20:27:28.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/get_url.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:30.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       69 2023-02-23 20:27:28.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/list/open_form.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      649 2023-02-23 20:27:28.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/list/publish.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       72 2023-02-23 20:27:28.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/list/publish.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1665 2023-02-23 20:27:28.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/list/records.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       78 2023-02-23 20:27:28.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/list/records.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1657 2023-02-23 20:27:28.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/record_registry.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      226 2023-02-23 20:27:28.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/record_registry.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:30.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:30.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/templates/core_dashboard_common_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:30.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/templates/core_dashboard_common_app/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2778 2023-02-23 20:27:28.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/templates/core_dashboard_common_app/list/my_dashboard_my_forms_table.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4888 2023-02-23 20:27:28.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/templates/core_dashboard_common_app/list/my_dashboard_my_records_table.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      194 2023-02-23 20:27:28.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/templates/core_dashboard_common_app/list/my_dashboard_my_records_table_pagination.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2796 2023-02-23 20:27:28.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/templates/core_dashboard_common_app/my_dashboard.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:30.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1180 2023-02-23 20:27:28.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/home.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:30.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1731 2023-02-23 20:27:28.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/list/my_dashboard_my_forms_table.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      192 2023-02-23 20:27:28.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/list/my_dashboard_my_forms_table_pagination.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5418 2023-02-23 20:27:28.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/list/my_dashboard_my_records_table.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      194 2023-02-23 20:27:28.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/list/my_dashboard_my_records_table_pagination.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4235 2023-02-23 20:27:28.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:30.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:28.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/utils/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:30.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/utils/query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:28.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/utils/query/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:30.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/utils/query/django/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:28.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/utils/query/django/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      622 2023-02-23 20:27:28.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/utils/query/django/prepare.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:30.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/utils/query/mongo/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:28.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/utils/query/mongo/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      786 2023-02-23 20:27:28.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/utils/query/mongo/prepare.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:30.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:28.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:31.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/views/common/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:28.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/views/common/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3843 2023-02-23 20:27:28.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/views/common/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      515 2023-02-23 20:27:28.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/views/common/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17472 2023-02-23 20:27:28.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/views/common/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:30.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1145 2023-02-23 20:27:29.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3199 2023-02-23 20:27:29.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-02-23 20:27:29.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      120 2023-02-23 20:27:29.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       34 2023-02-23 20:27:29.000000 core_dashboard_registry_app-2.2.0/core_dashboard_registry_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-02-23 20:27:28.000000 core_dashboard_registry_app-2.2.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       94 2023-02-23 20:27:28.000000 core_dashboard_registry_app-2.2.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-02-23 20:27:31.000000 core_dashboard_registry_app-2.2.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1104 2023-02-23 20:27:28.000000 core_dashboard_registry_app-2.2.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:31.000000 core_dashboard_registry_app-2.2.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:28.000000 core_dashboard_registry_app-2.2.0/tests/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1809 2023-02-23 20:27:28.000000 core_dashboard_registry_app-2.2.0/tests/test_settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:31.000000 core_dashboard_registry_app-2.2.0/tests/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:28.000000 core_dashboard_registry_app-2.2.0/tests/utils/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:31.000000 core_dashboard_registry_app-2.2.0/tests/utils/query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:28.000000 core_dashboard_registry_app-2.2.0/tests/utils/query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3483 2023-02-23 20:27:28.000000 core_dashboard_registry_app-2.2.0/tests/utils/query/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:31.000000 core_dashboard_registry_app-2.2.0/tests/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:28.000000 core_dashboard_registry_app-2.2.0/tests/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14065 2023-02-23 20:27:28.000000 core_dashboard_registry_app-2.2.0/tests/views/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:38.191435 core_dashboard_registry_app-2.3.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      162 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1145 2023-05-02 19:36:38.185245 core_dashboard_registry_app-2.3.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      633 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:37.503217 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3446 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/admin.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      661 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/constants.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2803 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/menus.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      415 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:37.231973 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:37.235153 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/static/core_dashboard_registry_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:37.248037 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:37.593119 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       98 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/css/home.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:37.605937 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/css/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1672 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/css/list/records.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:37.654413 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1056 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/get_url.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      107 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/get_url.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:37.724475 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       69 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/list/open_form.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      649 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/list/publish.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       72 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/list/publish.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1665 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/list/records.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       78 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/list/records.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1657 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/record_registry.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      226 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/record_registry.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:37.270550 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:37.736823 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/templates/core_dashboard_common_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:37.780681 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/templates/core_dashboard_common_app/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2778 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/templates/core_dashboard_common_app/list/my_dashboard_my_forms_table.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4888 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/templates/core_dashboard_common_app/list/my_dashboard_my_records_table.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      194 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/templates/core_dashboard_common_app/list/my_dashboard_my_records_table_pagination.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2960 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/templates/core_dashboard_common_app/my_dashboard.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:37.805457 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1180 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/home.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:37.861402 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1731 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/list/my_dashboard_my_forms_table.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      192 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/list/my_dashboard_my_forms_table_pagination.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5496 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/list/my_dashboard_my_records_table.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      194 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/list/my_dashboard_my_records_table_pagination.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3839 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:37.873824 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/utils/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:37.889082 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/utils/query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/utils/query/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:37.922689 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/utils/query/django/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/utils/query/django/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      622 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/utils/query/django/prepare.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:37.954970 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/utils/query/mongo/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/utils/query/mongo/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      786 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/utils/query/mongo/prepare.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:37.967110 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:38.037276 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/views/common/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/views/common/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3843 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/views/common/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      515 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/views/common/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17579 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/views/common/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:37.577747 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1145 2023-05-02 19:36:36.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3210 2023-05-02 19:36:37.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:36:36.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      120 2023-05-02 19:36:36.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       34 2023-05-02 19:36:36.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       94 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:36:38.193694 core_dashboard_registry_app-2.3.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1104 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:38.070918 core_dashboard_registry_app-2.3.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/tests/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1809 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:38.097606 core_dashboard_registry_app-2.3.0/tests/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/tests/utils/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:38.134305 core_dashboard_registry_app-2.3.0/tests/utils/query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/tests/utils/query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3483 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/tests/utils/query/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:38.165993 core_dashboard_registry_app-2.3.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/tests/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14651 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/tests/views/tests_unit.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `core_dashboard_registry_app-2.2.0/PKG-INFO` & `core_dashboard_registry_app-2.3.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_dashboard_registry_app
-Version: 2.2.0
+Version: 2.3.0
 Summary: Resource management via a dashboard for the registry core project
 Home-page: https://github.com/usnistgov/core_dashboard_registry_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: Core Dashboard Registry App
         ===========================
```

### Comparing `core_dashboard_registry_app-2.2.0/README.rst` & `core_dashboard_registry_app-2.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/admin.py` & `core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/admin.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/constants.py` & `core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/constants.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/menus.py` & `core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/menus.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/css/list/records.css` & `core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/css/list/records.css`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/get_url.js` & `core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/get_url.js`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/list/publish.js` & `core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/list/publish.js`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/list/records.js` & `core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/list/records.js`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/record_registry.js` & `core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/record_registry.js`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/templates/core_dashboard_common_app/list/my_dashboard_my_forms_table.html` & `core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/templates/core_dashboard_common_app/list/my_dashboard_my_forms_table.html`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/templates/core_dashboard_common_app/list/my_dashboard_my_records_table.html` & `core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/templates/core_dashboard_common_app/list/my_dashboard_my_records_table.html`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/templates/core_dashboard_common_app/my_dashboard.html` & `core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/templates/core_dashboard_common_app/my_dashboard.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 {% extends 'core_main_app/_render/admin/theme/tools/box.html' %}
 {% load special_plural %}
 
 {% block box_title %}
-
     {% if data.title %}
         {{data.title}}
-    {% else %}
-        {% if come_from_admin %} {{ data.document|title|special_plural}} list {% else %} My {{data.document|special_plural}} {% endif %}
+    {% elif come_from_admin %}
+        {{ data.document|title|special_plural}} list {% else %} My {{data.document|special_plural}}
     {% endif %}
-
 {% endblock %}
 
-
 {% block box_tools %}
     {% if data.create_workspace %}
-    <a class="m-3 btn btn-secondary create-workspace-btn">
-        <i class="fas fa-file-alt"></i> Create workspace
-    </a>
+        <a class="m-3 btn btn-secondary create-workspace-btn">
+            <i class="fas fa-file-alt"></i> Create workspace
+        </a>
     {% endif %}
 
     {% if data.title %}
         <a href="#" class="m-3 btn btn-secondary back-to-previous">
              <i class="fas fa-arrow-left"></i> Previous page
         </a>
     {% endif %}
 {% endblock %}
 
-
 {% block box_body %}
+    {% if data.administration and data.owner %}
+        <p>Owner: <a href="{{ data.owner_change_url }}">{{ data.owner }}</a></p>
+    {% endif %}
 
-{% if data.user_data %}
-    Total number of {{data.document|special_plural}}: {{ data.number_total }}
-{% endif %}
+    {% if data.user_data %}
+        Total number of {{data.document|special_plural}}: {{ data.number_total }}
+    {% endif %}
 
     {% if data.menu and not data.title %}
         <div class="dropdown" id="id_actions" style="display:none">
-            <button class="btn btn-secondary dropdown-toggle" type="button" id="dropdownMenu1" data-toggle="dropdown" aria-haspopup="true" aria-expanded="true">
+            <button class="btn btn-secondary dropdown-toggle" type="button" id="dropdownMenu1" data-toggle="dropdown"
+                    aria-haspopup="true" aria-expanded="true">
                 Choose action
                 <span class="caret"></span>
             </button>
             <ul class="dropdown-menu">
                 {% for value, text in data.action_form.fields.actions.choices %}
                     <li style="cursor:  pointer;" onclick="action_dashboard({{value}});">{{text}}</li>
                 {% endfor %}
```

#### html2text {}

```diff
@@ -1,18 +1,21 @@
 {% extends 'core_main_app/_render/admin/theme/tools/box.html' %} {% load
 special_plural %} {% block box_title %} {% if data.title %} {{data.title}} {%
-else %} {% if come_from_admin %} {{ data.document|title|special_plural}} list
-{% else %} My {{data.document|special_plural}} {% endif %} {% endif %} {%
-endblock %} {% block box_tools %} {% if data.create_workspace %}
+elif come_from_admin %} {{ data.document|title|special_plural}} list {% else %}
+My {{data.document|special_plural}} {% endif %} {% endblock %} {% block
+box_tools %} {% if data.create_workspace %}
  Create workspace
  {% endif %} {% if data.title %}
  Previous_page
- {% endif %} {% endblock %} {% block box_body %} {% if data.user_data %} Total
-number of {{data.document|special_plural}}: {{ data.number_total }} {% endif %}
-{% if data.menu and not data.title %}
+ {% endif %} {% endblock %} {% block box_body %} {% if data.administration and
+data.owner %}
+Owner: {{_data.owner_}}
+{% endif %} {% if data.user_data %} Total number of {
+{data.document|special_plural}}: {{ data.number_total }} {% endif %} {% if
+data.menu and not data.title %}
  Choose action
     * {% for value, text in data.action_form.fields.actions.choices %}
     * {{text}}
     * {% endfor %}
 {% endif %} {% if data.resources %} {% include 'core_main_registry_app/
 resource_banner/resource_banner.html' %}
     * All
```

### Comparing `core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/home.html` & `core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/home.html`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/list/my_dashboard_my_forms_table.html` & `core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/list/my_dashboard_my_forms_table.html`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/list/my_dashboard_my_records_table.html` & `core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/list/my_dashboard_my_records_table.html`

 * *Files 4% similar despite different names*

```diff
@@ -99,14 +99,15 @@
 
         </td>
         <td style="padding: 10px;">
             {% if data_loaded.can_set_public %}
                 <a class="btn btn-secondary publish-record-btn float-right">
                     <i class="fas fa-share-alt"></i> Publish
                 </a>
-            {% else %}
-                <span class="float-right" style="font-size: 0.6em;"> Published on: {{ data_loaded.data.last_modification_date|print_datetime_utc_unaware }} </span>
             {% endif %}
+            <span class="float-right" style="font-size: 0.6em; margin: 0.7em;">
+                {% if data_loaded.can_set_public %}Updated{% else%}Published{% endif %} on: {{ data_loaded.data.last_modification_date|print_datetime_utc_unaware }}
+            </span>
         </td>
     </tr>
 </table>
 {% endfor %}
```

#### html2text {}

```diff
@@ -19,21 +19,21 @@
 { data_loaded.username_list|get:key }} {% endwith %}
 {% if data_loaded.can_change_workspace %}
  Change workspace
  {% endif %} {% if data_loaded.is_owner %}
  Change owner
  {% endif %} {% if data_loaded.can_write %}
  {% if data_loaded.data|has_draft:request.user %}
-Edit draft {% else %} Create new version {% endif %}
-                                                     {% if data_loaded.can_set_public %}
- Open                                                 Publish
- {% endif %} {% if data_loaded.can_write %} {% if     {% else %}  Published on: {
+Edit draft {% else %} Create new version {% endif %} {% if data_loaded.can_set_public %}
+                                                      Publish
+ Open                                                 {% endif %}  {% if data_loaded.can_set_public %}Updated{%
+ {% endif %} {% if data_loaded.can_write %} {% if    else%}Published{% endif %} on: {
 data.administration %} {% url 'core-admin:           {
 core_dashboard_app_edit_data' data_loaded.data.id as data_loaded.data.last_modification_date|print_datetime_utc_unaware
-edit_url %} {% else %} {% url                        }}  {% endif %}
+edit_url %} {% else %} {% url                        }}
 'core_dashboard_app_edit_data' data_loaded.data.id
 as edit_url %} {% endif %} {% include
 'core_main_app/common/buttons/edit.html' with
 label="Edit Title" %} {% if data.administration %}
 {% with data_loaded.delete_url as delete_url %} {%
 include 'core_main_app/common/buttons/delete.html'
 %} {% endwith %} {% endif %} {% endif %}
```

### Comparing `core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/urls.py` & `core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/urls.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 """
     Url router for the user dashboard
 """
 from django.contrib.auth.decorators import login_required
 from django.urls import re_path
-from django.urls import reverse_lazy
 
 from core_dashboard_common_app import constants as dashboard_constants
 from core_dashboard_common_app.views.common import ajax, views as common_views
 from core_dashboard_common_app.views.common.views import (
     UserDashboardPasswordChangeFormView,
 )
-from core_main_registry_app.settings import ENABLE_BLOB_ENDPOINTS
 from core_dashboard_registry_app.views.common import (
     ajax as registry_common_ajax,
 )
 from core_dashboard_registry_app.views.common import (
     views as registry_common_views,
 )
 from core_dashboard_registry_app.views.common.ajax import EditDataView
-
+from core_main_registry_app.settings import ENABLE_BLOB_ENDPOINTS
 
 urlpatterns = [
     # Common
     re_path(r"^$", registry_common_views.home, name="core_dashboard_home"),
     re_path(
         r"^my-profile$", common_views.my_profile, name="core_dashboard_profile"
     ),
@@ -57,56 +55,51 @@
         r"^records$",
         login_required(
             registry_common_views.DashboardRegistryRecords.as_view(
                 document=dashboard_constants.FUNCTIONAL_OBJECT_ENUM.RECORD.value,
                 data_template="core_dashboard_registry_app/list/my_dashboard_my_records_table_pagination.html",
                 allow_change_workspace_if_public=False,
             ),
-            login_url=reverse_lazy("core_main_app_login"),
         ),
         name="core_dashboard_records",
     ),
     re_path(
         r"^switch-status-record",
         registry_common_ajax.switch_data_status,
         name="core_dashboard_switch_status_record",
     ),
     re_path(
         r"^forms$",
         login_required(
             registry_common_views.DashboardRegistryForms.as_view(
                 document=dashboard_constants.FUNCTIONAL_OBJECT_ENUM.FORM.value
             ),
-            login_url=reverse_lazy("core_main_app_login"),
         ),
         name="core_dashboard_forms",
     ),
     re_path(
         r"^workspaces$",
         login_required(
             common_views.DashboardWorkspaces.as_view(),
-            login_url=reverse_lazy("core_main_app_login"),
         ),
         name="core_dashboard_workspaces",
     ),
     re_path(
         r"^queries",
         login_required(
             common_views.DashboardQueries.as_view(),
-            login_url=reverse_lazy("core_main_app_login"),
         ),
         name="core_dashboard_queries",
     ),
     re_path(
         r"^workspace-list-records/(?P<workspace_id>\w+)$",
         login_required(
             registry_common_views.DashboardRegistryWorkspaceRecords.as_view(
                 data_template="core_dashboard_registry_app/list/my_dashboard_my_records_table_pagination.html"
             ),
-            login_url=reverse_lazy("core_main_app_login"),
         ),
         name="core_dashboard_workspace_list",
     ),
     re_path(
         r"^publish-resource",
         registry_common_ajax.publish,
         name="core_dashboard_publish_resource_registry",
@@ -120,12 +113,11 @@
 
 if ENABLE_BLOB_ENDPOINTS:
     urlpatterns.append(
         re_path(
             r"^files$",
             login_required(
                 common_views.DashboardFiles.as_view(),
-                login_url=reverse_lazy("core_main_app_login"),
             ),
             name="core_dashboard_files",
         ),
     )
```

### Comparing `core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/utils/query/django/prepare.py` & `core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/utils/query/django/prepare.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/utils/query/mongo/prepare.py` & `core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/utils/query/mongo/prepare.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/views/common/ajax.py` & `core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/views/common/ajax.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/views/common/forms.py` & `core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/views/common/forms.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.2.0/core_dashboard_registry_app/views/common/views.py` & `core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/views/common/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """ Common views for the registry dashboard
 """
 from django.conf import settings as conf_settings
 from django.contrib.auth.decorators import login_required
 from django.urls import reverse
-from django.urls import reverse_lazy
 from django.utils.decorators import method_decorator
 
 import core_curate_app.components.curate_data_structure.api as curate_data_structure_api
 from core_dashboard_common_app import constants as dashboard_common_constants
 from core_dashboard_common_app import settings
 from core_dashboard_common_app.views.common.forms import ActionForm, UserForm
 from core_dashboard_common_app.views.common.views import (
@@ -44,15 +43,15 @@
 from core_main_registry_app.constants import CUSTOM_RESOURCE_TYPE
 from core_main_registry_app.settings import ENABLE_BLOB_ENDPOINTS
 
 if "core_curate_registry_app" in INSTALLED_APPS:
     import core_curate_registry_app.components.curate_data_structure.api as curate_data_structure_registry_api
 
 
-@login_required(login_url=reverse_lazy("core_main_app_login"))
+@login_required
 def home(request):
     """Home page.
 
     Args:
         request:
 
     Returns:
@@ -443,14 +442,15 @@
                             _get_role_label(x, request=self.request)
                             for x in get_role(data)
                         ]
                     ),
                     "can_read": user_can_read or is_owner,
                     "can_write": user_can_write or is_owner,
                     "is_owner": is_owner,
+                    "can_set_public": not data_api.is_data_public(data),
                 }
             )
         return detailed_user_data
 
     def _get_modals(self):
         modals = super()._get_modals()
         modals.append(EditDataView.get_modal_html_path())
@@ -478,14 +478,17 @@
         )
         assets["js"].append(
             {
                 "path": "core_dashboard_registry_app/user/js/get_url.js",
                 "is_raw": False,
             }
         )
+        assets["js"].append(
+            {"path": dashboard_constants.JS_PUBLISH_RESOURCE, "is_raw": False}
+        )
         assets["js"].append(EditDataView.get_modal_js_path())
         return assets
 
 
 class DashboardRegistryForms(DashboardForms):
     """List the forms."""
```

### Comparing `core_dashboard_registry_app-2.2.0/core_dashboard_registry_app.egg-info/PKG-INFO` & `core_dashboard_registry_app-2.3.0/core_dashboard_registry_app.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-dashboard-registry-app
-Version: 2.2.0
+Version: 2.3.0
 Summary: Resource management via a dashboard for the registry core project
 Home-page: https://github.com/usnistgov/core_dashboard_registry_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: Core Dashboard Registry App
         ===========================
```

### Comparing `core_dashboard_registry_app-2.2.0/core_dashboard_registry_app.egg-info/SOURCES.txt` & `core_dashboard_registry_app-2.3.0/core_dashboard_registry_app.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.md
 MANIFEST.in
 README.rst
 pyproject.toml
 requirements.core.txt
 setup.py
 core_dashboard_registry_app/__init__.py
 core_dashboard_registry_app/admin.py
```

### Comparing `core_dashboard_registry_app-2.2.0/setup.py` & `core_dashboard_registry_app-2.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_dashboard_registry_app",
-    version="2.2.0",
+    version="2.3.0",
     description="Resource management via a dashboard for the registry core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_dashboard_registry_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_dashboard_registry_app-2.2.0/tests/test_settings.py` & `core_dashboard_registry_app-2.3.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.2.0/tests/utils/query/test_unit.py` & `core_dashboard_registry_app-2.3.0/tests/utils/query/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.2.0/tests/views/tests_unit.py` & `core_dashboard_registry_app-2.3.0/tests/views/tests_unit.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 """ Unit tests views
 """
 from unittest.mock import patch, MagicMock
 
 from django.contrib.auth.models import AnonymousUser
 from django.http import HttpResponse
-from django.test import RequestFactory, override_settings, tag
+from django.test import RequestFactory, override_settings, tag, SimpleTestCase
 
+from core_dashboard_registry_app import constants as dashboard_constants
 from core_dashboard_registry_app.views.common.views import (
     DashboardRegistryRecords,
+    DashboardRegistryWorkspaceRecords,
 )
 from core_main_app.access_control.exceptions import AccessControlError
 from core_main_app.commons.exceptions import ModelError
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 
 
-class TestDashboardRegistryRecords(MongoIntegrationBaseTestCase):
-    """TestViewData"""
+class TestDashboardRegistryRecords(IntegrationBaseTestCase):
+    """TestDashboardRegistryRecords"""
 
     def setUp(self):
         """setUp
 
         Returns:
 
         """
@@ -445,7 +447,23 @@
         view.request = request
 
         # Act
         result = view._format_draft_context_registry(draft_list=[draft])
 
         # Assert
         self.assertEqual(result[0]["role"], "None")
+
+
+class TestDashboardRegistryWorkspaceRecords(SimpleTestCase):
+    """TestDashboardRegistryWorkspaceRecords"""
+
+    def test_publish_script_added_to_assets(self):
+        """test_publish_script_added_to_assets
+
+        Returns:
+
+        """
+        assets = DashboardRegistryWorkspaceRecords()._get_assets()
+        self.assertTrue(
+            dashboard_constants.JS_PUBLISH_RESOURCE
+            in [asset["path"] for asset in assets["js"]]
+        )
```

