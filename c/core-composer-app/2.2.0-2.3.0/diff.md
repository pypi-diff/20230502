# Comparing `tmp/core_composer_app-2.2.0.tar.gz` & `tmp/core_composer_app-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/core_composer_app-2.2.0.tar", last modified: Thu Feb 23 20:26:33 2023, max compression
+gzip compressed data, was "core_composer_app-2.3.0.tar", last modified: Tue May  2 19:34:00 2023, max compression
```

## Comparing `core_composer_app-2.2.0.tar` & `core_composer_app-2.3.0.tar`

### file list

```diff
@@ -1,188 +1,189 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:33.000000 core_composer_app-2.2.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      142 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1038 2023-02-23 20:26:33.000000 core_composer_app-2.2.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      548 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:24.000000 core_composer_app-2.2.0/core_composer_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      105 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3401 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/admin.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      494 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/apps.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:24.000000 core_composer_app-2.2.0/core_composer_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:25.000000 core_composer_app-2.2.0/core_composer_app/components/bucket/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/components/bucket/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2542 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/components/bucket/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2390 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/components/bucket/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:26.000000 core_composer_app-2.2.0/core_composer_app/components/type/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/components/type/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      346 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/components/type/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1460 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/components/type/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1040 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/components/type/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:27.000000 core_composer_app-2.2.0/core_composer_app/components/type_version_manager/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/components/type_version_manager/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      355 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/components/type_version_manager/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3924 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/components/type_version_manager/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2375 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/components/type_version_manager/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      630 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/menus.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:27.000000 core_composer_app-2.2.0/core_composer_app/migrations/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3384 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/migrations/0001_initial.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/migrations/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      777 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:27.000000 core_composer_app-2.2.0/core_composer_app/permissions/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/permissions/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1295 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/permissions/discover.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      191 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/permissions/rights.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:27.000000 core_composer_app-2.2.0/core_composer_app/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:29.000000 core_composer_app-2.2.0/core_composer_app/rest/bucket/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/rest/bucket/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1680 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/rest/bucket/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10151 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/rest/bucket/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:29.000000 core_composer_app-2.2.0/core_composer_app/rest/type_version_manager/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/rest/type_version_manager/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5479 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/rest/type_version_manager/abstract_views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2390 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/rest/type_version_manager/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3366 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/rest/type_version_manager/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3225 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/rest/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      121 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:09.000000 core_composer_app-2.2.0/core_composer_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:19.000000 core_composer_app-2.2.0/core_composer_app/static/core_composer_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:09.000000 core_composer_app-2.2.0/core_composer_app/static/core_composer_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:29.000000 core_composer_app-2.2.0/core_composer_app/static/core_composer_app/admin/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      753 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/static/core_composer_app/admin/js/bucket.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       80 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/static/core_composer_app/admin/js/bucket.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:19.000000 core_composer_app-2.2.0/core_composer_app/static/core_composer_app/admin/js/types/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:29.000000 core_composer_app-2.2.0/core_composer_app/static/core_composer_app/admin/js/types/upload/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      983 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/static/core_composer_app/admin/js/types/upload/dependencies.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       98 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/static/core_composer_app/admin/js/types/upload/dependencies.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      143 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/static/core_composer_app/admin/js/types/upload/dependency_resolver.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:19.000000 core_composer_app-2.2.0/core_composer_app/static/core_composer_app/common/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:29.000000 core_composer_app-2.2.0/core_composer_app/static/core_composer_app/common/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      122 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/static/core_composer_app/common/css/bucket.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:19.000000 core_composer_app-2.2.0/core_composer_app/static/core_composer_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:29.000000 core_composer_app-2.2.0/core_composer_app/static/core_composer_app/user/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      532 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/static/core_composer_app/user/css/menu.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       56 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/static/core_composer_app/user/css/style.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       64 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/static/core_composer_app/user/css/xsd_tree.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:29.000000 core_composer_app-2.2.0/core_composer_app/static/core_composer_app/user/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3831 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/static/core_composer_app/user/js/build_template.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      713 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/static/core_composer_app/user/js/build_template.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10778 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/static/core_composer_app/user/js/menus.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1043 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/static/core_composer_app/user/js/xpath.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      444 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/static/core_composer_app/user/js/xsd_tree.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:29.000000 core_composer_app-2.2.0/core_composer_app/static/core_composer_app/user/xsd/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      202 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/static/core_composer_app/user/xsd/new_base_template.xsd
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:29.000000 core_composer_app-2.2.0/core_composer_app/static/core_composer_app/user/xsl/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4750 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/static/core_composer_app/user/xsl/xsd2html.xsl
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:19.000000 core_composer_app-2.2.0/core_composer_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:20.000000 core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:20.000000 core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:29.000000 core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/admin/buckets/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      168 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/admin/buckets/add.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      922 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/admin/buckets/add_content.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      348 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/admin/buckets/edit.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1204 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/admin/buckets/edit_content.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:29.000000 core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/admin/buckets/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1329 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/admin/buckets/list/available.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      165 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/admin/buckets/list.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:29.000000 core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/admin/buckets/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      558 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/admin/buckets/modals/delete.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:31.000000 core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/admin/types/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:31.000000 core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/admin/types/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1966 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/admin/types/list/available.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1207 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/admin/types/list/disabled.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      228 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/admin/types/list.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       58 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/admin/types/upload.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:31.000000 core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/admin/types/versions/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1199 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/admin/types/versions/available.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       68 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/admin/types/versions/disabled.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      360 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/admin/types/versions.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:31.000000 core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/user/
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      889 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/user/build_template.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:31.000000 core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/user/builder/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      413 2023-02-23 20:26:05.000000 core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/user/builder/list_types.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:31.000000 core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/user/builder/menus/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      276 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/user/builder/menus/element.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      126 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/user/builder/menus/element_root.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      198 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/user/builder/menus/sequence.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:32.000000 core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/user/builder/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      654 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/user/builder/modals/change_type.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      532 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/user/builder/modals/delete_element.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      712 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/user/builder/modals/element_name.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      418 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/user/builder/modals/errors.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1098 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/user/builder/modals/insert_element.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1079 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/user/builder/modals/occurrences.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      676 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/user/builder/modals/root_type_name.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      451 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/user/builder/modals/save_success.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      616 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/user/builder/modals/save_template.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      592 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/user/builder/modals/save_type.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      384 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/user/builder/new_element.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1930 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/user/index.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:32.000000 core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/user/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      275 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/user/list/list.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:32.000000 core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/user/types/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:32.000000 core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/user/types/versions/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      325 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/user/types/versions/available.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      262 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/user/types/versions.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2529 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/core_composer_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:32.000000 core_composer_app-2.2.0/core_composer_app/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/core_composer_app/utils/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    16675 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/core_composer_app/utils/xml.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:32.000000 core_composer_app-2.2.0/core_composer_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/core_composer_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:32.000000 core_composer_app-2.2.0/core_composer_app/views/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/core_composer_app/views/admin/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3892 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/core_composer_app/views/admin/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2157 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/core_composer_app/views/admin/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17258 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/core_composer_app/views/admin/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:33.000000 core_composer_app-2.2.0/core_composer_app/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/core_composer_app/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    16759 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/core_composer_app/views/user/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9482 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/core_composer_app/views/user/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:24.000000 core_composer_app-2.2.0/core_composer_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1038 2023-02-23 20:26:08.000000 core_composer_app-2.2.0/core_composer_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6754 2023-02-23 20:26:08.000000 core_composer_app-2.2.0/core_composer_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-02-23 20:26:08.000000 core_composer_app-2.2.0/core_composer_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       85 2023-02-23 20:26:08.000000 core_composer_app-2.2.0/core_composer_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       29 2023-02-23 20:26:08.000000 core_composer_app-2.2.0/core_composer_app.egg-info/top_level.txt
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:33.000000 core_composer_app-2.2.0/docs/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/docs/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11283 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/docs/conf.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      289 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/docs/conf_urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       39 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-02-23 20:26:33.000000 core_composer_app-2.2.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1408 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:33.000000 core_composer_app-2.2.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:33.000000 core_composer_app-2.2.0/tests/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/tests/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:33.000000 core_composer_app-2.2.0/tests/components/bucket/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/tests/components/bucket/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:33.000000 core_composer_app-2.2.0/tests/components/bucket/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/tests/components/bucket/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1047 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/tests/components/bucket/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7227 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/tests/components/bucket/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:33.000000 core_composer_app-2.2.0/tests/components/type/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/tests/components/type/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5598 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/tests/components/type/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:33.000000 core_composer_app-2.2.0/tests/components/type_version_manager/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/tests/components/type_version_manager/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:33.000000 core_composer_app-2.2.0/tests/components/type_version_manager/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/tests/components/type_version_manager/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4412 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/tests/components/type_version_manager/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    20928 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/tests/components/type_version_manager/tests_int_access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    16645 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/tests/components/type_version_manager/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:33.000000 core_composer_app-2.2.0/tests/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/tests/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:33.000000 core_composer_app-2.2.0/tests/rest/bucket/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/tests/rest/bucket/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    13720 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/tests/rest/bucket/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10519 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/tests/rest/bucket/tests_permission.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:33.000000 core_composer_app-2.2.0/tests/rest/type_version_manager/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/tests/rest/type_version_manager/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14895 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/tests/rest/type_version_manager/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9582 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/tests/rest/type_version_manager/tests_permission.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1552 2023-02-23 20:26:06.000000 core_composer_app-2.2.0/tests/test_settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:33.000000 core_composer_app-2.2.0/tests/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:07.000000 core_composer_app-2.2.0/tests/utils/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8032 2023-02-23 20:26:07.000000 core_composer_app-2.2.0/tests/utils/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:34:00.184523 core_composer_app-2.3.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      142 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1038 2023-05-02 19:34:00.179244 core_composer_app-2.3.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      548 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:58.274312 core_composer_app-2.3.0/core_composer_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      105 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3401 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/admin.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      494 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/apps.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:58.350881 core_composer_app-2.3.0/core_composer_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:58.414705 core_composer_app-2.3.0/core_composer_app/components/bucket/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/components/bucket/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2542 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/components/bucket/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2390 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/components/bucket/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:58.479158 core_composer_app-2.3.0/core_composer_app/components/type/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/components/type/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      346 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/components/type/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1460 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/components/type/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1040 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/components/type/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:58.541989 core_composer_app-2.3.0/core_composer_app/components/type_version_manager/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/components/type_version_manager/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      355 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/components/type_version_manager/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3924 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/components/type_version_manager/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2375 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/components/type_version_manager/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      630 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/menus.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:58.566271 core_composer_app-2.3.0/core_composer_app/migrations/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3384 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/migrations/0001_initial.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/migrations/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      777 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:58.607754 core_composer_app-2.3.0/core_composer_app/permissions/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/permissions/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1295 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/permissions/discover.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      191 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/permissions/rights.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:58.634706 core_composer_app-2.3.0/core_composer_app/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:58.669733 core_composer_app-2.3.0/core_composer_app/rest/bucket/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/rest/bucket/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1680 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/rest/bucket/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10151 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/rest/bucket/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:58.763719 core_composer_app-2.3.0/core_composer_app/rest/type_version_manager/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/rest/type_version_manager/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5479 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/rest/type_version_manager/abstract_views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2390 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/rest/type_version_manager/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3366 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/rest/type_version_manager/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3225 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/rest/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      121 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:51.141612 core_composer_app-2.3.0/core_composer_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:52.104184 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:51.146292 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:58.794430 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/admin/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      753 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/admin/js/bucket.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       80 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/admin/js/bucket.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:51.188857 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/admin/js/types/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:58.835860 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/admin/js/types/upload/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      983 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/admin/js/types/upload/dependencies.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       98 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/admin/js/types/upload/dependencies.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      143 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/admin/js/types/upload/dependency_resolver.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:52.099061 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/common/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:58.850302 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/common/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      122 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/common/css/bucket.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:52.120441 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:58.926123 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/user/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      532 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/user/css/menu.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       56 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/user/css/style.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       64 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/user/css/xsd_tree.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:58.988019 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/user/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3831 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/user/js/build_template.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      713 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/user/js/build_template.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10778 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/user/js/menus.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1043 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/user/js/xpath.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      444 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/user/js/xsd_tree.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:59.003004 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/user/xsd/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      202 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/user/xsd/new_base_template.xsd
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:59.018035 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/user/xsl/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4750 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/user/xsl/xsd2html.xsl
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:52.139505 core_composer_app-2.3.0/core_composer_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:58.016618 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:58.005528 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:59.090384 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/admin/buckets/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      168 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/admin/buckets/add.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      922 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/admin/buckets/add_content.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      348 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/admin/buckets/edit.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1204 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/admin/buckets/edit_content.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:59.105105 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/admin/buckets/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1329 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/admin/buckets/list/available.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      165 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/admin/buckets/list.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:59.119251 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/admin/buckets/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      558 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/admin/buckets/modals/delete.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:59.157319 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/admin/types/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:59.186425 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/admin/types/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1966 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/admin/types/list/available.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1207 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/admin/types/list/disabled.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      228 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/admin/types/list.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       58 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/admin/types/upload.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:59.234729 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/admin/types/versions/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1199 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/admin/types/versions/available.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       68 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/admin/types/versions/disabled.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      360 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/admin/types/versions.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:59.261819 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      889 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/build_template.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:59.293306 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/builder/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      413 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/builder/list_types.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:59.328431 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/builder/menus/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      276 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/builder/menus/element.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      126 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/builder/menus/element_root.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      198 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/builder/menus/sequence.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:59.491938 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/builder/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      654 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/builder/modals/change_type.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      532 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/builder/modals/delete_element.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      712 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/builder/modals/element_name.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      418 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/builder/modals/errors.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1098 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/builder/modals/insert_element.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1079 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/builder/modals/occurrences.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      676 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/builder/modals/root_type_name.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      451 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/builder/modals/save_success.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      616 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/builder/modals/save_template.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      592 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/builder/modals/save_type.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      384 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/builder/new_element.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1930 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/index.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:59.505957 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      275 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/list/list.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:59.520155 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/types/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:59.534711 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/types/versions/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      325 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/types/versions/available.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      262 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/types/versions.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2529 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:59.571353 core_composer_app-2.3.0/core_composer_app/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/utils/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    16675 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/utils/xml.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:59.585308 core_composer_app-2.3.0/core_composer_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:59.655331 core_composer_app-2.3.0/core_composer_app/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/views/admin/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3892 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/views/admin/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2157 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/views/admin/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17258 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/views/admin/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:59.717179 core_composer_app-2.3.0/core_composer_app/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    16759 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/views/user/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9293 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/views/user/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:58.336760 core_composer_app-2.3.0/core_composer_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1038 2023-05-02 19:33:47.000000 core_composer_app-2.3.0/core_composer_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6765 2023-05-02 19:33:47.000000 core_composer_app-2.3.0/core_composer_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:33:47.000000 core_composer_app-2.3.0/core_composer_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       85 2023-05-02 19:33:47.000000 core_composer_app-2.3.0/core_composer_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       29 2023-05-02 19:33:47.000000 core_composer_app-2.3.0/core_composer_app.egg-info/top_level.txt
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:59.766397 core_composer_app-2.3.0/docs/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/docs/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11283 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/docs/conf.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      289 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/docs/conf_urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:33:37.000000 core_composer_app-2.3.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       39 2023-05-02 19:33:37.000000 core_composer_app-2.3.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:34:00.186149 core_composer_app-2.3.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1408 2023-05-02 19:33:37.000000 core_composer_app-2.3.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:59.798836 core_composer_app-2.3.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:37.000000 core_composer_app-2.3.0/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:59.814869 core_composer_app-2.3.0/tests/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:37.000000 core_composer_app-2.3.0/tests/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:59.849532 core_composer_app-2.3.0/tests/components/bucket/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:37.000000 core_composer_app-2.3.0/tests/components/bucket/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:59.896220 core_composer_app-2.3.0/tests/components/bucket/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:37.000000 core_composer_app-2.3.0/tests/components/bucket/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1047 2023-05-02 19:33:37.000000 core_composer_app-2.3.0/tests/components/bucket/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7227 2023-05-02 19:33:37.000000 core_composer_app-2.3.0/tests/components/bucket/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:59.933396 core_composer_app-2.3.0/tests/components/type/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:37.000000 core_composer_app-2.3.0/tests/components/type/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5598 2023-05-02 19:33:37.000000 core_composer_app-2.3.0/tests/components/type/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:59.979785 core_composer_app-2.3.0/tests/components/type_version_manager/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:37.000000 core_composer_app-2.3.0/tests/components/type_version_manager/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:34:00.015325 core_composer_app-2.3.0/tests/components/type_version_manager/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:37.000000 core_composer_app-2.3.0/tests/components/type_version_manager/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4412 2023-05-02 19:33:37.000000 core_composer_app-2.3.0/tests/components/type_version_manager/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    20898 2023-05-02 19:33:37.000000 core_composer_app-2.3.0/tests/components/type_version_manager/tests_int_access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    16645 2023-05-02 19:33:37.000000 core_composer_app-2.3.0/tests/components/type_version_manager/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:34:00.031960 core_composer_app-2.3.0/tests/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:37.000000 core_composer_app-2.3.0/tests/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:34:00.081947 core_composer_app-2.3.0/tests/rest/bucket/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:37.000000 core_composer_app-2.3.0/tests/rest/bucket/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    13700 2023-05-02 19:33:37.000000 core_composer_app-2.3.0/tests/rest/bucket/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10519 2023-05-02 19:33:37.000000 core_composer_app-2.3.0/tests/rest/bucket/tests_permission.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:34:00.134670 core_composer_app-2.3.0/tests/rest/type_version_manager/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:37.000000 core_composer_app-2.3.0/tests/rest/type_version_manager/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14870 2023-05-02 19:33:37.000000 core_composer_app-2.3.0/tests/rest/type_version_manager/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9582 2023-05-02 19:33:37.000000 core_composer_app-2.3.0/tests/rest/type_version_manager/tests_permission.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1582 2023-05-02 19:33:37.000000 core_composer_app-2.3.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:34:00.164514 core_composer_app-2.3.0/tests/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:37.000000 core_composer_app-2.3.0/tests/utils/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8032 2023-05-02 19:33:37.000000 core_composer_app-2.3.0/tests/utils/tests_unit.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `core_composer_app-2.2.0/PKG-INFO` & `core_composer_app-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_composer_app
-Version: 2.2.0
+Version: 2.3.0
 Summary: Template and type composer for the curator core project
 Home-page: https://github.com/usnistgov/core_composer_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =================
         Core Composer App
```

