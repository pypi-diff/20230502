# Comparing `tmp/core_user_registration_app-2.2.0.tar.gz` & `tmp/core_user_registration_app-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/core_user_registration_app-2.2.0.tar", last modified: Thu Feb 23 20:34:33 2023, max compression
+gzip compressed data, was "core_user_registration_app-2.3.0.tar", last modified: Tue May  2 19:48:15 2023, max compression
```

## Comparing `core_user_registration_app-2.2.0.tar` & `core_user_registration_app-2.3.0.tar`

### file list

```diff
@@ -1,144 +1,145 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:33.000000 core_user_registration_app-2.2.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      185 2023-02-23 20:34:28.000000 core_user_registration_app-2.2.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1068 2023-02-23 20:34:33.000000 core_user_registration_app-2.2.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      586 2023-02-23 20:34:28.000000 core_user_registration_app-2.2.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:32.000000 core_user_registration_app-2.2.0/core_user_registration_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       89 2023-02-23 20:34:28.000000 core_user_registration_app-2.2.0/core_user_registration_app/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:32.000000 core_user_registration_app-2.2.0/core_user_registration_app/access_control/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:28.000000 core_user_registration_app-2.2.0/core_user_registration_app/access_control/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3113 2023-02-23 20:34:28.000000 core_user_registration_app-2.2.0/core_user_registration_app/access_control/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2683 2023-02-23 20:34:28.000000 core_user_registration_app-2.2.0/core_user_registration_app/admin.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      521 2023-02-23 20:34:28.000000 core_user_registration_app-2.2.0/core_user_registration_app/apps.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:32.000000 core_user_registration_app-2.2.0/core_user_registration_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:28.000000 core_user_registration_app-2.2.0/core_user_registration_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:32.000000 core_user_registration_app-2.2.0/core_user_registration_app/components/account_request_metadata/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:28.000000 core_user_registration_app-2.2.0/core_user_registration_app/components/account_request_metadata/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2833 2023-02-23 20:34:28.000000 core_user_registration_app-2.2.0/core_user_registration_app/components/account_request_metadata/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      721 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/core_user_registration_app/components/account_request_metadata/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:32.000000 core_user_registration_app-2.2.0/core_user_registration_app/components/user_data_structure/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/core_user_registration_app/components/user_data_structure/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2624 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/core_user_registration_app/components/user_data_structure/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5373 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/core_user_registration_app/components/user_data_structure/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:32.000000 core_user_registration_app-2.2.0/core_user_registration_app/components/user_metadata/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/core_user_registration_app/components/user_metadata/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1566 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/core_user_registration_app/components/user_metadata/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2025 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/core_user_registration_app/components/user_metadata/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:32.000000 core_user_registration_app-2.2.0/core_user_registration_app/components/user_template_version_manager/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/core_user_registration_app/components/user_template_version_manager/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1299 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/core_user_registration_app/components/user_template_version_manager/access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3131 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/core_user_registration_app/components/user_template_version_manager/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2628 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/core_user_registration_app/components/user_template_version_manager/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6592 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/core_user_registration_app/discover.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      514 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/core_user_registration_app/menus.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:32.000000 core_user_registration_app-2.2.0/core_user_registration_app/migrations/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7426 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/core_user_registration_app/migrations/0001_initial.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/core_user_registration_app/migrations/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      642 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/core_user_registration_app/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:32.000000 core_user_registration_app-2.2.0/core_user_registration_app/permissions/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/core_user_registration_app/permissions/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      190 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/core_user_registration_app/permissions/rights.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1596 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/core_user_registration_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:31.000000 core_user_registration_app-2.2.0/core_user_registration_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:31.000000 core_user_registration_app-2.2.0/core_user_registration_app/static/core_user_registration_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:31.000000 core_user_registration_app-2.2.0/core_user_registration_app/static/core_user_registration_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:32.000000 core_user_registration_app-2.2.0/core_user_registration_app/static/core_user_registration_app/admin/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      211 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/core_user_registration_app/static/core_user_registration_app/admin/js/view_meta.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       83 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/core_user_registration_app/static/core_user_registration_app/admin/js/view_meta.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:31.000000 core_user_registration_app-2.2.0/core_user_registration_app/static/core_user_registration_app/common/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:31.000000 core_user_registration_app-2.2.0/core_user_registration_app/static/core_user_registration_app/common/js/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:32.000000 core_user_registration_app-2.2.0/core_user_registration_app/static/core_user_registration_app/common/js/templates/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      650 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/core_user_registration_app/static/core_user_registration_app/common/js/templates/set_current.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      107 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/core_user_registration_app/static/core_user_registration_app/common/js/templates/set_current.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:32.000000 core_user_registration_app-2.2.0/core_user_registration_app/static/core_user_registration_app/common/js/templates/versions/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      652 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/core_user_registration_app/static/core_user_registration_app/common/js/templates/versions/set_current.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      125 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/core_user_registration_app/static/core_user_registration_app/common/js/templates/versions/set_current.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:31.000000 core_user_registration_app-2.2.0/core_user_registration_app/static/core_user_registration_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:33.000000 core_user_registration_app-2.2.0/core_user_registration_app/static/core_user_registration_app/user/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      934 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/core_user_registration_app/static/core_user_registration_app/user/js/autosave.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      100 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/core_user_registration_app/static/core_user_registration_app/user/js/autosave.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      756 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/core_user_registration_app/static/core_user_registration_app/user/js/report_data.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       89 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/core_user_registration_app/static/core_user_registration_app/user/js/report_data.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1049 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/core_user_registration_app/static/core_user_registration_app/user/js/save_data.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       68 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/core_user_registration_app/static/core_user_registration_app/user/js/save_data.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:33.000000 core_user_registration_app-2.2.0/core_user_registration_app/static/core_user_registration_app/user/xsd/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      559 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/core_user_registration_app/static/core_user_registration_app/user/xsd/user.xsd
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:33.000000 core_user_registration_app-2.2.0/core_user_registration_app/system/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/core_user_registration_app/system/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2012 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/core_user_registration_app/system/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1541 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/core_user_registration_app/tasks.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:31.000000 core_user_registration_app-2.2.0/core_user_registration_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:32.000000 core_user_registration_app-2.2.0/core_user_registration_app/templates/core_user_registration_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:33.000000 core_user_registration_app-2.2.0/core_user_registration_app/templates/core_user_registration_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:33.000000 core_user_registration_app-2.2.0/core_user_registration_app/templates/core_user_registration_app/admin/account_requests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1800 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/core_user_registration_app/templates/core_user_registration_app/admin/account_requests/pending.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:33.000000 core_user_registration_app-2.2.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:33.000000 core_user_registration_app-2.2.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1712 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/list/available.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      514 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/list.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:33.000000 core_user_registration_app-2.2.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/versions/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3152 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/versions/available.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      615 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/versions.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      338 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/core_user_registration_app/templates/core_user_registration_app/admin/user_requests.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:33.000000 core_user_registration_app-2.2.0/core_user_registration_app/templates/core_user_registration_app/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1003 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/core_user_registration_app/templates/core_user_registration_app/user/account_creation.html
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     1188 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/core_user_registration_app/templates/core_user_registration_app/user/request_new_account.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1623 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/core_user_registration_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:33.000000 core_user_registration_app-2.2.0/core_user_registration_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/core_user_registration_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:33.000000 core_user_registration_app-2.2.0/core_user_registration_app/views/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/core_user_registration_app/views/admin/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1592 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/core_user_registration_app/views/admin/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14677 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/core_user_registration_app/views/admin/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:33.000000 core_user_registration_app-2.2.0/core_user_registration_app/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/core_user_registration_app/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5566 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/core_user_registration_app/views/user/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7456 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/core_user_registration_app/views/user/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:32.000000 core_user_registration_app-2.2.0/core_user_registration_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1068 2023-02-23 20:34:31.000000 core_user_registration_app-2.2.0/core_user_registration_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5446 2023-02-23 20:34:31.000000 core_user_registration_app-2.2.0/core_user_registration_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-02-23 20:34:31.000000 core_user_registration_app-2.2.0/core_user_registration_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       36 2023-02-23 20:34:31.000000 core_user_registration_app-2.2.0/core_user_registration_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       33 2023-02-23 20:34:31.000000 core_user_registration_app-2.2.0/core_user_registration_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      170 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       91 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       36 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-02-23 20:34:33.000000 core_user_registration_app-2.2.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      939 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:33.000000 core_user_registration_app-2.2.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:33.000000 core_user_registration_app-2.2.0/tests/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/tests/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:33.000000 core_user_registration_app-2.2.0/tests/components/account_request_metadata/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/tests/components/account_request_metadata/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2900 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/tests/components/account_request_metadata/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:33.000000 core_user_registration_app-2.2.0/tests/components/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/tests/components/user/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:33.000000 core_user_registration_app-2.2.0/tests/components/user/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/tests/components/user/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1119 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/tests/components/user/fixtures/fixtures.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:33.000000 core_user_registration_app-2.2.0/tests/components/user_data_structure/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/tests/components/user_data_structure/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:33.000000 core_user_registration_app-2.2.0/tests/components/user_data_structure/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/tests/components/user_data_structure/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2343 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/tests/components/user_data_structure/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7960 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/tests/components/user_data_structure/test_int_access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3204 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/tests/components/user_data_structure/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:33.000000 core_user_registration_app-2.2.0/tests/components/user_metadata/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/tests/components/user_metadata/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:33.000000 core_user_registration_app-2.2.0/tests/components/user_metadata/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/tests/components/user_metadata/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4808 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/tests/components/user_metadata/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4664 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/tests/components/user_metadata/test_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1062 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/tests/components/user_metadata/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:33.000000 core_user_registration_app-2.2.0/tests/components/user_template_version_manager/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/tests/components/user_template_version_manager/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:33.000000 core_user_registration_app-2.2.0/tests/components/user_template_version_manager/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/tests/components/user_template_version_manager/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2472 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/tests/components/user_template_version_manager/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6638 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/tests/components/user_template_version_manager/test_int_access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2150 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/tests/test_settings.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2121 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/tests/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:33.000000 core_user_registration_app-2.2.0/tests/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/tests/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:33.000000 core_user_registration_app-2.2.0/tests/views/ajax/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:29.000000 core_user_registration_app-2.2.0/tests/views/ajax/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.904388 core_user_registration_app-2.3.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      185 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1068 2023-05-02 19:48:15.899420 core_user_registration_app-2.3.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      586 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:14.580563 core_user_registration_app-2.3.0/core_user_registration_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       89 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:14.682874 core_user_registration_app-2.3.0/core_user_registration_app/access_control/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/access_control/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3113 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/access_control/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2683 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/admin.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      521 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/apps.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:14.699214 core_user_registration_app-2.3.0/core_user_registration_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:14.748676 core_user_registration_app-2.3.0/core_user_registration_app/components/account_request_metadata/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/components/account_request_metadata/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2833 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/components/account_request_metadata/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      721 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/components/account_request_metadata/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:14.798073 core_user_registration_app-2.3.0/core_user_registration_app/components/user_data_structure/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/components/user_data_structure/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2624 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/components/user_data_structure/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5373 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/components/user_data_structure/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:14.851112 core_user_registration_app-2.3.0/core_user_registration_app/components/user_metadata/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/components/user_metadata/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1566 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/components/user_metadata/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2025 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/components/user_metadata/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:14.912566 core_user_registration_app-2.3.0/core_user_registration_app/components/user_template_version_manager/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/components/user_template_version_manager/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1299 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/components/user_template_version_manager/access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3131 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/components/user_template_version_manager/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2628 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/components/user_template_version_manager/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6592 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/discover.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      514 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/menus.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:14.942612 core_user_registration_app-2.3.0/core_user_registration_app/migrations/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7426 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/migrations/0001_initial.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/migrations/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      642 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:14.974551 core_user_registration_app-2.3.0/core_user_registration_app/permissions/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/permissions/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      190 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/permissions/rights.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1596 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:14.157791 core_user_registration_app-2.3.0/core_user_registration_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:14.200086 core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:14.164333 core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.002267 core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/admin/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      211 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/admin/js/view_meta.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       83 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/admin/js/view_meta.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:14.175344 core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/common/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:14.189019 core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/common/js/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.028253 core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/common/js/templates/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      650 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/common/js/templates/set_current.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      107 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/common/js/templates/set_current.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.053501 core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/common/js/templates/versions/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      652 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/common/js/templates/versions/set_current.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      125 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/common/js/templates/versions/set_current.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:14.208463 core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.147769 core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/user/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      934 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/user/js/autosave.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      100 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/user/js/autosave.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      756 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/user/js/report_data.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       89 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/user/js/report_data.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1049 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/user/js/save_data.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       68 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/user/js/save_data.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.164496 core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/user/xsd/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      559 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/user/xsd/user.xsd
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.192499 core_user_registration_app-2.3.0/core_user_registration_app/system/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/system/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2012 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/system/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1541 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/tasks.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:14.238794 core_user_registration_app-2.3.0/core_user_registration_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:14.266605 core_user_registration_app-2.3.0/core_user_registration_app/templates/core_user_registration_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.210960 core_user_registration_app-2.3.0/core_user_registration_app/templates/core_user_registration_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.225502 core_user_registration_app-2.3.0/core_user_registration_app/templates/core_user_registration_app/admin/account_requests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1849 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/templates/core_user_registration_app/admin/account_requests/pending.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.256444 core_user_registration_app-2.3.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.272293 core_user_registration_app-2.3.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1712 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/list/available.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      514 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/list.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.292578 core_user_registration_app-2.3.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/versions/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3152 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/versions/available.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      615 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/versions.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      338 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/templates/core_user_registration_app/admin/user_requests.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.320739 core_user_registration_app-2.3.0/core_user_registration_app/templates/core_user_registration_app/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1003 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/core_user_registration_app/templates/core_user_registration_app/user/account_creation.html
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     1188 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/core_user_registration_app/templates/core_user_registration_app/user/request_new_account.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1623 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/core_user_registration_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.335296 core_user_registration_app-2.3.0/core_user_registration_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/core_user_registration_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.381651 core_user_registration_app-2.3.0/core_user_registration_app/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/core_user_registration_app/views/admin/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1592 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/core_user_registration_app/views/admin/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14677 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/core_user_registration_app/views/admin/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.422731 core_user_registration_app-2.3.0/core_user_registration_app/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/core_user_registration_app/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5566 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/core_user_registration_app/views/user/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7456 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/core_user_registration_app/views/user/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:14.654182 core_user_registration_app-2.3.0/core_user_registration_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1068 2023-05-02 19:48:13.000000 core_user_registration_app-2.3.0/core_user_registration_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5457 2023-05-02 19:48:14.000000 core_user_registration_app-2.3.0/core_user_registration_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:48:13.000000 core_user_registration_app-2.3.0/core_user_registration_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       36 2023-05-02 19:48:13.000000 core_user_registration_app-2.3.0/core_user_registration_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       33 2023-05-02 19:48:13.000000 core_user_registration_app-2.3.0/core_user_registration_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      170 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       91 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       36 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:48:15.906557 core_user_registration_app-2.3.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      939 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.464506 core_user_registration_app-2.3.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.479256 core_user_registration_app-2.3.0/tests/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/tests/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.519677 core_user_registration_app-2.3.0/tests/components/account_request_metadata/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/tests/components/account_request_metadata/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2900 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/tests/components/account_request_metadata/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.533621 core_user_registration_app-2.3.0/tests/components/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/tests/components/user/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.581114 core_user_registration_app-2.3.0/tests/components/user/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/tests/components/user/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1119 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/tests/components/user/fixtures/fixtures.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.647807 core_user_registration_app-2.3.0/tests/components/user_data_structure/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/tests/components/user_data_structure/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.688272 core_user_registration_app-2.3.0/tests/components/user_data_structure/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/tests/components/user_data_structure/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2343 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/tests/components/user_data_structure/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7919 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/tests/components/user_data_structure/test_int_access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3204 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/tests/components/user_data_structure/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.744933 core_user_registration_app-2.3.0/tests/components/user_metadata/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/tests/components/user_metadata/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.776563 core_user_registration_app-2.3.0/tests/components/user_metadata/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/tests/components/user_metadata/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4808 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/tests/components/user_metadata/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4649 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/tests/components/user_metadata/test_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1062 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/tests/components/user_metadata/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.809754 core_user_registration_app-2.3.0/tests/components/user_template_version_manager/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/tests/components/user_template_version_manager/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.842400 core_user_registration_app-2.3.0/tests/components/user_template_version_manager/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/tests/components/user_template_version_manager/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2472 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/tests/components/user_template_version_manager/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6623 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/tests/components/user_template_version_manager/test_int_access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2150 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/tests/test_settings.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2121 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/tests/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.858207 core_user_registration_app-2.3.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/tests/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.878117 core_user_registration_app-2.3.0/tests/views/ajax/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/tests/views/ajax/__init__.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `core_user_registration_app-2.2.0/PKG-INFO` & `core_user_registration_app-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_user_registration_app
-Version: 2.2.0
+Version: 2.3.0
 Summary: User registration module for the core project
 Home-page: https://github.com/usnistgov/core_user_registration_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_user_registration_app
         ==========================
```

