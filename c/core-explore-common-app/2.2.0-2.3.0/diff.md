# Comparing `tmp/core_explore_common_app-2.2.0.tar.gz` & `tmp/core_explore_common_app-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/core_explore_common_app-2.2.0.tar", last modified: Thu Feb 23 20:28:02 2023, max compression
+gzip compressed data, was "core_explore_common_app-2.3.0.tar", last modified: Tue May  2 19:37:08 2023, max compression
```

## Comparing `core_explore_common_app-2.2.0.tar` & `core_explore_common_app-2.3.0.tar`

### file list

```diff
@@ -1,143 +1,168 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:02.000000 core_explore_common_app-2.2.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      154 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1108 2023-02-23 20:28:02.000000 core_explore_common_app-2.2.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      607 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:00.000000 core_explore_common_app-2.2.0/core_explore_common_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       79 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:00.000000 core_explore_common_app-2.2.0/core_explore_common_app/access_control/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/access_control/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4255 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/access_control/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      282 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/admin.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      450 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/apps.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:00.000000 core_explore_common_app-2.2.0/core_explore_common_app/commons/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/commons/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      409 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/commons/exceptions.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:00.000000 core_explore_common_app-2.2.0/core_explore_common_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:00.000000 core_explore_common_app-2.2.0/core_explore_common_app/components/abstract_persistent_query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/components/abstract_persistent_query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2123 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/components/abstract_persistent_query/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      552 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/components/abstract_persistent_query/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:00.000000 core_explore_common_app-2.2.0/core_explore_common_app/components/abstract_query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/components/abstract_query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1583 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/components/abstract_query/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:00.000000 core_explore_common_app-2.2.0/core_explore_common_app/components/query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/components/query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      372 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/components/query/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3404 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/components/query/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1335 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/components/query/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:00.000000 core_explore_common_app-2.2.0/core_explore_common_app/components/result/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/components/result/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      565 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/components/result/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      172 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/constants.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      876 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/discover.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:00.000000 core_explore_common_app-2.2.0/core_explore_common_app/migrations/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2499 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/migrations/0001_initial.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/migrations/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:01.000000 core_explore_common_app-2.2.0/core_explore_common_app/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:01.000000 core_explore_common_app-2.2.0/core_explore_common_app/rest/query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/rest/query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4032 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/rest/query/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:01.000000 core_explore_common_app-2.2.0/core_explore_common_app/rest/result/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/rest/result/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      485 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/rest/result/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1768 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/rest/result/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      522 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/rest/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2200 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:00.000000 core_explore_common_app-2.2.0/core_explore_common_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:00.000000 core_explore_common_app-2.2.0/core_explore_common_app/static/core_explore_common_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:00.000000 core_explore_common_app-2.2.0/core_explore_common_app/static/core_explore_common_app/common/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:01.000000 core_explore_common_app-2.2.0/core_explore_common_app/static/core_explore_common_app/common/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      734 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/static/core_explore_common_app/common/js/tools.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:00.000000 core_explore_common_app-2.2.0/core_explore_common_app/static/core_explore_common_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:01.000000 core_explore_common_app-2.2.0/core_explore_common_app/static/core_explore_common_app/user/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      121 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/static/core_explore_common_app/user/css/query_result.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2184 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/static/core_explore_common_app/user/css/results.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3484 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/static/core_explore_common_app/user/css/toggle.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:01.000000 core_explore_common_app-2.2.0/core_explore_common_app/static/core_explore_common_app/user/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1629 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/static/core_explore_common_app/user/js/local_selector.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2616 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/static/core_explore_common_app/user/js/persistent_query_config.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8510 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/static/core_explore_common_app/user/js/results.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      409 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/static/core_explore_common_app/user/js/results.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7244 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/static/core_explore_common_app/user/js/sorting_multi_criteria.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5507 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/static/core_explore_common_app/user/js/sorting_single_criteria.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:01.000000 core_explore_common_app-2.2.0/core_explore_common_app/system/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/system/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      190 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/system/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1049 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/tasks.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:00.000000 core_explore_common_app-2.2.0/core_explore_common_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:00.000000 core_explore_common_app-2.2.0/core_explore_common_app/templates/core_explore_common_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:00.000000 core_explore_common_app-2.2.0/core_explore_common_app/templates/core_explore_common_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:01.000000 core_explore_common_app-2.2.0/core_explore_common_app/templates/core_explore_common_app/admin/persistent_query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      300 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/templates/core_explore_common_app/admin/persistent_query/content_query_box.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      342 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/templates/core_explore_common_app/admin/persistent_query/view_query_content.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:01.000000 core_explore_common_app-2.2.0/core_explore_common_app/templates/core_explore_common_app/commons/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      363 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/templates/core_explore_common_app/commons/query_content.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:00.000000 core_explore_common_app-2.2.0/core_explore_common_app/templates/core_explore_common_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:01.000000 core_explore_common_app-2.2.0/core_explore_common_app/templates/core_explore_common_app/user/ordering_menu/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      592 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/templates/core_explore_common_app/user/ordering_menu/multi_criteria_sorting_menu.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      716 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/templates/core_explore_common_app/user/ordering_menu/single_criteria_sorting_menu.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:01.000000 core_explore_common_app-2.2.0/core_explore_common_app/templates/core_explore_common_app/user/persistent_query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      429 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/templates/core_explore_common_app/user/persistent_query/button.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      831 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/templates/core_explore_common_app/user/persistent_query/modal.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      317 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/templates/core_explore_common_app/user/persistent_query/persistent_query_content.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3163 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/templates/core_explore_common_app/user/persistent_query/persistent_query_pagination.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:01.000000 core_explore_common_app-2.2.0/core_explore_common_app/templates/core_explore_common_app/user/results/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1543 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/templates/core_explore_common_app/user/results/data_source_info.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1266 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/templates/core_explore_common_app/user/results/data_source_pagination.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      701 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/templates/core_explore_common_app/user/results/data_source_results.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2748 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/templates/core_explore_common_app/user/results/data_sources_results.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       92 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/templates/core_explore_common_app/user/results/results.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:01.000000 core_explore_common_app-2.2.0/core_explore_common_app/templates/core_explore_common_app/user/selector/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      784 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/templates/core_explore_common_app/user/selector/data_sources_selector.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      324 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/templates/core_explore_common_app/user/selector/list_selector_base.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      311 2023-02-23 20:27:56.000000 core_explore_common_app-2.2.0/core_explore_common_app/templates/core_explore_common_app/user/selector/local_content.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      723 2023-02-23 20:27:57.000000 core_explore_common_app-2.2.0/core_explore_common_app/templates/core_explore_common_app/user/selector/local_selector.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1359 2023-02-23 20:27:57.000000 core_explore_common_app-2.2.0/core_explore_common_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:01.000000 core_explore_common_app-2.2.0/core_explore_common_app/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:57.000000 core_explore_common_app-2.2.0/core_explore_common_app/utils/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:01.000000 core_explore_common_app-2.2.0/core_explore_common_app/utils/protocols/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:57.000000 core_explore_common_app-2.2.0/core_explore_common_app/utils/protocols/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      263 2023-02-23 20:27:57.000000 core_explore_common_app-2.2.0/core_explore_common_app/utils/protocols/commons.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3055 2023-02-23 20:27:57.000000 core_explore_common_app-2.2.0/core_explore_common_app/utils/protocols/oauth2.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:01.000000 core_explore_common_app-2.2.0/core_explore_common_app/utils/query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:57.000000 core_explore_common_app-2.2.0/core_explore_common_app/utils/query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4826 2023-02-23 20:27:57.000000 core_explore_common_app-2.2.0/core_explore_common_app/utils/query/query.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:01.000000 core_explore_common_app-2.2.0/core_explore_common_app/utils/result/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:57.000000 core_explore_common_app-2.2.0/core_explore_common_app/utils/result/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1377 2023-02-23 20:27:57.000000 core_explore_common_app-2.2.0/core_explore_common_app/utils/result/result.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:01.000000 core_explore_common_app-2.2.0/core_explore_common_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:57.000000 core_explore_common_app-2.2.0/core_explore_common_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:01.000000 core_explore_common_app-2.2.0/core_explore_common_app/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:57.000000 core_explore_common_app-2.2.0/core_explore_common_app/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12976 2023-02-23 20:27:57.000000 core_explore_common_app-2.2.0/core_explore_common_app/views/user/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8912 2023-02-23 20:27:57.000000 core_explore_common_app-2.2.0/core_explore_common_app/views/user/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:00.000000 core_explore_common_app-2.2.0/core_explore_common_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1108 2023-02-23 20:27:59.000000 core_explore_common_app-2.2.0/core_explore_common_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5442 2023-02-23 20:27:59.000000 core_explore_common_app-2.2.0/core_explore_common_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-02-23 20:27:59.000000 core_explore_common_app-2.2.0/core_explore_common_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       69 2023-02-23 20:27:59.000000 core_explore_common_app-2.2.0/core_explore_common_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       30 2023-02-23 20:27:59.000000 core_explore_common_app-2.2.0/core_explore_common_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-02-23 20:27:57.000000 core_explore_common_app-2.2.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       21 2023-02-23 20:27:57.000000 core_explore_common_app-2.2.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-02-23 20:28:02.000000 core_explore_common_app-2.2.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1479 2023-02-23 20:27:57.000000 core_explore_common_app-2.2.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:01.000000 core_explore_common_app-2.2.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:57.000000 core_explore_common_app-2.2.0/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:01.000000 core_explore_common_app-2.2.0/tests/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:57.000000 core_explore_common_app-2.2.0/tests/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:01.000000 core_explore_common_app-2.2.0/tests/components/abstract_persistent_query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:57.000000 core_explore_common_app-2.2.0/tests/components/abstract_persistent_query/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:01.000000 core_explore_common_app-2.2.0/tests/components/query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:57.000000 core_explore_common_app-2.2.0/tests/components/query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6566 2023-02-23 20:27:57.000000 core_explore_common_app-2.2.0/tests/components/query/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:02.000000 core_explore_common_app-2.2.0/tests/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:57.000000 core_explore_common_app-2.2.0/tests/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:02.000000 core_explore_common_app-2.2.0/tests/rest/query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:57.000000 core_explore_common_app-2.2.0/tests/rest/query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3859 2023-02-23 20:27:57.000000 core_explore_common_app-2.2.0/tests/rest/query/tests_permissions.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:02.000000 core_explore_common_app-2.2.0/tests/rest/result/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:57.000000 core_explore_common_app-2.2.0/tests/rest/result/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2544 2023-02-23 20:27:57.000000 core_explore_common_app-2.2.0/tests/rest/result/tests_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1656 2023-02-23 20:27:57.000000 core_explore_common_app-2.2.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:08.215032 core_explore_common_app-2.3.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      154 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1108 2023-05-02 19:37:08.209615 core_explore_common_app-2.3.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      607 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:06.280068 core_explore_common_app-2.3.0/core_explore_common_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       79 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:06.399536 core_explore_common_app-2.3.0/core_explore_common_app/access_control/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/access_control/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4733 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/access_control/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      282 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/admin.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      450 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/apps.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:06.442895 core_explore_common_app-2.3.0/core_explore_common_app/commons/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/commons/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      409 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/commons/exceptions.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:06.458115 core_explore_common_app-2.3.0/core_explore_common_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:06.518655 core_explore_common_app-2.3.0/core_explore_common_app/components/abstract_persistent_query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/components/abstract_persistent_query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2123 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/components/abstract_persistent_query/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      552 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/components/abstract_persistent_query/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:06.550774 core_explore_common_app-2.3.0/core_explore_common_app/components/abstract_query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/components/abstract_query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1583 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/components/abstract_query/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:06.624738 core_explore_common_app-2.3.0/core_explore_common_app/components/query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/components/query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      372 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/components/query/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3755 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/components/query/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1335 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/components/query/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:06.664917 core_explore_common_app-2.3.0/core_explore_common_app/components/result/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/components/result/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      565 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/components/result/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      172 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/constants.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      876 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/discover.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:06.692537 core_explore_common_app-2.3.0/core_explore_common_app/migrations/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2499 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/migrations/0001_initial.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/migrations/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:06.772621 core_explore_common_app-2.3.0/core_explore_common_app/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:06.825594 core_explore_common_app-2.3.0/core_explore_common_app/rest/query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/rest/query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5208 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/rest/query/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:06.870901 core_explore_common_app-2.3.0/core_explore_common_app/rest/result/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/rest/result/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      485 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/rest/result/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1768 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/rest/result/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      308 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/rest/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2200 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:05.872755 core_explore_common_app-2.3.0/core_explore_common_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:05.891308 core_explore_common_app-2.3.0/core_explore_common_app/static/core_explore_common_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:05.883813 core_explore_common_app-2.3.0/core_explore_common_app/static/core_explore_common_app/common/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:06.892797 core_explore_common_app-2.3.0/core_explore_common_app/static/core_explore_common_app/common/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      734 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/static/core_explore_common_app/common/js/tools.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:05.899977 core_explore_common_app-2.3.0/core_explore_common_app/static/core_explore_common_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:06.950914 core_explore_common_app-2.3.0/core_explore_common_app/static/core_explore_common_app/user/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      121 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/static/core_explore_common_app/user/css/query_result.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2208 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/static/core_explore_common_app/user/css/results.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3484 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/static/core_explore_common_app/user/css/toggle.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:07.053847 core_explore_common_app-2.3.0/core_explore_common_app/static/core_explore_common_app/user/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1629 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/static/core_explore_common_app/user/js/local_selector.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2616 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/static/core_explore_common_app/user/js/persistent_query_config.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8849 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/static/core_explore_common_app/user/js/results.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      479 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/static/core_explore_common_app/user/js/results.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7244 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/static/core_explore_common_app/user/js/sorting_multi_criteria.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5507 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/static/core_explore_common_app/user/js/sorting_single_criteria.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:07.091793 core_explore_common_app-2.3.0/core_explore_common_app/system/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/system/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      190 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/system/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1049 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/tasks.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:05.931352 core_explore_common_app-2.3.0/core_explore_common_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:05.949025 core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:05.937948 core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:07.138701 core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/admin/persistent_query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      300 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/admin/persistent_query/content_query_box.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      342 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/admin/persistent_query/view_query_content.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:07.154588 core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/commons/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      363 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/commons/query_content.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:05.965870 core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:07.186762 core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/ordering_menu/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      592 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/ordering_menu/multi_criteria_sorting_menu.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      716 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/ordering_menu/single_criteria_sorting_menu.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:07.252514 core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/persistent_query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      429 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/persistent_query/button.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      831 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/persistent_query/modal.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      317 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/persistent_query/persistent_query_content.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3163 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/persistent_query/persistent_query_pagination.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:07.381616 core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/results/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1785 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/results/data_source_info.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1266 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/results/data_source_pagination.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      701 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/results/data_source_results.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2748 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/results/data_sources_results.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       92 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/results/results.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:07.460884 core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/selector/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      784 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/selector/data_sources_selector.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      324 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/selector/list_selector_base.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      311 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/selector/local_content.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      723 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/selector/local_selector.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1359 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:07.479569 core_explore_common_app-2.3.0/core_explore_common_app/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/utils/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:07.525778 core_explore_common_app-2.3.0/core_explore_common_app/utils/linked_records/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/utils/linked_records/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1003 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/utils/linked_records/pid.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:07.562912 core_explore_common_app-2.3.0/core_explore_common_app/utils/oaipmh/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/utils/oaipmh/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      597 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/utils/oaipmh/oaipmh.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:07.627604 core_explore_common_app-2.3.0/core_explore_common_app/utils/protocols/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/utils/protocols/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      263 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/utils/protocols/commons.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3055 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/utils/protocols/oauth2.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:07.671207 core_explore_common_app-2.3.0/core_explore_common_app/utils/query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/utils/query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3361 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/utils/query/query.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:07.705013 core_explore_common_app-2.3.0/core_explore_common_app/utils/result/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/utils/result/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1377 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/utils/result/result.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:07.725114 core_explore_common_app-2.3.0/core_explore_common_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:07.786955 core_explore_common_app-2.3.0/core_explore_common_app/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14720 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/views/user/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8846 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/views/user/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:06.368117 core_explore_common_app-2.3.0/core_explore_common_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1108 2023-05-02 19:37:05.000000 core_explore_common_app-2.3.0/core_explore_common_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6019 2023-05-02 19:37:05.000000 core_explore_common_app-2.3.0/core_explore_common_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:37:05.000000 core_explore_common_app-2.3.0/core_explore_common_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       69 2023-05-02 19:37:05.000000 core_explore_common_app-2.3.0/core_explore_common_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       30 2023-05-02 19:37:05.000000 core_explore_common_app-2.3.0/core_explore_common_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:37:03.000000 core_explore_common_app-2.3.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       21 2023-05-02 19:37:03.000000 core_explore_common_app-2.3.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:37:08.216755 core_explore_common_app-2.3.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1479 2023-05-02 19:37:03.000000 core_explore_common_app-2.3.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:07.835449 core_explore_common_app-2.3.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:03.000000 core_explore_common_app-2.3.0/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:07.849887 core_explore_common_app-2.3.0/tests/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:03.000000 core_explore_common_app-2.3.0/tests/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:07.870136 core_explore_common_app-2.3.0/tests/components/abstract_persistent_query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:03.000000 core_explore_common_app-2.3.0/tests/components/abstract_persistent_query/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:07.905773 core_explore_common_app-2.3.0/tests/components/query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:03.000000 core_explore_common_app-2.3.0/tests/components/query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7526 2023-05-02 19:37:03.000000 core_explore_common_app-2.3.0/tests/components/query/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:07.922651 core_explore_common_app-2.3.0/tests/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:03.000000 core_explore_common_app-2.3.0/tests/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:07.940600 core_explore_common_app-2.3.0/tests/rest/query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:03.000000 core_explore_common_app-2.3.0/tests/rest/query/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:07.986041 core_explore_common_app-2.3.0/tests/rest/query/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:03.000000 core_explore_common_app-2.3.0/tests/rest/query/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4103 2023-05-02 19:37:03.000000 core_explore_common_app-2.3.0/tests/rest/query/views/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:08.039825 core_explore_common_app-2.3.0/tests/rest/result/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:03.000000 core_explore_common_app-2.3.0/tests/rest/result/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2544 2023-05-02 19:37:03.000000 core_explore_common_app-2.3.0/tests/rest/result/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3002 2023-05-02 19:37:03.000000 core_explore_common_app-2.3.0/tests/rest/result/tests_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1808 2023-05-02 19:37:03.000000 core_explore_common_app-2.3.0/tests/test_settings.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      733 2023-05-02 19:37:03.000000 core_explore_common_app-2.3.0/tests/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:08.057256 core_explore_common_app-2.3.0/tests/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:03.000000 core_explore_common_app-2.3.0/tests/utils/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:08.091976 core_explore_common_app-2.3.0/tests/utils/linked_records/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:03.000000 core_explore_common_app-2.3.0/tests/utils/linked_records/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3655 2023-05-02 19:37:03.000000 core_explore_common_app-2.3.0/tests/utils/linked_records/tests_pid.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:08.124052 core_explore_common_app-2.3.0/tests/utils/oaipmh/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:03.000000 core_explore_common_app-2.3.0/tests/utils/oaipmh/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1860 2023-05-02 19:37:03.000000 core_explore_common_app-2.3.0/tests/utils/oaipmh/tests_oaipmh.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:08.158259 core_explore_common_app-2.3.0/tests/utils/query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:03.000000 core_explore_common_app-2.3.0/tests/utils/query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2990 2023-05-02 19:37:03.000000 core_explore_common_app-2.3.0/tests/utils/query/tests_query.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:08.192794 core_explore_common_app-2.3.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:03.000000 core_explore_common_app-2.3.0/tests/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    13749 2023-05-02 19:37:03.000000 core_explore_common_app-2.3.0/tests/views/test_unit.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `core_explore_common_app-2.2.0/PKG-INFO` & `core_explore_common_app-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_explore_common_app
-Version: 2.2.0
+Version: 2.3.0
 Summary: Base exploration function for the curator core project
 Home-page: https://github.com/usnistgov/core_explore_common_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =======================
         Core Explore Common App
```