### Comparing `core_composer_app-2.2.0/README.rst` & `core_composer_app-2.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/core_composer_app/admin.py` & `core_composer_app-2.3.0/core_composer_app/admin.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/core_composer_app/components/bucket/api.py` & `core_composer_app-2.3.0/core_composer_app/components/bucket/api.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/core_composer_app/components/bucket/models.py` & `core_composer_app-2.3.0/core_composer_app/components/bucket/models.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/core_composer_app/components/type/api.py` & `core_composer_app-2.3.0/core_composer_app/components/type/api.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/core_composer_app/components/type/models.py` & `core_composer_app-2.3.0/core_composer_app/components/type/models.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/core_composer_app/components/type_version_manager/api.py` & `core_composer_app-2.3.0/core_composer_app/components/type_version_manager/api.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/core_composer_app/components/type_version_manager/models.py` & `core_composer_app-2.3.0/core_composer_app/components/type_version_manager/models.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/core_composer_app/menus.py` & `core_composer_app-2.3.0/core_composer_app/menus.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/core_composer_app/migrations/0001_initial.py` & `core_composer_app-2.3.0/core_composer_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/core_composer_app/models.py` & `core_composer_app-2.3.0/core_composer_app/models.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/core_composer_app/permissions/discover.py` & `core_composer_app-2.3.0/core_composer_app/permissions/discover.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/core_composer_app/rest/bucket/serializers.py` & `core_composer_app-2.3.0/core_composer_app/rest/bucket/serializers.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/core_composer_app/rest/bucket/views.py` & `core_composer_app-2.3.0/core_composer_app/rest/bucket/views.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/core_composer_app/rest/type_version_manager/abstract_views.py` & `core_composer_app-2.3.0/core_composer_app/rest/type_version_manager/abstract_views.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/core_composer_app/rest/type_version_manager/serializers.py` & `core_composer_app-2.3.0/core_composer_app/rest/type_version_manager/serializers.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/core_composer_app/rest/type_version_manager/views.py` & `core_composer_app-2.3.0/core_composer_app/rest/type_version_manager/views.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/core_composer_app/rest/urls.py` & `core_composer_app-2.3.0/core_composer_app/rest/urls.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/core_composer_app/static/core_composer_app/admin/js/bucket.js` & `core_composer_app-2.3.0/core_composer_app/static/core_composer_app/admin/js/bucket.js`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/core_composer_app/static/core_composer_app/admin/js/types/upload/dependencies.js` & `core_composer_app-2.3.0/core_composer_app/static/core_composer_app/admin/js/types/upload/dependencies.js`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/core_composer_app/static/core_composer_app/user/css/menu.css` & `core_composer_app-2.3.0/core_composer_app/static/core_composer_app/user/css/menu.css`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/core_composer_app/static/core_composer_app/user/js/build_template.js` & `core_composer_app-2.3.0/core_composer_app/static/core_composer_app/user/js/build_template.js`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/core_composer_app/static/core_composer_app/user/js/build_template.raw.js` & `core_composer_app-2.3.0/core_composer_app/static/core_composer_app/user/js/build_template.raw.js`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/core_composer_app/static/core_composer_app/user/js/menus.js` & `core_composer_app-2.3.0/core_composer_app/static/core_composer_app/user/js/menus.js`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/core_composer_app/static/core_composer_app/user/js/xpath.js` & `core_composer_app-2.3.0/core_composer_app/static/core_composer_app/user/js/xpath.js`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/core_composer_app/static/core_composer_app/user/xsl/xsd2html.xsl` & `core_composer_app-2.3.0/core_composer_app/static/core_composer_app/user/xsl/xsd2html.xsl`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/admin/buckets/add_content.html` & `core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/admin/buckets/add_content.html`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/admin/buckets/edit_content.html` & `core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/admin/buckets/edit_content.html`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/admin/buckets/list/available.html` & `core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/admin/buckets/list/available.html`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/admin/buckets/modals/delete.html` & `core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/admin/buckets/modals/delete.html`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/admin/types/list/available.html` & `core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/admin/types/list/available.html`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/admin/types/list/disabled.html` & `core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/admin/types/list/disabled.html`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/admin/types/versions/available.html` & `core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/admin/types/versions/available.html`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/user/build_template.html` & `core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/build_template.html`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/user/builder/modals/change_type.html` & `core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/builder/modals/change_type.html`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/user/builder/modals/delete_element.html` & `core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/builder/modals/delete_element.html`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/user/builder/modals/element_name.html` & `core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/builder/modals/element_name.html`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/user/builder/modals/insert_element.html` & `core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/builder/modals/insert_element.html`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/user/builder/modals/occurrences.html` & `core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/builder/modals/occurrences.html`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/user/builder/modals/root_type_name.html` & `core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/builder/modals/root_type_name.html`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/user/builder/modals/save_template.html` & `core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/builder/modals/save_template.html`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/user/builder/modals/save_type.html` & `core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/builder/modals/save_type.html`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/core_composer_app/templates/core_composer_app/user/index.html` & `core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/index.html`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/core_composer_app/urls.py` & `core_composer_app-2.3.0/core_composer_app/urls.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/core_composer_app/utils/xml.py` & `core_composer_app-2.3.0/core_composer_app/utils/xml.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/core_composer_app/views/admin/ajax.py` & `core_composer_app-2.3.0/core_composer_app/views/admin/ajax.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/core_composer_app/views/admin/forms.py` & `core_composer_app-2.3.0/core_composer_app/views/admin/forms.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/core_composer_app/views/admin/views.py` & `core_composer_app-2.3.0/core_composer_app/views/admin/views.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/core_composer_app/views/user/ajax.py` & `core_composer_app-2.3.0/core_composer_app/views/user/ajax.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/core_composer_app/views/user/views.py` & `core_composer_app-2.3.0/core_composer_app/views/user/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 """Composer app user views
 """
 from os.path import join
 
 from django.conf import settings
 from django.contrib.auth.decorators import login_required
 from django.contrib.staticfiles import finders
-from django.urls import reverse_lazy
 
+from core_composer_app.components.bucket import api as bucket_api
+from core_composer_app.components.type_version_manager import (
+    api as type_version_manager_api,
+)
+from core_composer_app.permissions import rights
 from core_main_app.components.template import api as template_api
 from core_main_app.components.template_version_manager import (
     api as template_version_manager_api,
 )
 from core_main_app.utils import decorators as decorators
 from core_main_app.utils.file import read_file_content, get_file_http_response
 from core_main_app.utils.rendering import render
 from core_main_app.utils.xml import xsl_transform
 from core_main_app.views.user.views import get_context_manage_template_versions
 from xml_utils.commons.constants import LXML_SCHEMA_NAMESPACE
 from xml_utils.xsd_tree.operations.annotation import remove_annotations
 from xml_utils.xsd_tree.xsd_tree import XSDTree
 from xml_utils.xsd_types.xsd_types import get_xsd_types
-from core_composer_app.components.bucket import api as bucket_api
-from core_composer_app.components.type_version_manager import (
-    api as type_version_manager_api,
-)
-from core_composer_app.permissions import rights
+
 
 # TODO: see if sessions are problematic
 
 
 @decorators.permission_required(
     content_type=rights.COMPOSER_CONTENT_TYPE,
     permission=rights.COMPOSER_ACCESS,
-    login_url=reverse_lazy("core_main_app_login"),
 )
 def index(request):
     """Page that allows to select a template to start composing.
 
     Args:
         request:
 
