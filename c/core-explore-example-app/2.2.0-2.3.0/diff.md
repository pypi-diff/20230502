# Comparing `tmp/core_explore_example_app-2.2.0.tar.gz` & `tmp/core_explore_example_app-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/core_explore_example_app-2.2.0.tar", last modified: Thu Feb 23 20:28:18 2023, max compression
+gzip compressed data, was "core_explore_example_app-2.3.0.tar", last modified: Tue May  2 19:37:25 2023, max compression
```

## Comparing `core_explore_example_app-2.2.0.tar` & `core_explore_example_app-2.3.0.tar`

### file list

```diff
@@ -1,179 +1,180 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:18.000000 core_explore_example_app-2.2.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      156 2023-02-23 20:28:11.000000 core_explore_example_app-2.2.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1114 2023-02-23 20:28:18.000000 core_explore_example_app-2.2.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      614 2023-02-23 20:28:11.000000 core_explore_example_app-2.2.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:15.000000 core_explore_example_app-2.2.0/core_explore_example_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-02-23 20:28:11.000000 core_explore_example_app-2.2.0/core_explore_example_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1093 2023-02-23 20:28:11.000000 core_explore_example_app-2.2.0/core_explore_example_app/admin.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      634 2023-02-23 20:28:11.000000 core_explore_example_app-2.2.0/core_explore_example_app/apps.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:16.000000 core_explore_example_app-2.2.0/core_explore_example_app/commons/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:11.000000 core_explore_example_app-2.2.0/core_explore_example_app/commons/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      205 2023-02-23 20:28:11.000000 core_explore_example_app-2.2.0/core_explore_example_app/commons/exceptions.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:16.000000 core_explore_example_app-2.2.0/core_explore_example_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:11.000000 core_explore_example_app-2.2.0/core_explore_example_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:16.000000 core_explore_example_app-2.2.0/core_explore_example_app/components/explore_data_structure/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:11.000000 core_explore_example_app-2.2.0/core_explore_example_app/components/explore_data_structure/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      442 2023-02-23 20:28:11.000000 core_explore_example_app-2.2.0/core_explore_example_app/components/explore_data_structure/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2006 2023-02-23 20:28:11.000000 core_explore_example_app-2.2.0/core_explore_example_app/components/explore_data_structure/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1764 2023-02-23 20:28:11.000000 core_explore_example_app-2.2.0/core_explore_example_app/components/explore_data_structure/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:16.000000 core_explore_example_app-2.2.0/core_explore_example_app/components/persistent_query_example/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:11.000000 core_explore_example_app-2.2.0/core_explore_example_app/components/persistent_query_example/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      372 2023-02-23 20:28:11.000000 core_explore_example_app-2.2.0/core_explore_example_app/components/persistent_query_example/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2283 2023-02-23 20:28:11.000000 core_explore_example_app-2.2.0/core_explore_example_app/components/persistent_query_example/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1973 2023-02-23 20:28:11.000000 core_explore_example_app-2.2.0/core_explore_example_app/components/persistent_query_example/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:16.000000 core_explore_example_app-2.2.0/core_explore_example_app/components/saved_query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:11.000000 core_explore_example_app-2.2.0/core_explore_example_app/components/saved_query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      356 2023-02-23 20:28:11.000000 core_explore_example_app-2.2.0/core_explore_example_app/components/saved_query/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      904 2023-02-23 20:28:11.000000 core_explore_example_app-2.2.0/core_explore_example_app/components/saved_query/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1565 2023-02-23 20:28:11.000000 core_explore_example_app-2.2.0/core_explore_example_app/components/saved_query/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      927 2023-02-23 20:28:11.000000 core_explore_example_app-2.2.0/core_explore_example_app/discover.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      321 2023-02-23 20:28:11.000000 core_explore_example_app-2.2.0/core_explore_example_app/menus.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:16.000000 core_explore_example_app-2.2.0/core_explore_example_app/migrations/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4401 2023-02-23 20:28:11.000000 core_explore_example_app-2.2.0/core_explore_example_app/migrations/0001_initial.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:11.000000 core_explore_example_app-2.2.0/core_explore_example_app/migrations/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1058 2023-02-23 20:28:11.000000 core_explore_example_app-2.2.0/core_explore_example_app/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:16.000000 core_explore_example_app-2.2.0/core_explore_example_app/permissions/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:11.000000 core_explore_example_app-2.2.0/core_explore_example_app/permissions/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1723 2023-02-23 20:28:11.000000 core_explore_example_app-2.2.0/core_explore_example_app/permissions/discover.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      320 2023-02-23 20:28:11.000000 core_explore_example_app-2.2.0/core_explore_example_app/permissions/rights.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:16.000000 core_explore_example_app-2.2.0/core_explore_example_app/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:11.000000 core_explore_example_app-2.2.0/core_explore_example_app/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:16.000000 core_explore_example_app-2.2.0/core_explore_example_app/rest/persistent_query_example/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:11.000000 core_explore_example_app-2.2.0/core_explore_example_app/rest/persistent_query_example/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3259 2023-02-23 20:28:11.000000 core_explore_example_app-2.2.0/core_explore_example_app/rest/persistent_query_example/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    13206 2023-02-23 20:28:11.000000 core_explore_example_app-2.2.0/core_explore_example_app/rest/persistent_query_example/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:16.000000 core_explore_example_app-2.2.0/core_explore_example_app/rest/saved_query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:11.000000 core_explore_example_app-2.2.0/core_explore_example_app/rest/saved_query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      395 2023-02-23 20:28:11.000000 core_explore_example_app-2.2.0/core_explore_example_app/rest/saved_query/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4767 2023-02-23 20:28:11.000000 core_explore_example_app-2.2.0/core_explore_example_app/rest/saved_query/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1653 2023-02-23 20:28:11.000000 core_explore_example_app-2.2.0/core_explore_example_app/rest/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      620 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/core_explore_example_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:15.000000 core_explore_example_app-2.2.0/core_explore_example_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:15.000000 core_explore_example_app-2.2.0/core_explore_example_app/static/core_explore_example_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:15.000000 core_explore_example_app-2.2.0/core_explore_example_app/static/core_explore_example_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:16.000000 core_explore_example_app-2.2.0/core_explore_example_app/static/core_explore_example_app/user/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      724 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/core_explore_example_app/static/core_explore_example_app/user/css/query_builder.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      465 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/core_explore_example_app/static/core_explore_example_app/user/css/style.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      170 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/core_explore_example_app/static/core_explore_example_app/user/css/xsd_form.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:16.000000 core_explore_example_app-2.2.0/core_explore_example_app/static/core_explore_example_app/user/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14448 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/core_explore_example_app/static/core_explore_example_app/user/js/build_query.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1044 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/core_explore_example_app/static/core_explore_example_app/user/js/build_query.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      147 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/core_explore_example_app/static/core_explore_example_app/user/js/buttons.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       84 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/core_explore_example_app/static/core_explore_example_app/user/js/choice.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      320 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/core_explore_example_app/static/core_explore_example_app/user/js/persistent_query.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1408 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/core_explore_example_app/static/core_explore_example_app/user/js/refresh_sorting.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       49 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/core_explore_example_app/static/core_explore_example_app/user/js/refresh_sorting.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1268 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/core_explore_example_app/static/core_explore_example_app/user/js/select_fields.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      138 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/core_explore_example_app/static/core_explore_example_app/user/js/select_fields.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:16.000000 core_explore_example_app-2.2.0/core_explore_example_app/system/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/core_explore_example_app/system/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      371 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/core_explore_example_app/system/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1140 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/core_explore_example_app/tasks.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:15.000000 core_explore_example_app-2.2.0/core_explore_example_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:15.000000 core_explore_example_app-2.2.0/core_explore_example_app/templates/core_explore_example_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:17.000000 core_explore_example_app-2.2.0/core_explore_example_app/templates/core_explore_example_app/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3030 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/core_explore_example_app/templates/core_explore_example_app/user/build_query.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       32 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/core_explore_example_app/templates/core_explore_example_app/user/errors.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1044 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/core_explore_example_app/templates/core_explore_example_app/user/index.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:17.000000 core_explore_example_app-2.2.0/core_explore_example_app/templates/core_explore_example_app/user/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      429 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/core_explore_example_app/templates/core_explore_example_app/user/list/list.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:17.000000 core_explore_example_app-2.2.0/core_explore_example_app/templates/core_explore_example_app/user/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1023 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/core_explore_example_app/templates/core_explore_example_app/user/modals/custom_tree.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      535 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/core_explore_example_app/templates/core_explore_example_app/user/modals/delete_all_queries.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      565 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/core_explore_example_app/templates/core_explore_example_app/user/modals/delete_query.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      391 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/core_explore_example_app/templates/core_explore_example_app/user/modals/errors.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      652 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/core_explore_example_app/templates/core_explore_example_app/user/modals/sub_elements_query_builder.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:17.000000 core_explore_example_app-2.2.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       86 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/add.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      148 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/and_or_not.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       97 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/criteria_select.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      121 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/enum.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      144 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/field_input.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       89 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/gregorian_strict_match.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      292 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/initial_form.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       64 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/input.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      403 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/new_criteria.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      749 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/new_query.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      244 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/numeric_select.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      103 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/remove.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      116 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/string_select.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      493 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/sub_elements_query.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      107 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/yes_no.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      648 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/core_explore_example_app/templates/core_explore_example_app/user/results.html
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      489 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/core_explore_example_app/templates/core_explore_example_app/user/select_fields.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3787 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/core_explore_example_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:17.000000 core_explore_example_app-2.2.0/core_explore_example_app/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/core_explore_example_app/utils/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1775 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/core_explore_example_app/utils/custom_checkbox_renderer.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4373 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/core_explore_example_app/utils/displayed_query.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    15354 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/core_explore_example_app/utils/mongo_query.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2998 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/core_explore_example_app/utils/parser.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10108 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/core_explore_example_app/utils/query_builder.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1899 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/core_explore_example_app/utils/xml.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:17.000000 core_explore_example_app-2.2.0/core_explore_example_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/core_explore_example_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:17.000000 core_explore_example_app-2.2.0/core_explore_example_app/views/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/core_explore_example_app/views/admin/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:17.000000 core_explore_example_app-2.2.0/core_explore_example_app/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/core_explore_example_app/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    21425 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/core_explore_example_app/views/user/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    19951 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/core_explore_example_app/views/user/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:16.000000 core_explore_example_app-2.2.0/core_explore_example_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1114 2023-02-23 20:28:15.000000 core_explore_example_app-2.2.0/core_explore_example_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7502 2023-02-23 20:28:15.000000 core_explore_example_app-2.2.0/core_explore_example_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-02-23 20:28:15.000000 core_explore_example_app-2.2.0/core_explore_example_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      146 2023-02-23 20:28:15.000000 core_explore_example_app-2.2.0/core_explore_example_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       36 2023-02-23 20:28:15.000000 core_explore_example_app-2.2.0/core_explore_example_app.egg-info/top_level.txt
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:18.000000 core_explore_example_app-2.2.0/docs/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/docs/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11127 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/docs/conf.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      311 2023-02-23 20:28:12.000000 core_explore_example_app-2.2.0/docs/conf_urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-02-23 20:28:13.000000 core_explore_example_app-2.2.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       93 2023-02-23 20:28:13.000000 core_explore_example_app-2.2.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-02-23 20:28:18.000000 core_explore_example_app-2.2.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1420 2023-02-23 20:28:13.000000 core_explore_example_app-2.2.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:18.000000 core_explore_example_app-2.2.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:13.000000 core_explore_example_app-2.2.0/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:18.000000 core_explore_example_app-2.2.0/tests/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:13.000000 core_explore_example_app-2.2.0/tests/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:18.000000 core_explore_example_app-2.2.0/tests/components/explore_data_structure/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:13.000000 core_explore_example_app-2.2.0/tests/components/explore_data_structure/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2970 2023-02-23 20:28:13.000000 core_explore_example_app-2.2.0/tests/components/explore_data_structure/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:18.000000 core_explore_example_app-2.2.0/tests/components/persistent_query_example/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:13.000000 core_explore_example_app-2.2.0/tests/components/persistent_query_example/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:18.000000 core_explore_example_app-2.2.0/tests/components/persistent_query_example/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:13.000000 core_explore_example_app-2.2.0/tests/components/persistent_query_example/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1899 2023-02-23 20:28:13.000000 core_explore_example_app-2.2.0/tests/components/persistent_query_example/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    15672 2023-02-23 20:28:13.000000 core_explore_example_app-2.2.0/tests/components/persistent_query_example/tests_int_access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6827 2023-02-23 20:28:13.000000 core_explore_example_app-2.2.0/tests/components/persistent_query_example/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:18.000000 core_explore_example_app-2.2.0/tests/components/saved_query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:13.000000 core_explore_example_app-2.2.0/tests/components/saved_query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3113 2023-02-23 20:28:13.000000 core_explore_example_app-2.2.0/tests/components/saved_query/tests_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      132 2023-02-23 20:28:13.000000 core_explore_example_app-2.2.0/tests/mocks.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:18.000000 core_explore_example_app-2.2.0/tests/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:13.000000 core_explore_example_app-2.2.0/tests/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:18.000000 core_explore_example_app-2.2.0/tests/rest/persistent_query_example/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:13.000000 core_explore_example_app-2.2.0/tests/rest/persistent_query_example/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11785 2023-02-23 20:28:13.000000 core_explore_example_app-2.2.0/tests/rest/persistent_query_example/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17575 2023-02-23 20:28:13.000000 core_explore_example_app-2.2.0/tests/rest/persistent_query_example/tests_permissions.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:18.000000 core_explore_example_app-2.2.0/tests/rest/saved_query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:13.000000 core_explore_example_app-2.2.0/tests/rest/saved_query/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:18.000000 core_explore_example_app-2.2.0/tests/rest/saved_query/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:13.000000 core_explore_example_app-2.2.0/tests/rest/saved_query/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1333 2023-02-23 20:28:13.000000 core_explore_example_app-2.2.0/tests/rest/saved_query/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4675 2023-02-23 20:28:13.000000 core_explore_example_app-2.2.0/tests/rest/saved_query/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5717 2023-02-23 20:28:13.000000 core_explore_example_app-2.2.0/tests/rest/saved_query/tests_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1614 2023-02-23 20:28:13.000000 core_explore_example_app-2.2.0/tests/test_settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:18.000000 core_explore_example_app-2.2.0/tests/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:13.000000 core_explore_example_app-2.2.0/tests/utils/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:18.000000 core_explore_example_app-2.2.0/tests/utils/mongo_query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:13.000000 core_explore_example_app-2.2.0/tests/utils/mongo_query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7156 2023-02-23 20:28:13.000000 core_explore_example_app-2.2.0/tests/utils/mongo_query/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:18.000000 core_explore_example_app-2.2.0/tests/utils/xml/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:13.000000 core_explore_example_app-2.2.0/tests/utils/xml/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1633 2023-02-23 20:28:13.000000 core_explore_example_app-2.2.0/tests/utils/xml/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:18.000000 core_explore_example_app-2.2.0/tests/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:13.000000 core_explore_example_app-2.2.0/tests/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:18.000000 core_explore_example_app-2.2.0/tests/views/ajax/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:13.000000 core_explore_example_app-2.2.0/tests/views/ajax/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11066 2023-02-23 20:28:13.000000 core_explore_example_app-2.2.0/tests/views/ajax/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:25.055685 core_explore_example_app-2.3.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      156 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1114 2023-05-02 19:37:25.050897 core_explore_example_app-2.3.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      614 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:22.721799 core_explore_example_app-2.3.0/core_explore_example_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1093 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/admin.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      634 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/apps.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:22.860450 core_explore_example_app-2.3.0/core_explore_example_app/commons/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/commons/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      205 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/commons/exceptions.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:22.879463 core_explore_example_app-2.3.0/core_explore_example_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:23.062487 core_explore_example_app-2.3.0/core_explore_example_app/components/explore_data_structure/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/components/explore_data_structure/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      442 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/components/explore_data_structure/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2006 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/components/explore_data_structure/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1764 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/components/explore_data_structure/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:23.147187 core_explore_example_app-2.3.0/core_explore_example_app/components/persistent_query_example/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/components/persistent_query_example/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      372 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/components/persistent_query_example/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2283 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/components/persistent_query_example/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1973 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/components/persistent_query_example/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:23.228171 core_explore_example_app-2.3.0/core_explore_example_app/components/saved_query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/components/saved_query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      356 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/components/saved_query/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      904 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/components/saved_query/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1565 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/components/saved_query/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      927 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/discover.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      321 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/menus.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:23.280526 core_explore_example_app-2.3.0/core_explore_example_app/migrations/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4401 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/migrations/0001_initial.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/migrations/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1058 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:23.334501 core_explore_example_app-2.3.0/core_explore_example_app/permissions/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/permissions/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1723 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/permissions/discover.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      320 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/permissions/rights.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:23.367622 core_explore_example_app-2.3.0/core_explore_example_app/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:23.430000 core_explore_example_app-2.3.0/core_explore_example_app/rest/persistent_query_example/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/rest/persistent_query_example/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3259 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/rest/persistent_query_example/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    13206 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/rest/persistent_query_example/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:23.479024 core_explore_example_app-2.3.0/core_explore_example_app/rest/saved_query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/rest/saved_query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      395 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/rest/saved_query/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4767 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/rest/saved_query/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1653 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/rest/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      620 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:22.306677 core_explore_example_app-2.3.0/core_explore_example_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:22.310787 core_explore_example_app-2.3.0/core_explore_example_app/static/core_explore_example_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:22.320340 core_explore_example_app-2.3.0/core_explore_example_app/static/core_explore_example_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:23.533027 core_explore_example_app-2.3.0/core_explore_example_app/static/core_explore_example_app/user/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      724 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/static/core_explore_example_app/user/css/query_builder.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      465 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/static/core_explore_example_app/user/css/style.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      170 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/static/core_explore_example_app/user/css/xsd_form.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:23.670482 core_explore_example_app-2.3.0/core_explore_example_app/static/core_explore_example_app/user/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14448 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/static/core_explore_example_app/user/js/build_query.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1044 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/static/core_explore_example_app/user/js/build_query.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      147 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/static/core_explore_example_app/user/js/buttons.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       84 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/static/core_explore_example_app/user/js/choice.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      320 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/static/core_explore_example_app/user/js/persistent_query.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1408 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/static/core_explore_example_app/user/js/refresh_sorting.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       49 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/static/core_explore_example_app/user/js/refresh_sorting.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1268 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/static/core_explore_example_app/user/js/select_fields.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      138 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/static/core_explore_example_app/user/js/select_fields.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:23.707906 core_explore_example_app-2.3.0/core_explore_example_app/system/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/system/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      371 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/system/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1140 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/tasks.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:22.347662 core_explore_example_app-2.3.0/core_explore_example_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:22.351891 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:23.795719 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3030 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/build_query.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       32 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/errors.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1044 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/index.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:23.818653 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      429 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/list/list.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:23.894486 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1023 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/modals/custom_tree.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      535 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/modals/delete_all_queries.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      565 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/modals/delete_query.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      391 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/modals/errors.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      652 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/modals/sub_elements_query_builder.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:24.144893 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       86 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/add.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      148 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/and_or_not.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       97 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/criteria_select.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      121 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/enum.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      144 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/field_input.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       89 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/gregorian_strict_match.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      292 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/initial_form.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       64 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/input.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      403 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/new_criteria.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      749 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/new_query.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      244 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/numeric_select.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      103 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/remove.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      116 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/string_select.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      493 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/sub_elements_query.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      107 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/yes_no.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      648 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/results.html
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      489 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/select_fields.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3787 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:24.260571 core_explore_example_app-2.3.0/core_explore_example_app/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/utils/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1775 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/utils/custom_checkbox_renderer.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4373 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/utils/displayed_query.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    15354 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/utils/mongo_query.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2998 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/utils/parser.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10108 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/utils/query_builder.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1899 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/utils/xml.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:24.291060 core_explore_example_app-2.3.0/core_explore_example_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:24.313038 core_explore_example_app-2.3.0/core_explore_example_app/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/views/admin/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:24.366705 core_explore_example_app-2.3.0/core_explore_example_app/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    21425 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/views/user/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    19641 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/views/user/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:22.829761 core_explore_example_app-2.3.0/core_explore_example_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1114 2023-05-02 19:37:21.000000 core_explore_example_app-2.3.0/core_explore_example_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7513 2023-05-02 19:37:22.000000 core_explore_example_app-2.3.0/core_explore_example_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:37:21.000000 core_explore_example_app-2.3.0/core_explore_example_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      146 2023-05-02 19:37:21.000000 core_explore_example_app-2.3.0/core_explore_example_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       36 2023-05-02 19:37:21.000000 core_explore_example_app-2.3.0/core_explore_example_app.egg-info/top_level.txt
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:24.423854 core_explore_example_app-2.3.0/docs/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/docs/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11127 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/docs/conf.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      311 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/docs/conf_urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       93 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:37:25.057653 core_explore_example_app-2.3.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1420 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:24.473058 core_explore_example_app-2.3.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:24.488567 core_explore_example_app-2.3.0/tests/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/tests/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:24.539673 core_explore_example_app-2.3.0/tests/components/explore_data_structure/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/tests/components/explore_data_structure/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2970 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/tests/components/explore_data_structure/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:24.586778 core_explore_example_app-2.3.0/tests/components/persistent_query_example/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/tests/components/persistent_query_example/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:24.634273 core_explore_example_app-2.3.0/tests/components/persistent_query_example/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/tests/components/persistent_query_example/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1899 2023-05-02 19:37:20.000000 core_explore_example_app-2.3.0/tests/components/persistent_query_example/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    15632 2023-05-02 19:37:20.000000 core_explore_example_app-2.3.0/tests/components/persistent_query_example/tests_int_access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6827 2023-05-02 19:37:20.000000 core_explore_example_app-2.3.0/tests/components/persistent_query_example/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:24.667850 core_explore_example_app-2.3.0/tests/components/saved_query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:20.000000 core_explore_example_app-2.3.0/tests/components/saved_query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3113 2023-05-02 19:37:20.000000 core_explore_example_app-2.3.0/tests/components/saved_query/tests_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      132 2023-05-02 19:37:20.000000 core_explore_example_app-2.3.0/tests/mocks.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:24.684881 core_explore_example_app-2.3.0/tests/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:20.000000 core_explore_example_app-2.3.0/tests/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:24.738428 core_explore_example_app-2.3.0/tests/rest/persistent_query_example/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:20.000000 core_explore_example_app-2.3.0/tests/rest/persistent_query_example/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11760 2023-05-02 19:37:20.000000 core_explore_example_app-2.3.0/tests/rest/persistent_query_example/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17575 2023-05-02 19:37:20.000000 core_explore_example_app-2.3.0/tests/rest/persistent_query_example/tests_permissions.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:24.822812 core_explore_example_app-2.3.0/tests/rest/saved_query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:20.000000 core_explore_example_app-2.3.0/tests/rest/saved_query/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:24.857122 core_explore_example_app-2.3.0/tests/rest/saved_query/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:20.000000 core_explore_example_app-2.3.0/tests/rest/saved_query/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1333 2023-05-02 19:37:20.000000 core_explore_example_app-2.3.0/tests/rest/saved_query/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4655 2023-05-02 19:37:20.000000 core_explore_example_app-2.3.0/tests/rest/saved_query/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5717 2023-05-02 19:37:20.000000 core_explore_example_app-2.3.0/tests/rest/saved_query/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1614 2023-05-02 19:37:20.000000 core_explore_example_app-2.3.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:24.873888 core_explore_example_app-2.3.0/tests/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:20.000000 core_explore_example_app-2.3.0/tests/utils/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:24.936221 core_explore_example_app-2.3.0/tests/utils/mongo_query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:20.000000 core_explore_example_app-2.3.0/tests/utils/mongo_query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7156 2023-05-02 19:37:20.000000 core_explore_example_app-2.3.0/tests/utils/mongo_query/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:24.969924 core_explore_example_app-2.3.0/tests/utils/xml/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:20.000000 core_explore_example_app-2.3.0/tests/utils/xml/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1633 2023-05-02 19:37:20.000000 core_explore_example_app-2.3.0/tests/utils/xml/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:24.986060 core_explore_example_app-2.3.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:20.000000 core_explore_example_app-2.3.0/tests/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:25.032931 core_explore_example_app-2.3.0/tests/views/ajax/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:20.000000 core_explore_example_app-2.3.0/tests/views/ajax/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11066 2023-05-02 19:37:20.000000 core_explore_example_app-2.3.0/tests/views/ajax/tests_unit.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `core_explore_example_app-2.2.0/PKG-INFO` & `core_explore_example_app-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_explore_example_app
-Version: 2.2.0
+Version: 2.3.0
 Summary: Exploration by example for the curator core project
 Home-page: https://github.com/usnistgov/core_explore_example_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: ========================
         Core Explore Example App
```