### Comparing `core_explore_common_app-2.2.0/README.rst` & `core_explore_common_app-2.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.2.0/core_explore_common_app/access_control/api.py` & `core_explore_common_app-2.3.0/core_explore_common_app/access_control/api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """ Set of functions to define the rules for access control
 """
 import logging
 
 from django.contrib.auth.models import User, AnonymousUser
+from django.http import HttpRequest
 
 from core_main_app.access_control.exceptions import AccessControlError
 from core_explore_common_app.components.abstract_persistent_query.models import (
     AbstractPersistentQuery,
 )
 from core_explore_common_app.components.query.models import Query
 from core_explore_common_app.settings import (
     CAN_ANONYMOUS_ACCESS_PUBLIC_DOCUMENT,
 )
+from core_main_app.access_control import api as access_control_api
 
 logger = logging.getLogger(__name__)
 
 
 def can_read(func, id_query, user):
     """Can user read
 
@@ -163,7 +165,24 @@
     if query.user_id == str(user.id):
         return func(*args, **kwargs)
 
     # Non-Owner
     raise AccessControlError(
         "The user doesn't have enough rights to access this query."
     )
+
+
+def can_access_explore_views(func, *args, **kwargs):
+    """Check if user can access explore views
+
+    Args:
+        func:
+        request:
+
+    Returns:
+
+    """
+    request = next((arg for arg in args if isinstance(arg, HttpRequest)), None)
+    access_control_api._check_anonymous_access(
+        request.user if request else None
+    )
+    return func(*args, **kwargs)
```

### Comparing `core_explore_common_app-2.2.0/core_explore_common_app/components/abstract_persistent_query/api.py` & `core_explore_common_app-2.3.0/core_explore_common_app/components/abstract_persistent_query/api.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.2.0/core_explore_common_app/components/abstract_persistent_query/models.py` & `core_explore_common_app-2.3.0/core_explore_common_app/components/abstract_persistent_query/models.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.2.0/core_explore_common_app/components/abstract_query/models.py` & `core_explore_common_app-2.3.0/core_explore_common_app/components/abstract_query/models.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.2.0/core_explore_common_app/components/query/api.py` & `core_explore_common_app-2.3.0/core_explore_common_app/components/query/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 """ Query api
 """
 
