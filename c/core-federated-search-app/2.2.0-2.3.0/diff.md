# Comparing `tmp/core_federated_search_app-2.2.0.tar.gz` & `tmp/core_federated_search_app-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/core_federated_search_app-2.2.0.tar", last modified: Thu Feb 23 20:29:45 2023, max compression
+gzip compressed data, was "core_federated_search_app-2.3.0.tar", last modified: Tue May  2 19:39:00 2023, max compression
```

## Comparing `core_federated_search_app-2.2.0.tar` & `core_federated_search_app-2.3.0.tar`

### file list

```diff
@@ -1,102 +1,103 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:45.000000 core_federated_search_app-2.2.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      183 2023-02-23 20:29:41.000000 core_federated_search_app-2.2.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1232 2023-02-23 20:29:45.000000 core_federated_search_app-2.2.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      720 2023-02-23 20:29:41.000000 core_federated_search_app-2.2.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:44.000000 core_federated_search_app-2.2.0/core_federated_search_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       91 2023-02-23 20:29:41.000000 core_federated_search_app-2.2.0/core_federated_search_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1343 2023-02-23 20:29:41.000000 core_federated_search_app-2.2.0/core_federated_search_app/admin.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      270 2023-02-23 20:29:41.000000 core_federated_search_app-2.2.0/core_federated_search_app/apps.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:44.000000 core_federated_search_app-2.2.0/core_federated_search_app/commons/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:41.000000 core_federated_search_app-2.2.0/core_federated_search_app/commons/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      229 2023-02-23 20:29:41.000000 core_federated_search_app-2.2.0/core_federated_search_app/commons/exceptions.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:44.000000 core_federated_search_app-2.2.0/core_federated_search_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:41.000000 core_federated_search_app-2.2.0/core_federated_search_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:44.000000 core_federated_search_app-2.2.0/core_federated_search_app/components/instance/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:41.000000 core_federated_search_app-2.2.0/core_federated_search_app/components/instance/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5844 2023-02-23 20:29:41.000000 core_federated_search_app-2.2.0/core_federated_search_app/components/instance/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3739 2023-02-23 20:29:41.000000 core_federated_search_app-2.2.0/core_federated_search_app/components/instance/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:44.000000 core_federated_search_app-2.2.0/core_federated_search_app/components/instance/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:41.000000 core_federated_search_app-2.2.0/core_federated_search_app/components/instance/tests/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      501 2023-02-23 20:29:41.000000 core_federated_search_app-2.2.0/core_federated_search_app/menus.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:44.000000 core_federated_search_app-2.2.0/core_federated_search_app/migrations/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1476 2023-02-23 20:29:41.000000 core_federated_search_app-2.2.0/core_federated_search_app/migrations/0001_initial.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:41.000000 core_federated_search_app-2.2.0/core_federated_search_app/migrations/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:44.000000 core_federated_search_app-2.2.0/core_federated_search_app/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:41.000000 core_federated_search_app-2.2.0/core_federated_search_app/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:44.000000 core_federated_search_app-2.2.0/core_federated_search_app/rest/instance/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:41.000000 core_federated_search_app-2.2.0/core_federated_search_app/rest/instance/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1697 2023-02-23 20:29:41.000000 core_federated_search_app-2.2.0/core_federated_search_app/rest/instance/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8872 2023-02-23 20:29:41.000000 core_federated_search_app-2.2.0/core_federated_search_app/rest/instance/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      775 2023-02-23 20:29:41.000000 core_federated_search_app-2.2.0/core_federated_search_app/rest/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      382 2023-02-23 20:29:41.000000 core_federated_search_app-2.2.0/core_federated_search_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:44.000000 core_federated_search_app-2.2.0/core_federated_search_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:44.000000 core_federated_search_app-2.2.0/core_federated_search_app/static/core_federated_search_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:44.000000 core_federated_search_app-2.2.0/core_federated_search_app/static/core_federated_search_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:44.000000 core_federated_search_app-2.2.0/core_federated_search_app/static/core_federated_search_app/admin/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       40 2023-02-23 20:29:41.000000 core_federated_search_app-2.2.0/core_federated_search_app/static/core_federated_search_app/admin/css/repositories.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:44.000000 core_federated_search_app-2.2.0/core_federated_search_app/static/core_federated_search_app/admin/js/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:44.000000 core_federated_search_app-2.2.0/core_federated_search_app/static/core_federated_search_app/admin/js/repositories/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:44.000000 core_federated_search_app-2.2.0/core_federated_search_app/static/core_federated_search_app/admin/js/repositories/list/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:44.000000 core_federated_search_app-2.2.0/core_federated_search_app/static/core_federated_search_app/admin/js/repositories/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      986 2023-02-23 20:29:41.000000 core_federated_search_app-2.2.0/core_federated_search_app/static/core_federated_search_app/admin/js/repositories/list/modals/delete.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      101 2023-02-23 20:29:41.000000 core_federated_search_app-2.2.0/core_federated_search_app/static/core_federated_search_app/admin/js/repositories/list/modals/delete.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1965 2023-02-23 20:29:41.000000 core_federated_search_app-2.2.0/core_federated_search_app/static/core_federated_search_app/admin/js/repositories/list/modals/refresh.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       99 2023-02-23 20:29:41.000000 core_federated_search_app-2.2.0/core_federated_search_app/static/core_federated_search_app/admin/js/repositories/list/modals/refresh.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:44.000000 core_federated_search_app-2.2.0/core_federated_search_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:44.000000 core_federated_search_app-2.2.0/core_federated_search_app/templates/core_federated_search_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:44.000000 core_federated_search_app-2.2.0/core_federated_search_app/templates/core_federated_search_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:44.000000 core_federated_search_app-2.2.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:44.000000 core_federated_search_app-2.2.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/add/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1014 2023-02-23 20:29:41.000000 core_federated_search_app-2.2.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/add/add_base.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      300 2023-02-23 20:29:41.000000 core_federated_search_app-2.2.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/add_repository.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:44.000000 core_federated_search_app-2.2.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2154 2023-02-23 20:29:41.000000 core_federated_search_app-2.2.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list/list_base.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:45.000000 core_federated_search_app-2.2.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      722 2023-02-23 20:29:41.000000 core_federated_search_app-2.2.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list/modals/delete.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      875 2023-02-23 20:29:41.000000 core_federated_search_app-2.2.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list/modals/refresh.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       18 2023-02-23 20:29:41.000000 core_federated_search_app-2.2.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list/refresh_form.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      349 2023-02-23 20:29:41.000000 core_federated_search_app-2.2.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list_repositories.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      216 2023-02-23 20:29:41.000000 core_federated_search_app-2.2.0/core_federated_search_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:45.000000 core_federated_search_app-2.2.0/core_federated_search_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:41.000000 core_federated_search_app-2.2.0/core_federated_search_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:45.000000 core_federated_search_app-2.2.0/core_federated_search_app/views/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:41.000000 core_federated_search_app-2.2.0/core_federated_search_app/views/admin/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3647 2023-02-23 20:29:41.000000 core_federated_search_app-2.2.0/core_federated_search_app/views/admin/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2712 2023-02-23 20:29:41.000000 core_federated_search_app-2.2.0/core_federated_search_app/views/admin/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3477 2023-02-23 20:29:41.000000 core_federated_search_app-2.2.0/core_federated_search_app/views/admin/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:44.000000 core_federated_search_app-2.2.0/core_federated_search_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1232 2023-02-23 20:29:43.000000 core_federated_search_app-2.2.0/core_federated_search_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3220 2023-02-23 20:29:44.000000 core_federated_search_app-2.2.0/core_federated_search_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-02-23 20:29:43.000000 core_federated_search_app-2.2.0/core_federated_search_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      135 2023-02-23 20:29:43.000000 core_federated_search_app-2.2.0/core_federated_search_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       37 2023-02-23 20:29:43.000000 core_federated_search_app-2.2.0/core_federated_search_app.egg-info/top_level.txt
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:45.000000 core_federated_search_app-2.2.0/docs/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:41.000000 core_federated_search_app-2.2.0/docs/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11132 2023-02-23 20:29:42.000000 core_federated_search_app-2.2.0/docs/conf.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      314 2023-02-23 20:29:42.000000 core_federated_search_app-2.2.0/docs/conf_urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-02-23 20:29:42.000000 core_federated_search_app-2.2.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       52 2023-02-23 20:29:42.000000 core_federated_search_app-2.2.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       83 2023-02-23 20:29:42.000000 core_federated_search_app-2.2.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-02-23 20:29:45.000000 core_federated_search_app-2.2.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1430 2023-02-23 20:29:42.000000 core_federated_search_app-2.2.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:45.000000 core_federated_search_app-2.2.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:42.000000 core_federated_search_app-2.2.0/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:45.000000 core_federated_search_app-2.2.0/tests/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:42.000000 core_federated_search_app-2.2.0/tests/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:45.000000 core_federated_search_app-2.2.0/tests/components/instance/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:42.000000 core_federated_search_app-2.2.0/tests/components/instance/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:45.000000 core_federated_search_app-2.2.0/tests/components/instance/api/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:42.000000 core_federated_search_app-2.2.0/tests/components/instance/api/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4950 2023-02-23 20:29:42.000000 core_federated_search_app-2.2.0/tests/components/instance/api/tests_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      150 2023-02-23 20:29:42.000000 core_federated_search_app-2.2.0/tests/mocks.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:45.000000 core_federated_search_app-2.2.0/tests/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:42.000000 core_federated_search_app-2.2.0/tests/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:45.000000 core_federated_search_app-2.2.0/tests/rest/instance/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:42.000000 core_federated_search_app-2.2.0/tests/rest/instance/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:45.000000 core_federated_search_app-2.2.0/tests/rest/instance/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:42.000000 core_federated_search_app-2.2.0/tests/rest/instance/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      962 2023-02-23 20:29:42.000000 core_federated_search_app-2.2.0/tests/rest/instance/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7960 2023-02-23 20:29:42.000000 core_federated_search_app-2.2.0/tests/rest/instance/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10748 2023-02-23 20:29:42.000000 core_federated_search_app-2.2.0/tests/rest/instance/tests_permission.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2214 2023-02-23 20:29:42.000000 core_federated_search_app-2.2.0/tests/rest/instance/tests_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1645 2023-02-23 20:29:42.000000 core_federated_search_app-2.2.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:00.859924 core_federated_search_app-2.3.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      183 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1232 2023-05-02 19:39:00.855010 core_federated_search_app-2.3.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      720 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:59.802863 core_federated_search_app-2.3.0/core_federated_search_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       91 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/core_federated_search_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1343 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/core_federated_search_app/admin.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      270 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/core_federated_search_app/apps.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:59.938668 core_federated_search_app-2.3.0/core_federated_search_app/commons/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/core_federated_search_app/commons/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      229 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/core_federated_search_app/commons/exceptions.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:59.950908 core_federated_search_app-2.3.0/core_federated_search_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/core_federated_search_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:00.003928 core_federated_search_app-2.3.0/core_federated_search_app/components/instance/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/core_federated_search_app/components/instance/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5844 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/core_federated_search_app/components/instance/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3739 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/core_federated_search_app/components/instance/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:00.018235 core_federated_search_app-2.3.0/core_federated_search_app/components/instance/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/core_federated_search_app/components/instance/tests/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      501 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/core_federated_search_app/menus.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:00.045670 core_federated_search_app-2.3.0/core_federated_search_app/migrations/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1476 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/core_federated_search_app/migrations/0001_initial.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/core_federated_search_app/migrations/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:00.076849 core_federated_search_app-2.3.0/core_federated_search_app/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/core_federated_search_app/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:00.127984 core_federated_search_app-2.3.0/core_federated_search_app/rest/instance/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/core_federated_search_app/rest/instance/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1697 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/core_federated_search_app/rest/instance/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8872 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/core_federated_search_app/rest/instance/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      775 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/core_federated_search_app/rest/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      382 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/core_federated_search_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:59.470459 core_federated_search_app-2.3.0/core_federated_search_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:59.474383 core_federated_search_app-2.3.0/core_federated_search_app/static/core_federated_search_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:59.487309 core_federated_search_app-2.3.0/core_federated_search_app/static/core_federated_search_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:00.145848 core_federated_search_app-2.3.0/core_federated_search_app/static/core_federated_search_app/admin/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       40 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/core_federated_search_app/static/core_federated_search_app/admin/css/repositories.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:59.490764 core_federated_search_app-2.3.0/core_federated_search_app/static/core_federated_search_app/admin/js/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:59.494075 core_federated_search_app-2.3.0/core_federated_search_app/static/core_federated_search_app/admin/js/repositories/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:59.497520 core_federated_search_app-2.3.0/core_federated_search_app/static/core_federated_search_app/admin/js/repositories/list/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:00.243295 core_federated_search_app-2.3.0/core_federated_search_app/static/core_federated_search_app/admin/js/repositories/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      986 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/core_federated_search_app/static/core_federated_search_app/admin/js/repositories/list/modals/delete.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      101 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/core_federated_search_app/static/core_federated_search_app/admin/js/repositories/list/modals/delete.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1965 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/core_federated_search_app/static/core_federated_search_app/admin/js/repositories/list/modals/refresh.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       99 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/core_federated_search_app/static/core_federated_search_app/admin/js/repositories/list/modals/refresh.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:59.519059 core_federated_search_app-2.3.0/core_federated_search_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:59.522901 core_federated_search_app-2.3.0/core_federated_search_app/templates/core_federated_search_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:59.526750 core_federated_search_app-2.3.0/core_federated_search_app/templates/core_federated_search_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:00.273676 core_federated_search_app-2.3.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:00.287142 core_federated_search_app-2.3.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/add/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1014 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/add/add_base.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      300 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/add_repository.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:00.327421 core_federated_search_app-2.3.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2154 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list/list_base.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:00.377797 core_federated_search_app-2.3.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      722 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list/modals/delete.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      875 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list/modals/refresh.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       18 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list/refresh_form.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      349 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list_repositories.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      216 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/core_federated_search_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:00.396896 core_federated_search_app-2.3.0/core_federated_search_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/core_federated_search_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:00.464623 core_federated_search_app-2.3.0/core_federated_search_app/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/core_federated_search_app/views/admin/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3647 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/core_federated_search_app/views/admin/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2712 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/core_federated_search_app/views/admin/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3477 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/core_federated_search_app/views/admin/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:59.900715 core_federated_search_app-2.3.0/core_federated_search_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1232 2023-05-02 19:38:58.000000 core_federated_search_app-2.3.0/core_federated_search_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3231 2023-05-02 19:38:59.000000 core_federated_search_app-2.3.0/core_federated_search_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:38:59.000000 core_federated_search_app-2.3.0/core_federated_search_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      135 2023-05-02 19:38:59.000000 core_federated_search_app-2.3.0/core_federated_search_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       37 2023-05-02 19:38:59.000000 core_federated_search_app-2.3.0/core_federated_search_app.egg-info/top_level.txt
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:00.547165 core_federated_search_app-2.3.0/docs/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/docs/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11132 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/docs/conf.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      314 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/docs/conf_urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       52 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       83 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:39:00.861613 core_federated_search_app-2.3.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1430 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:00.618840 core_federated_search_app-2.3.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:00.649797 core_federated_search_app-2.3.0/tests/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/tests/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:00.672615 core_federated_search_app-2.3.0/tests/components/instance/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/tests/components/instance/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:00.711065 core_federated_search_app-2.3.0/tests/components/instance/api/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/tests/components/instance/api/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4950 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/tests/components/instance/api/tests_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      150 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/tests/mocks.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:00.728796 core_federated_search_app-2.3.0/tests/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/tests/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:00.813991 core_federated_search_app-2.3.0/tests/rest/instance/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/tests/rest/instance/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:00.842364 core_federated_search_app-2.3.0/tests/rest/instance/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/tests/rest/instance/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      962 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/tests/rest/instance/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7935 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/tests/rest/instance/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10748 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/tests/rest/instance/tests_permission.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2214 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/tests/rest/instance/tests_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1645 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/tests/test_settings.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `core_federated_search_app-2.2.0/PKG-INFO` & `core_federated_search_app-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_federated_search_app
-Version: 2.2.0
+Version: 2.3.0
 Summary: Federated search backend for the curator core project
 Home-page: https://github.com/usnistgov/core_federated_search_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =========================
         Core Federated Search App
```

