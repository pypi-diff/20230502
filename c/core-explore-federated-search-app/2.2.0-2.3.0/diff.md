# Comparing `tmp/core_explore_federated_search_app-2.2.0.tar.gz` & `tmp/core_explore_federated_search_app-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/core_explore_federated_search_app-2.2.0.tar", last modified: Thu Feb 23 20:28:30 2023, max compression
+gzip compressed data, was "core_explore_federated_search_app-2.3.0.tar", last modified: Tue May  2 19:37:40 2023, max compression
```

## Comparing `core_explore_federated_search_app-2.2.0.tar` & `core_explore_federated_search_app-2.3.0.tar`

### file list

```diff
@@ -1,101 +1,102 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:30.000000 core_explore_federated_search_app-2.2.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      174 2023-02-23 20:28:26.000000 core_explore_federated_search_app-2.2.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1555 2023-02-23 20:28:30.000000 core_explore_federated_search_app-2.2.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      967 2023-02-23 20:28:26.000000 core_explore_federated_search_app-2.2.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:29.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:26.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:29.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:26.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:29.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/components/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:26.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/components/data/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      840 2023-02-23 20:28:26.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/components/data/api.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:29.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/migrations/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:26.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/migrations/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:29.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:26.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:29.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/rest/query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:26.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/rest/query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      354 2023-02-23 20:28:26.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/rest/query/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6626 2023-02-23 20:28:26.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/rest/query/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:29.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/rest/result/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:26.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/rest/result/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      303 2023-02-23 20:28:26.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/rest/result/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2758 2023-02-23 20:28:26.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/rest/result/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      571 2023-02-23 20:28:26.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/rest/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      637 2023-02-23 20:28:26.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:28.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:28.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/static/core_explore_federated_search_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:28.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:28.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:28.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:28.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:29.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      986 2023-02-23 20:28:26.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/delete.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      109 2023-02-23 20:28:26.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/delete.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1231 2023-02-23 20:28:26.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/edit.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      105 2023-02-23 20:28:26.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/edit.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1965 2023-02-23 20:28:26.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/refresh.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      107 2023-02-23 20:28:26.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/refresh.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:28.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/static/core_explore_federated_search_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:28.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/static/core_explore_federated_search_app/user/js/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:29.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/static/core_explore_federated_search_app/user/js/data_sources/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2419 2023-02-23 20:28:26.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/static/core_explore_federated_search_app/user/js/data_sources/list.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:28.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:28.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:28.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:29.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:29.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/add/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1013 2023-02-23 20:28:26.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/add/add_base.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      308 2023-02-23 20:28:26.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/add_repository.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:29.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2148 2023-02-23 20:28:26.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/list_base.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:29.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      722 2023-02-23 20:28:26.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/modals/delete.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1136 2023-02-23 20:28:26.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/modals/edit.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      875 2023-02-23 20:28:26.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/modals/refresh.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       18 2023-02-23 20:28:26.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/refresh_form.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      357 2023-02-23 20:28:26.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list_repositories.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:28.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:29.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/user/data_sources/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      663 2023-02-23 20:28:26.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/user/data_sources/list-content.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1104 2023-02-23 20:28:26.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/user/data_sources/list.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      857 2023-02-23 20:28:26.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:29.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:26.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:29.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:26.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5623 2023-02-23 20:28:26.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/views/user/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2710 2023-02-23 20:28:26.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/views/user/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:29.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1555 2023-02-23 20:28:28.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3818 2023-02-23 20:28:28.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-02-23 20:28:28.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      117 2023-02-23 20:28:28.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       40 2023-02-23 20:28:28.000000 core_explore_federated_search_app-2.2.0/core_explore_federated_search_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-02-23 20:28:26.000000 core_explore_federated_search_app-2.2.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       85 2023-02-23 20:28:26.000000 core_explore_federated_search_app-2.2.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-02-23 20:28:30.000000 core_explore_federated_search_app-2.2.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1114 2023-02-23 20:28:26.000000 core_explore_federated_search_app-2.2.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:29.000000 core_explore_federated_search_app-2.2.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:26.000000 core_explore_federated_search_app-2.2.0/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:29.000000 core_explore_federated_search_app-2.2.0/tests/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:26.000000 core_explore_federated_search_app-2.2.0/tests/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:29.000000 core_explore_federated_search_app-2.2.0/tests/components/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:26.000000 core_explore_federated_search_app-2.2.0/tests/components/data/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1083 2023-02-23 20:28:26.000000 core_explore_federated_search_app-2.2.0/tests/components/data/tests_int_access_control.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:29.000000 core_explore_federated_search_app-2.2.0/tests/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:26.000000 core_explore_federated_search_app-2.2.0/tests/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3029 2023-02-23 20:28:26.000000 core_explore_federated_search_app-2.2.0/tests/fixtures/fixtures.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:29.000000 core_explore_federated_search_app-2.2.0/tests/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:27.000000 core_explore_federated_search_app-2.2.0/tests/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:29.000000 core_explore_federated_search_app-2.2.0/tests/rest/result/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:27.000000 core_explore_federated_search_app-2.2.0/tests/rest/result/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:29.000000 core_explore_federated_search_app-2.2.0/tests/rest/result/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:27.000000 core_explore_federated_search_app-2.2.0/tests/rest/result/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      956 2023-02-23 20:28:27.000000 core_explore_federated_search_app-2.2.0/tests/rest/result/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1874 2023-02-23 20:28:27.000000 core_explore_federated_search_app-2.2.0/tests/rest/result/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2134 2023-02-23 20:28:27.000000 core_explore_federated_search_app-2.2.0/tests/test_settings.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      907 2023-02-23 20:28:27.000000 core_explore_federated_search_app-2.2.0/tests/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:29.000000 core_explore_federated_search_app-2.2.0/tests/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:27.000000 core_explore_federated_search_app-2.2.0/tests/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5167 2023-02-23 20:28:27.000000 core_explore_federated_search_app-2.2.0/tests/views/tests_permissions.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:40.905669 core_explore_federated_search_app-2.3.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:37:36.000000 core_explore_federated_search_app-2.3.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      174 2023-05-02 19:37:36.000000 core_explore_federated_search_app-2.3.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1555 2023-05-02 19:37:40.901085 core_explore_federated_search_app-2.3.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      967 2023-05-02 19:37:36.000000 core_explore_federated_search_app-2.3.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:40.027098 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:40.109497 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:40.177640 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/components/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/components/data/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      840 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/components/data/api.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:40.192057 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/migrations/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/migrations/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:40.221157 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:40.265711 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/rest/query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/rest/query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      354 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/rest/query/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6626 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/rest/query/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:40.308450 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/rest/result/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/rest/result/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      303 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/rest/result/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2758 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/rest/result/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      571 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/rest/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      637 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:39.756231 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:39.832746 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/static/core_explore_federated_search_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:39.804020 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:39.808459 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:39.810958 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:39.821008 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:40.397053 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      986 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/delete.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      109 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/delete.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1231 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/edit.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      105 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/edit.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1965 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/refresh.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      107 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/refresh.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:39.835828 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/static/core_explore_federated_search_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:39.838752 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/static/core_explore_federated_search_app/user/js/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:40.405654 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/static/core_explore_federated_search_app/user/js/data_sources/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2419 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/static/core_explore_federated_search_app/user/js/data_sources/list.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:39.865107 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:39.883599 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:39.870628 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:40.430285 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:40.464205 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/add/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1013 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/add/add_base.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      308 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/add_repository.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:40.489802 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2148 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/list_base.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:40.560434 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      722 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/modals/delete.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1136 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/modals/edit.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      875 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/modals/refresh.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       18 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/refresh_form.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      357 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list_repositories.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:39.885834 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:40.591623 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/user/data_sources/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      663 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/user/data_sources/list-content.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1104 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/user/data_sources/list.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      857 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:40.609459 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:40.654911 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5623 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/views/user/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2651 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/views/user/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:40.095255 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1555 2023-05-02 19:37:39.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3829 2023-05-02 19:37:39.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:37:39.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      117 2023-05-02 19:37:39.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       40 2023-05-02 19:37:39.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       85 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:37:40.907268 core_explore_federated_search_app-2.3.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1114 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:40.697470 core_explore_federated_search_app-2.3.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:40.713950 core_explore_federated_search_app-2.3.0/tests/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/tests/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:40.747427 core_explore_federated_search_app-2.3.0/tests/components/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/tests/components/data/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1073 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/tests/components/data/tests_int_access_control.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:40.778882 core_explore_federated_search_app-2.3.0/tests/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/tests/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3029 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/tests/fixtures/fixtures.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:40.792292 core_explore_federated_search_app-2.3.0/tests/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/tests/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:40.827485 core_explore_federated_search_app-2.3.0/tests/rest/result/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/tests/rest/result/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:40.859014 core_explore_federated_search_app-2.3.0/tests/rest/result/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/tests/rest/result/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      956 2023-05-02 19:37:38.000000 core_explore_federated_search_app-2.3.0/tests/rest/result/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1864 2023-05-02 19:37:38.000000 core_explore_federated_search_app-2.3.0/tests/rest/result/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2165 2023-05-02 19:37:38.000000 core_explore_federated_search_app-2.3.0/tests/test_settings.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      907 2023-05-02 19:37:38.000000 core_explore_federated_search_app-2.3.0/tests/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:40.890204 core_explore_federated_search_app-2.3.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:38.000000 core_explore_federated_search_app-2.3.0/tests/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5147 2023-05-02 19:37:38.000000 core_explore_federated_search_app-2.3.0/tests/views/tests_permissions.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `core_explore_federated_search_app-2.2.0/PKG-INFO` & `core_explore_federated_search_app-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_explore_federated_search_app
-Version: 2.2.0
+Version: 2.3.0
 Summary: Federation exploration functions for curator core project
 Home-page: https://github.com/usnistgov/core_explore_federated_search_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =================================
         Core Explore Federated Search App
```

