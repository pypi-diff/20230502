# Comparing `tmp/core_explore_keyword_app-2.2.0.tar.gz` & `tmp/core_explore_keyword_app-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/core_explore_keyword_app-2.2.0.tar", last modified: Thu Feb 23 20:28:43 2023, max compression
+gzip compressed data, was "core_explore_keyword_app-2.3.0.tar", last modified: Tue May  2 19:37:55 2023, max compression
```

## Comparing `core_explore_keyword_app-2.2.0.tar` & `core_explore_keyword_app-2.3.0.tar`

### file list

```diff
@@ -1,162 +1,166 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:43.000000 core_explore_keyword_app-2.2.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      156 2023-02-23 20:28:37.000000 core_explore_keyword_app-2.2.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3190 2023-02-23 20:28:43.000000 core_explore_keyword_app-2.2.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2305 2023-02-23 20:28:37.000000 core_explore_keyword_app-2.2.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:41.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       95 2023-02-23 20:28:37.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1696 2023-02-23 20:28:37.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/admin.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      512 2023-02-23 20:28:37.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/apps.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:41.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:37.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:41.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/components/persistent_query_keyword/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:37.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/components/persistent_query_keyword/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      372 2023-02-23 20:28:37.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/components/persistent_query_keyword/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2256 2023-02-23 20:28:37.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/components/persistent_query_keyword/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1972 2023-02-23 20:28:37.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/components/persistent_query_keyword/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:41.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/components/search_operator/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       34 2023-02-23 20:28:37.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/components/search_operator/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      372 2023-02-23 20:28:37.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/components/search_operator/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2367 2023-02-23 20:28:37.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/components/search_operator/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3134 2023-02-23 20:28:37.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/components/search_operator/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1988 2023-02-23 20:28:37.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      818 2023-02-23 20:28:37.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/menus.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:41.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/migrations/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3571 2023-02-23 20:28:37.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/migrations/0001_initial.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:37.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/migrations/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      541 2023-02-23 20:28:37.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:41.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/permissions/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:37.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/permissions/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1117 2023-02-23 20:28:37.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/permissions/discover.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      152 2023-02-23 20:28:37.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/permissions/rights.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:41.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:37.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:41.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/rest/persistent_query_keyword/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:37.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/rest/persistent_query_keyword/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3197 2023-02-23 20:28:37.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/rest/persistent_query_keyword/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12256 2023-02-23 20:28:37.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/rest/persistent_query_keyword/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:41.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/rest/search_operators/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:37.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/rest/search_operators/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1343 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/rest/search_operators/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7434 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/rest/search_operators/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1688 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/rest/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      510 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:40.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:41.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/static/core_explore_keyword_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:40.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/static/core_explore_keyword_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:41.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/static/core_explore_keyword_app/admin/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      129 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/static/core_explore_keyword_app/admin/css/search_ops_manager.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:41.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/static/core_explore_keyword_app/admin/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      183 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/static/core_explore_keyword_app/admin/js/search_operators.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3599 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/static/core_explore_keyword_app/admin/js/search_ops_manager.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      951 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/static/core_explore_keyword_app/admin/js/search_ops_manager_delete.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:40.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:41.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/stretchy/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2930 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/stretchy/stretchy.min.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:40.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/tag-it/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:41.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/tag-it/2.0/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:41.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/tag-it/2.0/css/
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     1398 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/tag-it/2.0/css/jquery.tagit.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:41.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/tag-it/2.0/js/
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)    23552 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/tag-it/2.0/js/tag-it.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:41.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/static/core_explore_keyword_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:41.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/static/core_explore_keyword_app/user/css/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:42.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/static/core_explore_keyword_app/user/css/search/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3398 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/static/core_explore_keyword_app/user/css/search/search.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:42.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/static/core_explore_keyword_app/user/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      320 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/static/core_explore_keyword_app/user/js/persistent_query.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:42.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/static/core_explore_keyword_app/user/js/search/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      554 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/static/core_explore_keyword_app/user/js/search/autocomplete_source.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      283 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/static/core_explore_keyword_app/user/js/search/embedded_search.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10050 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/static/core_explore_keyword_app/user/js/search/search.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      156 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/static/core_explore_keyword_app/user/js/search/search.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:41.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:41.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/templates/core_explore_keyword_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:42.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:42.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1694 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/box.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:41.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/modal/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:42.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/modal/config/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      856 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/modal/config/form.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      705 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/modal/config/modal.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:42.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/modal/delete/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      778 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/modal/delete/modal.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      282 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:42.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1081 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/embedded_search_bar.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      350 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/extras.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      978 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/index.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      575 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/search_bar.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1337 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/template_filter.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:42.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/templatetags/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/templatetags/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1789 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/templatetags/core_explore_keyword_app_search_bar.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1484 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:42.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/utils/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      689 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/utils/abstract_keyword_search_extras.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2059 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/utils/search_operators.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:42.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:42.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/views/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       43 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/views/admin/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3858 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/views/admin/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2421 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/views/admin/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2389 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/views/admin/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:42.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7205 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/views/user/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    16344 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app/views/user/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:41.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3190 2023-02-23 20:28:40.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5707 2023-02-23 20:28:40.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-02-23 20:28:40.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       98 2023-02-23 20:28:40.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       36 2023-02-23 20:28:40.000000 core_explore_keyword_app-2.2.0/core_explore_keyword_app.egg-info/top_level.txt
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:42.000000 core_explore_keyword_app-2.2.0/docs/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/docs/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11113 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/docs/conf.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      311 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/docs/conf_urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       52 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-02-23 20:28:43.000000 core_explore_keyword_app-2.2.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1078 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:42.000000 core_explore_keyword_app-2.2.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:42.000000 core_explore_keyword_app-2.2.0/tests/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/tests/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:42.000000 core_explore_keyword_app-2.2.0/tests/components/persistent_query_keyword/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/tests/components/persistent_query_keyword/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:42.000000 core_explore_keyword_app-2.2.0/tests/components/persistent_query_keyword/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/tests/components/persistent_query_keyword/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1545 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/tests/components/persistent_query_keyword/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    15827 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/tests/components/persistent_query_keyword/tests_int_access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12126 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/tests/components/persistent_query_keyword/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:42.000000 core_explore_keyword_app-2.2.0/tests/components/search_operator/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/tests/components/search_operator/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5362 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/tests/components/search_operator/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:42.000000 core_explore_keyword_app-2.2.0/tests/forms/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/tests/forms/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1772 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/tests/forms/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:42.000000 core_explore_keyword_app-2.2.0/tests/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/tests/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:42.000000 core_explore_keyword_app-2.2.0/tests/rest/persistent_query_keyword/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/tests/rest/persistent_query_keyword/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11631 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/tests/rest/persistent_query_keyword/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17581 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/tests/rest/persistent_query_keyword/tests_permissions.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:42.000000 core_explore_keyword_app-2.2.0/tests/rest/search_operators/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/tests/rest/search_operators/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9668 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/tests/rest/search_operators/tests_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14457 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/tests/rest/search_operators/tests_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1899 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/tests/test_settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:42.000000 core_explore_keyword_app-2.2.0/tests/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/tests/utils/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:42.000000 core_explore_keyword_app-2.2.0/tests/utils/search_operators/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/tests/utils/search_operators/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4248 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/tests/utils/search_operators/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:43.000000 core_explore_keyword_app-2.2.0/tests/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/tests/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:43.000000 core_explore_keyword_app-2.2.0/tests/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/tests/views/user/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:43.000000 core_explore_keyword_app-2.2.0/tests/views/user/ajax/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:28:38.000000 core_explore_keyword_app-2.2.0/tests/views/user/ajax/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12745 2023-02-23 20:28:39.000000 core_explore_keyword_app-2.2.0/tests/views/user/ajax/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:55.300497 core_explore_keyword_app-2.3.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:37:49.000000 core_explore_keyword_app-2.3.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      156 2023-05-02 19:37:49.000000 core_explore_keyword_app-2.3.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3190 2023-05-02 19:37:55.295951 core_explore_keyword_app-2.3.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2305 2023-05-02 19:37:49.000000 core_explore_keyword_app-2.3.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:53.542646 core_explore_keyword_app-2.3.0/core_explore_keyword_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       95 2023-05-02 19:37:49.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1696 2023-05-02 19:37:49.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/admin.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      512 2023-05-02 19:37:49.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/apps.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:53.651986 core_explore_keyword_app-2.3.0/core_explore_keyword_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:49.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:53.723610 core_explore_keyword_app-2.3.0/core_explore_keyword_app/components/persistent_query_keyword/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:49.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/components/persistent_query_keyword/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      372 2023-05-02 19:37:49.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/components/persistent_query_keyword/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2256 2023-05-02 19:37:49.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/components/persistent_query_keyword/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1972 2023-05-02 19:37:49.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/components/persistent_query_keyword/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:53.774318 core_explore_keyword_app-2.3.0/core_explore_keyword_app/components/search_operator/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       34 2023-05-02 19:37:49.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/components/search_operator/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      372 2023-05-02 19:37:49.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/components/search_operator/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2367 2023-05-02 19:37:49.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/components/search_operator/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3134 2023-05-02 19:37:49.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/components/search_operator/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1988 2023-05-02 19:37:49.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      818 2023-05-02 19:37:49.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/menus.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:53.802647 core_explore_keyword_app-2.3.0/core_explore_keyword_app/migrations/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3571 2023-05-02 19:37:49.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/migrations/0001_initial.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:49.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/migrations/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      541 2023-05-02 19:37:49.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:53.852909 core_explore_keyword_app-2.3.0/core_explore_keyword_app/permissions/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:49.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/permissions/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1117 2023-05-02 19:37:49.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/permissions/discover.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      152 2023-05-02 19:37:49.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/permissions/rights.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:53.902802 core_explore_keyword_app-2.3.0/core_explore_keyword_app/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:49.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:53.944966 core_explore_keyword_app-2.3.0/core_explore_keyword_app/rest/persistent_query_keyword/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:49.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/rest/persistent_query_keyword/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3197 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/rest/persistent_query_keyword/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12256 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/rest/persistent_query_keyword/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:53.997520 core_explore_keyword_app-2.3.0/core_explore_keyword_app/rest/search_operators/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/rest/search_operators/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1343 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/rest/search_operators/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7434 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/rest/search_operators/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1688 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/rest/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      510 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:53.038404 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:53.105840 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:53.049435 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:54.019501 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/admin/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      129 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/admin/css/search_ops_manager.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:54.087281 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/admin/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      183 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/admin/js/search_operators.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3599 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/admin/js/search_ops_manager.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      951 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/admin/js/search_ops_manager_delete.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:53.085800 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:54.107581 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/stretchy/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2930 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/stretchy/stretchy.min.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:53.089859 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/tag-it/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:53.098310 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/tag-it/2.0/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:54.127486 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/tag-it/2.0/css/
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     1398 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/tag-it/2.0/css/jquery.tagit.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:54.162464 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/tag-it/2.0/js/
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)    23552 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/tag-it/2.0/js/tag-it.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:53.130344 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:53.120169 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/user/css/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:54.182606 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/user/css/search/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3476 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/user/css/search/search.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:54.215008 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/user/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      320 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/user/js/persistent_query.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:54.303198 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/user/js/search/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      554 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/user/js/search/autocomplete_source.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      283 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/user/js/search/embedded_search.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10050 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/user/js/search/search.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      156 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/user/js/search/search.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:53.155071 core_explore_keyword_app-2.3.0/core_explore_keyword_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:53.197289 core_explore_keyword_app-2.3.0/core_explore_keyword_app/templates/core_explore_keyword_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:54.327239 core_explore_keyword_app-2.3.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:54.342385 core_explore_keyword_app-2.3.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1694 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/box.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:53.191901 core_explore_keyword_app-2.3.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/modal/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:54.372728 core_explore_keyword_app-2.3.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/modal/config/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      856 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/modal/config/form.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      705 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/modal/config/modal.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:54.386659 core_explore_keyword_app-2.3.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/modal/delete/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      778 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/modal/delete/modal.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      282 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:54.475830 core_explore_keyword_app-2.3.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1081 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/embedded_search_bar.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      350 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/extras.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      978 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/index.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      575 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/search_bar.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1415 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/template_filter.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:54.505218 core_explore_keyword_app-2.3.0/core_explore_keyword_app/templatetags/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/templatetags/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1725 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/templatetags/core_explore_keyword_app_search_bar.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1484 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:54.551290 core_explore_keyword_app-2.3.0/core_explore_keyword_app/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/utils/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      689 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/utils/abstract_keyword_search_extras.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2059 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/utils/search_operators.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:54.567191 core_explore_keyword_app-2.3.0/core_explore_keyword_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:54.625048 core_explore_keyword_app-2.3.0/core_explore_keyword_app/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       43 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/views/admin/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3858 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/views/admin/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2421 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/views/admin/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2389 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/views/admin/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:54.670234 core_explore_keyword_app-2.3.0/core_explore_keyword_app/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6904 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/views/user/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    16154 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/views/user/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:53.633334 core_explore_keyword_app-2.3.0/core_explore_keyword_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3190 2023-05-02 19:37:52.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5781 2023-05-02 19:37:52.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:37:52.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       98 2023-05-02 19:37:52.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       36 2023-05-02 19:37:52.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app.egg-info/top_level.txt
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:54.723987 core_explore_keyword_app-2.3.0/docs/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/docs/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11113 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/docs/conf.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      311 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/docs/conf_urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       52 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:37:55.302606 core_explore_keyword_app-2.3.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1078 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:54.759382 core_explore_keyword_app-2.3.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:54.776020 core_explore_keyword_app-2.3.0/tests/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/tests/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:54.822704 core_explore_keyword_app-2.3.0/tests/components/persistent_query_keyword/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/tests/components/persistent_query_keyword/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:54.854741 core_explore_keyword_app-2.3.0/tests/components/persistent_query_keyword/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/tests/components/persistent_query_keyword/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1545 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/tests/components/persistent_query_keyword/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    15787 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/tests/components/persistent_query_keyword/tests_int_access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12126 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/tests/components/persistent_query_keyword/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:54.886417 core_explore_keyword_app-2.3.0/tests/components/search_operator/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/tests/components/search_operator/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5362 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/tests/components/search_operator/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:54.917807 core_explore_keyword_app-2.3.0/tests/forms/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/tests/forms/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1772 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/tests/forms/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:54.933353 core_explore_keyword_app-2.3.0/tests/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/tests/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:54.986933 core_explore_keyword_app-2.3.0/tests/rest/persistent_query_keyword/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/tests/rest/persistent_query_keyword/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11606 2023-05-02 19:37:51.000000 core_explore_keyword_app-2.3.0/tests/rest/persistent_query_keyword/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17581 2023-05-02 19:37:51.000000 core_explore_keyword_app-2.3.0/tests/rest/persistent_query_keyword/tests_permissions.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:55.114725 core_explore_keyword_app-2.3.0/tests/rest/search_operators/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:51.000000 core_explore_keyword_app-2.3.0/tests/rest/search_operators/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9668 2023-05-02 19:37:51.000000 core_explore_keyword_app-2.3.0/tests/rest/search_operators/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14457 2023-05-02 19:37:51.000000 core_explore_keyword_app-2.3.0/tests/rest/search_operators/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:55.156314 core_explore_keyword_app-2.3.0/tests/templatetags/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:51.000000 core_explore_keyword_app-2.3.0/tests/templatetags/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1381 2023-05-02 19:37:51.000000 core_explore_keyword_app-2.3.0/tests/templatetags/test_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1929 2023-05-02 19:37:51.000000 core_explore_keyword_app-2.3.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:55.171191 core_explore_keyword_app-2.3.0/tests/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:51.000000 core_explore_keyword_app-2.3.0/tests/utils/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:55.206800 core_explore_keyword_app-2.3.0/tests/utils/search_operators/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:51.000000 core_explore_keyword_app-2.3.0/tests/utils/search_operators/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4248 2023-05-02 19:37:51.000000 core_explore_keyword_app-2.3.0/tests/utils/search_operators/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:55.220317 core_explore_keyword_app-2.3.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:51.000000 core_explore_keyword_app-2.3.0/tests/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:55.235762 core_explore_keyword_app-2.3.0/tests/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:51.000000 core_explore_keyword_app-2.3.0/tests/views/user/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:55.272966 core_explore_keyword_app-2.3.0/tests/views/user/ajax/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:51.000000 core_explore_keyword_app-2.3.0/tests/views/user/ajax/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12542 2023-05-02 19:37:51.000000 core_explore_keyword_app-2.3.0/tests/views/user/ajax/tests_unit.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `core_explore_keyword_app-2.2.0/PKG-INFO` & `core_explore_keyword_app-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_explore_keyword_app
-Version: 2.2.0
+Version: 2.3.0
 Summary: Exploration by keywords for the curator core project
 Home-page: https://github.com/usnistgov/core_explore_keyword_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: ========================
         Core Explore Keyword App
```