### Comparing `core_federated_search_app-2.2.0/README.rst` & `core_federated_search_app-2.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.2.0/core_federated_search_app/admin.py` & `core_federated_search_app-2.3.0/core_federated_search_app/admin.py`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.2.0/core_federated_search_app/components/instance/api.py` & `core_federated_search_app-2.3.0/core_federated_search_app/components/instance/api.py`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.2.0/core_federated_search_app/components/instance/models.py` & `core_federated_search_app-2.3.0/core_federated_search_app/components/instance/models.py`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.2.0/core_federated_search_app/migrations/0001_initial.py` & `core_federated_search_app-2.3.0/core_federated_search_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.2.0/core_federated_search_app/rest/instance/serializers.py` & `core_federated_search_app-2.3.0/core_federated_search_app/rest/instance/serializers.py`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.2.0/core_federated_search_app/rest/instance/views.py` & `core_federated_search_app-2.3.0/core_federated_search_app/rest/instance/views.py`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.2.0/core_federated_search_app/rest/urls.py` & `core_federated_search_app-2.3.0/core_federated_search_app/rest/urls.py`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.2.0/core_federated_search_app/static/core_federated_search_app/admin/js/repositories/list/modals/delete.js` & `core_federated_search_app-2.3.0/core_federated_search_app/static/core_federated_search_app/admin/js/repositories/list/modals/delete.js`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.2.0/core_federated_search_app/static/core_federated_search_app/admin/js/repositories/list/modals/refresh.js` & `core_federated_search_app-2.3.0/core_federated_search_app/static/core_federated_search_app/admin/js/repositories/list/modals/refresh.js`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.2.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/add/add_base.html` & `core_federated_search_app-2.3.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/add/add_base.html`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.2.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list/list_base.html` & `core_federated_search_app-2.3.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list/list_base.html`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.2.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list/modals/delete.html` & `core_federated_search_app-2.3.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list/modals/delete.html`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.2.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list/modals/refresh.html` & `core_federated_search_app-2.3.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list/modals/refresh.html`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.2.0/core_federated_search_app/views/admin/ajax.py` & `core_federated_search_app-2.3.0/core_federated_search_app/views/admin/ajax.py`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.2.0/core_federated_search_app/views/admin/forms.py` & `core_federated_search_app-2.3.0/core_federated_search_app/views/admin/forms.py`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.2.0/core_federated_search_app/views/admin/views.py` & `core_federated_search_app-2.3.0/core_federated_search_app/views/admin/views.py`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.2.0/core_federated_search_app.egg-info/PKG-INFO` & `core_federated_search_app-2.3.0/core_federated_search_app.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-federated-search-app
-Version: 2.2.0
+Version: 2.3.0
 Summary: Federated search backend for the curator core project
 Home-page: https://github.com/usnistgov/core_federated_search_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =========================
         Core Federated Search App