### Comparing `core_explore_federated_search_app-2.2.0/README.rst` & `core_explore_federated_search_app-2.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/components/data/api.py` & `core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/components/data/api.py`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/rest/query/views.py` & `core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/rest/query/views.py`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/rest/result/views.py` & `core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/rest/result/views.py`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/rest/urls.py` & `core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/rest/urls.py`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/settings.py` & `core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/settings.py`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/delete.js` & `core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/delete.js`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/edit.js` & `core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/edit.js`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/refresh.js` & `core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/refresh.js`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/static/core_explore_federated_search_app/user/js/data_sources/list.js` & `core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/static/core_explore_federated_search_app/user/js/data_sources/list.js`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/add/add_base.html` & `core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/add/add_base.html`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/list_base.html` & `core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/list_base.html`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/modals/delete.html` & `core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/modals/delete.html`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/modals/edit.html` & `core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/modals/edit.html`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/modals/refresh.html` & `core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/modals/refresh.html`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/user/data_sources/list-content.html` & `core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/user/data_sources/list-content.html`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/user/data_sources/list.html` & `core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/user/data_sources/list.html`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/urls.py` & `core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/urls.py`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/views/user/ajax.py` & `core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/views/user/ajax.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,17 +131,17 @@
                 authentication=authentication,
                 order_by_field=",".join(settings.DATA_SORTING_FIELDS),
             )
             data_source["query_options"] = {"instance_name": instance.name}
 
             if "core_linked_records_app" in settings.INSTALLED_APPS:
                 data_source["capabilities"] = {
-                    "url_pid": urljoin(
+                    "query_pid": urljoin(
                         instance.endpoint,
-                        reverse("core_linked_records_app_query_local"),
+                        reverse("core_linked_records_app_query_pid"),
                     )
                 }
 
             api_query.add_data_source(query, data_source, request.user)
         else:
             # Data source have to be remove from the query
             data_source = api_query.get_data_source_by_name_and_url_query(
```

### Comparing `core_explore_federated_search_app-2.2.0/core_explore_federated_search_app/views/user/views.py` & `core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/views/user/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """ Federated user views
 """
 import json
 
 from django.contrib.auth.decorators import login_required
-from django.urls import reverse, reverse_lazy
+from django.urls import reverse
 from django.utils.decorators import method_decorator
 
 from core_explore_federated_search_app.components.data.api import (
     get_data_from_instance,
 )
 from core_main_app.access_control.exceptions import AccessControlError
 from core_main_app.commons import exceptions
 from core_main_app.utils.view_builders import data as data_view_builder
 from core_main_app.views.common.views import CommonView
 
 
 @method_decorator(
-    login_required(login_url=reverse_lazy("core_main_app_login")),
+    login_required(),
     name="dispatch",
 )
 class ViewData(CommonView):
     """View detail from remote data."""
 
     def get(self, request):
         # get parameters
```

### Comparing `core_explore_federated_search_app-2.2.0/core_explore_federated_search_app.egg-info/PKG-INFO` & `core_explore_federated_search_app-2.3.0/core_explore_federated_search_app.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-explore-federated-search-app
-Version: 2.2.0
+Version: 2.3.0
 Summary: Federation exploration functions for curator core project
 Home-page: https://github.com/usnistgov/core_explore_federated_search_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =================================
         Core Explore Federated Search App
```

### Comparing `core_explore_federated_search_app-2.2.0/core_explore_federated_search_app.egg-info/SOURCES.txt` & `core_explore_federated_search_app-2.3.0/core_explore_federated_search_app.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.md
 MANIFEST.in
 README.rst
 pyproject.toml
 requirements.core.txt
 setup.py
 core_explore_federated_search_app/__init__.py
 core_explore_federated_search_app/settings.py
```

### Comparing `core_explore_federated_search_app-2.2.0/setup.py` & `core_explore_federated_search_app-2.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_explore_federated_search_app",
-    version="2.2.0",
+    version="2.3.0",
     description="Federation exploration functions for curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_explore_federated_search_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_explore_federated_search_app-2.2.0/tests/components/data/tests_int_access_control.py` & `core_explore_federated_search_app-2.3.0/tests/components/data/tests_int_access_control.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 from django.test import override_settings
 
 from core_explore_federated_search_app.components.data.api import (
     get_data_from_instance,
 )
 from core_main_app.access_control.exceptions import AccessControlError
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 from tests.fixtures.fixtures import AccessControlDataFixture
 
 fixture_data = AccessControlDataFixture()
 
 
-class TestGetDataFromInstance(MongoIntegrationBaseTestCase):
+class TestGetDataFromInstance(IntegrationBaseTestCase):
     """Test Get Data From Instance"""
 
     fixture = fixture_data
 
     @override_settings(CAN_ANONYMOUS_ACCESS_PUBLIC_DOCUMENT=False)
     def test_get_data_from_instance_raises_access_control_error_for_anonymous_user(
         self,
```

### Comparing `core_explore_federated_search_app-2.2.0/tests/fixtures/fixtures.py` & `core_explore_federated_search_app-2.3.0/tests/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.2.0/tests/rest/result/fixtures/fixtures.py` & `core_explore_federated_search_app-2.3.0/tests/rest/result/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.2.0/tests/rest/result/tests_int.py` & `core_explore_federated_search_app-2.3.0/tests/rest/result/tests_int.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """Integration tests for Result rest api
 """
 from django.test.utils import override_settings
 from rest_framework import status
 
 import core_explore_federated_search_app.rest.result.views as result_views
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from core_main_app.utils.tests_tools.RequestMock import RequestMock
 from tests.rest.result.fixtures.fixtures import ResultFixtures
 
 fixture_data = ResultFixtures()
 
 
-class TestGetResultDetail(MongoIntegrationBaseTestCase):
+class TestGetResultDetail(IntegrationBaseTestCase):
     """Test Get Result Detail"""
 
     fixture = fixture_data
 
     def setUp(self):
         """setUp"""
```

### Comparing `core_explore_federated_search_app-2.2.0/tests/test_settings.py` & `core_explore_federated_search_app-2.3.0/tests/test_settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,7 +77,9 @@
 CUSTOM_NAME = "Curator"
 
 DEFAULT_AUTO_FIELD = "django.db.models.BigAutoField"
 CELERYBEAT_SCHEDULER = "django_celery_beat.schedulers:DatabaseScheduler"
 
 MONGODB_INDEXING = False
 MONGODB_ASYNC_SAVE = False
+
+ENABLE_SAML2_SSO_AUTH = False
```

### Comparing `core_explore_federated_search_app-2.2.0/tests/urls.py` & `core_explore_federated_search_app-2.3.0/tests/urls.py`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.2.0/tests/views/tests_permissions.py` & `core_explore_federated_search_app-2.3.0/tests/views/tests_permissions.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 
 from core_explore_federated_search_app.views.user.ajax import (
     get_data_source_list_federated,
     update_data_source_list_federated,
 )
 from core_explore_federated_search_app.views.user.views import ViewData
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from tests.fixtures.fixtures import AccessControlDataFixture
 
 
-class TestGetDataSourceListFederated(MongoIntegrationBaseTestCase):
+class TestGetDataSourceListFederated(IntegrationBaseTestCase):
     """Test Get Data Source List Federated"""
 
     def setUp(self):
         """setUp"""
 
         self.factory = RequestFactory()
         self.user1 = create_mock_user(user_id="1")
@@ -36,15 +36,15 @@
         )
         request.user = self.anonymous
         request.GET = {"id_query": str(self.fixture.query_user1.id)}
         response = get_data_source_list_federated(request)
         self.assertEqual(response.status_code, 403)
 
 
-class TestUpdateDataSourceListFederated(MongoIntegrationBaseTestCase):
+class TestUpdateDataSourceListFederated(IntegrationBaseTestCase):
     """Test Update Data Source List Federated"""
 
     def setUp(self):
         """setUp"""
 
         self.factory = RequestFactory()
         self.user1 = create_mock_user(user_id="1")
@@ -62,15 +62,15 @@
         )
         request.user = self.anonymous
         request.GET = {"id_query": str(self.fixture.query_user1.id)}
         response = update_data_source_list_federated(request)
         self.assertEqual(response.status_code, 403)
 
 
-class TestViewData(MongoIntegrationBaseTestCase):
+class TestViewData(IntegrationBaseTestCase):
     """Test View Data"""
 
     def setUp(self):
         """setUp"""
 
         self.factory = RequestFactory()
         self.user1 = create_mock_user(user_id="1")
```