-from core_main_app.access_control.decorators import access_control
-from core_main_app.commons.exceptions import DoesNotExist
-from core_main_app.utils.query.constants import VISIBILITY_OPTION
 from core_explore_common_app import settings
 from core_explore_common_app.access_control.api import can_read, can_access
 from core_explore_common_app.components.query.models import Query
-from core_explore_common_app.constants import LOCAL_QUERY_NAME
 from core_explore_common_app.settings import (
     EXPLORE_ADD_DEFAULT_LOCAL_DATA_SOURCE_TO_QUERY,
 )
-from core_explore_common_app.utils.query.query import add_local_data_source
+from core_explore_common_app.utils.query.query import (
+    create_local_data_source,
+    is_local_data_source,
+)
+from core_main_app.access_control.decorators import access_control
+from core_main_app.commons.exceptions import DoesNotExist
+from core_main_app.utils.query.constants import VISIBILITY_OPTION
 
 
 @access_control(can_access)
 def upsert(query, user):
     """Saves or uploads query
 
     Args:
         query:
+        user:
 
     Returns:
 
     """
     query.save()
     return query
 
@@ -48,20 +51,37 @@
     # Save query in database
     upsert(query, request.user)
     # Set list of templates
     query.templates.set(template_ids)
     return query
 
 
