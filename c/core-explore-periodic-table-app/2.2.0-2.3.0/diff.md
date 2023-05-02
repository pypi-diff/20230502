# Comparing `tmp/core_explore_periodic_table_app-2.2.0.tar.gz` & `tmp/core_explore_periodic_table_app-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/core_explore_periodic_table_app-2.2.0.tar", last modified: Thu Feb 23 20:29:18 2023, max compression
+gzip compressed data, was "core_explore_periodic_table_app-2.3.0.tar", last modified: Tue May  2 19:38:29 2023, max compression
```

## Comparing `core_explore_periodic_table_app-2.2.0.tar` & `core_explore_periodic_table_app-2.3.0.tar`

### file list

```diff
@@ -1,127 +1,128 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:18.000000 core_explore_periodic_table_app-2.2.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      194 2023-02-23 20:29:13.000000 core_explore_periodic_table_app-2.2.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2483 2023-02-23 20:29:18.000000 core_explore_periodic_table_app-2.2.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1671 2023-02-23 20:29:13.000000 core_explore_periodic_table_app-2.2.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:16.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      128 2023-02-23 20:29:13.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1189 2023-02-23 20:29:13.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/admin.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      525 2023-02-23 20:29:13.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/apps.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:17.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:13.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:17.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/components/persistent_query_periodic_table/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:13.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/components/persistent_query_periodic_table/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      391 2023-02-23 20:29:13.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/components/persistent_query_periodic_table/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2524 2023-02-23 20:29:13.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/components/persistent_query_periodic_table/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2094 2023-02-23 20:29:13.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/components/persistent_query_periodic_table/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:17.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/components/search_operator_mapping/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:13.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/components/search_operator_mapping/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      342 2023-02-23 20:29:13.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/components/search_operator_mapping/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1124 2023-02-23 20:29:13.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/components/search_operator_mapping/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1053 2023-02-23 20:29:13.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/components/search_operator_mapping/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      498 2023-02-23 20:29:13.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/menus.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:17.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/migrations/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3194 2023-02-23 20:29:13.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/migrations/0001_initial.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:13.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/migrations/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      597 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:17.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/permissions/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/permissions/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1166 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/permissions/discover.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      187 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/permissions/rights.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:17.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:17.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/rest/persistent_query_periodic_table/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/rest/persistent_query_periodic_table/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3598 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/rest/persistent_query_periodic_table/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    13622 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/rest/persistent_query_periodic_table/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:17.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/rest/search_operator_mapping/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/rest/search_operator_mapping/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1455 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/rest/search_operator_mapping/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8161 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/rest/search_operator_mapping/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1947 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/rest/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      135 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:16.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:16.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:17.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       97 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/admin/form.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:16.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/common/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:17.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/common/xsd/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5699 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/common/xsd/default_chemical_element_type.xsd
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:16.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:16.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/css/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:17.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/css/periodic_table/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1747 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/css/periodic_table/periodic.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:17.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/js/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:17.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/js/periodic_table/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5531 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/js/periodic_table/periodic.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      354 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/js/persistent_query.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:16.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:16.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:16.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:17.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/admin/periodic_table_type/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      382 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/admin/periodic_table_type/manage_periodic_table_type.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:17.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/admin/periodic_table_type/selector/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      425 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/admin/periodic_table_type/selector/selector.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:17.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      914 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/user/index.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:17.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/user/periodic_table/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7406 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/user/periodic_table/periodic.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:17.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/user/selector/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      250 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/user/selector/data_sources_selector.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1001 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:17.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:17.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/views/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/views/admin/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1570 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/views/admin/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3600 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/views/admin/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:17.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      728 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/views/user/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2016 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/views/user/form.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14809 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/views/user/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:17.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2483 2023-02-23 20:29:16.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4816 2023-02-23 20:29:16.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-02-23 20:29:16.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      110 2023-02-23 20:29:16.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-02-23 20:29:16.000000 core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      170 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       84 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       26 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-02-23 20:29:18.000000 core_explore_periodic_table_app-2.2.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1463 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:17.000000 core_explore_periodic_table_app-2.2.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:17.000000 core_explore_periodic_table_app-2.2.0/tests/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/tests/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:17.000000 core_explore_periodic_table_app-2.2.0/tests/components/persistent_query_periodic_table/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/tests/components/persistent_query_periodic_table/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:17.000000 core_explore_periodic_table_app-2.2.0/tests/components/persistent_query_periodic_table/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/tests/components/persistent_query_periodic_table/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1788 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/tests/components/persistent_query_periodic_table/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17239 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/tests/components/persistent_query_periodic_table/tests_int_access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7296 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/tests/components/persistent_query_periodic_table/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:17.000000 core_explore_periodic_table_app-2.2.0/tests/components/search_operators_mapping/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/tests/components/search_operators_mapping/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4467 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/tests/components/search_operators_mapping/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:17.000000 core_explore_periodic_table_app-2.2.0/tests/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/tests/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:17.000000 core_explore_periodic_table_app-2.2.0/tests/rest/persistent_query_periodic_table/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/tests/rest/persistent_query_periodic_table/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12822 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/tests/rest/persistent_query_periodic_table/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    18854 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/tests/rest/persistent_query_periodic_table/tests_permissions.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:18.000000 core_explore_periodic_table_app-2.2.0/tests/rest/search_operators_mapping/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/tests/rest/search_operators_mapping/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:18.000000 core_explore_periodic_table_app-2.2.0/tests/rest/search_operators_mapping/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/tests/rest/search_operators_mapping/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3042 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/tests/rest/search_operators_mapping/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4444 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/tests/rest/search_operators_mapping/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11071 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/tests/rest/search_operators_mapping/tests_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1902 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/tests/test_settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:18.000000 core_explore_periodic_table_app-2.2.0/tests/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/tests/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:18.000000 core_explore_periodic_table_app-2.2.0/tests/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/tests/views/user/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:18.000000 core_explore_periodic_table_app-2.2.0/tests/views/user/forms/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/tests/views/user/forms/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1902 2023-02-23 20:29:14.000000 core_explore_periodic_table_app-2.2.0/tests/views/user/forms/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:29.531302 core_explore_periodic_table_app-2.3.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:38:24.000000 core_explore_periodic_table_app-2.3.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      194 2023-05-02 19:38:24.000000 core_explore_periodic_table_app-2.3.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2483 2023-05-02 19:38:29.525944 core_explore_periodic_table_app-2.3.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1671 2023-05-02 19:38:24.000000 core_explore_periodic_table_app-2.3.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:28.223165 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      128 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1189 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/admin.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      525 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/apps.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:28.347982 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:28.404736 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/components/persistent_query_periodic_table/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/components/persistent_query_periodic_table/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      391 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/components/persistent_query_periodic_table/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2524 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/components/persistent_query_periodic_table/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2094 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/components/persistent_query_periodic_table/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:28.466100 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/components/search_operator_mapping/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/components/search_operator_mapping/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      342 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/components/search_operator_mapping/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1124 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/components/search_operator_mapping/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1053 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/components/search_operator_mapping/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      498 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/menus.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:28.495948 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/migrations/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3194 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/migrations/0001_initial.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/migrations/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      597 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:28.572561 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/permissions/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/permissions/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1166 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/permissions/discover.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      187 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/permissions/rights.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:28.609959 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:28.670008 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/rest/persistent_query_periodic_table/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/rest/persistent_query_periodic_table/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3598 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/rest/persistent_query_periodic_table/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    13622 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/rest/persistent_query_periodic_table/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:28.726074 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/rest/search_operator_mapping/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/rest/search_operator_mapping/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1455 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/rest/search_operator_mapping/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8161 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/rest/search_operator_mapping/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1947 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/rest/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      135 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:27.802888 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:27.845489 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:28.744183 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       97 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/admin/form.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:27.824311 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/common/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:28.760705 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/common/xsd/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5699 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/common/xsd/default_chemical_element_type.xsd
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:27.856914 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:27.852135 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/css/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:28.780691 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/css/periodic_table/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1747 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/css/periodic_table/periodic.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:28.795607 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/js/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:28.811925 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/js/periodic_table/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5531 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/js/periodic_table/periodic.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      354 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/js/persistent_query.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:27.874597 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:27.896242 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:27.881298 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:28.832643 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/admin/periodic_table_type/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      382 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/admin/periodic_table_type/manage_periodic_table_type.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:28.847373 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/admin/periodic_table_type/selector/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      425 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/admin/periodic_table_type/selector/selector.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:28.885326 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      914 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/user/index.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:28.900873 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/user/periodic_table/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7406 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/user/periodic_table/periodic.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:28.917985 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/user/selector/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      250 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/user/selector/data_sources_selector.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1001 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:28.937184 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:28.987829 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/views/admin/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1570 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/views/admin/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3600 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/views/admin/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:29.048840 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      728 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/views/user/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2016 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/views/user/form.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14617 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/views/user/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:28.299639 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2483 2023-05-02 19:38:27.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4827 2023-05-02 19:38:27.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:38:27.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      110 2023-05-02 19:38:27.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:38:27.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      170 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       84 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       26 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:38:29.553960 core_explore_periodic_table_app-2.3.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1463 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:29.081654 core_explore_periodic_table_app-2.3.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:29.097543 core_explore_periodic_table_app-2.3.0/tests/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/tests/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:29.156423 core_explore_periodic_table_app-2.3.0/tests/components/persistent_query_periodic_table/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/tests/components/persistent_query_periodic_table/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:29.200154 core_explore_periodic_table_app-2.3.0/tests/components/persistent_query_periodic_table/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/tests/components/persistent_query_periodic_table/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1788 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/tests/components/persistent_query_periodic_table/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17193 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/tests/components/persistent_query_periodic_table/tests_int_access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7296 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/tests/components/persistent_query_periodic_table/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:29.235514 core_explore_periodic_table_app-2.3.0/tests/components/search_operators_mapping/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/tests/components/search_operators_mapping/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4467 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/tests/components/search_operators_mapping/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:29.255232 core_explore_periodic_table_app-2.3.0/tests/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/tests/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:29.311167 core_explore_periodic_table_app-2.3.0/tests/rest/persistent_query_periodic_table/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/tests/rest/persistent_query_periodic_table/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12797 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/tests/rest/persistent_query_periodic_table/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    18854 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/tests/rest/persistent_query_periodic_table/tests_permissions.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:29.375695 core_explore_periodic_table_app-2.3.0/tests/rest/search_operators_mapping/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/tests/rest/search_operators_mapping/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:29.412801 core_explore_periodic_table_app-2.3.0/tests/rest/search_operators_mapping/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/tests/rest/search_operators_mapping/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3042 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/tests/rest/search_operators_mapping/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4434 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/tests/rest/search_operators_mapping/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11061 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/tests/rest/search_operators_mapping/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1902 2023-05-02 19:38:26.000000 core_explore_periodic_table_app-2.3.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:29.436392 core_explore_periodic_table_app-2.3.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:26.000000 core_explore_periodic_table_app-2.3.0/tests/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:29.455752 core_explore_periodic_table_app-2.3.0/tests/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:26.000000 core_explore_periodic_table_app-2.3.0/tests/views/user/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:29.499180 core_explore_periodic_table_app-2.3.0/tests/views/user/forms/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:26.000000 core_explore_periodic_table_app-2.3.0/tests/views/user/forms/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1902 2023-05-02 19:38:26.000000 core_explore_periodic_table_app-2.3.0/tests/views/user/forms/tests_unit.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `core_explore_periodic_table_app-2.2.0/PKG-INFO` & `core_explore_periodic_table_app-2.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_explore_periodic_table_app
-Version: 2.2.0
+Version: 2.3.0
 Summary: Core explore periodic table capabilities for the curator core project
 Home-page: https://github.com/usnistgov/core_explore_periodic_table_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_explore_periodic_table_app
         ===============================
```