```

### Comparing `core_federated_search_app-2.2.0/core_federated_search_app.egg-info/SOURCES.txt` & `core_federated_search_app-2.3.0/core_federated_search_app.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.md
 MANIFEST.in
 README.rst
 pyproject.toml
 requirements.core.txt
 requirements.txt
 setup.py
 core_federated_search_app/__init__.py
```

### Comparing `core_federated_search_app-2.2.0/docs/conf.py` & `core_federated_search_app-2.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.2.0/setup.py` & `core_federated_search_app-2.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_federated_search_app",
-    version="2.2.0",
+    version="2.3.0",
     description="Federated search backend for the curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_federated_search_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_federated_search_app-2.2.0/tests/components/instance/api/tests_unit.py` & `core_federated_search_app-2.3.0/tests/components/instance/api/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.2.0/tests/rest/instance/fixtures/fixtures.py` & `core_federated_search_app-2.3.0/tests/rest/instance/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.2.0/tests/rest/instance/tests_int.py` & `core_federated_search_app-2.3.0/tests/rest/instance/tests_int.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """Integration tests for instance rest api
 """
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from core_main_app.utils.tests_tools.RequestMock import RequestMock
 from rest_framework import status
 
 import core_federated_search_app.rest.instance.views as instance_views
 from tests.rest.instance.fixtures.fixtures import InstanceFixtures
 
 fixture_data = InstanceFixtures()
 
 
-class TestGetAllInstanceList(MongoIntegrationBaseTestCase):
+class TestGetAllInstanceList(IntegrationBaseTestCase):
     """Test Get All Instance List"""
 
     fixture = fixture_data
 
     def setUp(self):
         """setUp"""
 
@@ -48,15 +48,15 @@
             instance_views.InstanceList.as_view(), user
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_200_OK)
 
 
-class TestGetInstanceDetail(MongoIntegrationBaseTestCase):
+class TestGetInstanceDetail(IntegrationBaseTestCase):
     """Test Get Instance Detail"""
 
     fixture = fixture_data
 
     def setUp(self):
         """setUp"""
 
@@ -116,15 +116,15 @@
 
         # Assert
         self.assertEqual(
             response.status_code, status.HTTP_500_INTERNAL_SERVER_ERROR
         )
 
 
-class TestDeleteInstanceDetail(MongoIntegrationBaseTestCase):
+class TestDeleteInstanceDetail(IntegrationBaseTestCase):
     """Test Delete Instance Detail"""
 
     fixture = fixture_data
 
     def setUp(self):
         """setUp"""
 
@@ -202,15 +202,15 @@
             self.param,
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_204_NO_CONTENT)
 
 
-class TestPatchInstanceDetail(MongoIntegrationBaseTestCase):
+class TestPatchInstanceDetail(IntegrationBaseTestCase):
     """Test Patch Instance Detail"""
 
     fixture = fixture_data
 
     def setUp(self):
         """setUp"""
```

### Comparing `core_federated_search_app-2.2.0/tests/rest/instance/tests_permission.py` & `core_federated_search_app-2.3.0/tests/rest/instance/tests_permission.py`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.2.0/tests/rest/instance/tests_unit.py` & `core_federated_search_app-2.3.0/tests/rest/instance/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.2.0/tests/test_settings.py` & `core_federated_search_app-2.3.0/tests/test_settings.py`

 * *Files identical despite different names*