+def add_local_data_source(request, query):
+    """Add local data source to query
+
+    Args:
+        request:
+        query:
+
+    Returns:
+
+    """
+    # Add Local to the query as a data source
+    data_source = create_local_data_source(request)
+    # Add data source to query (with access control)
+    add_data_source(query, data_source, request.user)
+
+
 @access_control(can_read)
 def get_by_id(id_query, user):
     """Returns a query with the given id
 
     Args:
         id_query:
+        user:
 
     Returns:
 
     """
     return Query.get_by_id(id_query)
 
 
@@ -135,13 +155,13 @@
 
     Returns:
 
     """
     # Set visibility option for local data source
     for data_source in query.data_sources:
         # find local data source
-        if data_source["name"] == LOCAL_QUERY_NAME:
+        if is_local_data_source(data_source):
             # set visibility to public
             data_source["query_options"] = {
                 VISIBILITY_OPTION: settings.QUERY_VISIBILITY
             }
             break
```

### Comparing `core_explore_common_app-2.2.0/core_explore_common_app/components/query/models.py` & `core_explore_common_app-2.3.0/core_explore_common_app/components/query/models.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.2.0/core_explore_common_app/components/result/models.py` & `core_explore_common_app-2.3.0/core_explore_common_app/components/result/models.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.2.0/core_explore_common_app/discover.py` & `core_explore_common_app-2.3.0/core_explore_common_app/discover.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.2.0/core_explore_common_app/migrations/0001_initial.py` & `core_explore_common_app-2.3.0/core_explore_common_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.2.0/core_explore_common_app/rest/query/views.py` & `core_explore_common_app-2.3.0/core_explore_common_app/rest/query/views.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,108 +1,162 @@
 """ REST views for the query API
 """
+import json
 import logging
+
 import pytz
+from django.conf import settings as conf_settings
 from django.urls import reverse
 
+from core_explore_common_app.components.result.models import Result
+from core_explore_common_app.utils.linked_records import pid as pid_utils
+from core_explore_common_app.utils.result import result as result_utils
+from core_main_app.commons.constants import DATA_JSON_FIELD
 from core_main_app.commons.exceptions import ApiError
+from core_main_app.components.data import api as data_api
 from core_main_app.rest.data.abstract_views import (
     AbstractExecuteLocalQueryView,
 )
-from core_main_app.utils.pagination.rest_framework_paginator.pagination import (
-    StandardResultsSetPagination,
+from core_main_app.settings import DATA_SORTING_FIELDS, RESULTS_PER_PAGE
+from core_main_app.utils.pagination.django_paginator.results_paginator import (
+    ResultsPaginator,
 )
-from core_explore_common_app import settings
-from core_explore_common_app.components.result.models import Result
-from core_explore_common_app.rest.result.serializers import ResultSerializer
-from core_explore_common_app.utils.result import result as result_utils
+from core_main_app.utils.pagination.mongoengine_paginator.paginator import (
+    MongoenginePaginator,
+)
+from core_main_app.utils.query.constants import VISIBILITY_OPTION
+from core_main_app.utils.query.mongo.query_builder import QueryBuilder
 
 logger = logging.getLogger(__name__)
 
 
-class ExecuteLocalQueryView(AbstractExecuteLocalQueryView):
-    """Execute Local Query View"""
+def build_local_query(query_data):
+    """Build a query for local data.
 