### Comparing `core_explore_periodic_table_app-2.2.0/README.rst` & `core_explore_periodic_table_app-2.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/admin.py` & `core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/admin.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/apps.py` & `core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/apps.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/components/persistent_query_periodic_table/api.py` & `core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/components/persistent_query_periodic_table/api.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/components/persistent_query_periodic_table/models.py` & `core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/components/persistent_query_periodic_table/models.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/components/search_operator_mapping/api.py` & `core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/components/search_operator_mapping/api.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/components/search_operator_mapping/models.py` & `core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/components/search_operator_mapping/models.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/migrations/0001_initial.py` & `core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/models.py` & `core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/models.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/permissions/discover.py` & `core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/permissions/discover.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/rest/persistent_query_periodic_table/serializers.py` & `core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/rest/persistent_query_periodic_table/serializers.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/rest/persistent_query_periodic_table/views.py` & `core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/rest/persistent_query_periodic_table/views.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/rest/search_operator_mapping/serializers.py` & `core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/rest/search_operator_mapping/serializers.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/rest/search_operator_mapping/views.py` & `core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/rest/search_operator_mapping/views.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/rest/urls.py` & `core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/rest/urls.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/common/xsd/default_chemical_element_type.xsd` & `core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/common/xsd/default_chemical_element_type.xsd`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/css/periodic_table/periodic.css` & `core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/css/periodic_table/periodic.css`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/js/periodic_table/periodic.js` & `core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/js/periodic_table/periodic.js`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/user/index.html` & `core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/user/index.html`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/user/periodic_table/periodic.html` & `core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/user/periodic_table/periodic.html`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/urls.py` & `core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/urls.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/views/admin/forms.py` & `core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/views/admin/forms.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/views/admin/views.py` & `core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/views/admin/views.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/views/user/ajax.py` & `core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/views/user/ajax.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/views/user/form.py` & `core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/views/user/form.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app/views/user/views.py` & `core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/views/user/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,57 +1,55 @@
 """ Periodic table's views
 """
 
 from typing import Dict, Any, List
 
