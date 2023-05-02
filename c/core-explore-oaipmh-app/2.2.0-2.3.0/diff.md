# Comparing `tmp/core_explore_oaipmh_app-2.2.0.tar.gz` & `tmp/core_explore_oaipmh_app-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/core_explore_oaipmh_app-2.2.0.tar", last modified: Thu Feb 23 20:29:07 2023, max compression
+gzip compressed data, was "core_explore_oaipmh_app-2.3.0.tar", last modified: Tue May  2 19:38:18 2023, max compression
```

## Comparing `core_explore_oaipmh_app-2.2.0.tar` & `core_explore_oaipmh_app-2.3.0.tar`

### file list

```diff
@@ -1,78 +1,79 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:07.000000 core_explore_oaipmh_app-2.2.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      154 2023-02-23 20:29:03.000000 core_explore_oaipmh_app-2.2.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1428 2023-02-23 20:29:07.000000 core_explore_oaipmh_app-2.2.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      855 2023-02-23 20:29:03.000000 core_explore_oaipmh_app-2.2.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:06.000000 core_explore_oaipmh_app-2.2.0/core_explore_oaipmh_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:03.000000 core_explore_oaipmh_app-2.2.0/core_explore_oaipmh_app/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:06.000000 core_explore_oaipmh_app-2.2.0/core_explore_oaipmh_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:03.000000 core_explore_oaipmh_app-2.2.0/core_explore_oaipmh_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:06.000000 core_explore_oaipmh_app-2.2.0/core_explore_oaipmh_app/components/query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:03.000000 core_explore_oaipmh_app-2.2.0/core_explore_oaipmh_app/components/query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1710 2023-02-23 20:29:03.000000 core_explore_oaipmh_app-2.2.0/core_explore_oaipmh_app/components/query/api.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:06.000000 core_explore_oaipmh_app-2.2.0/core_explore_oaipmh_app/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:03.000000 core_explore_oaipmh_app-2.2.0/core_explore_oaipmh_app/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:06.000000 core_explore_oaipmh_app-2.2.0/core_explore_oaipmh_app/rest/query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:03.000000 core_explore_oaipmh_app-2.2.0/core_explore_oaipmh_app/rest/query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3737 2023-02-23 20:29:03.000000 core_explore_oaipmh_app-2.2.0/core_explore_oaipmh_app/rest/query/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:06.000000 core_explore_oaipmh_app-2.2.0/core_explore_oaipmh_app/rest/result/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:03.000000 core_explore_oaipmh_app-2.2.0/core_explore_oaipmh_app/rest/result/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1755 2023-02-23 20:29:03.000000 core_explore_oaipmh_app-2.2.0/core_explore_oaipmh_app/rest/result/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      531 2023-02-23 20:29:03.000000 core_explore_oaipmh_app-2.2.0/core_explore_oaipmh_app/rest/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      333 2023-02-23 20:29:03.000000 core_explore_oaipmh_app-2.2.0/core_explore_oaipmh_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:06.000000 core_explore_oaipmh_app-2.2.0/core_explore_oaipmh_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:06.000000 core_explore_oaipmh_app-2.2.0/core_explore_oaipmh_app/static/core_explore_oaipmh_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:06.000000 core_explore_oaipmh_app-2.2.0/core_explore_oaipmh_app/static/core_explore_oaipmh_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:06.000000 core_explore_oaipmh_app-2.2.0/core_explore_oaipmh_app/static/core_explore_oaipmh_app/user/js/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:06.000000 core_explore_oaipmh_app-2.2.0/core_explore_oaipmh_app/static/core_explore_oaipmh_app/user/js/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      127 2023-02-23 20:29:04.000000 core_explore_oaipmh_app-2.2.0/core_explore_oaipmh_app/static/core_explore_oaipmh_app/user/js/data/change_display.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:06.000000 core_explore_oaipmh_app-2.2.0/core_explore_oaipmh_app/static/core_explore_oaipmh_app/user/js/data_sources/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2332 2023-02-23 20:29:04.000000 core_explore_oaipmh_app-2.2.0/core_explore_oaipmh_app/static/core_explore_oaipmh_app/user/js/data_sources/list.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:06.000000 core_explore_oaipmh_app-2.2.0/core_explore_oaipmh_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:06.000000 core_explore_oaipmh_app-2.2.0/core_explore_oaipmh_app/templates/core_explore_oaipmh_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:06.000000 core_explore_oaipmh_app-2.2.0/core_explore_oaipmh_app/templates/core_explore_oaipmh_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:06.000000 core_explore_oaipmh_app-2.2.0/core_explore_oaipmh_app/templates/core_explore_oaipmh_app/user/data_sources/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      673 2023-02-23 20:29:04.000000 core_explore_oaipmh_app-2.2.0/core_explore_oaipmh_app/templates/core_explore_oaipmh_app/user/data_sources/list-content.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1054 2023-02-23 20:29:04.000000 core_explore_oaipmh_app-2.2.0/core_explore_oaipmh_app/templates/core_explore_oaipmh_app/user/data_sources/list.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      934 2023-02-23 20:29:04.000000 core_explore_oaipmh_app-2.2.0/core_explore_oaipmh_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:06.000000 core_explore_oaipmh_app-2.2.0/core_explore_oaipmh_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:04.000000 core_explore_oaipmh_app-2.2.0/core_explore_oaipmh_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:07.000000 core_explore_oaipmh_app-2.2.0/core_explore_oaipmh_app/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:04.000000 core_explore_oaipmh_app-2.2.0/core_explore_oaipmh_app/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6437 2023-02-23 20:29:04.000000 core_explore_oaipmh_app-2.2.0/core_explore_oaipmh_app/views/user/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1871 2023-02-23 20:29:04.000000 core_explore_oaipmh_app-2.2.0/core_explore_oaipmh_app/views/user/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:06.000000 core_explore_oaipmh_app-2.2.0/core_explore_oaipmh_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1428 2023-02-23 20:29:06.000000 core_explore_oaipmh_app-2.2.0/core_explore_oaipmh_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1864 2023-02-23 20:29:06.000000 core_explore_oaipmh_app-2.2.0/core_explore_oaipmh_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-02-23 20:29:06.000000 core_explore_oaipmh_app-2.2.0/core_explore_oaipmh_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      147 2023-02-23 20:29:06.000000 core_explore_oaipmh_app-2.2.0/core_explore_oaipmh_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       30 2023-02-23 20:29:06.000000 core_explore_oaipmh_app-2.2.0/core_explore_oaipmh_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-02-23 20:29:04.000000 core_explore_oaipmh_app-2.2.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      115 2023-02-23 20:29:04.000000 core_explore_oaipmh_app-2.2.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-02-23 20:29:07.000000 core_explore_oaipmh_app-2.2.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1079 2023-02-23 20:29:04.000000 core_explore_oaipmh_app-2.2.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:07.000000 core_explore_oaipmh_app-2.2.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:04.000000 core_explore_oaipmh_app-2.2.0/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:07.000000 core_explore_oaipmh_app-2.2.0/tests/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:04.000000 core_explore_oaipmh_app-2.2.0/tests/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6073 2023-02-23 20:29:04.000000 core_explore_oaipmh_app-2.2.0/tests/fixtures/fixtures.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:07.000000 core_explore_oaipmh_app-2.2.0/tests/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:04.000000 core_explore_oaipmh_app-2.2.0/tests/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:07.000000 core_explore_oaipmh_app-2.2.0/tests/rest/query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:04.000000 core_explore_oaipmh_app-2.2.0/tests/rest/query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4647 2023-02-23 20:29:04.000000 core_explore_oaipmh_app-2.2.0/tests/rest/query/tests_permissions.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:07.000000 core_explore_oaipmh_app-2.2.0/tests/rest/result/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:04.000000 core_explore_oaipmh_app-2.2.0/tests/rest/result/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2845 2023-02-23 20:29:04.000000 core_explore_oaipmh_app-2.2.0/tests/rest/result/tests_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2127 2023-02-23 20:29:04.000000 core_explore_oaipmh_app-2.2.0/tests/test_settings.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      376 2023-02-23 20:29:04.000000 core_explore_oaipmh_app-2.2.0/tests/test_urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:07.000000 core_explore_oaipmh_app-2.2.0/tests/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:04.000000 core_explore_oaipmh_app-2.2.0/tests/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:07.000000 core_explore_oaipmh_app-2.2.0/tests/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:04.000000 core_explore_oaipmh_app-2.2.0/tests/views/user/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:07.000000 core_explore_oaipmh_app-2.2.0/tests/views/user/ajax/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:04.000000 core_explore_oaipmh_app-2.2.0/tests/views/user/ajax/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2234 2023-02-23 20:29:04.000000 core_explore_oaipmh_app-2.2.0/tests/views/user/ajax/tests_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    15234 2023-02-23 20:29:04.000000 core_explore_oaipmh_app-2.2.0/tests/views/user/ajax/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:07.000000 core_explore_oaipmh_app-2.2.0/tests/views/user/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:04.000000 core_explore_oaipmh_app-2.2.0/tests/views/user/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5482 2023-02-23 20:29:04.000000 core_explore_oaipmh_app-2.2.0/tests/views/user/views/tests_permissions.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:18.083128 core_explore_oaipmh_app-2.3.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:38:14.000000 core_explore_oaipmh_app-2.3.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      154 2023-05-02 19:38:14.000000 core_explore_oaipmh_app-2.3.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1428 2023-05-02 19:38:18.077890 core_explore_oaipmh_app-2.3.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      855 2023-05-02 19:38:14.000000 core_explore_oaipmh_app-2.3.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:17.535774 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:14.000000 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:17.620706 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:14.000000 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:17.641613 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/components/query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:14.000000 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/components/query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1713 2023-05-02 19:38:14.000000 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/components/query/api.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:17.660753 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:14.000000 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:17.678993 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/rest/query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:14.000000 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/rest/query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6516 2023-05-02 19:38:14.000000 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/rest/query/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:17.698221 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/rest/result/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:14.000000 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/rest/result/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1755 2023-05-02 19:38:14.000000 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/rest/result/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      313 2023-05-02 19:38:14.000000 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/rest/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      333 2023-05-02 19:38:14.000000 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:17.322252 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:17.325724 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/static/core_explore_oaipmh_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:17.328632 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/static/core_explore_oaipmh_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:17.335495 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/static/core_explore_oaipmh_app/user/js/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:17.709356 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/static/core_explore_oaipmh_app/user/js/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      127 2023-05-02 19:38:14.000000 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/static/core_explore_oaipmh_app/user/js/data/change_display.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:17.719789 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/static/core_explore_oaipmh_app/user/js/data_sources/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2332 2023-05-02 19:38:14.000000 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/static/core_explore_oaipmh_app/user/js/data_sources/list.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:17.346964 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:17.349990 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/templates/core_explore_oaipmh_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:17.353584 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/templates/core_explore_oaipmh_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:17.745564 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/templates/core_explore_oaipmh_app/user/data_sources/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      673 2023-05-02 19:38:14.000000 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/templates/core_explore_oaipmh_app/user/data_sources/list-content.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1054 2023-05-02 19:38:14.000000 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/templates/core_explore_oaipmh_app/user/data_sources/list.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      934 2023-05-02 19:38:14.000000 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:17.758027 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:14.000000 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:17.798950 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:14.000000 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5958 2023-05-02 19:38:14.000000 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/views/user/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1871 2023-05-02 19:38:14.000000 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/views/user/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:17.583092 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1428 2023-05-02 19:38:16.000000 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1868 2023-05-02 19:38:17.000000 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:38:16.000000 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      147 2023-05-02 19:38:16.000000 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       30 2023-05-02 19:38:16.000000 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:38:15.000000 core_explore_oaipmh_app-2.3.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      115 2023-05-02 19:38:15.000000 core_explore_oaipmh_app-2.3.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:38:18.085201 core_explore_oaipmh_app-2.3.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1079 2023-05-02 19:38:15.000000 core_explore_oaipmh_app-2.3.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:17.835550 core_explore_oaipmh_app-2.3.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:15.000000 core_explore_oaipmh_app-2.3.0/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:17.861446 core_explore_oaipmh_app-2.3.0/tests/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:15.000000 core_explore_oaipmh_app-2.3.0/tests/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6073 2023-05-02 19:38:15.000000 core_explore_oaipmh_app-2.3.0/tests/fixtures/fixtures.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:17.874413 core_explore_oaipmh_app-2.3.0/tests/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:15.000000 core_explore_oaipmh_app-2.3.0/tests/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:17.907399 core_explore_oaipmh_app-2.3.0/tests/rest/query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:15.000000 core_explore_oaipmh_app-2.3.0/tests/rest/query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7300 2023-05-02 19:38:15.000000 core_explore_oaipmh_app-2.3.0/tests/rest/query/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:17.934951 core_explore_oaipmh_app-2.3.0/tests/rest/result/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:15.000000 core_explore_oaipmh_app-2.3.0/tests/rest/result/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2845 2023-05-02 19:38:15.000000 core_explore_oaipmh_app-2.3.0/tests/rest/result/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2157 2023-05-02 19:38:15.000000 core_explore_oaipmh_app-2.3.0/tests/test_settings.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      316 2023-05-02 19:38:15.000000 core_explore_oaipmh_app-2.3.0/tests/test_urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:17.973178 core_explore_oaipmh_app-2.3.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:15.000000 core_explore_oaipmh_app-2.3.0/tests/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:17.993300 core_explore_oaipmh_app-2.3.0/tests/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:15.000000 core_explore_oaipmh_app-2.3.0/tests/views/user/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:18.036538 core_explore_oaipmh_app-2.3.0/tests/views/user/ajax/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:15.000000 core_explore_oaipmh_app-2.3.0/tests/views/user/ajax/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2219 2023-05-02 19:38:15.000000 core_explore_oaipmh_app-2.3.0/tests/views/user/ajax/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14034 2023-05-02 19:38:15.000000 core_explore_oaipmh_app-2.3.0/tests/views/user/ajax/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:18.068621 core_explore_oaipmh_app-2.3.0/tests/views/user/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:15.000000 core_explore_oaipmh_app-2.3.0/tests/views/user/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5472 2023-05-02 19:38:15.000000 core_explore_oaipmh_app-2.3.0/tests/views/user/views/tests_permissions.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `core_explore_oaipmh_app-2.2.0/PKG-INFO` & `core_explore_oaipmh_app-2.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_explore_oaipmh_app
-Version: 2.2.0
+Version: 2.3.0
 Summary: OAI-PMH exploration functions for curator core project
 Home-page: https://github.com/usnistgov/core_explore_oaipmh_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =======================
         Core Explore Oaipmh App
```