### Comparing `core_explore_keyword_app-2.2.0/README.rst` & `core_explore_keyword_app-2.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.2.0/core_explore_keyword_app/admin.py` & `core_explore_keyword_app-2.3.0/core_explore_keyword_app/admin.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.2.0/core_explore_keyword_app/apps.py` & `core_explore_keyword_app-2.3.0/core_explore_keyword_app/apps.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.2.0/core_explore_keyword_app/components/persistent_query_keyword/api.py` & `core_explore_keyword_app-2.3.0/core_explore_keyword_app/components/persistent_query_keyword/api.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.2.0/core_explore_keyword_app/components/persistent_query_keyword/models.py` & `core_explore_keyword_app-2.3.0/core_explore_keyword_app/components/persistent_query_keyword/models.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.2.0/core_explore_keyword_app/components/search_operator/api.py` & `core_explore_keyword_app-2.3.0/core_explore_keyword_app/components/search_operator/api.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.2.0/core_explore_keyword_app/components/search_operator/models.py` & `core_explore_keyword_app-2.3.0/core_explore_keyword_app/components/search_operator/models.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.2.0/core_explore_keyword_app/forms.py` & `core_explore_keyword_app-2.3.0/core_explore_keyword_app/forms.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.2.0/core_explore_keyword_app/menus.py` & `core_explore_keyword_app-2.3.0/core_explore_keyword_app/menus.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.2.0/core_explore_keyword_app/migrations/0001_initial.py` & `core_explore_keyword_app-2.3.0/core_explore_keyword_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.2.0/core_explore_keyword_app/models.py` & `core_explore_keyword_app-2.3.0/core_explore_keyword_app/models.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.2.0/core_explore_keyword_app/permissions/discover.py` & `core_explore_keyword_app-2.3.0/core_explore_keyword_app/permissions/discover.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.2.0/core_explore_keyword_app/rest/persistent_query_keyword/serializers.py` & `core_explore_keyword_app-2.3.0/core_explore_keyword_app/rest/persistent_query_keyword/serializers.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.2.0/core_explore_keyword_app/rest/persistent_query_keyword/views.py` & `core_explore_keyword_app-2.3.0/core_explore_keyword_app/rest/persistent_query_keyword/views.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.2.0/core_explore_keyword_app/rest/search_operators/serializers.py` & `core_explore_keyword_app-2.3.0/core_explore_keyword_app/rest/search_operators/serializers.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.2.0/core_explore_keyword_app/rest/search_operators/views.py` & `core_explore_keyword_app-2.3.0/core_explore_keyword_app/rest/search_operators/views.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.2.0/core_explore_keyword_app/rest/urls.py` & `core_explore_keyword_app-2.3.0/core_explore_keyword_app/rest/urls.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.2.0/core_explore_keyword_app/static/core_explore_keyword_app/admin/js/search_ops_manager.js` & `core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/admin/js/search_ops_manager.js`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.2.0/core_explore_keyword_app/static/core_explore_keyword_app/admin/js/search_ops_manager_delete.js` & `core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/admin/js/search_ops_manager_delete.js`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.2.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/stretchy/stretchy.min.js` & `core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/stretchy/stretchy.min.js`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.2.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/tag-it/2.0/css/jquery.tagit.css` & `core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/tag-it/2.0/css/jquery.tagit.css`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.2.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/tag-it/2.0/js/tag-it.js` & `core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/tag-it/2.0/js/tag-it.js`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.2.0/core_explore_keyword_app/static/core_explore_keyword_app/user/css/search/search.css` & `core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/user/css/search/search.css`

 * *Files 9% similar despite different names*