-from django.urls import reverse, reverse_lazy
+from django.urls import reverse
 from django.utils.decorators import method_decorator
 
 import core_main_app.components.template_version_manager.api as template_version_manager_api
 import core_main_app.utils.decorators as decorators
-from core_main_app.commons.exceptions import DoesNotExist
-from core_main_app.components.template import api as template_api
-from core_main_app.settings import DATA_SORTING_FIELDS
-from core_main_app.utils.rendering import render
 from core_explore_common_app.components.query import api as query_api
 from core_explore_common_app.views.user.views import (
     ResultsView,
     ResultQueryRedirectView,
 )
-
 from core_explore_keyword_app.components.search_operator import (
     api as search_operator_api,
 )
 from core_explore_keyword_app.views.user.views import KeywordSearchView
 from core_explore_periodic_table_app.components.persistent_query_periodic_table import (
     api as persistent_query_periodic_table_api,
 )
 from core_explore_periodic_table_app.components.persistent_query_periodic_table.models import (
     PersistentQueryPeriodicTable,
 )
 from core_explore_periodic_table_app.components.search_operator_mapping import (
     api as search_operator_mapping_api,
 )
-from core_explore_periodic_table_app.views.user.form import PeriodicTableForm
 from core_explore_periodic_table_app.permissions import rights