@@ -84,15 +83,14 @@
         context=context,
     )
 
 
 @decorators.permission_required(
     content_type=rights.COMPOSER_CONTENT_TYPE,
     permission=rights.COMPOSER_ACCESS,
-    login_url=reverse_lazy("core_main_app_login"),
 )
 def build_template(request, template_id):
     """View that allows to build the Template.
 
     Args:
         request:
         template_id:
@@ -217,15 +215,14 @@
         modals=modals,
     )
 
 
 @decorators.permission_required(
     content_type=rights.COMPOSER_CONTENT_TYPE,
     permission=rights.COMPOSER_ACCESS,
-    login_url=reverse_lazy("core_main_app_login"),
 )
 def download_xsd(request):
     """Make the current XSD available for download.
 
     Args:
         request:
```

### Comparing `core_composer_app-2.2.0/core_composer_app.egg-info/PKG-INFO` & `core_composer_app-2.3.0/core_composer_app.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-composer-app
-Version: 2.2.0
+Version: 2.3.0
 Summary: Template and type composer for the curator core project
 Home-page: https://github.com/usnistgov/core_composer_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =================
         Core Composer App
```

### Comparing `core_composer_app-2.2.0/core_composer_app.egg-info/SOURCES.txt` & `core_composer_app-2.3.0/core_composer_app.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.md
 MANIFEST.in
 README.rst
 pyproject.toml
 requirements.core.txt
 setup.py
 core_composer_app/__init__.py
 core_composer_app/admin.py
