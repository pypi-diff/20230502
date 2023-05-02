# Comparing `tmp/core_dashboard_app-2.2.0.tar.gz` & `tmp/core_dashboard_app-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/core_dashboard_app-2.2.0.tar", last modified: Thu Feb 23 20:27:09 2023, max compression
+gzip compressed data, was "core_dashboard_app-2.3.0.tar", last modified: Tue May  2 19:36:09 2023, max compression
```

## Comparing `core_dashboard_app-2.2.0.tar` & `core_dashboard_app-2.3.0.tar`

### file list

```diff
@@ -1,58 +1,66 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:09.000000 core_dashboard_app-2.2.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      144 2023-02-23 20:27:06.000000 core_dashboard_app-2.2.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1080 2023-02-23 20:27:09.000000 core_dashboard_app-2.2.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      579 2023-02-23 20:27:06.000000 core_dashboard_app-2.2.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:08.000000 core_dashboard_app-2.2.0/core_dashboard_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:06.000000 core_dashboard_app-2.2.0/core_dashboard_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4595 2023-02-23 20:27:06.000000 core_dashboard_app-2.2.0/core_dashboard_app/admin.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3262 2023-02-23 20:27:06.000000 core_dashboard_app-2.2.0/core_dashboard_app/menus.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      407 2023-02-23 20:27:06.000000 core_dashboard_app-2.2.0/core_dashboard_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:08.000000 core_dashboard_app-2.2.0/core_dashboard_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:08.000000 core_dashboard_app-2.2.0/core_dashboard_app/static/core_dashboard_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:08.000000 core_dashboard_app-2.2.0/core_dashboard_app/static/core_dashboard_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:08.000000 core_dashboard_app-2.2.0/core_dashboard_app/static/core_dashboard_app/admin/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       93 2023-02-23 20:27:06.000000 core_dashboard_app-2.2.0/core_dashboard_app/static/core_dashboard_app/admin/js/my_dashboard_tabs.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:08.000000 core_dashboard_app-2.2.0/core_dashboard_app/static/core_dashboard_app/common/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:08.000000 core_dashboard_app-2.2.0/core_dashboard_app/static/core_dashboard_app/common/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       74 2023-02-23 20:27:06.000000 core_dashboard_app-2.2.0/core_dashboard_app/static/core_dashboard_app/common/css/my_dashboard_tabs.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:08.000000 core_dashboard_app-2.2.0/core_dashboard_app/static/core_dashboard_app/common/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      605 2023-02-23 20:27:06.000000 core_dashboard_app-2.2.0/core_dashboard_app/static/core_dashboard_app/common/js/my_dashboard_tabs.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:08.000000 core_dashboard_app-2.2.0/core_dashboard_app/static/core_dashboard_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:09.000000 core_dashboard_app-2.2.0/core_dashboard_app/static/core_dashboard_app/user/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       82 2023-02-23 20:27:06.000000 core_dashboard_app-2.2.0/core_dashboard_app/static/core_dashboard_app/user/js/my_dashboard_tabs.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:08.000000 core_dashboard_app-2.2.0/core_dashboard_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:08.000000 core_dashboard_app-2.2.0/core_dashboard_app/templates/core_dashboard_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:09.000000 core_dashboard_app-2.2.0/core_dashboard_app/templates/core_dashboard_app/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      323 2023-02-23 20:27:06.000000 core_dashboard_app-2.2.0/core_dashboard_app/templates/core_dashboard_app/admin/my_dashboard_container.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1150 2023-02-23 20:27:06.000000 core_dashboard_app-2.2.0/core_dashboard_app/templates/core_dashboard_app/admin/my_dashboard_content.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:08.000000 core_dashboard_app-2.2.0/core_dashboard_app/templates/core_dashboard_app/common/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:09.000000 core_dashboard_app-2.2.0/core_dashboard_app/templates/core_dashboard_app/common/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1574 2023-02-23 20:27:06.000000 core_dashboard_app-2.2.0/core_dashboard_app/templates/core_dashboard_app/common/list/my_dashboard_tabs.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      176 2023-02-23 20:27:06.000000 core_dashboard_app-2.2.0/core_dashboard_app/templates/core_dashboard_app/common/list/my_dashboard_tabs_file_pagination.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:09.000000 core_dashboard_app-2.2.0/core_dashboard_app/templates/core_dashboard_app/common/pagination/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2681 2023-02-23 20:27:06.000000 core_dashboard_app-2.2.0/core_dashboard_app/templates/core_dashboard_app/common/pagination/pagination_tab.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:09.000000 core_dashboard_app-2.2.0/core_dashboard_app/templates/core_dashboard_app/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      343 2023-02-23 20:27:06.000000 core_dashboard_app-2.2.0/core_dashboard_app/templates/core_dashboard_app/user/my_dashboard_container.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4357 2023-02-23 20:27:06.000000 core_dashboard_app-2.2.0/core_dashboard_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:09.000000 core_dashboard_app-2.2.0/core_dashboard_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:06.000000 core_dashboard_app-2.2.0/core_dashboard_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:09.000000 core_dashboard_app-2.2.0/core_dashboard_app/views/common/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:06.000000 core_dashboard_app-2.2.0/core_dashboard_app/views/common/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10087 2023-02-23 20:27:06.000000 core_dashboard_app-2.2.0/core_dashboard_app/views/common/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:08.000000 core_dashboard_app-2.2.0/core_dashboard_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1080 2023-02-23 20:27:08.000000 core_dashboard_app-2.2.0/core_dashboard_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1455 2023-02-23 20:27:08.000000 core_dashboard_app-2.2.0/core_dashboard_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-02-23 20:27:08.000000 core_dashboard_app-2.2.0/core_dashboard_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      111 2023-02-23 20:27:08.000000 core_dashboard_app-2.2.0/core_dashboard_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       30 2023-02-23 20:27:08.000000 core_dashboard_app-2.2.0/core_dashboard_app.egg-info/top_level.txt
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:09.000000 core_dashboard_app-2.2.0/docs/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:06.000000 core_dashboard_app-2.2.0/docs/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11302 2023-02-23 20:27:06.000000 core_dashboard_app-2.2.0/docs/conf.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      292 2023-02-23 20:27:06.000000 core_dashboard_app-2.2.0/docs/conf_urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-02-23 20:27:07.000000 core_dashboard_app-2.2.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       85 2023-02-23 20:27:07.000000 core_dashboard_app-2.2.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-02-23 20:27:09.000000 core_dashboard_app-2.2.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1077 2023-02-23 20:27:07.000000 core_dashboard_app-2.2.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:09.000000 core_dashboard_app-2.2.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:07.000000 core_dashboard_app-2.2.0/tests/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1106 2023-02-23 20:27:07.000000 core_dashboard_app-2.2.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:09.755907 core_dashboard_app-2.3.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:36:06.000000 core_dashboard_app-2.3.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      144 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1080 2023-05-02 19:36:09.751021 core_dashboard_app-2.3.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      579 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:09.351952 core_dashboard_app-2.3.0/core_dashboard_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/core_dashboard_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4595 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/core_dashboard_app/admin.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3262 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/core_dashboard_app/menus.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      407 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/core_dashboard_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:09.106711 core_dashboard_app-2.3.0/core_dashboard_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:09.130807 core_dashboard_app-2.3.0/core_dashboard_app/static/core_dashboard_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:09.112427 core_dashboard_app-2.3.0/core_dashboard_app/static/core_dashboard_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:09.445096 core_dashboard_app-2.3.0/core_dashboard_app/static/core_dashboard_app/admin/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       93 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/core_dashboard_app/static/core_dashboard_app/admin/js/my_dashboard_tabs.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:09.125549 core_dashboard_app-2.3.0/core_dashboard_app/static/core_dashboard_app/common/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:09.457693 core_dashboard_app-2.3.0/core_dashboard_app/static/core_dashboard_app/common/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       74 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/core_dashboard_app/static/core_dashboard_app/common/css/my_dashboard_tabs.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:09.469998 core_dashboard_app-2.3.0/core_dashboard_app/static/core_dashboard_app/common/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      605 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/core_dashboard_app/static/core_dashboard_app/common/js/my_dashboard_tabs.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:09.134062 core_dashboard_app-2.3.0/core_dashboard_app/static/core_dashboard_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:09.481581 core_dashboard_app-2.3.0/core_dashboard_app/static/core_dashboard_app/user/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       82 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/core_dashboard_app/static/core_dashboard_app/user/js/my_dashboard_tabs.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:09.143832 core_dashboard_app-2.3.0/core_dashboard_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:09.177462 core_dashboard_app-2.3.0/core_dashboard_app/templates/core_dashboard_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:09.509808 core_dashboard_app-2.3.0/core_dashboard_app/templates/core_dashboard_app/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      323 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/core_dashboard_app/templates/core_dashboard_app/admin/my_dashboard_container.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1150 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/core_dashboard_app/templates/core_dashboard_app/admin/my_dashboard_content.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:09.173389 core_dashboard_app-2.3.0/core_dashboard_app/templates/core_dashboard_app/common/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:09.536161 core_dashboard_app-2.3.0/core_dashboard_app/templates/core_dashboard_app/common/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1720 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/core_dashboard_app/templates/core_dashboard_app/common/list/my_dashboard_tabs.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      176 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/core_dashboard_app/templates/core_dashboard_app/common/list/my_dashboard_tabs_file_pagination.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:09.549138 core_dashboard_app-2.3.0/core_dashboard_app/templates/core_dashboard_app/common/pagination/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2681 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/core_dashboard_app/templates/core_dashboard_app/common/pagination/pagination_tab.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:09.561730 core_dashboard_app-2.3.0/core_dashboard_app/templates/core_dashboard_app/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      343 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/core_dashboard_app/templates/core_dashboard_app/user/my_dashboard_container.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3885 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/core_dashboard_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:09.574128 core_dashboard_app-2.3.0/core_dashboard_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/core_dashboard_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:09.605603 core_dashboard_app-2.3.0/core_dashboard_app/views/common/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/core_dashboard_app/views/common/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10514 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/core_dashboard_app/views/common/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:09.430864 core_dashboard_app-2.3.0/core_dashboard_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1080 2023-05-02 19:36:08.000000 core_dashboard_app-2.3.0/core_dashboard_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1597 2023-05-02 19:36:09.000000 core_dashboard_app-2.3.0/core_dashboard_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:36:08.000000 core_dashboard_app-2.3.0/core_dashboard_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      111 2023-05-02 19:36:08.000000 core_dashboard_app-2.3.0/core_dashboard_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       30 2023-05-02 19:36:08.000000 core_dashboard_app-2.3.0/core_dashboard_app.egg-info/top_level.txt
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:09.653544 core_dashboard_app-2.3.0/docs/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/docs/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11302 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/docs/conf.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      292 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/docs/conf_urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       85 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:36:09.757864 core_dashboard_app-2.3.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1077 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:09.678652 core_dashboard_app-2.3.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/tests/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1621 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:09.689576 core_dashboard_app-2.3.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/tests/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:09.705675 core_dashboard_app-2.3.0/tests/views/common/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/tests/views/common/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:09.741517 core_dashboard_app-2.3.0/tests/views/common/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/tests/views/common/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4784 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/tests/views/common/views/tests_unit.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `core_dashboard_app-2.2.0/PKG-INFO` & `core_dashboard_app-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_dashboard_app
-Version: 2.2.0
+Version: 2.3.0
 Summary: Resource management via a dashboard for the curator core project
 Home-page: https://github.com/usnistgov/core_dashboard_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: ==================
         Core Dashboard App
```