+from core_explore_periodic_table_app.views.user.form import PeriodicTableForm
+from core_main_app.commons.exceptions import DoesNotExist
+from core_main_app.components.template import api as template_api
+from core_main_app.settings import DATA_SORTING_FIELDS
+from core_main_app.utils.rendering import render
 
 
 class PeriodicTableBuildQueryView(KeywordSearchView):
     """Periodic Table Build Query View"""
 
     results_url = "core_explore_periodic_table_results"
     query_builder_interface = (
         "core_explore_periodic_table_app/user/periodic_table/periodic.html"
     )
 
     @method_decorator(
         decorators.permission_required(
             content_type=rights.EXPLORE_PERIODIC_TABLE_CONTENT_TYPE,
             permission=rights.EXPLORE_PERIODIC_TABLE_ACCESS,
-            login_url=reverse_lazy("core_main_app_login"),
         )
     )
     def get(self, request, **kwargs):
         """GET
 
         Args:
             request:
@@ -138,15 +136,14 @@
             search_form, error, None, default_order
         )
 
     @method_decorator(
         decorators.permission_required(
             content_type=rights.EXPLORE_PERIODIC_TABLE_CONTENT_TYPE,
             permission=rights.EXPLORE_PERIODIC_TABLE_ACCESS,
-            login_url=reverse_lazy("core_main_app_login"),
         )
     )
     def post(self, request):
         """POST
 
         Args:
             request:
@@ -390,15 +387,14 @@
     object_name = "persistent_query_periodic_table"
     redirect_url = "core_explore_periodic_table_index"
 
     @method_decorator(
         decorators.permission_required(
             content_type=rights.EXPLORE_PERIODIC_TABLE_CONTENT_TYPE,
             permission=rights.EXPLORE_PERIODIC_TABLE_ACCESS,
-            login_url=reverse_lazy("core_main_app_login"),
         )
     )
     def get(self, request, *args, **kwargs):
         return super().get(self, request, *args, **kwargs)
 
     @staticmethod
     def _get_persistent_query_by_id(persistent_query_id, user):
```

### Comparing `core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app.egg-info/PKG-INFO` & `core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-explore-periodic-table-app
-Version: 2.2.0
+Version: 2.3.0
 Summary: Core explore periodic table capabilities for the curator core project
 Home-page: https://github.com/usnistgov/core_explore_periodic_table_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_explore_periodic_table_app
         ===============================
```

### Comparing `core_explore_periodic_table_app-2.2.0/core_explore_periodic_table_app.egg-info/SOURCES.txt` & `core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app.egg-info/SOURCES.txt`

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
 core_explore_periodic_table_app/__init__.py
```

### Comparing `core_explore_periodic_table_app-2.2.0/setup.py` & `core_explore_periodic_table_app-2.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_explore_periodic_table_app",
-    version="2.2.0",
+    version="2.3.0",
     description="Core explore periodic table capabilities for the curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_explore_periodic_table_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_explore_periodic_table_app-2.2.0/tests/components/persistent_query_periodic_table/fixtures/fixtures.py` & `core_explore_periodic_table_app-2.3.0/tests/components/persistent_query_periodic_table/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.2.0/tests/components/persistent_query_periodic_table/tests_int_access_control.py` & `core_explore_periodic_table_app-2.3.0/tests/components/persistent_query_periodic_table/tests_int_access_control.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """ Unit Test Persistent Query Periodic Table
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
 from core_explore_periodic_table_app.components.persistent_query_periodic_table import (
@@ -23,15 +23,15 @@
 )
 
 fixture_persistent_query_periodic_table = (
     PersistentQueryPeriodicTableFixtures()
 )
 
 
-class TestPersistentQueryPeriodicTableGetById(MongoIntegrationBaseTestCase):
+class TestPersistentQueryPeriodicTableGetById(IntegrationBaseTestCase):
     """Test Persistent Query Periodic Table Get By Id"""
 
     fixture = fixture_persistent_query_periodic_table
 
     def test_get_by_id_as_superuser_returns_persistent_query_periodic_table(
         self,
     ):
@@ -122,15 +122,15 @@
                     persistent_query_periodic_table_id, mock_user
                 ),
                 PersistentQueryPeriodicTable,
             )
         )
 
 
-class TestPersistentQueryPeriodicTableGetByName(MongoIntegrationBaseTestCase):
+class TestPersistentQueryPeriodicTableGetByName(IntegrationBaseTestCase):
     """Test Persistent Query Periodic Table Get By Name"""
 
     fixture = fixture_persistent_query_periodic_table
 
     def test_get_by_name_as_superuser_returns_persistent_query_periodic_table(
         self,
     ):
@@ -222,15 +222,15 @@
         else:
             with self.assertRaises(AccessControlError):
                 persistent_query_periodic_table_api.get_by_name(
                     persistent_query_periodic_table_name, AnonymousUser()
                 )
 
 
-class TestPersistentQueryPeriodicTableDelete(MongoIntegrationBaseTestCase):
+class TestPersistentQueryPeriodicTableDelete(IntegrationBaseTestCase):
     """Test Persistent Query Periodic Table Delete"""
 
     fixture = fixture_persistent_query_periodic_table
 
     def test_delete_others_as_superuser_deletes_persistent_query_periodic_table(
         self,
     ):