-    def build_response(self, data_list):
-        """Build the paginated list of data
+    Args:
+        query_data (dict): Query to execute locally.
 
-        Args:
-            data_list: List of data
-
-        Returns:
-            Paginated list of data
-        """
-        # get paginator
-        paginator = StandardResultsSetPagination()
-        # get requested page from list of results
-        page = paginator.paginate_queryset(data_list, self.request)
-
-        # Get detail view base url (to be completed with data id)
-        detail_url_base = reverse("core_main_app_data_detail")
-        url_access_data = reverse(
-            "core_explore_common_app_get_result_from_data_id"
-        )
-        url_permission_data = reverse("core_main_app_rest_data_permissions")
-
-        # Build list of results
-        results = []
-        # Template info
-        template_info = dict()
-        # Init pid settings
-        auto_set_pid = False
-        if "core_linked_records_app" in settings.INSTALLED_APPS:
-            from core_linked_records_app.components.pid_settings import (
-                api as pid_settings_api,
+    Returns:
+        dict: Raw query for local data.
+    """
+    # get query and templates
+    query = query_data.get("query", None)
+
+    if query is None:
+        raise ApiError("Query should be passed in parameter.")
+
+    templates = query_data.get("templates", [])
+    if type(templates) is str:
+        templates = json.loads(templates)
+    options = query_data.get("options", {})
+    if type(options) is str:
+        options = json.loads(options)
+    title = query_data.get("title", None)
+
+    # build query builder
+    query_builder = QueryBuilder(query, DATA_JSON_FIELD)
+
+    # update the criteria with templates information
+    if templates is not None and len(templates) > 0:
+        list_template_ids = [
+            AbstractExecuteLocalQueryView.parse_id(template["id"])
+            for template in templates
+        ]
+        query_builder.add_list_criteria("template", list_template_ids)
+    # update the criteria with visibility information
+    if options is not None and VISIBILITY_OPTION in options:
+        query_builder.add_visibility_criteria(options[VISIBILITY_OPTION])
+    # update the criteria with title information
+    if title is not None:
+        query_builder.add_title_criteria(title)
+
+    # get raw query
+    return query_builder.get_raw_query()
+
+
+def execute_local_query(query_data, page, request):
+    """Execute query on local database
+
+    Args:
+        query_data:
+        page:
+        request:
+
+    Returns:
+
+    """
+    # build raw query
+    raw_query = build_local_query(query_data)
+    # retrieve order_by_field field
+    order_by_field = query_data.get("order_by_field", None)
+    order_by_field = (
+        order_by_field.split(",") if order_by_field else DATA_SORTING_FIELDS
+    )
+    # execute query
+    data_list = data_api.execute_json_query(
+        raw_query, request.user, order_by_field
+    )
+    # build result page
+    if conf_settings.MONGODB_INDEXING:
+        paginator = MongoenginePaginator(data_list, RESULTS_PER_PAGE)
+        page = paginator.get_page(page)
+    else:
+        paginator = ResultsPaginator()
+        page = paginator.get_results(data_list, page, RESULTS_PER_PAGE)
+    return page
+
+
+def format_local_results(results, request):
+    """Format local results for explore app
+
+    Args:
+        results:
+        request:
+
+    Returns:
+
+    """
+    # Get detail view base url (to be completed with data id)
+    detail_url_base = reverse("core_main_app_data_detail")
+    url_access_data = reverse(
+        "core_explore_common_app_get_result_from_data_id"
+    )
+    url_permission_data = reverse("core_main_app_rest_data_permissions")
+
+    # Template info
+    template_info = dict()
+    # Init data list
+    data_list = []
+
+    for data in results.object_list:
+        # get data's template
+        template_id = data.template_id
+        # get and store data's template information
+        if template_id not in template_info:
+            template_info[template_id] = result_utils.get_template_info(
+                data.template
             )
 
-            auto_set_pid = pid_settings_api.get().auto_set_pid
-        for data in page:
-            # get data's template
-            template_id = data.template_id
-            # get and store data's template information
-            if template_id not in template_info:
-                template_info[template_id] = result_utils.get_template_info(
-                    data.template
-                )
-
-            detail_url = f"{detail_url_base}?id={str(data.id)}"
-
-            # Use the PID link if the app is installed, and a PID is defined for the
-            # document
-            if "core_linked_records_app" in settings.INSTALLED_APPS:
-                from core_linked_records_app.components.data import (
-                    api as data_api,
-                )
-
-                if auto_set_pid:
-                    try:
-                        pid_url = data_api.get_pid_for_data(
-                            data.id, self.request
-                        )
-                        if pid_url is not None:  # Ensure the PID is set
-                            detail_url = pid_url
-                    except ApiError as exc:
-                        # If there is an error with the PID, fallback to regular data
-                        # url.
-                        logger.warning(
-                            "An error occured while retrieving PID url: %s",
-                            str(exc),
-                        )
-
-            results.append(
-                Result(
-                    title=data.title,
-                    xml_content=data.xml_content,
-                    template_info=template_info[template_id],
-                    permission_url=f'{url_permission_data}?ids=%5B"{str(data.id)}"%5D',
-                    detail_url=detail_url,
-                    access_data_url=f"{url_access_data}?id={data.id}",
-                    last_modification_date=data.last_modification_date.replace(
-                        tzinfo=pytz.UTC
-                    ),
-                )
-            )
+        detail_url = f"{detail_url_base}?id={str(data.id)}"
 
-        # serialize results
-        serialized_results = ResultSerializer(results, many=True)
-        # return http response
-        return paginator.get_paginated_response(serialized_results.data)
+        # Use the PID link if the app is installed, and a PID is defined for the document
+        if pid_utils.auto_set_pid_enabled(
+            installed_apps=conf_settings.INSTALLED_APPS
+        ):
+            pid_url = pid_utils.get_pid_url(data, request)
+            # Ensure the PID is set
+            detail_url = pid_url if pid_url else detail_url
+
+        data_list.append(
+            Result(
+                title=data.title,
+                xml_content=data.xml_content,
+                template_info=template_info[template_id],
+                permission_url=f'{url_permission_data}?ids=%5B"{str(data.id)}"%5D',
+                detail_url=detail_url,
+                access_data_url=f"{url_access_data}?id={data.id}",
+                last_modification_date=data.last_modification_date.replace(
+                    tzinfo=pytz.UTC
+                ),
+            )
+        )
+    return data_list
```

### Comparing `core_explore_common_app-2.2.0/core_explore_common_app/rest/result/views.py` & `core_explore_common_app-2.3.0/core_explore_common_app/rest/result/views.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.2.0/core_explore_common_app/settings.py` & `core_explore_common_app-2.3.0/core_explore_common_app/settings.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.2.0/core_explore_common_app/static/core_explore_common_app/common/js/tools.js` & `core_explore_common_app-2.3.0/core_explore_common_app/static/core_explore_common_app/common/js/tools.js`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.2.0/core_explore_common_app/static/core_explore_common_app/user/css/results.css` & `core_explore_common_app-2.3.0/core_explore_common_app/static/core_explore_common_app/user/css/results.css`

 * *Files 5% similar despite different names*

```diff
@@ -108,15 +108,15 @@
     padding-right: 5px;
 }
 
 .tools-menu a {
     display: contents !important;
 }
 
-.permissions-link {
+.permissions-link, .permissions-link-open {
     float: right;
     display: none;
 }
 
 .permissions-icon {
     font-size: 20px;
     color: #007aa7;
```

### Comparing `core_explore_common_app-2.2.0/core_explore_common_app/static/core_explore_common_app/user/css/toggle.css` & `core_explore_common_app-2.3.0/core_explore_common_app/static/core_explore_common_app/user/css/toggle.css`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.2.0/core_explore_common_app/static/core_explore_common_app/user/js/local_selector.js` & `core_explore_common_app-2.3.0/core_explore_common_app/static/core_explore_common_app/user/js/local_selector.js`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.2.0/core_explore_common_app/static/core_explore_common_app/user/js/persistent_query_config.js` & `core_explore_common_app-2.3.0/core_explore_common_app/static/core_explore_common_app/user/js/persistent_query_config.js`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.2.0/core_explore_common_app/static/core_explore_common_app/user/js/results.js` & `core_explore_common_app-2.3.0/core_explore_common_app/static/core_explore_common_app/user/js/results.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -102,14 +102,19 @@
                         // create the click event listener
                         (function() {
                             var target_id = id;
                             $(editLinkElement).click(function() {
                                 openEditRecord(target_id, $(editLinkElement));
                             });
                         }());
+                        // show the open icon
+                        var openLinkElement = inputElement.siblings(".permissions-link-open");
+                        openLinkElement.css('display', "inline");
+                        // add link to text editor
+                        openLinkElement.attr("href", openRecordUrl + '?id=' + id);
                     }
                 }
             },
             error: function(data) {
                 console.log(data)
             }
         })
```

### Comparing `core_explore_common_app-2.2.0/core_explore_common_app/static/core_explore_common_app/user/js/sorting_multi_criteria.js` & `core_explore_common_app-2.3.0/core_explore_common_app/static/core_explore_common_app/user/js/sorting_multi_criteria.js`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.2.0/core_explore_common_app/static/core_explore_common_app/user/js/sorting_single_criteria.js` & `core_explore_common_app-2.3.0/core_explore_common_app/static/core_explore_common_app/user/js/sorting_single_criteria.js`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.2.0/core_explore_common_app/tasks.py` & `core_explore_common_app-2.3.0/core_explore_common_app/tasks.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.2.0/core_explore_common_app/templates/core_explore_common_app/user/ordering_menu/multi_criteria_sorting_menu.html` & `core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/ordering_menu/multi_criteria_sorting_menu.html`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.2.0/core_explore_common_app/templates/core_explore_common_app/user/ordering_menu/single_criteria_sorting_menu.html` & `core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/ordering_menu/single_criteria_sorting_menu.html`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.2.0/core_explore_common_app/templates/core_explore_common_app/user/persistent_query/modal.html` & `core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/persistent_query/modal.html`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.2.0/core_explore_common_app/templates/core_explore_common_app/user/persistent_query/persistent_query_pagination.html` & `core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/persistent_query/persistent_query_pagination.html`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.2.0/core_explore_common_app/templates/core_explore_common_app/user/results/data_source_info.html` & `core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/results/data_source_info.html`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,18 @@
                 {% else %}
                 {{ result.title }}
                 {% endif %}
             </span>
             <span class="template-info-name">{{result.template_info.name}}</span>
             {% if result.permission_url and display_edit_button %}
                 <input class="input-permission-url" type="hidden" value="{{result.permission_url}}">
-                <a class="permissions-link" href="#">
+                <a class="permissions-link-open mx-2" href="#" data-toggle="tooltip" title="Open in text editor">
+                    <i class="fas fa-code" aria-hidden="true"></i>
+                </a>
+                <a class="permissions-link mx-2" href="#" data-toggle="tooltip" title="Edit">
                     <i class="fas fa-pencil-alt permissions-icon edit" aria-hidden="true"></i>
                 </a>
             {% endif %}
             <div title="Last modification date" class="data-info-right-container">
                 {{result.last_modification_date|json_date:"N d Y g:iA"}}
             </div>
         </div>
```

#### html2text {}

```diff
@@ -1,6 +1,6 @@
 {% load json_date %}
 ⁰   {% if result.detail_url %} {{_result.title_}} {% else %} {{ result.title }}
 {% endif %}  {{result.template_info.name}} {% if result.permission_url and
-display_edit_button %}   {% endif %}
+display_edit_button %}    {% endif %}
 {{result.last_modification_date|json_date:"N d Y g:iA"}}
 {{ xml_representation }}
```

### Comparing `core_explore_common_app-2.2.0/core_explore_common_app/templates/core_explore_common_app/user/results/data_source_pagination.html` & `core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/results/data_source_pagination.html`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.2.0/core_explore_common_app/templates/core_explore_common_app/user/results/data_source_results.html` & `core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/results/data_source_results.html`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.2.0/core_explore_common_app/templates/core_explore_common_app/user/results/data_sources_results.html` & `core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/results/data_sources_results.html`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.2.0/core_explore_common_app/templates/core_explore_common_app/user/selector/data_sources_selector.html` & `core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/selector/data_sources_selector.html`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.2.0/core_explore_common_app/templates/core_explore_common_app/user/selector/local_selector.html` & `core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/selector/local_selector.html`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.2.0/core_explore_common_app/urls.py` & `core_explore_common_app-2.3.0/core_explore_common_app/urls.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.2.0/core_explore_common_app/utils/protocols/oauth2.py` & `core_explore_common_app-2.3.0/core_explore_common_app/utils/protocols/oauth2.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.2.0/core_explore_common_app/utils/query/query.py` & `core_explore_common_app-2.3.0/core_explore_common_app/utils/query/query.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,60 +1,44 @@
 """Explore Common query utils
 """
+
 import json
 
-from django.urls import reverse
 from django.utils import timezone
 from requests import ConnectionError
 
-from core_main_app.settings import DATA_SORTING_FIELDS
-from core_main_app.utils.requests_utils.requests_utils import send_get_request
-
-from core_explore_common_app import settings
 from core_explore_common_app.commons.exceptions import ExploreRequestError
 from core_explore_common_app.components.abstract_query.models import (
     Authentication,
     DataSource,
 )
-from core_explore_common_app.components.query import api as query_api
-from core_explore_common_app.constants import LOCAL_QUERY_NAME, LOCAL_QUERY_URL
+from core_explore_common_app.constants import LOCAL_QUERY_NAME
 from core_explore_common_app.rest.result.serializers import ResultSerializer
-from core_explore_common_app.utils.protocols.oauth2 import (
-    send_post_request as oauth2_request,
-)
+from core_explore_common_app.utils.protocols import oauth2
+from core_main_app.settings import DATA_SORTING_FIELDS, SERVER_URI
 
 
-def send(request, query, data_source_index, page):
+def send(request, json_query, data_source, page):
     """
 
     Args:
         request:
-        query:
-        data_source_index:
+        json_query:
+        data_source:
         page:
 
     Returns:
 
     """
     try:
-        # get data source to reach
-        data_source = query.data_sources[data_source_index]
-        # get serialized query to send to data source
-        json_query = _serialize_query(query, data_source)
         # add page number to query url
-        query_url = _get_paginated_url(data_source["url_query"], page)
+        query_url = f"{data_source['url_query']}/?page={page}"
         # send query to data source
-        if data_source["authentication"]["auth_type"] == "session":
-            response = send_get_request(
-                query_url,
-                data=json_query,
-                cookies={"sessionid": request.session.session_key},
-            )
-        elif data_source["authentication"]["auth_type"] == "oauth2":
-            response = oauth2_request(
+        if data_source["authentication"]["auth_type"] == "oauth2":
+            response = oauth2.send_post_request(
                 query_url,
                 json_query,
                 data_source["authentication"]["params"]["access_token"],
                 session_time_zone=timezone.get_current_timezone(),
             )
         else:
             raise ExploreRequestError("Unknown authentication type.")
@@ -81,90 +65,63 @@
         raise ExploreRequestError("The selected data source is not available.")
     except ConnectionError:
         raise ExploreRequestError("Unable to contact the remote server.")
     except Exception as exception:
         raise ExploreRequestError(str(exception))
 
 
-def add_local_data_source(request, query):
-    """Add local data source to query
-
-    Args:
-        request:
-        query:
-
-    Returns:
-
-    """
-    # Add Local to the query as a data source
-    data_source = create_local_data_source(request)
-    query_api.add_data_source(query, data_source, request.user)
-
-
 def create_local_data_source(request):
     """Create local datasource
 
     Args:
         request:
 
     Returns:
     """
     local_name = LOCAL_QUERY_NAME
-    local_query_url = get_local_query_absolute_url(request)
     authentication = Authentication(auth_type="session")
     data_source = DataSource(
         name=local_name,
-        url_query=local_query_url,
+        url_query=SERVER_URI,
         authentication=authentication,
         order_by_field=",".join(DATA_SORTING_FIELDS),
     )
 
-    if "core_linked_records_app" in settings.INSTALLED_APPS:
-        data_source["capabilities"] = {
-            "url_pid": request.build_absolute_uri(
-                reverse("core_linked_records_app_query_local")
-            )
-        }
-
     return data_source
 
 
-def get_local_query_absolute_url(request):
-    """Return local query absolute URL.
+def is_local_data_source(data_source):
+    """Check if local data source
 
     Args:
-        request:
-        query:
+        data_source:
 
     Returns:
-        String: Absolute URL
 
     """
-    return request.build_absolute_uri(reverse(LOCAL_QUERY_URL))
+    return (
+        data_source["name"] == LOCAL_QUERY_NAME
+        and data_source["url_query"] == SERVER_URI
+    )
+
 
+def serialize_query(query, data_source):
+    """Serialize the query
 
-# TODO: see if can be done using a Serializer
-def _serialize_query(query, data_source):
+    Args:
+        query:
+        data_source:
+
+    Returns:
+
+    """
     return {
         "query": query.content,
         "templates": json.dumps(
             [
                 {"id": template.id, "hash": template.hash}
                 for template in query.templates.all()
             ]
         ),
         "options": json.dumps(data_source["query_options"]),
         "order_by_field": data_source["order_by_field"],
     }
-
-
-def _get_paginated_url(url, page):
-    """Add a page number to the url
-
-    Args:
-        url:
-        page:
-
-    Returns:
-
-    """
-    return f"{url}/?page={page}"
```

### Comparing `core_explore_common_app-2.2.0/core_explore_common_app/utils/result/result.py` & `core_explore_common_app-2.3.0/core_explore_common_app/utils/result/result.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.2.0/core_explore_common_app/views/user/ajax.py` & `core_explore_common_app-2.3.0/core_explore_common_app/views/user/ajax.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,45 +2,49 @@
 """
 import json
 import math
 from abc import ABCMeta, abstractmethod
 from os.path import join
 
 from django.contrib.auth.decorators import login_required
+from django.core.paginator import EmptyPage
 from django.http.response import HttpResponse, HttpResponseBadRequest
 from django.shortcuts import render as django_render
 from django.template import loader
 from django.urls import reverse
 from django.utils.decorators import method_decorator
 from django.utils.html import escape
 from django.views import View
 
-from core_main_app.commons.exceptions import DoesNotExist
-from core_main_app.utils.pagination.rest_framework_paginator.rest_framework_paginator import (
-    get_page_number,
-)
-from core_main_app.views.common.views import CommonView
-
 from core_explore_common_app import settings
 from core_explore_common_app.commons.exceptions import ExploreRequestError
 from core_explore_common_app.components.abstract_persistent_query import (
     api as abstract_persistent_query_api,
 )
 from core_explore_common_app.components.abstract_persistent_query.models import (
     AbstractPersistentQuery,
 )
 from core_explore_common_app.components.query import api as query_api
 from core_explore_common_app.constants import LOCAL_QUERY_NAME
-from core_explore_common_app.utils.query.query import (
-    send as send_query,
-    add_local_data_source,
-    get_local_query_absolute_url,
+from core_explore_common_app.rest.query import views as query_views
+from core_explore_common_app.utils.oaipmh import oaipmh as oaipmh_utils
+from core_explore_common_app.utils.query import query as query_utils
+from core_explore_common_app.access_control import (
+    api as explore_common_acl_api,
 )
+from core_main_app.access_control.decorators import access_control
+from core_main_app.commons.exceptions import DoesNotExist
+from core_main_app.settings import SERVER_URI
+from core_main_app.utils.pagination.rest_framework_paginator.rest_framework_paginator import (
+    get_page_number,
+)
+from core_main_app.views.common.views import CommonView
 
 
+@access_control(explore_common_acl_api.can_access_explore_views)
 def get_local_data_source(request):
     """Ajax method to get the local data source
 
     Args:
         request:
 
     Returns:
@@ -54,24 +58,20 @@
             query = query_api.get_by_id(id_query, request.user)
 
             context_params = {
                 "enabled": True,
                 "selected": False,
             }
             if len(settings.DATA_SOURCES_EXPLORE_APPS) == 0:
-                add_local_data_source(request, query)
+                query_api.add_local_data_source(request, query)
                 context_params["enabled"] = False
 
             # check query to see if local data source was selected
-            local_query_url = get_local_query_absolute_url(request)
             for data_source in query.data_sources:
-                if (
-                    data_source["name"] == LOCAL_QUERY_NAME
-                    and data_source["url_query"] == local_query_url
-                ):
+                if query_utils.is_local_data_source(data_source):
                     context_params["selected"] = True
 
             context = {}
             context.update(request)
             context.update(context_params)
             return django_render(
                 request,
@@ -87,14 +87,15 @@
         return HttpResponseBadRequest("The query does not exist.")
     except Exception:
         return HttpResponseBadRequest(
             "An unexpected error occurred while getting local data source selector."
         )
 
 
+@access_control(explore_common_acl_api.can_access_explore_views)
 def update_local_data_source(request):
     """Ajax method to update query with local data source
 
     Args:
         request:
 
     Returns:
@@ -105,31 +106,31 @@
         selected = json.loads(request.GET["selected"])
 
         # Get query from id
         query = query_api.get_by_id(query_id, request.user)
 
         if selected:
             # Local data source is selected, add it to the query as a data source
-            add_local_data_source(request, query)
+            query_api.add_local_data_source(request, query)
         else:
             # Local data source is not selected, remove it from the query
-            local_query_url = get_local_query_absolute_url(request)
             data_source = query_api.get_data_source_by_name_and_url_query(
-                query, LOCAL_QUERY_NAME, local_query_url, request.user
+                query, LOCAL_QUERY_NAME, SERVER_URI, request.user
             )
             query_api.remove_data_source(query, data_source, request.user)
 
         return HttpResponse()
 
     except DoesNotExist:
         return HttpResponseBadRequest("The query does not exist.")
     except Exception as exception:
         return HttpResponseBadRequest(escape(str(exception)))
 
 
+@access_control(explore_common_acl_api.can_access_explore_views)
 def get_data_sources_html(request):
     """Gets data sources html for results
 
     Args:
         request:
 
     Returns:
@@ -178,55 +179,97 @@
         )
     except DoesNotExist:
         return HttpResponseBadRequest("The query does not exist.")
     except Exception as exception:
         return HttpResponseBadRequest(escape(str(exception)))
 
 
+@access_control(explore_common_acl_api.can_access_explore_views)
 def get_data_source_results(request, query_id, data_source_index, page=1):
     """Gets results from a data source
 
     Args:
         request:
         query_id:
         data_source_index:
         page:
 
     Returns:
 
     """
+
     try:
         # get query
         query = query_api.get_by_id(query_id, request.user)
+        data_source = query.data_sources[int(data_source_index)]
+        json_query = query_utils.serialize_query(query, data_source)
 
-        # send query, and get results from data source
-        results = send_query(request, query, int(data_source_index), page)
-
-        # get pagination information
-        previous_page_number = get_page_number(results["previous"])
-        next_page_number = get_page_number(results["next"])
-        results_count = results["count"]
-        page_count = int(
-            math.ceil(float(results_count) / settings.RESULTS_PER_PAGE)
-        )
-
-        # pagination has other pages?
-        has_other_pages = results_count > settings.RESULTS_PER_PAGE
-
-        # pagination has previous?
-        has_previous = previous_page_number is not None
-
-        # pagination has next?
-        has_next = (
-            next_page_number is not None and next_page_number <= page_count
-        )
+        # If querying the local system
+        if data_source["authentication"]["auth_type"] == "session":
+            if query_utils.is_local_data_source(data_source):
+                results = query_views.execute_local_query(
+                    json_query, page, request
+                )
+                data_list = query_views.format_local_results(results, request)
+            elif oaipmh_utils.is_oai_data_source(data_source):
+                from core_explore_oaipmh_app.rest.query.views import (
+                    execute_oaipmh_query,
+                    format_oaipmh_results,
+                )
+
+                results = execute_oaipmh_query(json_query, page, request)
+                data_list = format_oaipmh_results(results, request)
+            else:
+                raise ExploreRequestError("Unknown data source.")
+            # Get pagination info for local sources
+            results_count = results.paginator.count
+            page_count = int(
+                math.ceil(float(results_count) / settings.RESULTS_PER_PAGE)
+            )
+
+            try:
+                previous_page_number = results.previous_page_number()
+            except EmptyPage:
+                previous_page_number = None
+
+            try:
+                next_page_number = results.next_page_number()
+            except EmptyPage:
+                next_page_number = None
+
+            has_other_pages = results.has_other_pages()
+            has_previous = results.has_previous()
+            has_next = results.has_next()
+        else:
+            # send query, and get results from data source
+            results = query_utils.send(request, json_query, data_source, page)
+            data_list = results["results"]
+
+            # get pagination information
+            previous_page_number = get_page_number(results["previous"])
+            next_page_number = get_page_number(results["next"])
+            results_count = results["count"]
+            page_count = int(
+                math.ceil(float(results_count) / settings.RESULTS_PER_PAGE)
+            )
+
+            # pagination has other pages?
+            has_other_pages = results_count > settings.RESULTS_PER_PAGE
+
+            # pagination has previous?
+            has_previous = previous_page_number is not None
+
+            # pagination has next?
+            has_next = (
+                next_page_number is not None and next_page_number <= page_count
+            )
 
         # set results in context
         context_data = {
-            "results": results["results"],
+            "results": data_list,
             "query_id": query_id,
             "data_source_index": data_source_index,
             "pagination": {
                 "number": int(page),
                 "paginator": {"num_pages": page_count},
                 "has_other_pages": has_other_pages,
                 "previous_page_number": previous_page_number,
@@ -255,15 +298,15 @@
             )
         )
         # render html
         results_html = html_template.render(context)
         # set response with html results
         response_dict = {
             "results": results_html,
-            "nb_results": results["count"],
+            "nb_results": results_count,
         }
         return HttpResponse(
             json.dumps(response_dict), content_type="application/json"
         )
 
     except DoesNotExist:
         return HttpResponseBadRequest("The query does not exist.")
@@ -388,24 +431,14 @@
         }
         assets = {
             "js": [
                 {
                     "path": "core_main_app/common/js/backtoprevious.js",
                     "is_raw": True,
                 },
-                {
-                    "path": "core_main_app/libs/highlight/11.0.0/js/highlight.min.js",
-                    "is_raw": False,
-                },
-                {
-                    "path": "core_main_app/libs/highlight/11.0.0/js/init_highlight.js",
-                    "is_raw": False,
-                },
-            ],
-            "css": [
-                "core_main_app/libs/highlight/11.0.0/css/atom-one-light.css"
             ],
+            "css": ["core_main_app/common/css/highlight.css"],
         }
 
         return self.common_render(
             request, self.template, assets=assets, context=context
         )