```diff
@@ -181,8 +181,16 @@
 
 ul.tagit li.operator-bg-success-color input {
     margin-top: 3px;
 }
 
 ul.tagit li.operator-bg-error-color input{
     margin-top: 3px;
+}
+
+.row-template{
+    margin-top:0px;
+}
+
+.col-template{
+    padding-top: 0px;
 }
```

### Comparing `core_explore_keyword_app-2.2.0/core_explore_keyword_app/static/core_explore_keyword_app/user/js/search/autocomplete_source.js` & `core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/user/js/search/autocomplete_source.js`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.2.0/core_explore_keyword_app/static/core_explore_keyword_app/user/js/search/search.js` & `core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/user/js/search/search.js`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.2.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/box.html` & `core_explore_keyword_app-2.3.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/box.html`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.2.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/modal/config/form.html` & `core_explore_keyword_app-2.3.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/modal/config/form.html`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.2.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/modal/config/modal.html` & `core_explore_keyword_app-2.3.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/modal/config/modal.html`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.2.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/modal/delete/modal.html` & `core_explore_keyword_app-2.3.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/modal/delete/modal.html`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.2.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/embedded_search_bar.html` & `core_explore_keyword_app-2.3.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/embedded_search_bar.html`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.2.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/index.html` & `core_explore_keyword_app-2.3.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/index.html`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.2.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/search_bar.html` & `core_explore_keyword_app-2.3.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/search_bar.html`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.2.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/template_filter.html` & `core_explore_keyword_app-2.3.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/template_filter.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 {% if data.search_form.global_templates|length > 0 or data.search_form.user_templates|length > 0 %}
 {% if data.search_form.global_templates|length > 0 %}
 <div class="card">
     <div class="card-header">