### Comparing `core_user_registration_app-2.2.0/README.rst` & `core_user_registration_app-2.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.2.0/core_user_registration_app/access_control/api.py` & `core_user_registration_app-2.3.0/core_user_registration_app/access_control/api.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.2.0/core_user_registration_app/admin.py` & `core_user_registration_app-2.3.0/core_user_registration_app/admin.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.2.0/core_user_registration_app/apps.py` & `core_user_registration_app-2.3.0/core_user_registration_app/apps.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.2.0/core_user_registration_app/components/account_request_metadata/api.py` & `core_user_registration_app-2.3.0/core_user_registration_app/components/account_request_metadata/api.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.2.0/core_user_registration_app/components/account_request_metadata/models.py` & `core_user_registration_app-2.3.0/core_user_registration_app/components/account_request_metadata/models.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.2.0/core_user_registration_app/components/user_data_structure/api.py` & `core_user_registration_app-2.3.0/core_user_registration_app/components/user_data_structure/api.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.2.0/core_user_registration_app/components/user_data_structure/models.py` & `core_user_registration_app-2.3.0/core_user_registration_app/components/user_data_structure/models.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.2.0/core_user_registration_app/components/user_metadata/api.py` & `core_user_registration_app-2.3.0/core_user_registration_app/components/user_metadata/api.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.2.0/core_user_registration_app/components/user_metadata/models.py` & `core_user_registration_app-2.3.0/core_user_registration_app/components/user_metadata/models.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.2.0/core_user_registration_app/components/user_template_version_manager/access_control.py` & `core_user_registration_app-2.3.0/core_user_registration_app/components/user_template_version_manager/access_control.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.2.0/core_user_registration_app/components/user_template_version_manager/api.py` & `core_user_registration_app-2.3.0/core_user_registration_app/components/user_template_version_manager/api.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.2.0/core_user_registration_app/components/user_template_version_manager/models.py` & `core_user_registration_app-2.3.0/core_user_registration_app/components/user_template_version_manager/models.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.2.0/core_user_registration_app/discover.py` & `core_user_registration_app-2.3.0/core_user_registration_app/discover.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.2.0/core_user_registration_app/menus.py` & `core_user_registration_app-2.3.0/core_user_registration_app/menus.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.2.0/core_user_registration_app/migrations/0001_initial.py` & `core_user_registration_app-2.3.0/core_user_registration_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.2.0/core_user_registration_app/models.py` & `core_user_registration_app-2.3.0/core_user_registration_app/models.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.2.0/core_user_registration_app/settings.py` & `core_user_registration_app-2.3.0/core_user_registration_app/settings.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.2.0/core_user_registration_app/static/core_user_registration_app/common/js/templates/set_current.js` & `core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/common/js/templates/set_current.js`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.2.0/core_user_registration_app/static/core_user_registration_app/common/js/templates/versions/set_current.js` & `core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/common/js/templates/versions/set_current.js`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.2.0/core_user_registration_app/static/core_user_registration_app/user/js/autosave.js` & `core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/user/js/autosave.js`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.2.0/core_user_registration_app/static/core_user_registration_app/user/js/report_data.js` & `core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/user/js/report_data.js`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.2.0/core_user_registration_app/static/core_user_registration_app/user/js/save_data.js` & `core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/user/js/save_data.js`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.2.0/core_user_registration_app/static/core_user_registration_app/user/xsd/user.xsd` & `core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/user/xsd/user.xsd`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.2.0/core_user_registration_app/system/api.py` & `core_user_registration_app-2.3.0/core_user_registration_app/system/api.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.2.0/core_user_registration_app/tasks.py` & `core_user_registration_app-2.3.0/core_user_registration_app/tasks.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.2.0/core_user_registration_app/templates/core_user_registration_app/admin/account_requests/pending.html` & `core_user_registration_app-2.3.0/core_user_registration_app/templates/core_user_registration_app/admin/account_requests/pending.html`

 * *Files 12% similar despite different names*