### Comparing `core_explore_example_app-2.2.0/README.rst` & `core_explore_example_app-2.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.2.0/core_explore_example_app/admin.py` & `core_explore_example_app-2.3.0/core_explore_example_app/admin.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.2.0/core_explore_example_app/apps.py` & `core_explore_example_app-2.3.0/core_explore_example_app/apps.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.2.0/core_explore_example_app/components/explore_data_structure/api.py` & `core_explore_example_app-2.3.0/core_explore_example_app/components/explore_data_structure/api.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.2.0/core_explore_example_app/components/explore_data_structure/models.py` & `core_explore_example_app-2.3.0/core_explore_example_app/components/explore_data_structure/models.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.2.0/core_explore_example_app/components/persistent_query_example/api.py` & `core_explore_example_app-2.3.0/core_explore_example_app/components/persistent_query_example/api.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.2.0/core_explore_example_app/components/persistent_query_example/models.py` & `core_explore_example_app-2.3.0/core_explore_example_app/components/persistent_query_example/models.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.2.0/core_explore_example_app/components/saved_query/api.py` & `core_explore_example_app-2.3.0/core_explore_example_app/components/saved_query/api.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.2.0/core_explore_example_app/components/saved_query/models.py` & `core_explore_example_app-2.3.0/core_explore_example_app/components/saved_query/models.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.2.0/core_explore_example_app/discover.py` & `core_explore_example_app-2.3.0/core_explore_example_app/discover.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.2.0/core_explore_example_app/migrations/0001_initial.py` & `core_explore_example_app-2.3.0/core_explore_example_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.2.0/core_explore_example_app/models.py` & `core_explore_example_app-2.3.0/core_explore_example_app/models.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.2.0/core_explore_example_app/permissions/discover.py` & `core_explore_example_app-2.3.0/core_explore_example_app/permissions/discover.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.2.0/core_explore_example_app/rest/persistent_query_example/serializers.py` & `core_explore_example_app-2.3.0/core_explore_example_app/rest/persistent_query_example/serializers.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.2.0/core_explore_example_app/rest/persistent_query_example/views.py` & `core_explore_example_app-2.3.0/core_explore_example_app/rest/persistent_query_example/views.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.2.0/core_explore_example_app/rest/saved_query/views.py` & `core_explore_example_app-2.3.0/core_explore_example_app/rest/saved_query/views.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.2.0/core_explore_example_app/rest/urls.py` & `core_explore_example_app-2.3.0/core_explore_example_app/rest/urls.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.2.0/core_explore_example_app/settings.py` & `core_explore_example_app-2.3.0/core_explore_example_app/settings.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.2.0/core_explore_example_app/static/core_explore_example_app/user/css/query_builder.css` & `core_explore_example_app-2.3.0/core_explore_example_app/static/core_explore_example_app/user/css/query_builder.css`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.2.0/core_explore_example_app/static/core_explore_example_app/user/js/build_query.js` & `core_explore_example_app-2.3.0/core_explore_example_app/static/core_explore_example_app/user/js/build_query.js`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.2.0/core_explore_example_app/static/core_explore_example_app/user/js/build_query.raw.js` & `core_explore_example_app-2.3.0/core_explore_example_app/static/core_explore_example_app/user/js/build_query.raw.js`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.2.0/core_explore_example_app/static/core_explore_example_app/user/js/refresh_sorting.js` & `core_explore_example_app-2.3.0/core_explore_example_app/static/core_explore_example_app/user/js/refresh_sorting.js`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.2.0/core_explore_example_app/static/core_explore_example_app/user/js/select_fields.js` & `core_explore_example_app-2.3.0/core_explore_example_app/static/core_explore_example_app/user/js/select_fields.js`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.2.0/core_explore_example_app/tasks.py` & `core_explore_example_app-2.3.0/core_explore_example_app/tasks.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.2.0/core_explore_example_app/templates/core_explore_example_app/user/build_query.html` & `core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/build_query.html`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.2.0/core_explore_example_app/templates/core_explore_example_app/user/index.html` & `core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/index.html`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.2.0/core_explore_example_app/templates/core_explore_example_app/user/modals/custom_tree.html` & `core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/modals/custom_tree.html`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.2.0/core_explore_example_app/templates/core_explore_example_app/user/modals/delete_all_queries.html` & `core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/modals/delete_all_queries.html`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.2.0/core_explore_example_app/templates/core_explore_example_app/user/modals/delete_query.html` & `core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/modals/delete_query.html`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.2.0/core_explore_example_app/templates/core_explore_example_app/user/modals/sub_elements_query_builder.html` & `core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/modals/sub_elements_query_builder.html`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.2.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/new_query.html` & `core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/new_query.html`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.2.0/core_explore_example_app/templates/core_explore_example_app/user/results.html` & `core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/results.html`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.2.0/core_explore_example_app/urls.py` & `core_explore_example_app-2.3.0/core_explore_example_app/urls.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.2.0/core_explore_example_app/utils/custom_checkbox_renderer.py` & `core_explore_example_app-2.3.0/core_explore_example_app/utils/custom_checkbox_renderer.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.2.0/core_explore_example_app/utils/displayed_query.py` & `core_explore_example_app-2.3.0/core_explore_example_app/utils/displayed_query.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.2.0/core_explore_example_app/utils/mongo_query.py` & `core_explore_example_app-2.3.0/core_explore_example_app/utils/mongo_query.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.2.0/core_explore_example_app/utils/parser.py` & `core_explore_example_app-2.3.0/core_explore_example_app/utils/parser.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.2.0/core_explore_example_app/utils/query_builder.py` & `core_explore_example_app-2.3.0/core_explore_example_app/utils/query_builder.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.2.0/core_explore_example_app/utils/xml.py` & `core_explore_example_app-2.3.0/core_explore_example_app/utils/xml.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.2.0/core_explore_example_app/views/user/ajax.py` & `core_explore_example_app-2.3.0/core_explore_example_app/views/user/ajax.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.2.0/core_explore_example_app/views/user/views.py` & `core_explore_example_app-2.3.0/core_explore_example_app/views/user/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,45 +1,44 @@
 """Explore example user views
 """
 import json
 