-        <div class="row">
-            <div class="col-md-8">
+        <div class="row row-template">
+            <div class="col-md-8 col-template">
                 Filter by Template
             </div>
-            <div class="pl-0 col-md-4">
+            <div class="pl-0 col-md-4 col-template">
                 <div class="float-right">
                     <a class="selectAllGlobalTemplateButton" href="javascript:void(0)">
                         Select All
                     </a>
                 </div>
             </div>
         </div>
@@ -19,19 +19,19 @@
 <div class="list-group">
     {{ data.search_form.global_templates }}
 </div>
 {% endif %}
 {% if data.search_form.user_templates|length > 0 %}
 <div class="card">
     <div class="card-header">
-        <div class="row">
-            <div class="col-md-9">
+        <div class="row row-template">
+            <div class="col-md-9 col-template">
                 Filter by User Template
             </div>
-            <div class="pl-0 col-md-3">
+            <div class="pl-0 col-md-3 col-template">
                 <div class="float-right">
                     <a class="selectAllUserTemplateButton" href="javascript:void(0)">
                         Select All
                     </a>
                 </div>
             </div>
         </div>
```

### Comparing `core_explore_keyword_app-2.2.0/core_explore_keyword_app/templatetags/core_explore_keyword_app_search_bar.py` & `core_explore_keyword_app-2.3.0/core_explore_keyword_app/templatetags/core_explore_keyword_app_search_bar.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 from django import template
 
 from core_main_app.access_control.exceptions import AccessControlError
 from core_main_app.settings import DATA_SORTING_FIELDS
 from core_explore_common_app.components.query import api as query_api
 from core_explore_common_app.components.query.models import Query
-from core_explore_common_app.views.user.ajax import add_local_data_source
 from core_explore_keyword_app.forms import KeywordForm
 
 
 register = template.Library()
 
 
 @register.inclusion_tag(
@@ -29,15 +28,15 @@
     """
     request = context["request"]
     try:
         # create Query
         query = Query(user_id=str(request.user.id))
 
         # add local data source to the query
-        add_local_data_source(request, query)
+        query_api.add_local_data_source(request, query)
 
         # set visibility
         query_api.set_visibility_to_query(query, request.user)
 
         # upsert the query
         query_api.upsert(query, request.user)
```

### Comparing `core_explore_keyword_app-2.2.0/core_explore_keyword_app/urls.py` & `core_explore_keyword_app-2.3.0/core_explore_keyword_app/urls.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.2.0/core_explore_keyword_app/utils/abstract_keyword_search_extras.py` & `core_explore_keyword_app-2.3.0/core_explore_keyword_app/utils/abstract_keyword_search_extras.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.2.0/core_explore_keyword_app/utils/search_operators.py` & `core_explore_keyword_app-2.3.0/core_explore_keyword_app/utils/search_operators.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.2.0/core_explore_keyword_app/views/admin/ajax.py` & `core_explore_keyword_app-2.3.0/core_explore_keyword_app/views/admin/ajax.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.2.0/core_explore_keyword_app/views/admin/forms.py` & `core_explore_keyword_app-2.3.0/core_explore_keyword_app/views/admin/forms.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.2.0/core_explore_keyword_app/views/admin/views.py` & `core_explore_keyword_app-2.3.0/core_explore_keyword_app/views/admin/views.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.2.0/core_explore_keyword_app/views/user/ajax.py` & `core_explore_keyword_app-2.3.0/core_explore_keyword_app/views/user/ajax.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,80 +1,66 @@
 """Explore keyword app Ajax views
 """
 import json
 import logging
 import re
 
 from django.http import HttpResponse, HttpResponseBadRequest
-from django.urls import reverse_lazy
 from django.utils.decorators import method_decorator
 from django.views.generic import View
 
-from core_main_app.components.template import api as template_api
-from core_main_app.utils.databases.mongo.pymongo_database import (
-    get_full_text_query,
-)
 import core_main_app.components.template_version_manager.api as template_version_manager_api
-from core_main_app.utils import decorators
-
 from core_explore_common_app.components.query import api as query_api
-from core_explore_common_app.constants import LOCAL_QUERY_NAME
+from core_explore_common_app.rest.query.views import execute_local_query
 from core_explore_common_app.utils.query.query import (
-    send,
     create_local_data_source,
+    serialize_query,
+    is_local_data_source,
 )
 from core_explore_common_app.views.user.ajax import (
     CreatePersistentQueryUrlView,
 )
-from core_explore_keyword_app.permissions import rights
 from core_explore_keyword_app.components.persistent_query_keyword.models import (
     PersistentQueryKeyword,
 )
 from core_explore_keyword_app.forms import KeywordForm
+from core_explore_keyword_app.permissions import rights
+from core_main_app.components.template import api as template_api
+from core_main_app.utils import decorators
+from core_main_app.utils.databases.mongo.pymongo_database import (
+    get_full_text_query,
+)
 from core_main_app.utils.query.mongo.prepare import sanitize_value
 
 logger = logging.getLogger("core_explore_keyword_app.views.user.ajax")
 
 
-def _is_local_in_data_source(query):
+def _get_local_data_source(query):
     """Check if there is a data source that is local.
 
     Args:
         query:
 
     Returns:
     """
     # If we find a data source that is local
     for data_source in query.data_sources:
         # find local data source
-        if data_source["name"] == LOCAL_QUERY_NAME:
-            return True
-    return False
-
-
-def check_data_source(query):
-    """Check the data sources. We will not provide suggestions if there are data sources selected but none of them is local.
-
-    Args:
-        query:
-
-    Returns:
-    """
-
-    return len(query.data_sources) == 0 or _is_local_in_data_source(query)
+        if is_local_data_source(data_source):
+            return data_source
+    return None
 
 
 class SuggestionsKeywordSearchView(View):
     """Suggestions Keyword Search View"""
 
     @method_decorator(
         decorators.permission_required(
             content_type=rights.EXPLORE_KEYWORD_CONTENT_TYPE,
             permission=rights.EXPLORE_KEYWORD_ACCESS,
-            login_url=reverse_lazy("core_main_app_login"),
         )
     )
     def post(self, request, *args, **kwargs):
         """POST
 
         Args:
             request:
@@ -120,30 +106,31 @@
                 [template_ids.extend(x.versions) for x in version_manager_list]
             )
 
             if query_id is not None and keywords is not None:
                 # get query
                 query = query_api.get_by_id(query_id, request.user)
 