### Comparing `core_dashboard_app-2.2.0/README.rst` & `core_dashboard_app-2.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_dashboard_app-2.2.0/core_dashboard_app/admin.py` & `core_dashboard_app-2.3.0/core_dashboard_app/admin.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_app-2.2.0/core_dashboard_app/menus.py` & `core_dashboard_app-2.3.0/core_dashboard_app/menus.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_app-2.2.0/core_dashboard_app/static/core_dashboard_app/common/js/my_dashboard_tabs.js` & `core_dashboard_app-2.3.0/core_dashboard_app/static/core_dashboard_app/common/js/my_dashboard_tabs.js`

 * *Files identical despite different names*

### Comparing `core_dashboard_app-2.2.0/core_dashboard_app/templates/core_dashboard_app/admin/my_dashboard_content.html` & `core_dashboard_app-2.3.0/core_dashboard_app/templates/core_dashboard_app/admin/my_dashboard_content.html`

 * *Files identical despite different names*

### Comparing `core_dashboard_app-2.2.0/core_dashboard_app/templates/core_dashboard_app/common/list/my_dashboard_tabs.html` & `core_dashboard_app-2.3.0/core_dashboard_app/templates/core_dashboard_app/common/list/my_dashboard_tabs.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,99 +1,108 @@
-00000000: 3c64 6976 3e0a 2020 2020 3c75 6c20 636c  <div>.    <ul cl
-00000010: 6173 733d 226e 6176 206e 6176 2d74 6162  ass="nav nav-tab
-00000020: 7322 726f 6c65 3d22 7461 626c 6973 7422  s"role="tablist"
-00000030: 3e0a 2020 2020 2020 2020 3c6c 6920 726f  >.        <li ro
-00000040: 6c65 3d22 7072 6573 656e 7461 7469 6f6e  le="presentation
-00000050: 2220 636c 6173 733d 226e 6176 2d69 7465  " class="nav-ite
-00000060: 6d22 3e0a 2020 2020 2020 2020 2020 2020  m">.            
-00000070: 3c61 2063 6c61 7373 3d22 6e61 762d 6c69  <a class="nav-li
-00000080: 6e6b 7b25 2069 6620 6461 7461 2e74 6162  nk{% if data.tab
-00000090: 203d 3d20 2764 6174 6127 2025 7d20 6163   == 'data' %} ac
-000000a0: 7469 7665 207b 2520 656e 6469 6620 257d  tive {% endif %}
-000000b0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-000000c0: 2069 643d 2274 6162 5f64 6174 615f 7461   id="tab_data_ta
-000000d0: 626c 6522 0a20 2020 2020 2020 2020 2020  ble".           
-000000e0: 2020 2020 6461 7461 2d74 6162 2d76 616c      data-tab-val
-000000f0: 7565 3d22 6461 7461 220a 2020 2020 2020  ue="data".      
-00000100: 2020 2020 2020 2020 2061 7269 612d 636f           aria-co
-00000110: 6e74 726f 6c73 3d22 7072 6f66 696c 6522  ntrols="profile"
-00000120: 2072 6f6c 653d 2274 6162 223e 0a20 2020   role="tab">.   
-00000130: 2020 2020 2020 2020 2020 2020 2044 6174               Dat
-00000140: 6120 287b 7b64 6174 612e 6e75 6d62 6572  a ({{data.number
-00000150: 5f74 6f74 616c 5f64 6174 617d 7d29 0a20  _total_data}}). 
-00000160: 2020 2020 2020 2020 2020 203c 2f61 3e0a             </a>.
-00000170: 2020 2020 2020 2020 3c2f 6c69 3e0a 2020          </li>.  
-00000180: 2020 2020 2020 3c6c 6920 726f 6c65 3d22        <li role="
-00000190: 7072 6573 656e 7461 7469 6f6e 2220 636c  presentation" cl
-000001a0: 6173 733d 226e 6176 2d69 7465 6d22 3e0a  ass="nav-item">.
-000001b0: 2020 2020 2020 2020 2020 2020 3c61 2063              <a c
-000001c0: 6c61 7373 3d22 6e61 762d 6c69 6e6b 7b25  lass="nav-link{%
-000001d0: 2069 6620 6461 7461 2e74 6162 203d 3d20   if data.tab == 
-000001e0: 2766 696c 6527 2025 7d20 6163 7469 7665  'file' %} active
-000001f0: 207b 2520 656e 6469 6620 257d 220a 2020   {% endif %}".  
-00000200: 2020 2020 2020 2020 2020 2020 2069 643d               id=
-00000210: 2274 6162 5f66 696c 655f 7461 626c 6522  "tab_file_table"
-00000220: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000230: 6461 7461 2d74 6162 2d76 616c 7565 3d22  data-tab-value="
-00000240: 6669 6c65 220a 2020 2020 2020 2020 2020  file".          
-00000250: 2020 2020 2061 7269 612d 636f 6e74 726f       aria-contro
-00000260: 6c73 3d22 7072 6f66 696c 6522 2072 6f6c  ls="profile" rol
-00000270: 653d 2274 6162 223e 0a20 2020 2020 2020  e="tab">.       
-00000280: 2020 2020 2020 2020 2046 696c 6573 2028           Files (
-00000290: 7b7b 6461 7461 2e6e 756d 6265 725f 746f  {{data.number_to
-000002a0: 7461 6c5f 6669 6c65 737d 7d29 0a20 2020  tal_files}}).   
-000002b0: 2020 2020 2020 2020 203c 2f61 3e0a 2020           </a>.  
-000002c0: 2020 2020 2020 3c2f 6c69 3e0a 2020 2020        </li>.    
-000002d0: 3c2f 756c 3e0a 2020 2020 3c64 6976 2063  </ul>.    <div c
-000002e0: 6c61 7373 3d22 7461 622d 636f 6e74 656e  lass="tab-conten
-000002f0: 7422 3e0a 2020 2020 2020 2020 7b25 2069  t">.        {% i
-00000300: 6620 6461 7461 2e75 7365 725f 6461 7461  f data.user_data
-00000310: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
-00000320: 7b25 2069 6620 6461 7461 2e74 6162 203d  {% if data.tab =
-00000330: 3d20 2764 6174 6127 2025 7d0a 2020 2020  = 'data' %}.    
-00000340: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-00000350: 2072 6f6c 653d 2274 6162 7061 6e65 6c22   role="tabpanel"
-00000360: 2069 643d 2264 6174 615f 7461 626c 6522   id="data_table"
-00000370: 2063 6c61 7373 3d22 7461 622d 7061 6e65   class="tab-pane
-00000380: 207b 2520 6966 2064 6174 612e 7461 6220   {% if data.tab 
-00000390: 3d3d 2027 6461 7461 2720 257d 2061 6374  == 'data' %} act
-000003a0: 6976 6520 7b25 2065 6e64 6966 2025 7d22  ive {% endif %}"
-000003b0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-000003c0: 2020 2020 2020 2020 2020 7b25 2069 6e63            {% inc
-000003d0: 6c75 6465 2027 636f 7265 5f64 6173 6862  lude 'core_dashb
-000003e0: 6f61 7264 5f63 6f6d 6d6f 6e5f 6170 702f  oard_common_app/
-000003f0: 6c69 7374 2f6d 795f 6461 7368 626f 6172  list/my_dashboar
-00000400: 645f 6d79 5f72 6563 6f72 6473 5f74 6162  d_my_records_tab
-00000410: 6c65 5f70 6167 696e 6174 696f 6e2e 6874  le_pagination.ht
-00000420: 6d6c 2720 257d 0a20 2020 2020 2020 2020  ml' %}.         
-00000430: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
-00000440: 2020 2020 2020 2020 2020 7b25 2065 6e64            {% end
-00000450: 6966 2025 7d0a 2020 2020 2020 2020 2020  if %}.          
-00000460: 2020 7b25 2069 6620 6461 7461 2e74 6162    {% if data.tab
-00000470: 203d 3d20 2766 696c 6527 2025 7d0a 2020   == 'file' %}.  
-00000480: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-00000490: 6976 2072 6f6c 653d 2274 6162 7061 6e65  iv role="tabpane
-000004a0: 6c22 2069 643d 2266 696c 655f 7461 626c  l" id="file_tabl
-000004b0: 6522 2063 6c61 7373 3d22 7461 622d 7061  e" class="tab-pa
-000004c0: 6e65 207b 2520 6966 2064 6174 612e 7461  ne {% if data.ta
-000004d0: 6220 3d3d 2027 6669 6c65 2720 257d 2061  b == 'file' %} a
-000004e0: 6374 6976 6520 7b25 2065 6e64 6966 2025  ctive {% endif %
-000004f0: 7d22 3e0a 2020 2020 2020 2020 2020 2020  }">.            
-00000500: 2020 2020 2020 2020 2020 2020 7b25 2069              {% i
-00000510: 6e63 6c75 6465 2027 636f 7265 5f64 6173  nclude 'core_das
-00000520: 6862 6f61 7264 5f61 7070 2f63 6f6d 6d6f  hboard_app/commo
-00000530: 6e2f 6c69 7374 2f6d 795f 6461 7368 626f  n/list/my_dashbo
-00000540: 6172 645f 7461 6273 5f66 696c 655f 7061  ard_tabs_file_pa
-00000550: 6769 6e61 7469 6f6e 2e68 746d 6c27 2025  gination.html' %
-00000560: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-00000570: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
-00000580: 2020 2020 207b 2520 656e 6469 6620 257d       {% endif %}
-00000590: 0a20 2020 2020 2020 207b 2520 656c 7365  .        {% else
-000005a0: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
-000005b0: 3c64 6976 2063 6c61 7373 3d22 616c 6572  <div class="aler
-000005c0: 7422 3e0a 2020 2020 2020 2020 2020 2020  t">.            
-000005d0: 2020 2020 5468 6520 636f 6c6c 6563 7469      The collecti
-000005e0: 6f6e 2069 7320 656d 7074 792e 0a20 2020  on is empty..   
-000005f0: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
-00000600: 2020 2020 2020 2020 7b25 2065 6e64 6966          {% endif
-00000610: 2025 7d0a 2020 2020 3c2f 6469 763e 0a3c   %}.    </div>.<
-00000620: 2f64 6976 3e0a                           /div>.
+00000000: 3c64 6976 3e0a 2020 2020 7b25 2069 6620  <div>.    {% if 
+00000010: 6461 7461 2e61 646d 696e 6973 7472 6174  data.administrat
+00000020: 696f 6e20 616e 6420 6461 7461 2e6f 776e  ion and data.own
+00000030: 6572 2025 7d0a 2020 2020 2020 2020 3c70  er %}.        <p
+00000040: 3e4f 776e 6572 3a20 3c61 2068 7265 663d  >Owner: <a href=
+00000050: 227b 7b20 6461 7461 2e6f 776e 6572 5f63  "{{ data.owner_c
+00000060: 6861 6e67 655f 7572 6c20 7d7d 223e 7b7b  hange_url }}">{{
+00000070: 2064 6174 612e 6f77 6e65 7220 7d7d 3c2f   data.owner }}</
+00000080: 613e 3c2f 703e 0a20 2020 207b 2520 656e  a></p>.    {% en
+00000090: 6469 6620 257d 0a20 2020 203c 756c 2063  dif %}.    <ul c
+000000a0: 6c61 7373 3d22 6e61 7620 6e61 762d 7461  lass="nav nav-ta
+000000b0: 6273 2220 726f 6c65 3d22 7461 626c 6973  bs" role="tablis
+000000c0: 7422 3e0a 2020 2020 2020 2020 3c6c 6920  t">.        <li 
+000000d0: 726f 6c65 3d22 7072 6573 656e 7461 7469  role="presentati
+000000e0: 6f6e 2220 636c 6173 733d 226e 6176 2d69  on" class="nav-i
+000000f0: 7465 6d22 3e0a 2020 2020 2020 2020 2020  tem">.          
+00000100: 2020 3c61 2063 6c61 7373 3d22 6e61 762d    <a class="nav-
+00000110: 6c69 6e6b 7b25 2069 6620 6461 7461 2e74  link{% if data.t
+00000120: 6162 203d 3d20 2764 6174 6127 2025 7d20  ab == 'data' %} 
+00000130: 6163 7469 7665 207b 2520 656e 6469 6620  active {% endif 
+00000140: 257d 220a 2020 2020 2020 2020 2020 2020  %}".            
+00000150: 2020 2069 643d 2274 6162 5f64 6174 615f     id="tab_data_
+00000160: 7461 626c 6522 0a20 2020 2020 2020 2020  table".         
+00000170: 2020 2020 2020 6461 7461 2d74 6162 2d76        data-tab-v
+00000180: 616c 7565 3d22 6461 7461 220a 2020 2020  alue="data".    
+00000190: 2020 2020 2020 2020 2020 2061 7269 612d             aria-
+000001a0: 636f 6e74 726f 6c73 3d22 7072 6f66 696c  controls="profil
+000001b0: 6522 2072 6f6c 653d 2274 6162 223e 0a20  e" role="tab">. 
+000001c0: 2020 2020 2020 2020 2020 2020 2020 2044                 D
+000001d0: 6174 6120 287b 7b64 6174 612e 6e75 6d62  ata ({{data.numb
+000001e0: 6572 5f74 6f74 616c 5f64 6174 617d 7d29  er_total_data}})
+000001f0: 0a20 2020 2020 2020 2020 2020 203c 2f61  .            </a
+00000200: 3e0a 2020 2020 2020 2020 3c2f 6c69 3e0a  >.        </li>.
+00000210: 2020 2020 2020 2020 3c6c 6920 726f 6c65          <li role
+00000220: 3d22 7072 6573 656e 7461 7469 6f6e 2220  ="presentation" 
+00000230: 636c 6173 733d 226e 6176 2d69 7465 6d22  class="nav-item"
+00000240: 3e0a 2020 2020 2020 2020 2020 2020 3c61  >.            <a
+00000250: 2063 6c61 7373 3d22 6e61 762d 6c69 6e6b   class="nav-link
+00000260: 7b25 2069 6620 6461 7461 2e74 6162 203d  {% if data.tab =
+00000270: 3d20 2766 696c 6527 2025 7d20 6163 7469  = 'file' %} acti
+00000280: 7665 207b 2520 656e 6469 6620 257d 220a  ve {% endif %}".
+00000290: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000002a0: 643d 2274 6162 5f66 696c 655f 7461 626c  d="tab_file_tabl
+000002b0: 6522 0a20 2020 2020 2020 2020 2020 2020  e".             
+000002c0: 2020 6461 7461 2d74 6162 2d76 616c 7565    data-tab-value
+000002d0: 3d22 6669 6c65 220a 2020 2020 2020 2020  ="file".        
+000002e0: 2020 2020 2020 2061 7269 612d 636f 6e74         aria-cont
+000002f0: 726f 6c73 3d22 7072 6f66 696c 6522 2072  rols="profile" r
+00000300: 6f6c 653d 2274 6162 223e 0a20 2020 2020  ole="tab">.     
+00000310: 2020 2020 2020 2020 2020 2046 696c 6573             Files
+00000320: 2028 7b7b 6461 7461 2e6e 756d 6265 725f   ({{data.number_
+00000330: 746f 7461 6c5f 6669 6c65 737d 7d29 0a20  total_files}}). 
+00000340: 2020 2020 2020 2020 2020 203c 2f61 3e0a             </a>.
+00000350: 2020 2020 2020 2020 3c2f 6c69 3e0a 2020          </li>.  
+00000360: 2020 3c2f 756c 3e0a 2020 2020 3c64 6976    </ul>.    <div
+00000370: 2063 6c61 7373 3d22 7461 622d 636f 6e74   class="tab-cont
+00000380: 656e 7422 3e0a 2020 2020 2020 2020 7b25  ent">.        {%
+00000390: 2069 6620 6461 7461 2e75 7365 725f 6461   if data.user_da
+000003a0: 7461 2025 7d0a 2020 2020 2020 2020 2020  ta %}.          
+000003b0: 2020 7b25 2069 6620 6461 7461 2e74 6162    {% if data.tab
+000003c0: 203d 3d20 2764 6174 6127 2025 7d0a 2020   == 'data' %}.  
+000003d0: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+000003e0: 6976 2072 6f6c 653d 2274 6162 7061 6e65  iv role="tabpane
+000003f0: 6c22 2069 643d 2264 6174 615f 7461 626c  l" id="data_tabl
+00000400: 6522 2063 6c61 7373 3d22 7461 622d 7061  e" class="tab-pa
+00000410: 6e65 207b 2520 6966 2064 6174 612e 7461  ne {% if data.ta
+00000420: 6220 3d3d 2027 6461 7461 2720 257d 2061  b == 'data' %} a
+00000430: 6374 6976 6520 7b25 2065 6e64 6966 2025  ctive {% endif %
+00000440: 7d22 3e0a 2020 2020 2020 2020 2020 2020  }">.            
+00000450: 2020 2020 2020 2020 2020 2020 7b25 2069              {% i
+00000460: 6e63 6c75 6465 2027 636f 7265 5f64 6173  nclude 'core_das
+00000470: 6862 6f61 7264 5f63 6f6d 6d6f 6e5f 6170  hboard_common_ap
+00000480: 702f 6c69 7374 2f6d 795f 6461 7368 626f  p/list/my_dashbo
+00000490: 6172 645f 6d79 5f72 6563 6f72 6473 5f74  ard_my_records_t
+000004a0: 6162 6c65 5f70 6167 696e 6174 696f 6e2e  able_pagination.
+000004b0: 6874 6d6c 2720 257d 0a20 2020 2020 2020  html' %}.       
+000004c0: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
+000004d0: 2020 2020 2020 2020 2020 2020 7b25 2065              {% e
+000004e0: 6e64 6966 2025 7d0a 2020 2020 2020 2020  ndif %}.        
+000004f0: 2020 2020 7b25 2069 6620 6461 7461 2e74      {% if data.t
+00000500: 6162 203d 3d20 2766 696c 6527 2025 7d0a  ab == 'file' %}.
+00000510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000520: 3c64 6976 2072 6f6c 653d 2274 6162 7061  <div role="tabpa
+00000530: 6e65 6c22 2069 643d 2266 696c 655f 7461  nel" id="file_ta
+00000540: 626c 6522 2063 6c61 7373 3d22 7461 622d  ble" class="tab-
+00000550: 7061 6e65 207b 2520 6966 2064 6174 612e  pane {% if data.
+00000560: 7461 6220 3d3d 2027 6669 6c65 2720 257d  tab == 'file' %}
+00000570: 2061 6374 6976 6520 7b25 2065 6e64 6966   active {% endif
+00000580: 2025 7d22 3e0a 2020 2020 2020 2020 2020   %}">.          
+00000590: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
+000005a0: 2069 6e63 6c75 6465 2027 636f 7265 5f64   include 'core_d
+000005b0: 6173 6862 6f61 7264 5f61 7070 2f63 6f6d  ashboard_app/com
+000005c0: 6d6f 6e2f 6c69 7374 2f6d 795f 6461 7368  mon/list/my_dash
+000005d0: 626f 6172 645f 7461 6273 5f66 696c 655f  board_tabs_file_
+000005e0: 7061 6769 6e61 7469 6f6e 2e68 746d 6c27  pagination.html'
+000005f0: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+00000600: 2020 2020 3c2f 6469 763e 0a20 2020 2020      </div>.     
+00000610: 2020 2020 2020 207b 2520 656e 6469 6620         {% endif 
+00000620: 257d 0a20 2020 2020 2020 207b 2520 656c  %}.        {% el
+00000630: 7365 2025 7d0a 2020 2020 2020 2020 2020  se %}.          
+00000640: 2020 3c64 6976 2063 6c61 7373 3d22 616c    <div class="al
+00000650: 6572 7422 3e0a 2020 2020 2020 2020 2020  ert">.          
+00000660: 2020 2020 2020 5468 6520 636f 6c6c 6563        The collec
+00000670: 7469 6f6e 2069 7320 656d 7074 792e 0a20  tion is empty.. 
+00000680: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
+00000690: 3e0a 2020 2020 2020 2020 7b25 2065 6e64  >.        {% end
+000006a0: 6966 2025 7d0a 2020 2020 3c2f 6469 763e  if %}.    </div>
+000006b0: 0a3c 2f64 6976 3e0a                      .</div>.
```

### Comparing `core_dashboard_app-2.2.0/core_dashboard_app/templates/core_dashboard_app/common/pagination/pagination_tab.html` & `core_dashboard_app-2.3.0/core_dashboard_app/templates/core_dashboard_app/common/pagination/pagination_tab.html`

 * *Files identical despite different names*

### Comparing `core_dashboard_app-2.2.0/core_dashboard_app/urls.py` & `core_dashboard_app-2.3.0/core_dashboard_app/urls.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
     Url router for the user dashboard
 """
 from django.contrib.auth.decorators import login_required
 from django.urls import re_path
 from django.urls import reverse_lazy
 
+from core_dashboard_app.views.common import views as dashboard_app_common_views
 from core_dashboard_common_app.views.common import (
     ajax,
     views as dashboard_common_app_common_views,
 )
 from core_dashboard_common_app.views.common.views import (
     UserDashboardPasswordChangeFormView,
 )
 from core_main_app.settings import INSTALLED_APPS
 from core_main_app.views.common.ajax import EditTemplateVersionManagerView
-from core_dashboard_app.views.common import views as dashboard_app_common_views
 
 urlpatterns = [
     # Common
     re_path(
         r"^$",
         dashboard_common_app_common_views.home,
         name="core_dashboard_home",
@@ -55,71 +55,63 @@
         r"^edit-record", ajax.edit_record, name="core_dashboard_edit_record"
     ),
     # User
     re_path(
         r"^records$",
         login_required(
             dashboard_common_app_common_views.DashboardRecords.as_view(),
-            login_url=reverse_lazy("core_main_app_login"),
         ),
         name="core_dashboard_records",
     ),
     re_path(
         r"^forms$",
         login_required(
             dashboard_common_app_common_views.DashboardForms.as_view(),
-            login_url=reverse_lazy("core_main_app_login"),
         ),
         name="core_dashboard_forms",
     ),
     re_path(
         r"^templates$",
         login_required(
             dashboard_common_app_common_views.DashboardTemplates.as_view(),
-            login_url=reverse_lazy("core_main_app_login"),
         ),
         name="core_dashboard_templates",
     ),
     re_path(
         r"^types$",
         login_required(
             dashboard_common_app_common_views.DashboardTypes.as_view(),
-            login_url=reverse_lazy("core_main_app_login"),
         ),
         name="core_dashboard_types",
     ),
     re_path(
         r"^files$",
         login_required(
             dashboard_common_app_common_views.DashboardFiles.as_view(),
-            login_url=reverse_lazy("core_main_app_login"),
         ),
         name="core_dashboard_files",
     ),
     re_path(
         r"^queries$",
         login_required(
             dashboard_common_app_common_views.DashboardQueries.as_view(),
-            login_url=reverse_lazy("core_main_app_login"),
         ),
         name="core_dashboard_queries",
     ),
     re_path(
         r"^workspaces$",
         login_required(
             dashboard_common_app_common_views.DashboardWorkspaces.as_view(),
-            login_url=reverse_lazy("core_main_app_login"),
         ),
         name="core_dashboard_workspaces",
     ),
     re_path(
         r"^workspace/(?P<workspace_id>\w+)$",
         login_required(
             dashboard_app_common_views.DashboardWorkspaceTabs.as_view(),
-            login_url=reverse_lazy("core_main_app_login"),
         ),
         name="core_dashboard_workspace_list",
     ),
     re_path(
         r"^template/(?P<pk>[\w-]+)/edit/$",
         EditTemplateVersionManagerView.as_view(
             success_url=reverse_lazy("core_dashboard_templates")
```

### Comparing `core_dashboard_app-2.2.0/core_dashboard_app/views/common/views.py` & `core_dashboard_app-2.3.0/core_dashboard_app/views/common/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """ User Views
 """
 import copy
 
 from django.core.exceptions import ObjectDoesNotExist
+from django.urls import reverse
 
 from core_dashboard_common_app import constants as dashboard_constants
 from core_dashboard_common_app import settings
 from core_dashboard_common_app.views.common.forms import UserForm
 from core_main_app.access_control.exceptions import AccessControlError
 from core_main_app.commons import exceptions
 from core_main_app.components.blob import api as workspace_blob_api
@@ -33,32 +34,40 @@
         Args:
             request:
             workspace_id:
 
         Returns:
 
         """
+        # Initialize necessary variables
+        user_can_read = False
+
+        tab_selected = request.GET.get("tab", "data")
+        data_count = 0
+        files_count = 0
+        context = {}
 
         try:
             workspace = workspace_api.get_by_id(workspace_id)
+        except exceptions.DoesNotExist:
+            error_message = "Workspace not found"
+            status_code = 404
+            return self._show_error(request, error_message, status_code)
+
+        try:
             user_can_read = workspace_api.can_user_read_workspace(
                 workspace, request.user
             )
             if not user_can_read:
                 error_message = "Access Forbidden"
                 status_code = 403
                 return self._show_error(request, error_message, status_code)
 
-            # Get the selected tab if given, otherwise data will be selected by default
-            tab_selected = request.GET.get("tab", "data")
+            # Figure out the items to render on the page
             items_to_render = []
-
-            context = {}
-            data_count = 0
-            files_count = 0
             data = workspace_data_api.get_all_by_workspace(
                 workspace, request.user
             )
             data_count = data.count()
             files = workspace_blob_api.get_all_by_workspace(
                 workspace, request.user
             )
@@ -76,18 +85,14 @@
                 context.update(
                     {
                         "document": dashboard_constants.FUNCTIONAL_OBJECT_ENUM.FILE.value
                     }
                 )
         except AccessControlError:
             items_to_render = workspace_data_api.get_none()
-        except exceptions.DoesNotExist:
-            error_message = "Workspace not found"
-            status_code = 404
-            return self._show_error(request, error_message, status_code)
 
         user_can_write = workspace_api.can_user_write_workspace(
             workspace, request.user
         )
 
         # Paginator
         page = request.GET.get("page", 1)
@@ -120,14 +125,24 @@
                 "tab": tab_selected,
                 "title": workspace.title,
                 "number_total_data": data_count,
                 "number_total_files": files_count,
             }
         )
 