-from django.urls import reverse_lazy, reverse
+from django.urls import reverse
 from django.utils.decorators import method_decorator
 from django.views.generic import View
 
-from core_main_app.commons import exceptions as exceptions
-from core_main_app.components.template import api as template_api
-from core_main_app.components.template_version_manager import (
-    api as template_version_manager_api,
-)
-from core_main_app.settings import DATA_SORTING_FIELDS
 import core_main_app.utils.decorators as decorators
-from core_main_app.utils.rendering import render
-
 from core_explore_common_app.components.query import api as query_api
 from core_explore_common_app.settings import DEFAULT_DATE_TOGGLE_VALUE
 from core_explore_common_app.views.user.views import (
     ResultQueryRedirectView,
     ResultsView,
 )
-from core_explore_example_app.permissions import rights
 from core_explore_example_app.components.explore_data_structure import (
     api as explore_data_structure_api,
 )
 from core_explore_example_app.components.persistent_query_example import (
     api as persistent_query_example_api,
 )
 from core_explore_example_app.components.persistent_query_example.models import (
     PersistentQueryExample,
 )
 from core_explore_example_app.components.saved_query import (
     api as saved_query_api,
 )
+from core_explore_example_app.permissions import rights
 from core_explore_example_app.settings import INSTALLED_APPS
 from core_explore_example_app.utils.parser import render_form
