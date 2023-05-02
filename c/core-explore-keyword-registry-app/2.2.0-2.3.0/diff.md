# Comparing `tmp/core_explore_keyword_registry_app-2.2.0.tar.gz` & `tmp/core_explore_keyword_registry_app-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/core_explore_keyword_registry_app-2.2.0.tar", last modified: Thu Feb 23 20:28:56 2023, max compression
+gzip compressed data, was "core_explore_keyword_registry_app-2.3.0.tar", last modified: Tue May  2 19:38:05 2023, max compression
```

## Comparing `core_explore_keyword_registry_app-2.2.0.tar` & `core_explore_keyword_registry_app-2.3.0.tar`

### file list

```diff
@@ -1,79 +1,80 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:56.000000 core_explore_keyword_registry_app-2.2.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      199 2023-02-23 20:28:54.000000 core_explore_keyword_registry_app-2.2.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1581 2023-02-23 20:28:56.000000 core_explore_keyword_registry_app-2.2.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1042 2023-02-23 20:28:54.000000 core_explore_keyword_registry_app-2.2.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:56.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      120 2023-02-23 20:28:54.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      710 2023-02-23 20:28:54.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/apps.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3508 2023-02-23 20:28:54.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/discover.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:56.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/permissions/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:54.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/permissions/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1063 2023-02-23 20:28:54.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/permissions/discover.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      883 2023-02-23 20:28:54.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:56.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:56.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:56.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:56.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/css/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:56.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/css/fancytree/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      813 2023-02-23 20:28:54.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/css/fancytree/fancytree.custom.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:56.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/css/search/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      310 2023-02-23 20:28:54.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/css/search/filters.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1016 2023-02-23 20:28:54.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/css/search/search.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:56.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:56.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3328 2023-02-23 20:28:54.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/fancytree.custom.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       76 2023-02-23 20:28:54.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/fancytree.custom.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2544 2023-02-23 20:28:54.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/filters.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9169 2023-02-23 20:28:54.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/resource_type_icons_table.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      257 2023-02-23 20:28:54.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/resource_type_icons_table.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      322 2023-02-23 20:28:54.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/search.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      650 2023-02-23 20:28:54.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/tagit.custom.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:56.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/libs/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:56.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/libs/jquery-shorten/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:56.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/libs/jquery-shorten/1.1.0/
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     6230 2023-02-23 20:28:54.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/libs/jquery-shorten/1.1.0/jquery.shorten.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:56.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/xsl/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6809 2023-02-23 20:28:54.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/xsl/registry-detail.xsl
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4178 2023-02-23 20:28:54.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/xsl/registry-list.xsl
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:56.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:56.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/templates/core_explore_common_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:56.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/templates/core_explore_common_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:56.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/templates/core_explore_common_app/user/results/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      937 2023-02-23 20:28:54.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/templates/core_explore_common_app/user/results/data_source_info.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      846 2023-02-23 20:28:54.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/templates/core_explore_common_app/user/results/data_source_results.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:56.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/templates/core_explore_keyword_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:56.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/templates/core_explore_keyword_app/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1702 2023-02-23 20:28:54.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/templates/core_explore_keyword_app/user/index.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:56.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/templates/core_explore_keyword_registry_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:56.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/templates/core_explore_keyword_registry_app/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      956 2023-02-23 20:28:54.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/templates/core_explore_keyword_registry_app/user/refinements.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:56.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/templatetags/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:54.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/templatetags/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1016 2023-02-23 20:28:54.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/templatetags/render_extras.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1446 2023-02-23 20:28:54.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:56.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:54.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:56.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:54.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    13020 2023-02-23 20:28:54.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/views/user/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1475 2023-02-23 20:28:54.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/views/user/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12589 2023-02-23 20:28:54.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/views/user/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:56.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1581 2023-02-23 20:28:55.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3033 2023-02-23 20:28:55.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-02-23 20:28:55.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      152 2023-02-23 20:28:55.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       40 2023-02-23 20:28:55.000000 core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-02-23 20:28:54.000000 core_explore_keyword_registry_app-2.2.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      200 2023-02-23 20:28:54.000000 core_explore_keyword_registry_app-2.2.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       26 2023-02-23 20:28:54.000000 core_explore_keyword_registry_app-2.2.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-02-23 20:28:56.000000 core_explore_keyword_registry_app-2.2.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1090 2023-02-23 20:28:54.000000 core_explore_keyword_registry_app-2.2.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:56.000000 core_explore_keyword_registry_app-2.2.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:54.000000 core_explore_keyword_registry_app-2.2.0/tests/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1793 2023-02-23 20:28:54.000000 core_explore_keyword_registry_app-2.2.0/tests/test_settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:56.000000 core_explore_keyword_registry_app-2.2.0/tests/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:54.000000 core_explore_keyword_registry_app-2.2.0/tests/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:56.000000 core_explore_keyword_registry_app-2.2.0/tests/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:54.000000 core_explore_keyword_registry_app-2.2.0/tests/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1113 2023-02-23 20:28:54.000000 core_explore_keyword_registry_app-2.2.0/tests/views/user/tests_views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:05.407371 core_explore_keyword_registry_app-2.3.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      199 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1581 2023-05-02 19:38:05.402353 core_explore_keyword_registry_app-2.3.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1042 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:04.789449 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      120 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      710 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/apps.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3508 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/discover.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:04.913045 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/permissions/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/permissions/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1063 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/permissions/discover.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      883 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:04.452353 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:04.524962 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:04.513929 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:04.481869 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/css/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:04.926033 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/css/fancytree/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      813 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/css/fancytree/fancytree.custom.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:04.952168 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/css/search/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      310 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/css/search/filters.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1016 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/css/search/search.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:04.505686 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:05.068055 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3328 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/fancytree.custom.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       76 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/fancytree.custom.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2544 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/filters.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9169 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/resource_type_icons_table.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      257 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/resource_type_icons_table.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      322 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/search.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      650 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/tagit.custom.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:04.517043 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/libs/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:04.520270 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/libs/jquery-shorten/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:05.081689 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/libs/jquery-shorten/1.1.0/
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     6230 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/libs/jquery-shorten/1.1.0/jquery.shorten.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:05.110719 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/xsl/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6809 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/xsl/registry-detail.xsl
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4178 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/xsl/registry-list.xsl
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:04.586551 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:04.569269 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/templates/core_explore_common_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:04.572379 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/templates/core_explore_common_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:05.136832 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/templates/core_explore_common_app/user/results/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      937 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/templates/core_explore_common_app/user/results/data_source_info.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      846 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/templates/core_explore_common_app/user/results/data_source_results.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:04.581165 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/templates/core_explore_keyword_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:05.152271 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/templates/core_explore_keyword_app/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1702 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/templates/core_explore_keyword_app/user/index.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:04.589716 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/templates/core_explore_keyword_registry_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:05.164869 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/templates/core_explore_keyword_registry_app/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      956 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/templates/core_explore_keyword_registry_app/user/refinements.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:05.199846 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/templatetags/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/templatetags/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1016 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/templatetags/render_extras.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1446 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:05.228426 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:05.287799 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12995 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/views/user/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1475 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/views/user/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12589 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/views/user/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:04.869855 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1581 2023-05-02 19:38:04.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3044 2023-05-02 19:38:04.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:38:04.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      152 2023-05-02 19:38:04.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       40 2023-05-02 19:38:04.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      200 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       26 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:38:05.409133 core_explore_keyword_registry_app-2.3.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1090 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:05.320713 core_explore_keyword_registry_app-2.3.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/tests/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1793 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:05.338430 core_explore_keyword_registry_app-2.3.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/tests/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:05.380801 core_explore_keyword_registry_app-2.3.0/tests/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/tests/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5093 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/tests/views/user/tests_views.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `core_explore_keyword_registry_app-2.2.0/PKG-INFO` & `core_explore_keyword_registry_app-2.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_explore_keyword_registry_app
-Version: 2.2.0
+Version: 2.3.0
 Summary: Exploration by keywords for the registry project
 Home-page: https://github.com/usnistgov/core_explore_keyword_registry_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =================================
         Core Explore Keyword Registry App
```