```diff
@@ -33,24 +33,24 @@
                 <div class="btn btn-success accept_request">
                     <i class="fa fa-check"></i> Accept
                 </div>
                 <div class="btn btn-danger deny_request">
                     <i class="fa fa-times"></i> Deny
                 </div>
             </td>
-            {% if request.metadata  %}
-
-            <td><div class="btn btn-view-metadata">
-
-                <i class ="fa fa-file-text-o"></i> View metadata
-            </div>
-            {% endif %}
+            <td>
+                {% if request.metadata  %}
+                <div class="btn btn-view-metadata">
+                    <i class ="fa fa-file-text-o"></i> View metadata
+                </div>
+                {% endif %}
+            </td>
         </tr>
     {% empty %}
         <tr>
-            <td class="empty" colspan="6">
+            <td class="empty" colspan="7">
                 No account requests pending at the moment.
             </td>
         </tr>
     {% endfor %}
 </table>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,10 +1,11 @@
 {% extends 'core_main_app/_render/admin/theme/tools/box.html' %} {% load
 timestamptags %} {% block box_title %}Pending requests{% endblock %} {% block
 box_body %}
 User             First Name         Late Name         Email Address Date                                    Actions Metadata
-{                {                  {                 {             {                                                View
-{                {                  {                 {             {                                        Accept metadata
-request.username request.first_name request.last_name request.email request.date|print_datetime_utc_unaware  Deny   {% endif
-}}               }}                 }}                }}            }}                                              %}
+{                {                  {                 {             {                                               {% if
+{                {                  {                 {             {                                        Accept request.metadata
+request.username request.first_name request.last_name request.email request.date|print_datetime_utc_unaware  Deny   %}
+}}               }}                 }}                }}            }}                                               View metadata
+                                                                                                                    {% endif %}
 No account requests pending at the moment.
 {% endblock %}
```