```

### Comparing `core_explore_common_app-2.2.0/core_explore_common_app/views/user/views.py` & `core_explore_common_app-2.3.0/core_explore_common_app/views/user/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
 from core_explore_common_app import settings
 from core_explore_common_app.components.query import api as query_api
 from core_explore_common_app.components.query.models import Query
 from core_explore_common_app.settings import (
     EXPLORE_ADD_DEFAULT_LOCAL_DATA_SOURCE_TO_QUERY,
 )
-from core_explore_common_app.utils.query.query import add_local_data_source
 
 
 class ResultsView(View):
     """Results View"""
 
     def __init__(self, **kwargs):
         self.assets = self._load_assets()
@@ -198,15 +197,15 @@
                 data_sources=persistent_query.data_sources,
             )
             # add the local data source by default
             if (
                 not query.data_sources
                 and EXPLORE_ADD_DEFAULT_LOCAL_DATA_SOURCE_TO_QUERY
             ):
-                add_local_data_source(self.request, query)
+                query_api.add_local_data_source(self.request, query)
 
             query = query_api.upsert(query, self.request.user)
             query.templates.set(persistent_query.templates.all())
 
             # then redirect to the result page core_explore_example_results with /<template_id>/<query_id>
             return self._get_reversed_url(query)
         except AccessControlError:
```

### Comparing `core_explore_common_app-2.2.0/core_explore_common_app.egg-info/PKG-INFO` & `core_explore_common_app-2.3.0/core_explore_common_app.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-explore-common-app
-Version: 2.2.0
+Version: 2.3.0
 Summary: Base exploration function for the curator core project
 Home-page: https://github.com/usnistgov/core_explore_common_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =======================
         Core Explore Common App
```

### Comparing `core_explore_common_app-2.2.0/core_explore_common_app.egg-info/SOURCES.txt` & `core_explore_common_app-2.3.0/core_explore_common_app.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.md
 MANIFEST.in
 README.rst
 pyproject.toml
 requirements.core.txt
 setup.py
 core_explore_common_app/__init__.py
 core_explore_common_app/admin.py
@@ -68,29 +69,45 @@
 core_explore_common_app/templates/core_explore_common_app/user/results/data_sources_results.html
 core_explore_common_app/templates/core_explore_common_app/user/results/results.html
 core_explore_common_app/templates/core_explore_common_app/user/selector/data_sources_selector.html
 core_explore_common_app/templates/core_explore_common_app/user/selector/list_selector_base.html
 core_explore_common_app/templates/core_explore_common_app/user/selector/local_content.html
 core_explore_common_app/templates/core_explore_common_app/user/selector/local_selector.html
 core_explore_common_app/utils/__init__.py