+from core_main_app.commons import exceptions as exceptions
+from core_main_app.components.template import api as template_api
+from core_main_app.components.template_version_manager import (
+    api as template_version_manager_api,
+)
+from core_main_app.settings import DATA_SORTING_FIELDS
+from core_main_app.utils.rendering import render
 
 
 class IndexView(View):
     """Index View"""
 
     api = template_version_manager_api
     get_redirect = "core_explore_example_app/user/index.html"
@@ -47,15 +46,14 @@
     build_query_redirect = "core_explore_example_build_query"
     object_name = "template"
 
     @method_decorator(
         decorators.permission_required(
             content_type=rights.EXPLORE_EXAMPLE_CONTENT_TYPE,
             permission=rights.EXPLORE_EXAMPLE_ACCESS,
-            login_url=reverse_lazy("core_main_app_login"),
         )
     )
     def get(self, request, *args, **kwargs):
         """Page that allows to select a template to start exploring data
 
         Args:
             request:
@@ -119,15 +117,14 @@
     remove_element_url = "core_explore_example_remove_element"
     generate_choice_url = "core_explore_example_generate_choice"
 
     @method_decorator(
         decorators.permission_required(
             content_type=rights.EXPLORE_EXAMPLE_CONTENT_TYPE,
             permission=rights.EXPLORE_EXAMPLE_ACCESS,
-            login_url=reverse_lazy("core_main_app_login"),
         )
     )
     def get(self, request, template_id, *args, **kwargs):
         """Loads view to customize exploration tree
 
         Args:
             request:
@@ -237,15 +234,14 @@
         "core_explore_example_app/user/query_builder/initial_form.html"
     )
 
     @method_decorator(
         decorators.permission_required(
             content_type=rights.EXPLORE_EXAMPLE_CONTENT_TYPE,
             permission=rights.EXPLORE_EXAMPLE_ACCESS,
-            login_url=reverse_lazy("core_main_app_login"),
         )
     )
     def get(self, request, template_id, query_id=None):
         """Page that allows to build and submit queries
 
         Args:
             request:
@@ -429,15 +425,14 @@
     back_to_query_redirect = "core_explore_example_build_query"
     get_query_url = "core_explore_example_get_query"
 
     @method_decorator(
         decorators.permission_required(
             content_type=rights.EXPLORE_EXAMPLE_CONTENT_TYPE,
             permission=rights.EXPLORE_EXAMPLE_ACCESS,
-            login_url=reverse_lazy("core_main_app_login"),
         )
     )
     def get(self, request, template_id, query_id):
         """Query results view
 
         Args:
             request:
@@ -527,15 +522,14 @@
     object_name = "persistent_query_example"
     redirect_url = "core_explore_example_results"
 
     @method_decorator(
         decorators.permission_required(
             content_type=rights.EXPLORE_EXAMPLE_CONTENT_TYPE,
             permission=rights.EXPLORE_EXAMPLE_ACCESS,
-            login_url=reverse_lazy("core_main_app_login"),
         )
     )
     def get(self, request, *args, **kwargs):
         return super().get(self, request, *args, **kwargs)
 
     @staticmethod
     def _get_persistent_query_by_id(persistent_query_id, user):