@@ -291,15 +291,15 @@
         # Act # Assert
         with self.assertRaises(AccessControlError):
             persistent_query_periodic_table_api.delete(
                 persistent_query_periodic_table, AnonymousUser()
             )
 
 
-class TestPersistentQueryPeriodicTableUpdate(MongoIntegrationBaseTestCase):
+class TestPersistentQueryPeriodicTableUpdate(IntegrationBaseTestCase):
     """Test Persistent Query Periodic Table Update"""
 
     fixture = fixture_persistent_query_periodic_table
 
     def test_update_others_as_superuser_updates_persistent_query_periodic_table(
         self,
     ):
@@ -377,15 +377,15 @@
         # Act # Assert
         with self.assertRaises(AccessControlError):
             persistent_query_periodic_table_api.upsert(
                 persistent_query_periodic_table, AnonymousUser()
             )
 
 
-class TestPersistentQueryPeriodicTableCreate(MongoIntegrationBaseTestCase):
+class TestPersistentQueryPeriodicTableCreate(IntegrationBaseTestCase):
     """Test Persistent Query Periodic Table Create"""
 
     fixture = fixture_persistent_query_periodic_table
 
     def test_create_for_others_as_superuser_creates_persistent_query_periodic_table(
         self,
     ):
@@ -443,15 +443,15 @@
         else:
             with self.assertRaises(AccessControlError):
                 persistent_query_periodic_table_api.upsert(
                     persistent_query_periodic_table, AnonymousUser()
                 )
 
 
-class TestPersistentQueryPeriodicTableGetAll(MongoIntegrationBaseTestCase):
+class TestPersistentQueryPeriodicTableGetAll(IntegrationBaseTestCase):
     """Test Persistent Query Periodic Table Get All"""
 
     fixture = fixture_persistent_query_periodic_table
 
     def test_get_all_as_superuser_returns_all_persistent_query_periodic_table(
         self,
     ):
@@ -480,17 +480,15 @@
         """test_get_all_as_anonymous_user_raises_error"""
 
         # Assert
         with self.assertRaises(AccessControlError):
             persistent_query_periodic_table_api.get_all(AnonymousUser())
 
 
-class TestPersistentQueryPeriodicTableGetAllByUser(
-    MongoIntegrationBaseTestCase
-):
+class TestPersistentQueryPeriodicTableGetAllByUser(IntegrationBaseTestCase):
     """Test Persistent Query Periodic Table Get All By User"""
 
     fixture = fixture_persistent_query_periodic_table
 
     def test_get_all_by_user_as_superuser_returns_all_user_persistent_query_periodic_table(
         self,
     ):
```

### Comparing `core_explore_periodic_table_app-2.2.0/tests/components/persistent_query_periodic_table/tests_unit.py` & `core_explore_periodic_table_app-2.3.0/tests/components/persistent_query_periodic_table/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.2.0/tests/components/search_operators_mapping/tests_unit.py` & `core_explore_periodic_table_app-2.3.0/tests/components/search_operators_mapping/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.2.0/tests/rest/persistent_query_periodic_table/tests_int.py` & `core_explore_periodic_table_app-2.3.0/tests/rest/persistent_query_periodic_table/tests_int.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 """ Integration Test for Persistent Query PeriodicTable Rest API
 """
 
 from django.contrib.auth.models import AnonymousUser
 from rest_framework import status
 
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from core_main_app.utils.tests_tools.RequestMock import RequestMock
 from core_explore_periodic_table_app.rest.persistent_query_periodic_table import (
     views as persistent_query_periodic_table_views,
 )
 from tests.components.persistent_query_periodic_table.fixtures.fixtures import (
     PersistentQueryPeriodicTableFixtures,
 )
 
 fixture_data_structure = PersistentQueryPeriodicTableFixtures()
 
 
-class TestPersistentQueryPeriodicTableListAdmin(MongoIntegrationBaseTestCase):
+class TestPersistentQueryPeriodicTableListAdmin(IntegrationBaseTestCase):
     """Test Persistent Query Periodic Table List Admin"""
 
     fixture = fixture_data_structure
 
     def setUp(self):
         """setUp"""
 