-                # Check the selected data sources
-                if check_data_source(query):
+                # Get local data source
+                local_data_source = _get_local_data_source(query)
+
+                if local_data_source:
 
                     # Prepare query
                     query = self._get_query_prepared(
                         keywords, query, request, template_ids
                     )
 
                     # Send query
-                    dict_results = send(
-                        request, query, len(query.data_sources) - 1, 1
-                    )
+                    json_query = serialize_query(query, local_data_source)
+                    dict_results = execute_local_query(json_query, 1, request)
 
-                    if dict_results["count"] > 0:
+                    if dict_results.paginator.count > 0:
                         self._extract_suggestion_from_results(
-                            dict_results, keywords, suggestions
+                            dict_results.object_list, keywords, suggestions
                         )
 
             return HttpResponse(
                 json.dumps({"suggestions": suggestions}),
                 content_type="application/javascript",
             )
         except Exception as exception:
@@ -173,36 +160,34 @@
         )
         # TODO: improve query to get better results
         query.content = json.dumps(get_full_text_query(keywords))
         # Data source is local
         query.data_sources = [create_local_data_source(request)]
         return query
 
-    def _extract_suggestion_from_results(
-        self, dict_results, keywords, suggestions
-    ):
+    @staticmethod
+    def _extract_suggestion_from_results(results, keywords, suggestions):
         """Extract suggestion from
 
         Args:
-            dict_results:
+            results:
             keywords:
             suggestions:
 
         Returns:
         """
-        results = dict_results["results"]
         # Prepare keywords
         word_list = re.sub(r"[^\w]", " ", keywords).split()
         word_list = [x + "|" + x + r"\w+" for x in word_list]
         word_list = "|".join(word_list)
         for result in results:
             # Extract suggestions from data
             list_whole_keywords = re.findall(
                 "\\b(" + word_list + ")\\b",
-                result["xml_content"],
+                result.xml_content,
                 flags=re.IGNORECASE,
             )
             labels = list(set(list_whole_keywords))
 
             for label in labels:
                 label = label.lower()
                 result_json = dict()
```

### Comparing `core_explore_keyword_app-2.2.0/core_explore_keyword_app/views/user/views.py` & `core_explore_keyword_app-2.3.0/core_explore_keyword_app/views/user/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Core Explore Keyword App views
 """
 import json
+from typing import Dict, Any, List
+
 from django.http import HttpResponseRedirect
-from django.urls import reverse_lazy, reverse
+from django.urls import reverse
 from django.utils.decorators import method_decorator
-from typing import Dict, Any, List
 
 import core_explore_keyword_app.components.persistent_query_keyword.api as persistent_query_keyword_api
 import core_main_app.components.template_version_manager.api as template_version_manager_api
 from core_explore_common_app.components.query import api as query_api
 from core_explore_common_app.settings import DEFAULT_DATE_TOGGLE_VALUE
 from core_explore_common_app.views.user.views import (
     ResultQueryRedirectView,
@@ -36,15 +37,14 @@
 
     query_builder_interface = "core_explore_keyword_app/user/search_bar.html"
 
     @method_decorator(
         decorators.permission_required(
             content_type=rights.EXPLORE_KEYWORD_CONTENT_TYPE,
             permission=rights.EXPLORE_KEYWORD_ACCESS,
-            login_url=reverse_lazy("core_main_app_login"),
         )
     )
     def get(self, request, **kwargs):
         """GET
 
         Args:
             request:
@@ -67,15 +67,14 @@
             context=context,
         )
 
     @method_decorator(
         decorators.permission_required(
             content_type=rights.EXPLORE_KEYWORD_CONTENT_TYPE,
             permission=rights.EXPLORE_KEYWORD_ACCESS,
-            login_url=reverse_lazy("core_main_app_login"),
         )
     )
     def post(self, request):
         """POST
 
         Args:
             request:
@@ -433,15 +432,14 @@
     object_name = "persistent_query_keyword"
     redirect_url = "core_explore_keyword_app_search"
 
     @method_decorator(
         decorators.permission_required(
             content_type=rights.EXPLORE_KEYWORD_CONTENT_TYPE,
             permission=rights.EXPLORE_KEYWORD_ACCESS,
-            login_url=reverse_lazy("core_main_app_login"),
         )
     )
     def get(self, request, *args, **kwargs):
         return super().get(self, request, *args, **kwargs)
 
     @staticmethod
     def _get_persistent_query_by_id(persistent_query_id, user):
```

### Comparing `core_explore_keyword_app-2.2.0/core_explore_keyword_app.egg-info/PKG-INFO` & `core_explore_keyword_app-2.3.0/core_explore_keyword_app.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-explore-keyword-app
-Version: 2.2.0
+Version: 2.3.0
 Summary: Exploration by keywords for the curator core project
 Home-page: https://github.com/usnistgov/core_explore_keyword_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: ========================
         Core Explore Keyword App
```

### Comparing `core_explore_keyword_app-2.2.0/core_explore_keyword_app.egg-info/SOURCES.txt` & `core_explore_keyword_app-2.3.0/core_explore_keyword_app.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.md
 MANIFEST.in
 README.rst
 pyproject.toml
 requirements.core.txt
 setup.py
 core_explore_keyword_app/__init__.py
 core_explore_keyword_app/admin.py
@@ -92,14 +93,16 @@
 tests/rest/__init__.py
 tests/rest/persistent_query_keyword/__init__.py
 tests/rest/persistent_query_keyword/tests_int.py
 tests/rest/persistent_query_keyword/tests_permissions.py
 tests/rest/search_operators/__init__.py
 tests/rest/search_operators/tests_permissions.py
 tests/rest/search_operators/tests_unit.py
+tests/templatetags/__init__.py
+tests/templatetags/test_unit.py
 tests/utils/__init__.py
 tests/utils/search_operators/__init__.py
 tests/utils/search_operators/tests_unit.py
 tests/views/__init__.py
 tests/views/user/__init__.py
 tests/views/user/ajax/__init__.py
 tests/views/user/ajax/tests_unit.py
```

### Comparing `core_explore_keyword_app-2.2.0/docs/conf.py` & `core_explore_keyword_app-2.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.2.0/setup.py` & `core_explore_keyword_app-2.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_explore_keyword_app",
-    version="2.2.0",
+    version="2.3.0",
     description="Exploration by keywords for the curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_explore_keyword_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_explore_keyword_app-2.2.0/tests/components/persistent_query_keyword/fixtures/fixtures.py` & `core_explore_keyword_app-2.3.0/tests/components/persistent_query_keyword/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.2.0/tests/components/persistent_query_keyword/tests_int_access_control.py` & `core_explore_keyword_app-2.3.0/tests/components/persistent_query_keyword/tests_int_access_control.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """ Unit Test Persistent Query Keyword
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
 import core_explore_keyword_app.components.persistent_query_keyword.api as persistent_query_keyword_api
 