```

### Comparing `core_explore_example_app-2.2.0/core_explore_example_app.egg-info/PKG-INFO` & `core_explore_example_app-2.3.0/core_explore_example_app.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-explore-example-app
-Version: 2.2.0
+Version: 2.3.0
 Summary: Exploration by example for the curator core project
 Home-page: https://github.com/usnistgov/core_explore_example_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: ========================
         Core Explore Example App
```

### Comparing `core_explore_example_app-2.2.0/core_explore_example_app.egg-info/SOURCES.txt` & `core_explore_example_app-2.3.0/core_explore_example_app.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.md
 MANIFEST.in
 README.rst
 pyproject.toml
 requirements.core.txt
 setup.py
 core_explore_example_app/__init__.py
 core_explore_example_app/admin.py
```

### Comparing `core_explore_example_app-2.2.0/docs/conf.py` & `core_explore_example_app-2.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.2.0/setup.py` & `core_explore_example_app-2.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_explore_example_app",
-    version="2.2.0",
+    version="2.3.0",
     description="Exploration by example for the curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_explore_example_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_explore_example_app-2.2.0/tests/components/explore_data_structure/tests_unit.py` & `core_explore_example_app-2.3.0/tests/components/explore_data_structure/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.2.0/tests/components/persistent_query_example/fixtures/fixtures.py` & `core_explore_example_app-2.3.0/tests/components/persistent_query_example/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.2.0/tests/components/persistent_query_example/tests_int_access_control.py` & `core_explore_example_app-2.3.0/tests/components/persistent_query_example/tests_int_access_control.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
 
 from django.contrib.auth.models import AnonymousUser
 
 
 from core_main_app.access_control.exceptions import AccessControlError
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from core_explore_common_app.settings import (
     CAN_ANONYMOUS_ACCESS_PUBLIC_DOCUMENT,
 )
 import core_explore_example_app.components.persistent_query_example.api as persistent_query_example_api
 from core_explore_example_app.components.persistent_query_example.models import (
@@ -19,15 +19,15 @@
 from tests.components.persistent_query_example.fixtures.fixtures import (
     PersistentQueryExampleFixtures,
 )
 
 fixture_persistent_query_example = PersistentQueryExampleFixtures()
 
 
-class TestPersistentQueryExampleGetById(MongoIntegrationBaseTestCase):
+class TestPersistentQueryExampleGetById(IntegrationBaseTestCase):
     """Test Persistent Query Example Get By Id"""
 
     fixture = fixture_persistent_query_example
 
     def test_get_by_id_as_superuser_returns_persistent_query_example(self):
         """test_get_by_id_as_superuser_returns_persistent_query_example"""
 
@@ -109,15 +109,15 @@
         else:
             with self.assertRaises(AccessControlError):
                 persistent_query_example_api.get_by_id(
                     persistent_query_example_id, AnonymousUser()
                 )
 
 
-class TestPersistentQueryExampleGetByName(MongoIntegrationBaseTestCase):
+class TestPersistentQueryExampleGetByName(IntegrationBaseTestCase):
     """Test Persistent Query Example Get By Name"""
 
     fixture = fixture_persistent_query_example
 
     def test_get_by_name_as_superuser_returns_persistent_query_example(self):
         """test_get_by_name_as_superuser_returns_persistent_query_example"""
 
@@ -199,15 +199,15 @@
         else:
             with self.assertRaises(AccessControlError):
                 persistent_query_example_api.get_by_name(
                     persistent_query_example_name, AnonymousUser()
                 )
 
 
-class TestPersistentQueryExampleDelete(MongoIntegrationBaseTestCase):
+class TestPersistentQueryExampleDelete(IntegrationBaseTestCase):
     """Test Persistent Query Example Delete"""
 
     fixture = fixture_persistent_query_example
 
     def test_delete_others_persistent_query_example_as_superuser_deletes_persistent_query_example(
         self,
     ):
@@ -260,15 +260,15 @@
         # Act # Assert
         with self.assertRaises(AccessControlError):
             persistent_query_example_api.delete(
                 persistent_query_example, AnonymousUser()
             )
 
 
-class TestPersistentQueryExampleUpdate(MongoIntegrationBaseTestCase):
+class TestPersistentQueryExampleUpdate(IntegrationBaseTestCase):
     """Test Persistent Query Example Update"""
 
     fixture = fixture_persistent_query_example
 
     def test_update_others_persistent_query_example_as_superuser_updates_data_structure(
         self,
     ):
@@ -327,15 +327,15 @@
         # Act # Assert
         with self.assertRaises(AccessControlError):
             persistent_query_example_api.upsert(
                 persistent_query_example, AnonymousUser()
             )
 
 
-class TestPersistentQueryExampleCreate(MongoIntegrationBaseTestCase):
+class TestPersistentQueryExampleCreate(IntegrationBaseTestCase):
     """Test Persistent Query Example Create"""
 
     fixture = fixture_persistent_query_example
 
     def test_create_others_persistent_query_example_as_superuser_creates_persistent_query_example(
         self,
     ):
@@ -392,15 +392,15 @@
         else:
             with self.assertRaises(AccessControlError):
                 persistent_query_example_api.upsert(
                     persistent_query_example, AnonymousUser()
                 )
 
 
-class TestPersistentQueryExampleGetAll(MongoIntegrationBaseTestCase):
+class TestPersistentQueryExampleGetAll(IntegrationBaseTestCase):
     """Test Persistent Query Example Get All"""
 
     fixture = fixture_persistent_query_example
 
     def test_get_all_as_superuser_returns_all_persistent_query_example(self):
         """test_get_all_as_superuser_returns_all_persistent_query_example"""
 
@@ -427,15 +427,15 @@
         """test_get_all_as_anonymous_user_raises_error"""
 
         # Assert
         with self.assertRaises(AccessControlError):
             persistent_query_example_api.get_all(AnonymousUser())
 
 
-class TestPersistentQueryExampleGetAllByUser(MongoIntegrationBaseTestCase):
+class TestPersistentQueryExampleGetAllByUser(IntegrationBaseTestCase):
     """Test Persistent Query Example Get All By User"""
 
     fixture = fixture_persistent_query_example
 
     def test_get_all_by_user_as_superuser_returns_all_user_persistent_query_example(
         self,
     ):
```

### Comparing `core_explore_example_app-2.2.0/tests/components/persistent_query_example/tests_unit.py` & `core_explore_example_app-2.3.0/tests/components/persistent_query_example/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.2.0/tests/components/saved_query/tests_unit.py` & `core_explore_example_app-2.3.0/tests/components/saved_query/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.2.0/tests/rest/persistent_query_example/tests_int.py` & `core_explore_example_app-2.3.0/tests/rest/persistent_query_example/tests_int.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 """ Integration Test for Persistent Query Example Rest API
 """
 
 from django.contrib.auth.models import AnonymousUser
 from rest_framework import status
 
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from core_main_app.utils.tests_tools.RequestMock import RequestMock
 from core_explore_example_app.rest.persistent_query_example import (
     views as persistent_query_example_views,
 )
 from tests.components.persistent_query_example.fixtures.fixtures import (
     PersistentQueryExampleFixtures,
 )
 
 fixture_data_structure = PersistentQueryExampleFixtures()
 
 
-class TestPersistentQueryExampleListAdmin(MongoIntegrationBaseTestCase):
+class TestPersistentQueryExampleListAdmin(IntegrationBaseTestCase):
     """Test Persistent Query Example List Admin"""
 
     fixture = fixture_data_structure
 
     def setUp(self):
         """setUp"""
 
@@ -60,15 +60,15 @@
             data=self.data,
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_201_CREATED)
 
 
-class TestPersistentQueryExampleList(MongoIntegrationBaseTestCase):
+class TestPersistentQueryExampleList(IntegrationBaseTestCase):
     """Test Persistent Query Example List"""
 
     fixture = fixture_data_structure
 
     def setUp(self):
         """setUp"""
 