@@ -60,15 +60,15 @@
             data=self.data,
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_201_CREATED)
 
 
-class TestPersistentQueryPeriodicTableList(MongoIntegrationBaseTestCase):
+class TestPersistentQueryPeriodicTableList(IntegrationBaseTestCase):
     """Test Persistent Query Periodic Table List"""
 
     fixture = fixture_data_structure
 
     def setUp(self):
         """setUp"""
 
@@ -103,15 +103,15 @@
             data=self.data,
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_201_CREATED)
 
 
-class TestPersistentQueryPeriodicTableDetail(MongoIntegrationBaseTestCase):
+class TestPersistentQueryPeriodicTableDetail(IntegrationBaseTestCase):
     """Test Persistent Query Periodic Table Detail"""
 
     fixture = fixture_data_structure
 
     def setUp(self):
         """setUp"""
 
@@ -317,15 +317,15 @@
             param={"pk": "-1"},
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_404_NOT_FOUND)
 
 
-class TestPersistentQueryPeriodicTableGetByName(MongoIntegrationBaseTestCase):
+class TestPersistentQueryPeriodicTableGetByName(IntegrationBaseTestCase):
     """Test Persistent Query Periodic Table Get By Name"""
 
     fixture = fixture_data_structure
 
     def setUp(self):
         """setUp"""
```

### Comparing `core_explore_periodic_table_app-2.2.0/tests/rest/persistent_query_periodic_table/tests_permissions.py` & `core_explore_periodic_table_app-2.3.0/tests/rest/persistent_query_periodic_table/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.2.0/tests/rest/search_operators_mapping/fixtures/fixtures.py` & `core_explore_periodic_table_app-2.3.0/tests/rest/search_operators_mapping/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.2.0/tests/rest/search_operators_mapping/tests_int.py` & `core_explore_periodic_table_app-2.3.0/tests/rest/search_operators_mapping/tests_int.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """ Integration Test Persistent Query Periodic Table
 """
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from core_main_app.utils.tests_tools.RequestMock import RequestMock
 
 from core_explore_periodic_table_app.rest.search_operator_mapping import (
     views as search_operator_mapping_views,
 )
 from tests.rest.search_operators_mapping.fixtures.fixtures import (
     SearchOperatorMappingFixtures,
 )
 
 fixture_search_operator_mapping = SearchOperatorMappingFixtures()
 
 
-class TestSearchOperatorMapping(MongoIntegrationBaseTestCase):
+class TestSearchOperatorMapping(IntegrationBaseTestCase):
     """Test Search Operator Mapping"""
 
     fixture = fixture_search_operator_mapping
 
     def test_get_all_search_operator_mapping_return_collection(self):
         """test_get_all_search_operator_mapping_return_collection"""
```

### Comparing `core_explore_periodic_table_app-2.2.0/tests/rest/search_operators_mapping/tests_permissions.py` & `core_explore_periodic_table_app-2.3.0/tests/rest/search_operators_mapping/tests_permissions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """ Permission Tests for Persistent Query Periodic Table
 """
 
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from core_main_app.utils.tests_tools.RequestMock import RequestMock
 from core_explore_periodic_table_app.rest.search_operator_mapping import (
     views as search_operator_mapping_views,
 )
 from tests.rest.search_operators_mapping.fixtures.fixtures import (
     SearchOperatorMappingFixtures,
 )
 
 fixture_search_operator_mapping = SearchOperatorMappingFixtures()
 
 
-class TestSearchOperatorMappingPermissions(MongoIntegrationBaseTestCase):
+class TestSearchOperatorMappingPermissions(IntegrationBaseTestCase):
     """Test Search Operator Mapping Permissions"""
 
     fixture = fixture_search_operator_mapping
 
     def test_get_all_staff_return_200(self):
         """test_get_all_staff_return_200"""
```

### Comparing `core_explore_periodic_table_app-2.2.0/tests/test_settings.py` & `core_explore_periodic_table_app-2.3.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.2.0/tests/views/user/forms/tests_unit.py` & `core_explore_periodic_table_app-2.3.0/tests/views/user/forms/tests_unit.py`

 * *Files identical despite different names*