```

### Comparing `core_composer_app-2.2.0/docs/conf.py` & `core_composer_app-2.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/setup.py` & `core_composer_app-2.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_composer_app",
-    version="2.2.0",
+    version="2.3.0",
     description="Template and type composer for the curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_composer_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_composer_app-2.2.0/tests/components/bucket/fixtures/fixtures.py` & `core_composer_app-2.3.0/tests/components/bucket/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/tests/components/bucket/tests_unit.py` & `core_composer_app-2.3.0/tests/components/bucket/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/tests/components/type/tests_unit.py` & `core_composer_app-2.3.0/tests/components/type/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/tests/components/type_version_manager/fixtures/fixtures.py` & `core_composer_app-2.3.0/tests/components/type_version_manager/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/tests/components/type_version_manager/tests_int_access_control.py` & `core_composer_app-2.3.0/tests/components/type_version_manager/tests_int_access_control.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from django.test import override_settings
 
 from core_main_app.access_control.exceptions import AccessControlError
 from core_composer_app.components.type_version_manager import (
     api as type_vm_api,
 )
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 from core_composer_app.components.type_version_manager.models import (
     TypeVersionManager,
 )
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from core_main_app.utils.tests_tools.RequestMock import create_mock_request
 
@@ -21,15 +21,15 @@
     TypeVersionManagerAccessControlFixtures,
 )
 
 fixture_type_vm = TypeVersionManagerFixtures()
 fixture_type_vm2 = TypeVersionManagerAccessControlFixtures()
 
 