@@ -102,15 +102,15 @@
             data=self.data,
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_201_CREATED)
 
 
-class TestPersistentQueryExampleDetail(MongoIntegrationBaseTestCase):
+class TestPersistentQueryExampleDetail(IntegrationBaseTestCase):
     """Test Persistent Query Example Detail"""
 
     fixture = fixture_data_structure
 
     def setUp(self):
         """setUp"""
 
@@ -293,15 +293,15 @@
             param={"pk": -1},
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_404_NOT_FOUND)
 
 
-class TestPersistentQueryExampleByName(MongoIntegrationBaseTestCase):
+class TestPersistentQueryExampleByName(IntegrationBaseTestCase):
     """Test Persistent Query Example By Name"""
 
     fixture = fixture_data_structure
 
     def setUp(self):
         """setUp"""
```

### Comparing `core_explore_example_app-2.2.0/tests/rest/persistent_query_example/tests_permissions.py` & `core_explore_example_app-2.3.0/tests/rest/persistent_query_example/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.2.0/tests/rest/saved_query/fixtures/fixtures.py` & `core_explore_example_app-2.3.0/tests/rest/saved_query/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.2.0/tests/rest/saved_query/tests_int.py` & `core_explore_example_app-2.3.0/tests/rest/saved_query/tests_int.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """Integration tests for Saved Query rest api
 """
 
 from rest_framework import status
 
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from core_main_app.utils.tests_tools.RequestMock import RequestMock
 import core_explore_example_app.rest.saved_query.views as saved_query_views
 from tests.rest.saved_query.fixtures.fixtures import SavedQueryFixtures
 
 fixture_data = SavedQueryFixtures()
 
 