### Comparing `core_user_registration_app-2.2.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/list/available.html` & `core_user_registration_app-2.3.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/list/available.html`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.2.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/list.html` & `core_user_registration_app-2.3.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/list.html`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.2.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/versions/available.html` & `core_user_registration_app-2.3.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/versions/available.html`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.2.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/versions.html` & `core_user_registration_app-2.3.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/versions.html`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.2.0/core_user_registration_app/templates/core_user_registration_app/user/account_creation.html` & `core_user_registration_app-2.3.0/core_user_registration_app/templates/core_user_registration_app/user/account_creation.html`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.2.0/core_user_registration_app/templates/core_user_registration_app/user/request_new_account.html` & `core_user_registration_app-2.3.0/core_user_registration_app/templates/core_user_registration_app/user/request_new_account.html`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.2.0/core_user_registration_app/urls.py` & `core_user_registration_app-2.3.0/core_user_registration_app/urls.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.2.0/core_user_registration_app/views/admin/ajax.py` & `core_user_registration_app-2.3.0/core_user_registration_app/views/admin/ajax.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.2.0/core_user_registration_app/views/admin/views.py` & `core_user_registration_app-2.3.0/core_user_registration_app/views/admin/views.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.2.0/core_user_registration_app/views/user/ajax.py` & `core_user_registration_app-2.3.0/core_user_registration_app/views/user/ajax.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.2.0/core_user_registration_app/views/user/views.py` & `core_user_registration_app-2.3.0/core_user_registration_app/views/user/views.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.2.0/core_user_registration_app.egg-info/PKG-INFO` & `core_user_registration_app-2.3.0/core_user_registration_app.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-user-registration-app
-Version: 2.2.0
+Version: 2.3.0
 Summary: User registration module for the core project
 Home-page: https://github.com/usnistgov/core_user_registration_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_user_registration_app
         ==========================