### Comparing `core_explore_oaipmh_app-2.2.0/README.rst` & `core_explore_oaipmh_app-2.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_explore_oaipmh_app-2.2.0/core_explore_oaipmh_app/components/query/api.py` & `core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/components/query/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     # the unique identifier for an oaipmh data source is its instance_id
     # because there is no constraint on the name
     data_source_found = False
     for data_source_item in query.data_sources:
         if (
             "instance_id" in data_source_item["query_options"]
             and data_source_item["query_options"]["instance_id"]
-            == data_source.query_options["instance_id"]
+            == data_source["query_options"]["instance_id"]
         ):
             data_source_found = True
 
     if not data_source_found:
         # add data source to query if not present
         query.data_sources.append(data_source)
         # update query
```

### Comparing `core_explore_oaipmh_app-2.2.0/core_explore_oaipmh_app/rest/result/views.py` & `core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/rest/result/views.py`

 * *Files identical despite different names*

### Comparing `core_explore_oaipmh_app-2.2.0/core_explore_oaipmh_app/static/core_explore_oaipmh_app/user/js/data_sources/list.js` & `core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/static/core_explore_oaipmh_app/user/js/data_sources/list.js`

 * *Files identical despite different names*

### Comparing `core_explore_oaipmh_app-2.2.0/core_explore_oaipmh_app/templates/core_explore_oaipmh_app/user/data_sources/list-content.html` & `core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/templates/core_explore_oaipmh_app/user/data_sources/list-content.html`

 * *Files identical despite different names*

### Comparing `core_explore_oaipmh_app-2.2.0/core_explore_oaipmh_app/templates/core_explore_oaipmh_app/user/data_sources/list.html` & `core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/templates/core_explore_oaipmh_app/user/data_sources/list.html`

 * *Files identical despite different names*

### Comparing `core_explore_oaipmh_app-2.2.0/core_explore_oaipmh_app/urls.py` & `core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/urls.py`

 * *Files identical despite different names*

### Comparing `core_explore_oaipmh_app-2.2.0/core_explore_oaipmh_app/views/user/ajax.py` & `core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/views/user/ajax.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 """ Ajax User core explore OAI-PMH
 """
 import json
 
 from django.http import HttpResponseForbidden
 from django.http.response import HttpResponseBadRequest, HttpResponse
 from django.shortcuts import render