-class TestTypeVersionManagerGet(MongoIntegrationBaseTestCase):
+class TestTypeVersionManagerGet(IntegrationBaseTestCase):
     """TestTypeVersionManagerGet"""
 
     fixture = fixture_type_vm
 
     def setUp(self):
         """setUp
 
@@ -163,15 +163,15 @@
         with self.assertRaises(AccessControlError):
             type_vm_api.get_by_id(
                 self.fixture.type_vm_2.id, request=mock_request
             )
 
 
 class TestTypeVersionManagerGetActiveGlobalVersionManager(
-    MongoIntegrationBaseTestCase
+    IntegrationBaseTestCase
 ):
     """TestTypeVersionManagerGetActiveGlobalVersionManager"""
 
     fixture = fixture_type_vm
 
     def setUp(self):
         """setUp
@@ -251,15 +251,15 @@
         mock_request = create_mock_request(user=self.staff_user1)
         version_manager = type_vm_api.get_active_global_version_manager(
             request=mock_request
         )
         self.assertTrue(self.fixture.type_vm_1 in version_manager)
 
 
-class TestTypeVersionManagerInsert(MongoIntegrationBaseTestCase):
+class TestTypeVersionManagerInsert(IntegrationBaseTestCase):
     """TestTypeVersionManagerInsert"""
 
     fixture = fixture_type_vm2
 
     def setUp(self):
         """setUp
 
@@ -470,15 +470,15 @@
             self.fixture.global_type,
             request=mock_request,
         )
 
         self.assertIsInstance(result, TypeVersionManager)
 
 
-class TestTypeVersionManagerGetNoBucketsTypes(MongoIntegrationBaseTestCase):
+class TestTypeVersionManagerGetNoBucketsTypes(IntegrationBaseTestCase):
     """Test Type Version Manager Get No Buckets Types"""
 
     fixture = fixture_type_vm2
 
     def setUp(self):
         """setUp
 