### Comparing `core_explore_keyword_registry_app-2.2.0/README.rst` & `core_explore_keyword_registry_app-2.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/apps.py` & `core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/apps.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/discover.py` & `core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/discover.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/permissions/discover.py` & `core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/permissions/discover.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/settings.py` & `core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/settings.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/css/fancytree/fancytree.custom.css` & `core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/css/fancytree/fancytree.custom.css`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/css/search/search.css` & `core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/css/search/search.css`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/fancytree.custom.js` & `core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/fancytree.custom.js`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/filters.js` & `core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/filters.js`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/resource_type_icons_table.js` & `core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/resource_type_icons_table.js`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/tagit.custom.js` & `core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/tagit.custom.js`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/libs/jquery-shorten/1.1.0/jquery.shorten.js` & `core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/libs/jquery-shorten/1.1.0/jquery.shorten.js`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/xsl/registry-detail.xsl` & `core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/xsl/registry-detail.xsl`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/xsl/registry-list.xsl` & `core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/xsl/registry-list.xsl`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/templates/core_explore_common_app/user/results/data_source_info.html` & `core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/templates/core_explore_common_app/user/results/data_source_info.html`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/templates/core_explore_common_app/user/results/data_source_results.html` & `core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/templates/core_explore_common_app/user/results/data_source_results.html`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/templates/core_explore_keyword_app/user/index.html` & `core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/templates/core_explore_keyword_app/user/index.html`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/templates/core_explore_keyword_registry_app/user/refinements.html` & `core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/templates/core_explore_keyword_registry_app/user/refinements.html`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/templatetags/render_extras.py` & `core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/templatetags/render_extras.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/urls.py` & `core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/urls.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/views/user/ajax.py` & `core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/views/user/ajax.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,23 +4,26 @@
 import json
 import re
 from collections import defaultdict, deque
 from itertools import groupby
 from logging import getLogger
 
 from django.http import HttpResponse, HttpResponseBadRequest