-class TestGetSavedQueryList(MongoIntegrationBaseTestCase):
+class TestGetSavedQueryList(IntegrationBaseTestCase):
     """Test Get Saved Query List"""
 
     fixture = fixture_data
 
     def setUp(self):
         """setUp"""
 
@@ -35,15 +35,15 @@
             saved_query_views.SavedQueryList.as_view(), user
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_200_OK)
 
 
-class TestGetSavedQueryDetail(MongoIntegrationBaseTestCase):
+class TestGetSavedQueryDetail(IntegrationBaseTestCase):
     """Test Get Saved Query Detail"""
 
     fixture = fixture_data
 
     def setUp(self):
         """setUp"""
 
@@ -103,15 +103,15 @@
 
         # Assert
         self.assertEqual(
             response.status_code, status.HTTP_500_INTERNAL_SERVER_ERROR
         )
 
 
-class TestDeleteSavedQueryDetail(MongoIntegrationBaseTestCase):
+class TestDeleteSavedQueryDetail(IntegrationBaseTestCase):
     """Test Delete Saved Query Detail"""
 
     fixture = fixture_data
 
     def setUp(self):
         """setUp"""
```

### Comparing `core_explore_example_app-2.2.0/tests/rest/saved_query/tests_permissions.py` & `core_explore_example_app-2.3.0/tests/rest/saved_query/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.2.0/tests/test_settings.py` & `core_explore_example_app-2.3.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.2.0/tests/utils/mongo_query/tests_unit.py` & `core_explore_example_app-2.3.0/tests/utils/mongo_query/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.2.0/tests/utils/xml/tests_unit.py` & `core_explore_example_app-2.3.0/tests/utils/xml/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.2.0/tests/views/ajax/tests_unit.py` & `core_explore_example_app-2.3.0/tests/views/ajax/tests_unit.py`

 * *Files identical despite different names*