@@ -558,15 +558,15 @@
         mock_request = create_mock_request(user=self.staff_user1)
 
         result = type_vm_api.get_no_buckets_types(request=mock_request)
 
         self.assertEqual(len(result), 1)
 
 
-class TestTypeVersionManagerGetAllVersionManager(MongoIntegrationBaseTestCase):
+class TestTypeVersionManagerGetAllVersionManager(IntegrationBaseTestCase):
     """Test Type Version Manager Get All Version Manager"""
 
     fixture = fixture_type_vm2
 
     def setUp(self):
         """setUp
```

### Comparing `core_composer_app-2.2.0/tests/components/type_version_manager/tests_unit.py` & `core_composer_app-2.3.0/tests/components/type_version_manager/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/tests/rest/bucket/tests_int.py` & `core_composer_app-2.3.0/tests/rest/bucket/tests_int.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """ Integration Test for Bucket Rest API
 """
 
 from rest_framework import status
 
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from core_main_app.utils.tests_tools.RequestMock import RequestMock
 from core_composer_app.rest.bucket import views
 from tests.components.bucket.fixtures.fixtures import BucketFixtures
 
 fixture_bucket = BucketFixtures()
 
 
-class TestBucketList(MongoIntegrationBaseTestCase):
+class TestBucketList(IntegrationBaseTestCase):
     """Test Bucket List"""
 
     fixture = fixture_bucket
 
     def setUp(self):
         """setUp"""
 
@@ -222,15 +222,15 @@
             views.BucketList.as_view(), user, data=self.data
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_400_BAD_REQUEST)
 
 
-class TestBucketDetail(MongoIntegrationBaseTestCase):
+class TestBucketDetail(IntegrationBaseTestCase):
     """Test Bucket Detail"""
 
     fixture = fixture_bucket
 
     def setUp(self):
         """setUp"""
 
@@ -358,15 +358,15 @@
             views.BucketDetail.as_view(), user, param={"pk": -1}
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_404_NOT_FOUND)
 
 
-class TestTypeVersionManagerBuckets(MongoIntegrationBaseTestCase):
+class TestTypeVersionManagerBuckets(IntegrationBaseTestCase):
     """Test Type Version Manager Buckets"""
 
     fixture = fixture_bucket
 
     def setUp(self):
         """setUp"""
```

### Comparing `core_composer_app-2.2.0/tests/rest/bucket/tests_permission.py` & `core_composer_app-2.3.0/tests/rest/bucket/tests_permission.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/tests/rest/type_version_manager/tests_int.py` & `core_composer_app-2.3.0/tests/rest/type_version_manager/tests_int.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import json
 
 from django.test import override_settings
 from django.urls import reverse
 from rest_framework import status
 
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from core_main_app.utils.tests_tools.RequestMock import (
     RequestMock,
     create_mock_request,
 )
 from core_composer_app.components.type import api as type_api
@@ -20,15 +20,15 @@
 from tests.components.type_version_manager.fixtures.fixtures import (
     TypeVersionManagerFixtures,
 )
 
 fixture_type = TypeVersionManagerFixtures()
 
 
-class TestGlobalTypeVersionManagerList(MongoIntegrationBaseTestCase):
+class TestGlobalTypeVersionManagerList(IntegrationBaseTestCase):
     """Test"""
 
     fixture = fixture_type
 
     def setUp(self):
         """setUp"""
 
@@ -137,15 +137,15 @@
             data={"is_disabled": not self.fixture.type_vm_1.is_disabled},
         )
 
         # Assert
         self.assertEqual(len(response.data), 0)
 
 
-class TestUserTypeVersionManagerList(MongoIntegrationBaseTestCase):
+class TestUserTypeVersionManagerList(IntegrationBaseTestCase):
     """Test User Type Version Manager List"""
 
     fixture = fixture_type
 
     def setUp(self):
         """setUp"""
 
@@ -254,15 +254,15 @@
             data={"is_disabled": not self.fixture.type_vm_2.is_disabled},
         )
 
         # Assert
         self.assertEqual(len(response.data), 0)
 
 
-class TestUserTypeList(MongoIntegrationBaseTestCase):
+class TestUserTypeList(IntegrationBaseTestCase):
     """Test User Type List"""
 
     fixture = fixture_type
 
     def setUp(self):
         """setUp"""
 
@@ -408,15 +408,15 @@
             views.UserTypeList.as_view(), user, data=self.data
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_400_BAD_REQUEST)
 
 
-class TestGlobalTypeList(MongoIntegrationBaseTestCase):
+class TestGlobalTypeList(IntegrationBaseTestCase):
     """Test Global Type List"""
 
     fixture = fixture_type
 
     def setUp(self):
         """setUp"""
```

### Comparing `core_composer_app-2.2.0/tests/rest/type_version_manager/tests_permission.py` & `core_composer_app-2.3.0/tests/rest/type_version_manager/tests_permission.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.2.0/tests/test_settings.py` & `core_composer_app-2.3.0/tests/test_settings.py`

 * *Files 18% similar despite different names*

```diff
@@ -55,7 +55,8 @@
 DEFAULT_AUTO_FIELD = "django.db.models.BigAutoField"
 CELERYBEAT_SCHEDULER = "django_celery_beat.schedulers:DatabaseScheduler"
 
 CAN_ANONYMOUS_ACCESS_PUBLIC_DOCUMENT = False
 
 MONGODB_INDEXING = False
 MONGODB_ASYNC_SAVE = False
+ENABLE_SAML2_SSO_AUTH = False
```

### Comparing `core_composer_app-2.2.0/tests/utils/tests_unit.py` & `core_composer_app-2.3.0/tests/utils/tests_unit.py`

 * *Files identical despite different names*