+core_explore_common_app/utils/linked_records/__init__.py
+core_explore_common_app/utils/linked_records/pid.py
+core_explore_common_app/utils/oaipmh/__init__.py
+core_explore_common_app/utils/oaipmh/oaipmh.py
 core_explore_common_app/utils/protocols/__init__.py
 core_explore_common_app/utils/protocols/commons.py
 core_explore_common_app/utils/protocols/oauth2.py
 core_explore_common_app/utils/query/__init__.py
 core_explore_common_app/utils/query/query.py
 core_explore_common_app/utils/result/__init__.py
 core_explore_common_app/utils/result/result.py
 core_explore_common_app/views/__init__.py
 core_explore_common_app/views/user/__init__.py
 core_explore_common_app/views/user/ajax.py
 core_explore_common_app/views/user/views.py
 tests/__init__.py
 tests/test_settings.py
+tests/urls.py
 tests/components/__init__.py
 tests/components/abstract_persistent_query/__init__.py
 tests/components/query/__init__.py
 tests/components/query/tests_unit.py
 tests/rest/__init__.py
 tests/rest/query/__init__.py
-tests/rest/query/tests_permissions.py
+tests/rest/query/views/__init__.py
+tests/rest/query/views/tests_unit.py
 tests/rest/result/__init__.py
-tests/rest/result/tests_permissions.py
+tests/rest/result/tests_permissions.py
+tests/rest/result/tests_unit.py
+tests/utils/__init__.py
+tests/utils/linked_records/__init__.py
+tests/utils/linked_records/tests_pid.py
+tests/utils/oaipmh/__init__.py
+tests/utils/oaipmh/tests_oaipmh.py
+tests/utils/query/__init__.py
+tests/utils/query/tests_query.py
+tests/views/__init__.py
+tests/views/test_unit.py
```

### Comparing `core_explore_common_app-2.2.0/setup.py` & `core_explore_common_app-2.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 chdir(normpath(join(abspath(__file__), pardir)))
 
 dep_links = [r for r in required if r.startswith("https://")]
 required = [req_link(r) if r.startswith("https://") else r for r in required]
 
 setup(
     name="core_explore_common_app",
-    version="2.2.0",
+    version="2.3.0",
     description="Base exploration function for the curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_explore_common_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_explore_common_app-2.2.0/tests/components/query/tests_unit.py` & `core_explore_common_app-2.3.0/tests/components/query/tests_unit.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 """ Unit Test Query
 """
 from unittest.case import TestCase
+from unittest.mock import patch, MagicMock
+
+from django.test import override_settings
 
-from unittest.mock import patch
-from core_main_app.commons import exceptions
-from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from core_explore_common_app.components.abstract_query.models import (
     Authentication,
     DataSource,
 )
-from core_explore_common_app.settings import QUERY_VISIBILITY
 from core_explore_common_app.components.query import api as query_api
 from core_explore_common_app.components.query.models import Query
+from core_explore_common_app.settings import QUERY_VISIBILITY, SERVER_URI
+from core_main_app.commons import exceptions
+from core_main_app.utils.tests_tools.MockUser import create_mock_user
+from core_main_app.utils.tests_tools.RequestMock import create_mock_request
 
 
 class TestQueryUpsert(TestCase):
     """Test Query Upsert"""
 
     @patch.object(Query, "save")
     def test_upsert_query_returns_query(self, mock_save):
@@ -197,15 +200,41 @@
 
         for data_source in query.data_sources:
             self.assertTrue(
                 data_source["query_options"]["visibility"], QUERY_VISIBILITY
             )
 
 
-def _create_data_source(name="Local", url="/url"):
+class TestAddLocalDataSource(TestCase):
+    """TestAddLocalDataSource"""
+
+    @override_settings(INSTALLED_APPS=[])
+    @patch(
+        "core_explore_common_app.utils.query.query.create_local_data_source"
+    )
+    @patch("core_explore_common_app.components.query.api.add_data_source")
+    def test_add_local_data_source(
+        self, mock_create_local_data_source, mock_add_data_source
+    ):
+        """test_upsert_query_returns_query
+
+        Returns:
+
+        """
+        # Arrange
+        mock_user = create_mock_user(1)
+        mock_request = create_mock_request(mock_user)
+
+        mock_data_source = MagicMock()
+        mock_create_local_data_source.return_value = mock_data_source
+        mock_add_data_source.return_value = None
+        query_api.add_local_data_source(mock_request, mock_data_source)
+
+
+def _create_data_source(name="Local", url=SERVER_URI):
     """_create_data_source
 
     Returns:
     """
     authentication = Authentication(auth_type="session")
     data_source = DataSource(
         name=name, url_query=url, authentication=authentication
```

### Comparing `core_explore_common_app-2.2.0/tests/rest/result/tests_permissions.py` & `core_explore_common_app-2.3.0/tests/rest/result/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.2.0/tests/test_settings.py` & `core_explore_common_app-2.3.0/tests/test_settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,18 @@
     "django.contrib.sessions",
     "django.contrib.messages",
     "django.contrib.sites",
     "django_celery_beat",
     # Local apps
     "tests",
     "core_main_app",
+    "core_linked_records_app",
+    "core_oaipmh_harvester_app",
     "core_explore_common_app",
+    "core_explore_oaipmh_app",
 ]
 
 # IN-MEMORY TEST DATABASE
 DATABASES = {
     "default": {
         "ENGINE": "django.db.backends.sqlite3",
         "NAME": ":memory:",
@@ -54,12 +57,14 @@
                 "django.contrib.messages.context_processors.messages",
                 "django.template.context_processors.i18n",
             ],
         },
     },
 ]
 
-ROOT_URLCONF = "core_explore_common_app.urls"
+ROOT_URLCONF = "tests.urls"
 DEFAULT_AUTO_FIELD = "django.db.models.AutoField"
 CELERYBEAT_SCHEDULER = "django_celery_beat.schedulers:DatabaseScheduler"
 MONGODB_INDEXING = False
 MONGODB_ASYNC_SAVE = False
+CAN_ANONYMOUS_ACCESS_PUBLIC_DOCUMENT = False
+ENABLE_SAML2_SSO_AUTH = False
```