-from django.urls import reverse
 from django.utils.html import escape
 
-from core_main_app.access_control.exceptions import AccessControlError
-from core_main_app.settings import DATA_SORTING_FIELDS
 import core_explore_common_app.components.query.api as api_query
 from core_explore_common_app.components.abstract_query.models import (
     Authentication,
     DataSource,
 )
+from core_explore_oaipmh_app.components.query import api as oaipmh_query_api
+from core_main_app.access_control.exceptions import AccessControlError
+from core_main_app.settings import DATA_SORTING_FIELDS, SERVER_URI
 from core_main_app.templatetags.xsl_transform_tag import (
     render_xml_as_html_detail,
 )
 from core_oaipmh_harvester_app.components.oai_record import (
     api as oai_record_api,
 )
 from core_oaipmh_harvester_app.components.oai_registry import (
     api as oai_registry_api,
 )
-from core_explore_oaipmh_app import settings
-from core_explore_oaipmh_app.components.query import api as oaipmh_query_api
 
 
 def get_data_source_list_oaipmh(request):
     """Ajax method to fill the list of data sources.
 
     Args:
         request:
@@ -114,36 +112,26 @@
         # Get query from id
         if id_query is None:
             return HttpResponseBadRequest(
                 "Error during data source selection."
             )
 
         query = api_query.get_by_id(id_query, request.user)
-        url_instance = request.build_absolute_uri(
-            reverse("core_explore_oaipmh_rest_execute_query")
-        )
         instance = oai_registry_api.get_by_id(id_instance)
         if to_be_added:
             # Instance have to be added in the query as a data source
             authentication = Authentication(auth_type="session")
             data_source = DataSource(
                 name=instance.name,
-                url_query=url_instance,
+                url_query=SERVER_URI,
                 authentication=authentication,
                 order_by_field=",".join(DATA_SORTING_FIELDS),
                 query_options={"instance_id": str(instance.id)},
             )
 
-            if "core_linked_records_app" in settings.INSTALLED_APPS:
-                data_source["capabilities"] = {
-                    "url_pid": request.build_absolute_uri(
-                        reverse("core_linked_records_app_query_oaipmh")
-                    )
-                }
-
             oaipmh_query_api.add_oaipmh_data_source(
                 query, data_source, request.user
             )
         else:
             oaipmh_query_api.remove_oaipmh_data_source(
                 query, id_instance, request.user
             )
```

### Comparing `core_explore_oaipmh_app-2.2.0/core_explore_oaipmh_app/views/user/views.py` & `core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/views/user/views.py`

 * *Files identical despite different names*

### Comparing `core_explore_oaipmh_app-2.2.0/core_explore_oaipmh_app.egg-info/PKG-INFO` & `core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-explore-oaipmh-app
-Version: 2.2.0
+Version: 2.3.0
 Summary: OAI-PMH exploration functions for curator core project
 Home-page: https://github.com/usnistgov/core_explore_oaipmh_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =======================
         Core Explore Oaipmh App
```

### Comparing `core_explore_oaipmh_app-2.2.0/core_explore_oaipmh_app.egg-info/SOURCES.txt` & `core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.md
 MANIFEST.in
 README.rst
 pyproject.toml
 requirements.core.txt
 setup.py
 core_explore_oaipmh_app/__init__.py
 core_explore_oaipmh_app/settings.py
@@ -31,15 +32,15 @@
 tests/__init__.py
 tests/test_settings.py
 tests/test_urls.py
 tests/fixtures/__init__.py
 tests/fixtures/fixtures.py
 tests/rest/__init__.py
 tests/rest/query/__init__.py
-tests/rest/query/tests_permissions.py
+tests/rest/query/tests_unit.py
 tests/rest/result/__init__.py
 tests/rest/result/tests_permissions.py
 tests/views/__init__.py
 tests/views/user/__init__.py
 tests/views/user/ajax/__init__.py
 tests/views/user/ajax/tests_permissions.py
 tests/views/user/ajax/tests_unit.py
```

### Comparing `core_explore_oaipmh_app-2.2.0/setup.py` & `core_explore_oaipmh_app-2.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_explore_oaipmh_app",
-    version="2.2.0",
+    version="2.3.0",
     description="OAI-PMH exploration functions for curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_explore_oaipmh_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_explore_oaipmh_app-2.2.0/tests/fixtures/fixtures.py` & `core_explore_oaipmh_app-2.3.0/tests/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_explore_oaipmh_app-2.2.0/tests/rest/result/tests_permissions.py` & `core_explore_oaipmh_app-2.3.0/tests/rest/result/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_explore_oaipmh_app-2.2.0/tests/test_settings.py` & `core_explore_oaipmh_app-2.3.0/tests/test_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,7 +78,8 @@
 DEFAULT_AUTO_FIELD = "django.db.models.BigAutoField"
 CELERYBEAT_SCHEDULER = "django_celery_beat.schedulers:DatabaseScheduler"
 
 AUTO_SET_PID = False
 
 MONGODB_INDEXING = False
 MONGODB_ASYNC_SAVE = False
+ENABLE_SAML2_SSO_AUTH = False
```

### Comparing `core_explore_oaipmh_app-2.2.0/tests/views/user/ajax/tests_permissions.py` & `core_explore_oaipmh_app-2.3.0/tests/views/user/ajax/tests_permissions.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 from django.test import RequestFactory
 
 from core_explore_oaipmh_app.views.user.ajax import (
     get_data_source_list_oaipmh,
     update_data_source_list_oaipmh,
 )
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from tests.fixtures.fixtures import AccessControlDataFixture
 
 
-class TestGetDataSourceListOaipmh(MongoIntegrationBaseTestCase):
+class TestGetDataSourceListOaipmh(IntegrationBaseTestCase):
     """Test Get Data Source List Oaipmh"""
 
     def setUp(self):
         """setUp"""
 
         self.factory = RequestFactory()
         self.user1 = create_mock_user(user_id="1")
@@ -33,15 +33,15 @@
         request = self.factory.get("core_explore_oaipmh_app_get_data_sources")
         request.user = self.anonymous
         request.GET = {"id_query": str(self.fixture.query_user1.id)}
         response = get_data_source_list_oaipmh(request)
         self.assertEqual(response.status_code, 403)
 
 
-class TestUpdateDataSourceListOaipmh(MongoIntegrationBaseTestCase):
+class TestUpdateDataSourceListOaipmh(IntegrationBaseTestCase):
     """Test Update Data Source List Oaipmh"""
 
     def setUp(self):
         """setUp"""
 
         self.factory = RequestFactory()
         self.user1 = create_mock_user(user_id="1")
```

### Comparing `core_explore_oaipmh_app-2.2.0/tests/views/user/ajax/tests_unit.py` & `core_explore_oaipmh_app-2.3.0/tests/views/user/ajax/tests_unit.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 )
 from core_main_app.components.template.models import Template
 from core_oaipmh_harvester_app.components.oai_record.models import OaiRecord
 from core_oaipmh_harvester_app.components.oai_harvester_metadata_format.models import (
     OaiHarvesterMetadataFormat,
 )
 from core_main_app.access_control.exceptions import AccessControlError
-from core_main_app.settings import DATA_SORTING_FIELDS
+from core_main_app.settings import DATA_SORTING_FIELDS, SERVER_URI
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from core_main_app.templatetags.xsl_transform_tag import (
     _render_xml_as_html,
 )
 
 
 class TestUpdateDataSourceListOaipmh(TestCase):
@@ -135,84 +135,73 @@
         self._send_request(
             {"id_query": "mock_id_query", "to_be_added": "true"}
         )
         mock_add_oaipmh_data_source.assert_called_with(
             "mock_query",
             {
                 "name": mock_oai_registry.name,
-                "url_query": mock_url_instance,
+                "url_query": SERVER_URI,
                 "authentication": {"auth_type": "session", "params": {}},
                 "order_by_field": ",".join(DATA_SORTING_FIELDS),
                 "query_options": {"instance_id": str(mock_oai_registry.id)},
-                "capabilities": {"url_pid": "mock_url_instance"},
+                "capabilities": {},
             },
             self.user,
         )
 
-    @patch("core_explore_oaipmh_app.views.user.ajax.settings.INSTALLED_APPS")
     @patch(
         "core_explore_oaipmh_app.views.user.ajax.oaipmh_query_api.add_oaipmh_data_source"
     )
     @patch(
         "core_explore_oaipmh_app.views.user.ajax.oai_registry_api.get_by_id"
     )
-    @patch("django.http.HttpRequest.build_absolute_uri")
     @patch("core_explore_oaipmh_app.views.user.ajax.api_query.get_by_id")
     def test_data_source_capabilities_empty_when_linked_records_not_installed(
         self,
         mock_query_get_by_id,
-        mock_build_absolute_uri,
         mock_oai_registry_get_by_id,
         mock_add_oaipmh_data_source,
-        mock_installed_apps,
     ):
         """test_data_source_capabilities_empty_when_linked_records_not_installed"""
         mock_oai_registry = MagicMock()
-        mock_url_instance = "mock_url_instance"
         mock_query_get_by_id.return_value = "mock_query"
-        mock_build_absolute_uri.return_value = mock_url_instance
         mock_oai_registry_get_by_id.return_value = mock_oai_registry
-        mock_installed_apps.return_value = []
 
         self._send_request(
             {"id_query": "mock_id_query", "to_be_added": "true"}
         )
         mock_add_oaipmh_data_source.assert_called_with(
             "mock_query",
             {
                 "name": mock_oai_registry.name,
-                "url_query": mock_url_instance,
+                "url_query": SERVER_URI,
                 "authentication": {"auth_type": "session", "params": {}},
                 "order_by_field": ",".join(DATA_SORTING_FIELDS),
                 "query_options": {"instance_id": str(mock_oai_registry.id)},
                 "capabilities": {},
             },
             self.user,
         )
 
     @patch(
         "core_explore_oaipmh_app.views.user.ajax.oaipmh_query_api.add_oaipmh_data_source"
     )
     @patch(
         "core_explore_oaipmh_app.views.user.ajax.oai_registry_api.get_by_id"
     )
-    @patch("django.http.HttpRequest.build_absolute_uri")
     @patch("core_explore_oaipmh_app.views.user.ajax.api_query.get_by_id")
     def test_add_oaipmh_data_source_fails_returns_400(
         self,
         mock_query_get_by_id,
-        mock_build_absolute_uri,
         mock_oai_registry_get_by_id,
         mock_add_oaipmh_data_source,
     ):
         """test_add_oaipmh_data_source_fails_returns_400"""
         mock_oai_registry = MagicMock()
-        mock_url_instance = "mock_url_instance"
         mock_query_get_by_id.return_value = "mock_query"
-        mock_build_absolute_uri.return_value = mock_url_instance
         mock_oai_registry_get_by_id.return_value = mock_oai_registry
         mock_add_oaipmh_data_source.side_effect = Exception(
             "mock_add_oaipmh_data_source_exception"
         )
 
         self.assertEquals(
             self._send_request(
@@ -223,28 +212,24 @@
 
     @patch(
         "core_explore_oaipmh_app.views.user.ajax.oaipmh_query_api.remove_oaipmh_data_source"
     )
     @patch(
         "core_explore_oaipmh_app.views.user.ajax.oai_registry_api.get_by_id"
     )
-    @patch("django.http.HttpRequest.build_absolute_uri")
     @patch("core_explore_oaipmh_app.views.user.ajax.api_query.get_by_id")
     def test_remove_oaipmh_data_source_called_when_not_to_be_added(
         self,
         mock_query_get_by_id,
-        mock_build_absolute_uri,
         mock_oai_registry_get_by_id,
         mock_remove_oaipmh_data_source,
     ):
         """test_remove_oaipmh_data_source_called_when_not_to_be_added"""
         mock_oai_registry = MagicMock()
-        mock_url_instance = "mock_url_instance"
         mock_query_get_by_id.return_value = "mock_query"
-        mock_build_absolute_uri.return_value = mock_url_instance
         mock_oai_registry_get_by_id.return_value = mock_oai_registry
 
         self._send_request(
             {"id_query": "mock_id_query", "to_be_added": "false"}
         )
         mock_remove_oaipmh_data_source.assert_called_with(
             "mock_query",
@@ -254,29 +239,25 @@
 
     @patch(
         "core_explore_oaipmh_app.views.user.ajax.oaipmh_query_api.remove_oaipmh_data_source"
     )
     @patch(
         "core_explore_oaipmh_app.views.user.ajax.oai_registry_api.get_by_id"
     )
-    @patch("django.http.HttpRequest.build_absolute_uri")
     @patch("core_explore_oaipmh_app.views.user.ajax.api_query.get_by_id")
     def test_remove_oaipmh_data_source_fails_returns_400(
         self,
         mock_query_get_by_id,
-        mock_build_absolute_uri,
         mock_oai_registry_get_by_id,
         mock_remove_oaipmh_data_source,
     ):
         """test_remove_oaipmh_data_source_fails_returns_400"""
 
         mock_oai_registry = MagicMock()
-        mock_url_instance = "mock_url_instance"
         mock_query_get_by_id.return_value = "mock_query"
-        mock_build_absolute_uri.return_value = mock_url_instance
         mock_oai_registry_get_by_id.return_value = mock_oai_registry
         mock_remove_oaipmh_data_source.side_effect = Exception(
             "mock_remove_oaipmh_data_source_exception"
         )
 
         self.assertEquals(
             self._send_request(
@@ -287,29 +268,25 @@
 
     @patch(
         "core_explore_oaipmh_app.views.user.ajax.oaipmh_query_api.remove_oaipmh_data_source"
     )
     @patch(
         "core_explore_oaipmh_app.views.user.ajax.oai_registry_api.get_by_id"
     )
-    @patch("django.http.HttpRequest.build_absolute_uri")
     @patch("core_explore_oaipmh_app.views.user.ajax.api_query.get_by_id")
     def test_success_returns_200(
         self,
         mock_query_get_by_id,
-        mock_build_absolute_uri,
         mock_oai_registry_get_by_id,
         mock_remove_oaipmh_data_source,
     ):
         """test_success_returns_200"""
 
         mock_oai_registry = MagicMock()
-        mock_url_instance = "mock_url_instance"
         mock_query_get_by_id.return_value = "mock_query"
-        mock_build_absolute_uri.return_value = mock_url_instance
         mock_oai_registry_get_by_id.return_value = mock_oai_registry
         mock_remove_oaipmh_data_source.return_value = None
 
         self.assertEquals(
             self._send_request(
                 {"id_query": "mock_id_query", "to_be_added": "false"}
             ).status_code,
```

### Comparing `core_explore_oaipmh_app-2.2.0/tests/views/user/views/tests_permissions.py` & `core_explore_oaipmh_app-2.3.0/tests/views/user/views/tests_permissions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """ Permission tests on views
 """
 from django.test import RequestFactory, override_settings
 
 from core_explore_oaipmh_app.views.user.views import data_detail
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 from rest_framework import status
 from unittest.mock import patch
 from core_main_app.components.template.models import Template
 from core_oaipmh_harvester_app.components.oai_record.models import OaiRecord
 from core_oaipmh_harvester_app.components.oai_harvester_metadata_format.models import (
     OaiHarvesterMetadataFormat,
@@ -17,15 +17,15 @@
 from core_oaipmh_harvester_app.components.oai_registry.models import (
     OaiRegistry,
 )
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from tests.fixtures.fixtures import AccessControlDataFixture
 
 
-class TestViewData(MongoIntegrationBaseTestCase):
+class TestViewData(IntegrationBaseTestCase):
     """Test View Data"""
 
     def setUp(self):
         """setUp"""
 
         self.factory = RequestFactory()
         self.user1 = create_mock_user(user_id="1")
```