@@ -19,15 +19,15 @@
 from tests.components.persistent_query_keyword.fixtures.fixtures import (
     PersistentQueryKeywordFixtures,
 )
 
 fixture_persistent_query_keyword = PersistentQueryKeywordFixtures()
 
 
-class TestPersistentQueryKeywordGetById(MongoIntegrationBaseTestCase):
+class TestPersistentQueryKeywordGetById(IntegrationBaseTestCase):
     """Test Persistent Query Keyword Get By Id"""
 
     fixture = fixture_persistent_query_keyword
 
     def test_get_by_id_as_superuser_returns_persistent_query_keyword(self):
         """test_get_by_id_as_superuser_returns_persistent_query_keyword"""
 
@@ -108,15 +108,15 @@
                     persistent_query_keyword_id, mock_user
                 ),
                 PersistentQueryKeyword,
             )
         )
 
 
-class TestPersistentQueryKeywordGetByName(MongoIntegrationBaseTestCase):
+class TestPersistentQueryKeywordGetByName(IntegrationBaseTestCase):
     """Test Persistent Query Keyword Get By Name"""
 
     fixture = fixture_persistent_query_keyword
 
     def test_get_by_name_as_superuser_returns_persistent_query_keyword(self):
         """test_get_by_name_as_superuser_returns_persistent_query_keyword"""
 
@@ -196,15 +196,15 @@
         else:
             with self.assertRaises(AccessControlError):
                 persistent_query_keyword_api.get_by_name(
                     persistent_query_keyword_name, AnonymousUser()
                 )
 
 
-class TestPersistentQueryKeywordDelete(MongoIntegrationBaseTestCase):
+class TestPersistentQueryKeywordDelete(IntegrationBaseTestCase):
     """Test Persistent Query Keyword Delete"""
 
     fixture = fixture_persistent_query_keyword
 
     def test_delete_others_persistent_query_keyword_as_superuser_deletes_persistent_query_keyword(
         self,
     ):
@@ -257,15 +257,15 @@
         # Act # Assert
         with self.assertRaises(AccessControlError):
             persistent_query_keyword_api.delete(
                 persistent_query_keyword, AnonymousUser()
             )
 
 
-class TestPersistentQueryKeywordUpdate(MongoIntegrationBaseTestCase):
+class TestPersistentQueryKeywordUpdate(IntegrationBaseTestCase):
     """Test Persistent Query Keyword Update"""
 
     fixture = fixture_persistent_query_keyword
 
     def test_update_others_persistent_query_keyword_as_superuser_updates_persistent_query_keyword(
         self,
     ):
@@ -325,15 +325,15 @@
         # Act # Assert
         with self.assertRaises(AccessControlError):
             persistent_query_keyword_api.upsert(
                 persistent_query_keyword, AnonymousUser()
             )
 
 
-class TestPersistentQueryKeywordCreate(MongoIntegrationBaseTestCase):
+class TestPersistentQueryKeywordCreate(IntegrationBaseTestCase):
     """Test Persistent Query Keyword Create"""
 
     fixture = fixture_persistent_query_keyword
 
     def test_create_others_persistent_query_keyword_as_superuser_creates_persistent_query_keyword(
         self,
     ):
@@ -391,15 +391,15 @@
         else:
             with self.assertRaises(AccessControlError):
                 persistent_query_keyword_api.upsert(
                     persistent_query_keyword, AnonymousUser()
                 )
 
 
-class TestPersistentQueryKeywordGetAll(MongoIntegrationBaseTestCase):
+class TestPersistentQueryKeywordGetAll(IntegrationBaseTestCase):
     """Test Persistent Query Keyword Get All"""
 
     fixture = fixture_persistent_query_keyword
 
     def test_get_all_as_superuser_returns_all_persistent_query_keyword(self):
         """test_get_all_as_superuser_returns_all_persistent_query_keyword"""
 
@@ -426,15 +426,15 @@
         """test_get_all_as_anonymous_user_raises_error"""
 
         # Assert
         with self.assertRaises(AccessControlError):
             persistent_query_keyword_api.get_all(AnonymousUser())
 
 
-class TestPersistentQueryKeywordGetAllByUser(MongoIntegrationBaseTestCase):
+class TestPersistentQueryKeywordGetAllByUser(IntegrationBaseTestCase):
     """Test Persistent Query Keyword Get All By User"""
 
     fixture = fixture_persistent_query_keyword
 
     def test_get_all_by_user_as_superuser_returns_all_user_persistent_query_keyword(
         self,
     ):
```

### Comparing `core_explore_keyword_app-2.2.0/tests/components/persistent_query_keyword/tests_unit.py` & `core_explore_keyword_app-2.3.0/tests/components/persistent_query_keyword/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.2.0/tests/components/search_operator/tests_unit.py` & `core_explore_keyword_app-2.3.0/tests/components/search_operator/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.2.0/tests/forms/tests_unit.py` & `core_explore_keyword_app-2.3.0/tests/forms/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.2.0/tests/rest/persistent_query_keyword/tests_int.py` & `core_explore_keyword_app-2.3.0/tests/rest/persistent_query_keyword/tests_int.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 """ Integration Test for Persistent Query Keyword Rest API
 """
 
 from django.contrib.auth.models import AnonymousUser
 from rest_framework import status
 
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from core_main_app.utils.tests_tools.RequestMock import RequestMock
 
 from core_explore_keyword_app.rest.persistent_query_keyword import (
     views as persistent_query_keyword_views,
 )
 from tests.components.persistent_query_keyword.fixtures.fixtures import (
     PersistentQueryKeywordFixtures,
 )
 
 fixture_data_structure = PersistentQueryKeywordFixtures()
 
 
-class TestPersistentQueryKeywordListAdmin(MongoIntegrationBaseTestCase):
+class TestPersistentQueryKeywordListAdmin(IntegrationBaseTestCase):
     """Test Persistent Query Keyword List Admin"""
 
     fixture = fixture_data_structure
 
     def setUp(self):
         """setUp"""
 
@@ -61,15 +61,15 @@
             data=self.data,
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_201_CREATED)
 
 
-class TestPersistentQueryKeywordList(MongoIntegrationBaseTestCase):
+class TestPersistentQueryKeywordList(IntegrationBaseTestCase):
     """Test Persistent Query Keyword List"""
 
     fixture = fixture_data_structure
 
     def setUp(self):
         """setUp"""
 
@@ -104,15 +104,15 @@
             data=self.data,
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_201_CREATED)
 
 
-class TestPersistentQueryKeywordDetail(MongoIntegrationBaseTestCase):
+class TestPersistentQueryKeywordDetail(IntegrationBaseTestCase):
     """Test Persistent Query Keyword Detail"""
 
     fixture = fixture_data_structure
 
     def setUp(self):
         """setUp"""
 