```

### Comparing `core_user_registration_app-2.2.0/core_user_registration_app.egg-info/SOURCES.txt` & `core_user_registration_app-2.3.0/core_user_registration_app.egg-info/SOURCES.txt`

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
 core_user_registration_app/__init__.py
```

### Comparing `core_user_registration_app-2.2.0/setup.py` & `core_user_registration_app-2.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_user_registration_app",
-    version="2.2.0",
+    version="2.3.0",
     description="User registration module for the core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_user_registration_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_user_registration_app-2.2.0/tests/components/account_request_metadata/tests_unit.py` & `core_user_registration_app-2.3.0/tests/components/account_request_metadata/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.2.0/tests/components/user/fixtures/fixtures.py` & `core_user_registration_app-2.3.0/tests/components/user/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.2.0/tests/components/user_data_structure/fixtures/fixtures.py` & `core_user_registration_app-2.3.0/tests/components/user_data_structure/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.2.0/tests/components/user_data_structure/test_int_access_control.py` & `core_user_registration_app-2.3.0/tests/components/user_data_structure/test_int_access_control.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
 
 from django.contrib.auth.models import AnonymousUser
 
 import core_user_registration_app.components.user_data_structure.api as user_data_structure_api
 from core_main_app.access_control.exceptions import AccessControlError
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from core_parser_app.components.data_structure.models import (
     DataStructureElement,
 )
 from core_user_registration_app.components.user_data_structure.models import (
     UserDataStructure,
@@ -18,15 +18,15 @@
 from tests.components.user_data_structure.fixtures.fixtures import (
     UserDataStructureFixtures,
 )
 
 fixture_data_structure = UserDataStructureFixtures()
 
 
-class TestUserDataStructureGetAll(MongoIntegrationBaseTestCase):
+class TestUserDataStructureGetAll(IntegrationBaseTestCase):
     fixture = fixture_data_structure
 
     def test_get_all_as_superuser_returns_all_data_structure(self):
         mock_user = create_mock_user("1", is_staff=True, is_superuser=True)
         result = user_data_structure_api.get_all(mock_user)
         self.assertTrue(
             all(isinstance(item, UserDataStructure) for item in result)
@@ -38,15 +38,15 @@
             user_data_structure_api.get_all(mock_user)
 
     def test_get_all_as_anonymous_user_raises_error(self):
         with self.assertRaises(AccessControlError):
             user_data_structure_api.get_all(AnonymousUser())
 
 
-class TestUserDataStructureDelete(MongoIntegrationBaseTestCase):
+class TestUserDataStructureDelete(IntegrationBaseTestCase):
     fixture = fixture_data_structure
 
     def test_delete_others_data_structure_as_superuser_deletes_data_structure(
         self,
     ):
         data_structure = self.fixture.data_structure_3
         mock_user = create_mock_user(
@@ -58,17 +58,15 @@
 
     def test_delete_own_data_structure_deletes_data_structure(self):
         data_structure = self.fixture.data_structure_1
         mock_user = create_mock_user(self.fixture.data_structure_1.user)
         user_data_structure_api.delete(data_structure, mock_user)
 
 
-class TestUserDataStructureUpdateDataStructureRoot(
-    MongoIntegrationBaseTestCase
-):
+class TestUserDataStructureUpdateDataStructureRoot(IntegrationBaseTestCase):
     fixture = fixture_data_structure
 
     def test_update_others_data_structure_root_as_superuser_updates_data_structure(
         self,
     ):
         data_structure = self.fixture.data_structure_1
         new_data_structure_element_root = DataStructureElement()
@@ -98,28 +96,28 @@
         result = user_data_structure_api.get_by_id(data_structure.id)
         self.assertTrue(isinstance(result, UserDataStructure))
         self.assertTrue(
             result.data_structure_element_root, new_data_structure_element_root
         )
 
 
-class TestUserDataStructureCreateOrUpdate(MongoIntegrationBaseTestCase):
+class TestUserDataStructureCreateOrUpdate(IntegrationBaseTestCase):
     fixture = fixture_data_structure
 
     def test_upsert_own_data_structure_updates_data_structure(self):
         data_structure = self.fixture.data_structure_1
         data_structure.name = "new_name_1"
         mock_user = create_mock_user(self.fixture.data_structure_1.user)
         user_data_structure_api.upsert(data_structure, mock_user)
         result = user_data_structure_api.get_by_id(data_structure.id)
         self.assertTrue(isinstance(result, UserDataStructure))
         self.assertTrue(data_structure.name, result.name)
 
 
-class TestUserDataStructureGetByDataId(MongoIntegrationBaseTestCase):
+class TestUserDataStructureGetByDataId(IntegrationBaseTestCase):
     fixture = fixture_data_structure
 
     def test_get_by_data_id_as_superuser_returns_data_structure(self):
 
         mock_user = create_mock_user(
             self.fixture.data_structure_3.user,
             is_staff=True,
@@ -149,15 +147,15 @@
     def test_get_by_data_id_as_anonymous_user_raises_error(self):
         with self.assertRaises(AccessControlError):
             user_data_structure_api.get_by_data_id(
                 self.fixture.data.id, AnonymousUser()
             )
 
 
-class TestDataStructureChangeOwner(MongoIntegrationBaseTestCase):
+class TestDataStructureChangeOwner(IntegrationBaseTestCase):
 
     fixture = fixture_data_structure
 
     def test_change_owner_from_owner_to_owner_ok(self):
         mock_owner = create_mock_user(self.fixture.data_structure_1.user)
         user_data_structure_api.change_owner(
             document=fixture_data_structure.data_structure_1,
```

### Comparing `core_user_registration_app-2.2.0/tests/components/user_data_structure/tests_unit.py` & `core_user_registration_app-2.3.0/tests/components/user_data_structure/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.2.0/tests/components/user_metadata/fixtures/fixtures.py` & `core_user_registration_app-2.3.0/tests/components/user_metadata/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.2.0/tests/components/user_metadata/test_int.py` & `core_user_registration_app-2.3.0/tests/components/user_metadata/test_int.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """ Unit Test UserMetadata
 """
 
 from core_main_app.commons import exceptions
 from core_main_app.settings import DATA_SORTING_FIELDS
 from core_main_app.utils.datetime import datetime_now
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from core_user_registration_app.components.user_metadata.api import (
     check_xml_file_is_valid,
 )
 from core_user_registration_app.components.user_metadata.models import (
     UserMetadata,
@@ -19,15 +19,15 @@
     AccessControlDataFixture,
 )
 
 fixture_data = DataFixtures()
 access_control_data_fixture = AccessControlDataFixture()
 
 
-class TestDataGetAll(MongoIntegrationBaseTestCase):
+class TestDataGetAll(IntegrationBaseTestCase):
 
     fixture = access_control_data_fixture
 
     def test_data_get_all_return_collection_of_data(self):
         # Act
         result = UserMetadata.get_all(DATA_SORTING_FIELDS)
         # Assert
@@ -103,15 +103,15 @@
             self.fixture.data_4.user_id, descending_result.all()[3].user_id
         )
         self.assertEqual(
             self.fixture.data_5.user_id, descending_result.all()[4].user_id
         )
 
 
-class TestDataGetById(MongoIntegrationBaseTestCase):
+class TestDataGetById(IntegrationBaseTestCase):
 
     fixture = fixture_data
 
     def test_data_get_by_id_raises_api_error_if_not_found(self):
         # Act # Assert
         with self.assertRaises(exceptions.DoesNotExist):
             UserMetadata.get_by_id(-1)
```

### Comparing `core_user_registration_app-2.2.0/tests/components/user_metadata/test_unit.py` & `core_user_registration_app-2.3.0/tests/components/user_metadata/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.2.0/tests/components/user_template_version_manager/fixtures/fixtures.py` & `core_user_registration_app-2.3.0/tests/components/user_template_version_manager/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.2.0/tests/components/user_template_version_manager/test_int_access_control.py` & `core_user_registration_app-2.3.0/tests/components/user_template_version_manager/test_int_access_control.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """ Access control testing
 """
 
 from core_main_app.access_control.exceptions import AccessControlError
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from core_main_app.utils.tests_tools.RequestMock import create_mock_request
 from core_user_registration_app.components.user_template_version_manager import (
     api as user_template_vm_api,
 )
 from tests.components.user_template_version_manager.fixtures.fixtures import (
@@ -16,15 +16,15 @@
 
 fixture_template_vm = UserTemplateVersionManagerAccessControlFixtures()
 
 
 # FIXME: missing tests where CAN_ANONYMOUS_ACCESS_PUBLIC_DOCUMENT is True
 
 
-class TestTemplateVersionManagerInsert(MongoIntegrationBaseTestCase):
+class TestTemplateVersionManagerInsert(IntegrationBaseTestCase):
 
     fixture = fixture_template_vm
 
     def setUp(self):
         self.anonymous_user = create_mock_user(user_id=None, is_anonymous=True)
         self.user1 = create_mock_user(user_id="1")
         self.staff_user1 = create_mock_user(user_id="1", is_staff=True)
@@ -129,15 +129,15 @@
         user_template_vm_api.insert(
             self.fixture.global_tvm,
             self.fixture.global_template,
             request=mock_request,
         )
 
 
-class TestTemplateGetGlobalVersionManagers(MongoIntegrationBaseTestCase):
+class TestTemplateGetGlobalVersionManagers(IntegrationBaseTestCase):
 
     fixture = fixture_template_vm
 
     def setUp(self):
         self.anonymous_user = create_mock_user(user_id=None, is_anonymous=True)
         self.user1 = create_mock_user(user_id="1")
         self.staff_user1 = create_mock_user(user_id="1", is_staff=True)
```

### Comparing `core_user_registration_app-2.2.0/tests/test_settings.py` & `core_user_registration_app-2.3.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.2.0/tests/urls.py` & `core_user_registration_app-2.3.0/tests/urls.py`

 * *Files identical despite different names*