+        if self.administration and workspace.owner:
+            context.update(
+                {
+                    "owner": user_api.get_user_by_id(workspace.owner).username,
+                    "owner_change_url": reverse(
+                        "admin:auth_user_change", args=[workspace.owner]
+                    ),
+                }
+            )
+
         # Get all username and corresponding ids
         user_names = dict(
             (str(x.id), x.username) for x in user_api.get_all_users()
         )
         context.update({"usernames": user_names})
 
         modals = [
@@ -146,14 +161,15 @@
                     }
                 ]
             )
             assets["css"].append(
                 "core_file_preview_app/user/css/file_preview.css"
             )
             modals.append("core_file_preview_app/user/file_preview_modal.html")
+
         # Set page title
         context.update({"page_title": "Dashboard"})
         return self.common_render(
             request,
             self.template,
             context=context,
             assets=assets,
```

### Comparing `core_dashboard_app-2.2.0/core_dashboard_app.egg-info/PKG-INFO` & `core_dashboard_app-2.3.0/core_dashboard_app.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-dashboard-app
-Version: 2.2.0
+Version: 2.3.0
 Summary: Resource management via a dashboard for the curator core project
 Home-page: https://github.com/usnistgov/core_dashboard_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: ==================
         Core Dashboard App
```

### Comparing `core_dashboard_app-2.2.0/core_dashboard_app.egg-info/SOURCES.txt` & `core_dashboard_app-2.3.0/core_dashboard_app.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.md
 MANIFEST.in
 README.rst
 pyproject.toml
 requirements.core.txt
 setup.py
 core_dashboard_app/__init__.py
 core_dashboard_app/admin.py
@@ -26,8 +27,12 @@
 core_dashboard_app/views/__init__.py
 core_dashboard_app/views/common/__init__.py
 core_dashboard_app/views/common/views.py
 docs/__init__.py
 docs/conf.py
 docs/conf_urls.py
 tests/__init__.py
-tests/test_settings.py
+tests/test_settings.py
+tests/views/__init__.py
+tests/views/common/__init__.py
+tests/views/common/views/__init__.py
+tests/views/common/views/tests_unit.py
```

### Comparing `core_dashboard_app-2.2.0/docs/conf.py` & `core_dashboard_app-2.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_app-2.2.0/setup.py` & `core_dashboard_app-2.3.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_dashboard_app",
-    version="2.2.0",
+    version="2.3.0",
     description="Resource management via a dashboard for the curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_dashboard_app",
     packages=find_packages(),
     include_package_data=True,
```