@@ -294,15 +294,15 @@
             param={"pk": -1},
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_404_NOT_FOUND)
 
 
-class TestPersistentQueryKeywordByName(MongoIntegrationBaseTestCase):
+class TestPersistentQueryKeywordByName(IntegrationBaseTestCase):
     """Test Persistent Query Keyword By Name"""
 
     fixture = fixture_data_structure
 
     def setUp(self):
         """setUp"""
```

### Comparing `core_explore_keyword_app-2.2.0/tests/rest/persistent_query_keyword/tests_permissions.py` & `core_explore_keyword_app-2.3.0/tests/rest/persistent_query_keyword/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.2.0/tests/rest/search_operators/tests_permissions.py` & `core_explore_keyword_app-2.3.0/tests/rest/search_operators/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.2.0/tests/rest/search_operators/tests_unit.py` & `core_explore_keyword_app-2.3.0/tests/rest/search_operators/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.2.0/tests/test_settings.py` & `core_explore_keyword_app-2.3.0/tests/test_settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,7 +65,8 @@
 ROOT_URLCONF = "core_main_app.urls"
 
 DEFAULT_AUTO_FIELD = "django.db.models.BigAutoField"
 
 CELERYBEAT_SCHEDULER = "django_celery_beat.schedulers:DatabaseScheduler"
 MONGODB_INDEXING = False
 MONGODB_ASYNC_SAVE = False
+ENABLE_SAML2_SSO_AUTH = False
```

### Comparing `core_explore_keyword_app-2.2.0/tests/utils/search_operators/tests_unit.py` & `core_explore_keyword_app-2.3.0/tests/utils/search_operators/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.2.0/tests/views/user/ajax/tests_unit.py` & `core_explore_keyword_app-2.3.0/tests/views/user/ajax/tests_unit.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,18 +3,21 @@
 import json
 from unittest import TestCase
 from unittest.mock import MagicMock, patch
 
 from django.test import RequestFactory
 from rest_framework import status
 
+from core_explore_common_app.constants import LOCAL_QUERY_NAME
 from core_explore_keyword_app.views.user.ajax import (
     SuggestionsKeywordSearchView,
+    _get_local_data_source,
 )
 from core_main_app.commons.exceptions import QueryError, DoesNotExist
+from core_main_app.settings import SERVER_URI
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 
 
 class TestSuggestionsKeywordSearchViewPost(TestCase):
     """Test SuggestionsKeywordSearchView post method"""
 
     @classmethod
@@ -106,220 +109,223 @@
             "mock_does_not_exist_error"
         )
 
         response = self._send_post_request()
 
         self.assertEquals(response.status_code, status.HTTP_400_BAD_REQUEST)
 
-    @patch("core_explore_keyword_app.views.user.ajax.check_data_source")
+    @patch("core_explore_keyword_app.views.user.ajax._get_local_data_source")
     @patch("core_explore_keyword_app.views.user.ajax.query_api.get_by_id")
     @patch(
         "core_explore_keyword_app.views.user.ajax.template_version_manager_api.get_by_id_list"
     )
     @patch("core_explore_keyword_app.views.user.ajax.sanitize_value")
     @patch("core_explore_keyword_app.views.user.ajax.KeywordForm")