-from django.urls import reverse
 from django.utils.html import escape
 from django.views.generic import View
 
 from core_explore_common_app.components.query import api as query_api
-from core_explore_common_app.constants import LOCAL_QUERY_NAME
+from core_explore_common_app.utils.oaipmh import oaipmh as oaipmh_utils
+from core_explore_common_app.utils.query import query as query_utils
 from core_explore_keyword_app.views.user.ajax import (
     SuggestionsKeywordSearchView,
 )
+from core_explore_keyword_registry_app.views.user.views import (
+    update_content_not_deleted_status_criteria,
+)
 from core_main_app.rest.data.views import ExecuteLocalQueryView
 from core_main_app.settings import MONGODB_INDEXING
 from core_main_registry_app.components.category import api as category_api
 from core_main_registry_app.components.refinement import api as refinement_api
 from core_main_registry_app.components.template import (
     api as template_registry_api,
 )
@@ -33,17 +36,15 @@
 )
 
 if MONGODB_INDEXING:
     from core_main_app.components.mongo import api as main_mongo_api
     from core_oaipmh_harvester_app.components.mongo import (
         api as oai_harvester_mongo_api,
     )
-from core_explore_keyword_registry_app.views.user.views import (
-    update_content_not_deleted_status_criteria,
-)
+
 
 logger = getLogger(__name__)
 
 
 class SuggestionsKeywordRegistrySearchView(SuggestionsKeywordSearchView):
     """Suggestions Keyword Registry Search View"""
 
@@ -142,21 +143,19 @@
             categories = category_api.get_all().filter(refinement=refinement)
             # Prepare pipeline
             self._prepare_pipeline_categories(categories)
             # Only selected data provider
             # FIXME: Decouple data source.
             for data_source in self.query.data_sources:
                 # find local data source
-                if data_source["name"] == LOCAL_QUERY_NAME:
+                if query_utils.is_local_data_source(data_source):
                     self._get_local_data(data_source, data_sources_res)
 
                 # OAI-PMH
-                elif data_source["url_query"].endswith(
-                    reverse("core_explore_oaipmh_rest_execute_query")
-                ):
+                elif oaipmh_utils.is_oai_data_source(data_source):
                     self._get_oai_data(data_source, data_sources_res)
                 # Not supported
                 else:
                     logger.info(
                         "No treatment available for the data source %s, "
                         "%s. Counters will not take into account this data "
                         "source.",
```

### Comparing `core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/views/user/forms.py` & `core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/views/user/forms.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app/views/user/views.py` & `core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/views/user/views.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app.egg-info/PKG-INFO` & `core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-explore-keyword-registry-app
-Version: 2.2.0
+Version: 2.3.0
 Summary: Exploration by keywords for the registry project
 Home-page: https://github.com/usnistgov/core_explore_keyword_registry_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =================================
         Core Explore Keyword Registry App
```

### Comparing `core_explore_keyword_registry_app-2.2.0/core_explore_keyword_registry_app.egg-info/SOURCES.txt` & `core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app.egg-info/SOURCES.txt`

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
 core_explore_keyword_registry_app/__init__.py
```

### Comparing `core_explore_keyword_registry_app-2.2.0/setup.py` & `core_explore_keyword_registry_app-2.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_explore_keyword_registry_app",
-    version="2.2.0",
+    version="2.3.0",
     description="Exploration by keywords for the registry project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_explore_keyword_registry_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_explore_keyword_registry_app-2.2.0/tests/test_settings.py` & `core_explore_keyword_registry_app-2.3.0/tests/test_settings.py`

 * *Files identical despite different names*