-    def test_check_data_source_fails_returns_400(
+    def test_get_local_data_source_fails_returns_400(
         self,
         mock_keyword_form,
         mock_sanitize_value,
         mock_template_get_by_id,
         mock_query_get_by_id,
-        mock_check_data_source,
+        mock_get_local_data_source,
     ):
-        """test_check_data_source_fails_returns_400"""
+        """test_get_local_data_source_fails_returns_400"""
         mock_keyword_form.return_value = MagicMock()
         mock_sanitize_value.return_value = None
         mock_template_get_by_id.return_value = []
         mock_query_get_by_id.return_value = MagicMock()
-        mock_check_data_source.side_effect = Exception(
-            "mock_check_data_source_exception"
+        mock_get_local_data_source.side_effect = Exception(
+            "mock_get_local_data_source_exception"
         )
 
         response = self._send_post_request()
 
         self.assertEquals(response.status_code, status.HTTP_400_BAD_REQUEST)
 
     @patch(
         "core_explore_keyword_app.views.user.ajax.SuggestionsKeywordSearchView._get_query_prepared"
     )
-    @patch("core_explore_keyword_app.views.user.ajax.check_data_source")
+    @patch("core_explore_keyword_app.views.user.ajax._get_local_data_source")
     @patch("core_explore_keyword_app.views.user.ajax.query_api.get_by_id")
     @patch(
         "core_explore_keyword_app.views.user.ajax.template_version_manager_api.get_by_id_list"
     )
     @patch("core_explore_keyword_app.views.user.ajax.sanitize_value")
     @patch("core_explore_keyword_app.views.user.ajax.KeywordForm")
     def test_get_query_prepared_fails_returns_400(
         self,
         mock_keyword_form,
         mock_sanitize_value,
         mock_template_get_by_id,
         mock_query_get_by_id,
-        mock_check_data_source,
+        mock_get_local_data_source,
         mock_get_query_prepared,
     ):
         """test_get_query_prepared_fails_returns_400"""
         mock_keyword_form.return_value = MagicMock()
         mock_sanitize_value.return_value = None
         mock_template_get_by_id.return_value = []
         mock_query_get_by_id.return_value = MagicMock()
-        mock_check_data_source.return_value = True
+        mock_get_local_data_source.return_value = {
+            "query_options": {},
+            "order_by_field": "title",
+        }
         mock_get_query_prepared.side_effect = Exception(
             "mock_get_query_prepared_exception"
         )
 
         response = self._send_post_request()
 
         self.assertEquals(response.status_code, status.HTTP_400_BAD_REQUEST)
 
-    @patch("core_explore_keyword_app.views.user.ajax.send")
-    @patch(
-        "core_explore_keyword_app.views.user.ajax.SuggestionsKeywordSearchView._get_query_prepared"
-    )
-    @patch("core_explore_keyword_app.views.user.ajax.check_data_source")
-    @patch("core_explore_keyword_app.views.user.ajax.query_api.get_by_id")
-    @patch(
-        "core_explore_keyword_app.views.user.ajax.template_version_manager_api.get_by_id_list"
-    )
-    @patch("core_explore_keyword_app.views.user.ajax.sanitize_value")
-    @patch("core_explore_keyword_app.views.user.ajax.KeywordForm")
-    def test_send_query_fails_returns_400(
-        self,
-        mock_keyword_form,
-        mock_sanitize_value,
-        mock_template_get_by_id,
-        mock_query_get_by_id,
-        mock_check_data_source,
-        mock_get_query_prepared,
-        mock_send_query,
-    ):
-        """test_send_query_fails_returns_400"""
-        mock_keyword_form.return_value = MagicMock()
-        mock_sanitize_value.return_value = None
-        mock_template_get_by_id.return_value = []
-        mock_query_get_by_id.return_value = MagicMock()
-        mock_check_data_source.return_value = True
-        mock_get_query_prepared.return_value = MagicMock()
-        mock_send_query.side_effect = Exception("mock_send_query_exception")
-
-        response = self._send_post_request()
-
-        self.assertEquals(response.status_code, status.HTTP_400_BAD_REQUEST)
-
     @patch(
         "core_explore_keyword_app.views.user.ajax.SuggestionsKeywordSearchView._extract_suggestion_from_results"
     )
-    @patch("core_explore_keyword_app.views.user.ajax.send")
     @patch(
         "core_explore_keyword_app.views.user.ajax.SuggestionsKeywordSearchView._get_query_prepared"
     )
-    @patch("core_explore_keyword_app.views.user.ajax.check_data_source")
+    @patch("core_explore_keyword_app.views.user.ajax._get_local_data_source")
     @patch("core_explore_keyword_app.views.user.ajax.query_api.get_by_id")
     @patch(
         "core_explore_keyword_app.views.user.ajax.template_version_manager_api.get_by_id_list"
     )
     @patch("core_explore_keyword_app.views.user.ajax.sanitize_value")
     @patch("core_explore_keyword_app.views.user.ajax.KeywordForm")
     def test_extract_suggestions_fails_returns_400(
         self,
         mock_keyword_form,
         mock_sanitize_value,
         mock_template_get_by_id,
         mock_query_get_by_id,
-        mock_check_data_source,
+        mock_get_local_data_source,
         mock_get_query_prepared,
-        mock_send_query,
         mock_extract_suggestion_from_results,
     ):
         """test_extract_suggestions_fails_returns_400"""
         mock_keyword_form.return_value = MagicMock()
         mock_sanitize_value.return_value = None
         mock_template_get_by_id.return_value = []
         mock_query_get_by_id.return_value = MagicMock()
-        mock_check_data_source.return_value = True
+        mock_get_local_data_source.return_value = {
+            "query_options": {},
+            "order_by_field": "title",
+        }
         mock_get_query_prepared.return_value = MagicMock()
-        mock_send_query.return_value = {"count": 1}
         mock_extract_suggestion_from_results.side_effect = Exception(
             "mock_extract_suggestion_from_results_exception"
         )
 
         response = self._send_post_request()
 
         self.assertEquals(response.status_code, status.HTTP_400_BAD_REQUEST)
 
     @patch(
         "core_explore_keyword_app.views.user.ajax.SuggestionsKeywordSearchView._extract_suggestion_from_results"
     )
-    @patch("core_explore_keyword_app.views.user.ajax.send")
+    @patch("core_main_app.components.data.api.execute_json_query")
     @patch(
         "core_explore_keyword_app.views.user.ajax.SuggestionsKeywordSearchView._get_query_prepared"
     )
-    @patch("core_explore_keyword_app.views.user.ajax.check_data_source")
+    @patch("core_explore_keyword_app.views.user.ajax._get_local_data_source")
     @patch("core_explore_keyword_app.views.user.ajax.query_api.get_by_id")
     @patch(
         "core_explore_keyword_app.views.user.ajax.template_version_manager_api.get_by_id_list"
     )
     @patch("core_explore_keyword_app.views.user.ajax.sanitize_value")
     @patch("core_explore_keyword_app.views.user.ajax.KeywordForm")
     def test_empty_dict_results_returns_200(
         self,
         mock_keyword_form,
         mock_sanitize_value,
         mock_template_get_by_id,
         mock_query_get_by_id,
-        mock_check_data_source,
+        mock_get_local_data_source,
         mock_get_query_prepared,
-        mock_send_query,
+        mock_execute_local_query,
         mock_extract_suggestion_from_results,
     ):
         """test_empty_dict_results_returns_200"""
         mock_keyword_form.return_value = MagicMock()
         mock_sanitize_value.return_value = None
         mock_template_get_by_id.return_value = []
         mock_query_get_by_id.return_value = MagicMock()
-        mock_check_data_source.return_value = True
+        mock_get_local_data_source.return_value = {
+            "query_options": {},
+            "order_by_field": "title",
+        }
         mock_get_query_prepared.return_value = MagicMock()
-        mock_send_query.return_value = {"count": 0}
+        mock_execute_local_query.return_value = MagicMock()
         mock_extract_suggestion_from_results.return_value = None
 
         response = self._send_post_request()
 
         self.assertEquals(response.status_code, status.HTTP_200_OK)
 
     @patch(
         "core_explore_keyword_app.views.user.ajax.SuggestionsKeywordSearchView._extract_suggestion_from_results"
     )
-    @patch("core_explore_keyword_app.views.user.ajax.send")
+    @patch("core_main_app.components.data.api.execute_json_query")
     @patch(
         "core_explore_keyword_app.views.user.ajax.SuggestionsKeywordSearchView._get_query_prepared"
     )
-    @patch("core_explore_keyword_app.views.user.ajax.check_data_source")
+    @patch("core_explore_keyword_app.views.user.ajax._get_local_data_source")
     @patch("core_explore_keyword_app.views.user.ajax.query_api.get_by_id")
     @patch(
         "core_explore_keyword_app.views.user.ajax.template_version_manager_api.get_by_id_list"
     )
     @patch("core_explore_keyword_app.views.user.ajax.sanitize_value")
     @patch("core_explore_keyword_app.views.user.ajax.KeywordForm")
     def test_dict_results_returns_suggestions(
         self,
         mock_keyword_form,
         mock_sanitize_value,
         mock_template_get_by_id,
         mock_query_get_by_id,
-        mock_check_data_source,
+        mock_get_local_data_source,
         mock_get_query_prepared,
-        mock_send_query,
+        mock_execute_json_query,
         mock_extract_suggestion_from_results,
     ):
         """test_dict_results_returns_suggestions"""
         mock_keyword_form.return_value = MagicMock()
         mock_sanitize_value.return_value = None
         mock_template_get_by_id.return_value = []
         mock_query_get_by_id.return_value = MagicMock()
-        mock_check_data_source.return_value = True
+        mock_get_local_data_source.return_value = {
+            "query_options": {},
+            "order_by_field": "title",
+        }
         mock_get_query_prepared.return_value = MagicMock()
-        mock_send_query.return_value = {"count": 0}
+        mock_execute_json_query.return_value = MagicMock()
         mock_extract_suggestion_from_results.return_value = None
 
         response = self._send_post_request()
 
         self.assertEquals(json.loads(response.content), {"suggestions": []})
+
+
+class TestGetLocalDataSource(TestCase):
+    """TestGetLocalDataSource"""
+
+    def test_get_local_data_source(self):
+        """test_get_local_data_source
+
+        Returns:
+
+        """
+        mock_query = MagicMock()
+        mock_query.data_sources = [
+            {"name": LOCAL_QUERY_NAME, "url_query": SERVER_URI}
+        ]
+        data_source = _get_local_data_source(mock_query)
+        self.assertIsNotNone(data_source)
+
+    def test_get_local_data_source_returns_none(self):
+        """test_get_local_data_source_returns_none
+
+        Returns:
+
+        """
+        mock_query = MagicMock()
+        mock_query.data_sources = [{"name": "test", "url_query": SERVER_URI}]
+        data_source = _get_local_data_source(mock_query)
+        self.assertIsNone(data_source)
```

