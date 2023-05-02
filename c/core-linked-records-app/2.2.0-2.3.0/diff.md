# Comparing `tmp/core_linked_records_app-2.2.0.tar.gz` & `tmp/core_linked_records_app-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/core_linked_records_app-2.2.0.tar", last modified: Thu Feb 23 20:30:11 2023, max compression
+gzip compressed data, was "core_linked_records_app-2.3.0.tar", last modified: Tue May  2 19:39:28 2023, max compression
```

## Comparing `core_linked_records_app-2.2.0.tar` & `core_linked_records_app-2.3.0.tar`

### file list

```diff
@@ -1,280 +1,286 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:11.000000 core_linked_records_app-2.2.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      179 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6496 2023-02-23 20:30:11.000000 core_linked_records_app-2.2.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4718 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:08.000000 core_linked_records_app-2.2.0/core_linked_records_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      122 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1222 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/admin.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1065 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/apps.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:08.000000 core_linked_records_app-2.2.0/core_linked_records_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:08.000000 core_linked_records_app-2.2.0/core_linked_records_app/components/blob/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/components/blob/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4188 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/components/blob/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1841 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/components/blob/watch.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:08.000000 core_linked_records_app-2.2.0/core_linked_records_app/components/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/components/data/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3595 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/components/data/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3775 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/components/data/watch.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:08.000000 core_linked_records_app-2.2.0/core_linked_records_app/components/local_id/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/components/local_id/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      359 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/components/local_id/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2187 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/components/local_id/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2604 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/components/local_id/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:08.000000 core_linked_records_app-2.2.0/core_linked_records_app/components/oai_record/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/components/oai_record/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1279 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/components/oai_record/api.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:08.000000 core_linked_records_app-2.2.0/core_linked_records_app/components/pid_settings/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/components/pid_settings/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      433 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/components/pid_settings/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1093 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/components/pid_settings/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      890 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/components/pid_settings/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      622 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/components/pid_settings/watch.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:08.000000 core_linked_records_app-2.2.0/core_linked_records_app/components/pid_xpath/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/components/pid_xpath/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      191 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/components/pid_xpath/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1892 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/components/pid_xpath/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1951 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/components/pid_xpath/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      470 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/menus.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:08.000000 core_linked_records_app-2.2.0/core_linked_records_app/migrations/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2800 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/migrations/0001_initial.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/migrations/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:08.000000 core_linked_records_app-2.2.0/core_linked_records_app/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:08.000000 core_linked_records_app-2.2.0/core_linked_records_app/rest/blob/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/rest/blob/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2526 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/rest/blob/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:08.000000 core_linked_records_app-2.2.0/core_linked_records_app/rest/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/rest/data/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:08.000000 core_linked_records_app-2.2.0/core_linked_records_app/rest/data/renderers/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/rest/data/renderers/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2971 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/rest/data/renderers/data_html_user_renderer.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      948 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/rest/data/renderers/data_xml_renderer.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:09.000000 core_linked_records_app-2.2.0/core_linked_records_app/rest/pid/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/rest/pid/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      467 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/rest/pid/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7709 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/rest/pid/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:09.000000 core_linked_records_app-2.2.0/core_linked_records_app/rest/pid_settings/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/rest/pid_settings/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      817 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/rest/pid_settings/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2887 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/rest/pid_settings/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:09.000000 core_linked_records_app-2.2.0/core_linked_records_app/rest/pid_xpath/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/rest/pid_xpath/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      349 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/rest/pid_xpath/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      841 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/rest/pid_xpath/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:09.000000 core_linked_records_app-2.2.0/core_linked_records_app/rest/providers/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/rest/providers/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7677 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/rest/providers/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:09.000000 core_linked_records_app-2.2.0/core_linked_records_app/rest/query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/rest/query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6090 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/rest/query/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2310 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/rest/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1634 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:07.000000 core_linked_records_app-2.2.0/core_linked_records_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:07.000000 core_linked_records_app-2.2.0/core_linked_records_app/static/core_linked_records_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:07.000000 core_linked_records_app-2.2.0/core_linked_records_app/static/core_linked_records_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:09.000000 core_linked_records_app-2.2.0/core_linked_records_app/static/core_linked_records_app/admin/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       72 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/static/core_linked_records_app/admin/css/pid_settings.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:07.000000 core_linked_records_app-2.2.0/core_linked_records_app/static/core_linked_records_app/admin/js/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:09.000000 core_linked_records_app-2.2.0/core_linked_records_app/static/core_linked_records_app/admin/js/pid_settings/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1694 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/static/core_linked_records_app/admin/js/pid_settings/auto_set_pid.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:07.000000 core_linked_records_app-2.2.0/core_linked_records_app/static/core_linked_records_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:09.000000 core_linked_records_app-2.2.0/core_linked_records_app/static/core_linked_records_app/user/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       43 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/static/core_linked_records_app/user/css/sharing.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:07.000000 core_linked_records_app-2.2.0/core_linked_records_app/static/core_linked_records_app/user/js/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:09.000000 core_linked_records_app-2.2.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      494 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/blob_list.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       78 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/blob_list.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      735 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/common_list.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1199 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/data_detail.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      236 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/data_detail.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      494 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/data_list.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       78 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/data_list.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1309 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/explore.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       78 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/explore.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:09.000000 core_linked_records_app-2.2.0/core_linked_records_app/system/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/system/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5237 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/system/api.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:07.000000 core_linked_records_app-2.2.0/core_linked_records_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:07.000000 core_linked_records_app-2.2.0/core_linked_records_app/templates/core_linked_records_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:09.000000 core_linked_records_app-2.2.0/core_linked_records_app/templates/core_linked_records_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:09.000000 core_linked_records_app-2.2.0/core_linked_records_app/templates/core_linked_records_app/admin/pid_settings/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2320 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/templates/core_linked_records_app/admin/pid_settings/box.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      233 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/templates/core_linked_records_app/admin/pid_settings.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      290 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/templates/core_linked_records_app/admin/pid_settings_error.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:07.000000 core_linked_records_app-2.2.0/core_linked_records_app/templates/core_linked_records_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:07.000000 core_linked_records_app-2.2.0/core_linked_records_app/templates/core_linked_records_app/user/sharing/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:09.000000 core_linked_records_app-2.2.0/core_linked_records_app/templates/core_linked_records_app/user/sharing/data_detail/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      253 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/templates/core_linked_records_app/user/sharing/data_detail/button.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      236 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/templates/core_linked_records_app/user/sharing/data_detail/button_inline.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      283 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/templates/core_linked_records_app/user/sharing/data_detail/modal.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:09.000000 core_linked_records_app-2.2.0/core_linked_records_app/templates/core_linked_records_app/user/sharing/explore/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      246 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/templates/core_linked_records_app/user/sharing/explore/button.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      298 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/templates/core_linked_records_app/user/sharing/explore/modal.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      177 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:09.000000 core_linked_records_app-2.2.0/core_linked_records_app/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/utils/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1536 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/utils/blob.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1941 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/utils/data.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1835 2023-02-23 20:30:03.000000 core_linked_records_app-2.2.0/core_linked_records_app/utils/dict.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      661 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/core_linked_records_app/utils/path.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1023 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/core_linked_records_app/utils/pid.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:09.000000 core_linked_records_app-2.2.0/core_linked_records_app/utils/providers/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6104 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/core_linked_records_app/utils/providers/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4747 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/core_linked_records_app/utils/providers/handle_net.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4802 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/core_linked_records_app/utils/providers/local.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4076 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/core_linked_records_app/utils/xml.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:09.000000 core_linked_records_app-2.2.0/core_linked_records_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/core_linked_records_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:09.000000 core_linked_records_app-2.2.0/core_linked_records_app/views/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/core_linked_records_app/views/admin/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3675 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/core_linked_records_app/views/admin/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:08.000000 core_linked_records_app-2.2.0/core_linked_records_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6496 2023-02-23 20:30:06.000000 core_linked_records_app-2.2.0/core_linked_records_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8455 2023-02-23 20:30:07.000000 core_linked_records_app-2.2.0/core_linked_records_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-02-23 20:30:06.000000 core_linked_records_app-2.2.0/core_linked_records_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      137 2023-02-23 20:30:06.000000 core_linked_records_app-2.2.0/core_linked_records_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       30 2023-02-23 20:30:06.000000 core_linked_records_app-2.2.0/core_linked_records_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       70 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       67 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-02-23 20:30:11.000000 core_linked_records_app-2.2.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1034 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:09.000000 core_linked_records_app-2.2.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       49 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:09.000000 core_linked_records_app-2.2.0/tests/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:09.000000 core_linked_records_app-2.2.0/tests/components/blob/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/components/blob/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:09.000000 core_linked_records_app-2.2.0/tests/components/blob/api/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/components/blob/api/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12750 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/components/blob/api/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:09.000000 core_linked_records_app-2.2.0/tests/components/blob/watch/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/components/blob/watch/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8727 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/components/blob/watch/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:09.000000 core_linked_records_app-2.2.0/tests/components/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/components/data/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:10.000000 core_linked_records_app-2.2.0/tests/components/data/api/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/components/data/api/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10274 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/components/data/api/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:10.000000 core_linked_records_app-2.2.0/tests/components/data/watch/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/components/data/watch/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    21118 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/components/data/watch/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:10.000000 core_linked_records_app-2.2.0/tests/components/local_id/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/components/local_id/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:10.000000 core_linked_records_app-2.2.0/tests/components/local_id/api/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/components/local_id/api/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3614 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/components/local_id/api/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:10.000000 core_linked_records_app-2.2.0/tests/components/local_id/models/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/components/local_id/models/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4057 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/components/local_id/models/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:10.000000 core_linked_records_app-2.2.0/tests/components/oai_record/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/components/oai_record/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:10.000000 core_linked_records_app-2.2.0/tests/components/oai_record/api/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/components/oai_record/api/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3030 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/components/oai_record/api/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:10.000000 core_linked_records_app-2.2.0/tests/components/pid_settings/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/components/pid_settings/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:10.000000 core_linked_records_app-2.2.0/tests/components/pid_settings/api/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/components/pid_settings/api/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1760 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/components/pid_settings/api/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:10.000000 core_linked_records_app-2.2.0/tests/components/pid_settings/models/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/components/pid_settings/models/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1460 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/components/pid_settings/models/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:10.000000 core_linked_records_app-2.2.0/tests/components/pid_settings/watch/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/components/pid_settings/watch/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2765 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/components/pid_settings/watch/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:10.000000 core_linked_records_app-2.2.0/tests/components/pid_xpath/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/components/pid_xpath/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:10.000000 core_linked_records_app-2.2.0/tests/components/pid_xpath/admin_site/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/components/pid_xpath/admin_site/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      566 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/components/pid_xpath/admin_site/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:10.000000 core_linked_records_app-2.2.0/tests/components/pid_xpath/api/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/components/pid_xpath/api/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4208 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/components/pid_xpath/api/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:10.000000 core_linked_records_app-2.2.0/tests/components/pid_xpath/models/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/components/pid_xpath/models/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3121 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/components/pid_xpath/models/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:10.000000 core_linked_records_app-2.2.0/tests/menus/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/menus/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      553 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/menus/test_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4151 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/mocks.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:10.000000 core_linked_records_app-2.2.0/tests/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:10.000000 core_linked_records_app-2.2.0/tests/rest/blob/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/rest/blob/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:10.000000 core_linked_records_app-2.2.0/tests/rest/blob/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/rest/blob/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2639 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/rest/blob/views/test_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5112 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/rest/blob/views/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:10.000000 core_linked_records_app-2.2.0/tests/rest/pid/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/rest/pid/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:10.000000 core_linked_records_app-2.2.0/tests/rest/pid/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/rest/pid/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6100 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/rest/pid/views/test_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10991 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/rest/pid/views/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:10.000000 core_linked_records_app-2.2.0/tests/rest/pid_settings/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/rest/pid_settings/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:10.000000 core_linked_records_app-2.2.0/tests/rest/pid_settings/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/rest/pid_settings/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4244 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/rest/pid_settings/views/test_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5951 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/rest/pid_settings/views/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:10.000000 core_linked_records_app-2.2.0/tests/rest/pid_xpath/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/rest/pid_xpath/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:10.000000 core_linked_records_app-2.2.0/tests/rest/pid_xpath/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/rest/pid_xpath/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7569 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/rest/pid_xpath/views/test_permissions.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:10.000000 core_linked_records_app-2.2.0/tests/rest/providers/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/rest/providers/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:10.000000 core_linked_records_app-2.2.0/tests/rest/providers/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/rest/providers/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8187 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/rest/providers/views/test_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17141 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/rest/providers/views/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:10.000000 core_linked_records_app-2.2.0/tests/rest/query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/rest/query/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:10.000000 core_linked_records_app-2.2.0/tests/rest/query/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/rest/query/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5379 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/rest/query/views/test_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8668 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/rest/query/views/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:10.000000 core_linked_records_app-2.2.0/tests/system/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/system/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:11.000000 core_linked_records_app-2.2.0/tests/system/api/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/system/api/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    16785 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/system/api/test_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2113 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/test_settings.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      458 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/test_urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:11.000000 core_linked_records_app-2.2.0/tests/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/utils/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:11.000000 core_linked_records_app-2.2.0/tests/utils/blob/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/utils/blob/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      421 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/utils/blob/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:11.000000 core_linked_records_app-2.2.0/tests/utils/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/utils/data/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      421 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/utils/data/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:11.000000 core_linked_records_app-2.2.0/tests/utils/dict/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/utils/dict/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4213 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/utils/dict/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:11.000000 core_linked_records_app-2.2.0/tests/utils/path/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/utils/path/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      378 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/utils/path/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:11.000000 core_linked_records_app-2.2.0/tests/utils/pid/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:04.000000 core_linked_records_app-2.2.0/tests/utils/pid/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2298 2023-02-23 20:30:05.000000 core_linked_records_app-2.2.0/tests/utils/pid/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:11.000000 core_linked_records_app-2.2.0/tests/utils/providers/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:05.000000 core_linked_records_app-2.2.0/tests/utils/providers/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:11.000000 core_linked_records_app-2.2.0/tests/utils/providers/handle_net/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:05.000000 core_linked_records_app-2.2.0/tests/utils/providers/handle_net/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3952 2023-02-23 20:30:05.000000 core_linked_records_app-2.2.0/tests/utils/providers/handle_net/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:11.000000 core_linked_records_app-2.2.0/tests/utils/providers/local/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:05.000000 core_linked_records_app-2.2.0/tests/utils/providers/local/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12238 2023-02-23 20:30:05.000000 core_linked_records_app-2.2.0/tests/utils/providers/local/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:11.000000 core_linked_records_app-2.2.0/tests/utils/xml/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:05.000000 core_linked_records_app-2.2.0/tests/utils/xml/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1454 2023-02-23 20:30:05.000000 core_linked_records_app-2.2.0/tests/utils/xml/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:11.000000 core_linked_records_app-2.2.0/tests/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:05.000000 core_linked_records_app-2.2.0/tests/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:11.000000 core_linked_records_app-2.2.0/tests/views/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:05.000000 core_linked_records_app-2.2.0/tests/views/admin/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:11.000000 core_linked_records_app-2.2.0/tests/views/admin/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:30:05.000000 core_linked_records_app-2.2.0/tests/views/admin/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6799 2023-02-23 20:30:05.000000 core_linked_records_app-2.2.0/tests/views/admin/views/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:28.227119 core_linked_records_app-2.3.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:39:19.000000 core_linked_records_app-2.3.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      179 2023-05-02 19:39:19.000000 core_linked_records_app-2.3.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6496 2023-05-02 19:39:28.222294 core_linked_records_app-2.3.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4718 2023-05-02 19:39:19.000000 core_linked_records_app-2.3.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:25.115064 core_linked_records_app-2.3.0/core_linked_records_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      122 2023-05-02 19:39:19.000000 core_linked_records_app-2.3.0/core_linked_records_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1226 2023-05-02 19:39:19.000000 core_linked_records_app-2.3.0/core_linked_records_app/admin.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1065 2023-05-02 19:39:19.000000 core_linked_records_app-2.3.0/core_linked_records_app/apps.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:25.208337 core_linked_records_app-2.3.0/core_linked_records_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:19.000000 core_linked_records_app-2.3.0/core_linked_records_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:25.252329 core_linked_records_app-2.3.0/core_linked_records_app/components/blob/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:19.000000 core_linked_records_app-2.3.0/core_linked_records_app/components/blob/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4188 2023-05-02 19:39:19.000000 core_linked_records_app-2.3.0/core_linked_records_app/components/blob/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2418 2023-05-02 19:39:19.000000 core_linked_records_app-2.3.0/core_linked_records_app/components/blob/watch.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:25.306026 core_linked_records_app-2.3.0/core_linked_records_app/components/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:19.000000 core_linked_records_app-2.3.0/core_linked_records_app/components/data/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3595 2023-05-02 19:39:19.000000 core_linked_records_app-2.3.0/core_linked_records_app/components/data/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4243 2023-05-02 19:39:19.000000 core_linked_records_app-2.3.0/core_linked_records_app/components/data/watch.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:25.359090 core_linked_records_app-2.3.0/core_linked_records_app/components/local_id/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:19.000000 core_linked_records_app-2.3.0/core_linked_records_app/components/local_id/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      428 2023-05-02 19:39:19.000000 core_linked_records_app-2.3.0/core_linked_records_app/components/local_id/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2187 2023-05-02 19:39:19.000000 core_linked_records_app-2.3.0/core_linked_records_app/components/local_id/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2604 2023-05-02 19:39:19.000000 core_linked_records_app-2.3.0/core_linked_records_app/components/local_id/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:25.385063 core_linked_records_app-2.3.0/core_linked_records_app/components/oai_record/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:19.000000 core_linked_records_app-2.3.0/core_linked_records_app/components/oai_record/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1279 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/components/oai_record/api.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:25.455077 core_linked_records_app-2.3.0/core_linked_records_app/components/pid_settings/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/components/pid_settings/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      433 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/components/pid_settings/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1093 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/components/pid_settings/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      890 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/components/pid_settings/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      622 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/components/pid_settings/watch.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:25.529376 core_linked_records_app-2.3.0/core_linked_records_app/components/pid_xpath/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/components/pid_xpath/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      191 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/components/pid_xpath/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1892 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/components/pid_xpath/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1951 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/components/pid_xpath/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      470 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/menus.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:25.575147 core_linked_records_app-2.3.0/core_linked_records_app/migrations/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2800 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/migrations/0001_initial.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      659 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/migrations/0002_alter_pidxpath_xpath.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/migrations/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:25.606323 core_linked_records_app-2.3.0/core_linked_records_app/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:25.635729 core_linked_records_app-2.3.0/core_linked_records_app/rest/blob/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/rest/blob/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2526 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/rest/blob/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:25.651714 core_linked_records_app-2.3.0/core_linked_records_app/rest/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/rest/data/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:25.713657 core_linked_records_app-2.3.0/core_linked_records_app/rest/data/renderers/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/rest/data/renderers/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2971 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/rest/data/renderers/data_html_user_renderer.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      948 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/rest/data/renderers/data_xml_renderer.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:25.755447 core_linked_records_app-2.3.0/core_linked_records_app/rest/pid/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/rest/pid/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      467 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/rest/pid/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8298 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/rest/pid/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:25.800353 core_linked_records_app-2.3.0/core_linked_records_app/rest/pid_settings/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/rest/pid_settings/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      817 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/rest/pid_settings/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2887 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/rest/pid_settings/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:25.846637 core_linked_records_app-2.3.0/core_linked_records_app/rest/pid_xpath/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/rest/pid_xpath/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      349 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/rest/pid_xpath/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      841 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/rest/pid_xpath/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:25.877340 core_linked_records_app-2.3.0/core_linked_records_app/rest/providers/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/rest/providers/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7677 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/rest/providers/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:25.908985 core_linked_records_app-2.3.0/core_linked_records_app/rest/query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/rest/query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      736 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/rest/query/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1925 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/rest/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1634 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:24.576120 core_linked_records_app-2.3.0/core_linked_records_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:24.598407 core_linked_records_app-2.3.0/core_linked_records_app/static/core_linked_records_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:24.589299 core_linked_records_app-2.3.0/core_linked_records_app/static/core_linked_records_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:25.935042 core_linked_records_app-2.3.0/core_linked_records_app/static/core_linked_records_app/admin/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       72 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/static/core_linked_records_app/admin/css/pid_settings.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:24.592436 core_linked_records_app-2.3.0/core_linked_records_app/static/core_linked_records_app/admin/js/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:25.954529 core_linked_records_app-2.3.0/core_linked_records_app/static/core_linked_records_app/admin/js/pid_settings/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1694 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/static/core_linked_records_app/admin/js/pid_settings/auto_set_pid.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:24.607542 core_linked_records_app-2.3.0/core_linked_records_app/static/core_linked_records_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:25.976717 core_linked_records_app-2.3.0/core_linked_records_app/static/core_linked_records_app/user/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       43 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/static/core_linked_records_app/user/css/sharing.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:24.610830 core_linked_records_app-2.3.0/core_linked_records_app/static/core_linked_records_app/user/js/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:26.122574 core_linked_records_app-2.3.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      494 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/blob_list.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       78 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/blob_list.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      735 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/common_list.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1199 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/data_detail.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      236 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/data_detail.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      494 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/data_list.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       78 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/data_list.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1309 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/explore.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       78 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/explore.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:26.154545 core_linked_records_app-2.3.0/core_linked_records_app/system/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/system/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7189 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/system/api.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:24.627300 core_linked_records_app-2.3.0/core_linked_records_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:24.641805 core_linked_records_app-2.3.0/core_linked_records_app/templates/core_linked_records_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:26.184045 core_linked_records_app-2.3.0/core_linked_records_app/templates/core_linked_records_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:26.197983 core_linked_records_app-2.3.0/core_linked_records_app/templates/core_linked_records_app/admin/pid_settings/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2320 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/templates/core_linked_records_app/admin/pid_settings/box.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      233 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/templates/core_linked_records_app/admin/pid_settings.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      290 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/templates/core_linked_records_app/admin/pid_settings_error.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:24.644788 core_linked_records_app-2.3.0/core_linked_records_app/templates/core_linked_records_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:24.665981 core_linked_records_app-2.3.0/core_linked_records_app/templates/core_linked_records_app/user/sharing/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:26.254051 core_linked_records_app-2.3.0/core_linked_records_app/templates/core_linked_records_app/user/sharing/data_detail/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      253 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/templates/core_linked_records_app/user/sharing/data_detail/button.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      236 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/templates/core_linked_records_app/user/sharing/data_detail/button_inline.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      283 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/templates/core_linked_records_app/user/sharing/data_detail/modal.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:26.280155 core_linked_records_app-2.3.0/core_linked_records_app/templates/core_linked_records_app/user/sharing/explore/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      246 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/templates/core_linked_records_app/user/sharing/explore/button.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      298 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/templates/core_linked_records_app/user/sharing/explore/modal.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      177 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:26.405423 core_linked_records_app-2.3.0/core_linked_records_app/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/utils/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1536 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/utils/blob.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1941 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/utils/data.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1835 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/utils/dict.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      661 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/utils/path.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1023 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/utils/pid.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:26.453705 core_linked_records_app-2.3.0/core_linked_records_app/utils/providers/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6104 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/utils/providers/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4747 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/utils/providers/handle_net.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4802 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/utils/providers/local.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4914 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/utils/query.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4076 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/utils/xml.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:26.476506 core_linked_records_app-2.3.0/core_linked_records_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:26.512771 core_linked_records_app-2.3.0/core_linked_records_app/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/views/admin/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3675 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/views/admin/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:25.184388 core_linked_records_app-2.3.0/core_linked_records_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6496 2023-05-02 19:39:23.000000 core_linked_records_app-2.3.0/core_linked_records_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8645 2023-05-02 19:39:24.000000 core_linked_records_app-2.3.0/core_linked_records_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:39:23.000000 core_linked_records_app-2.3.0/core_linked_records_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      137 2023-05-02 19:39:23.000000 core_linked_records_app-2.3.0/core_linked_records_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       30 2023-05-02 19:39:23.000000 core_linked_records_app-2.3.0/core_linked_records_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       70 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       67 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:39:28.229171 core_linked_records_app-2.3.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1034 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:26.596362 core_linked_records_app-2.3.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       49 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:26.613737 core_linked_records_app-2.3.0/tests/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/tests/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:26.635324 core_linked_records_app-2.3.0/tests/components/blob/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/tests/components/blob/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:26.670905 core_linked_records_app-2.3.0/tests/components/blob/api/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/tests/components/blob/api/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12750 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/blob/api/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:26.709830 core_linked_records_app-2.3.0/tests/components/blob/watch/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/blob/watch/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9762 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/blob/watch/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:26.727610 core_linked_records_app-2.3.0/tests/components/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/data/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:26.764941 core_linked_records_app-2.3.0/tests/components/data/api/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/data/api/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10274 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/data/api/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:26.798326 core_linked_records_app-2.3.0/tests/components/data/watch/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/data/watch/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    22092 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/data/watch/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:26.815207 core_linked_records_app-2.3.0/tests/components/local_id/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/local_id/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:26.849540 core_linked_records_app-2.3.0/tests/components/local_id/admin_site/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/local_id/admin_site/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      953 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/local_id/admin_site/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:26.887421 core_linked_records_app-2.3.0/tests/components/local_id/api/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/local_id/api/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3614 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/local_id/api/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:26.921313 core_linked_records_app-2.3.0/tests/components/local_id/models/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/local_id/models/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4057 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/local_id/models/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:26.935161 core_linked_records_app-2.3.0/tests/components/oai_record/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/oai_record/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:26.968820 core_linked_records_app-2.3.0/tests/components/oai_record/api/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/oai_record/api/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3030 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/oai_record/api/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:26.985958 core_linked_records_app-2.3.0/tests/components/pid_settings/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/pid_settings/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.024124 core_linked_records_app-2.3.0/tests/components/pid_settings/api/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/pid_settings/api/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1760 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/pid_settings/api/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.053716 core_linked_records_app-2.3.0/tests/components/pid_settings/models/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/pid_settings/models/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1460 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/pid_settings/models/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.087232 core_linked_records_app-2.3.0/tests/components/pid_settings/watch/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/pid_settings/watch/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2765 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/pid_settings/watch/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.103301 core_linked_records_app-2.3.0/tests/components/pid_xpath/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/pid_xpath/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.139390 core_linked_records_app-2.3.0/tests/components/pid_xpath/admin_site/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/pid_xpath/admin_site/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      566 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/pid_xpath/admin_site/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.181995 core_linked_records_app-2.3.0/tests/components/pid_xpath/api/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/pid_xpath/api/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4208 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/pid_xpath/api/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.216184 core_linked_records_app-2.3.0/tests/components/pid_xpath/models/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/pid_xpath/models/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3121 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/pid_xpath/models/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.250423 core_linked_records_app-2.3.0/tests/menus/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/menus/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      553 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/menus/test_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4156 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/mocks.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.266520 core_linked_records_app-2.3.0/tests/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.286261 core_linked_records_app-2.3.0/tests/rest/blob/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/rest/blob/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.335153 core_linked_records_app-2.3.0/tests/rest/blob/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/rest/blob/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2639 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/rest/blob/views/test_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5112 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/rest/blob/views/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.351067 core_linked_records_app-2.3.0/tests/rest/pid/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/rest/pid/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.402748 core_linked_records_app-2.3.0/tests/rest/pid/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/rest/pid/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6123 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/rest/pid/views/test_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17555 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/rest/pid/views/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.429129 core_linked_records_app-2.3.0/tests/rest/pid_settings/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/rest/pid_settings/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.477747 core_linked_records_app-2.3.0/tests/rest/pid_settings/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/rest/pid_settings/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4244 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/rest/pid_settings/views/test_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5951 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/rest/pid_settings/views/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.493114 core_linked_records_app-2.3.0/tests/rest/pid_xpath/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/rest/pid_xpath/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.528400 core_linked_records_app-2.3.0/tests/rest/pid_xpath/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/rest/pid_xpath/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7569 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/rest/pid_xpath/views/test_permissions.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.551046 core_linked_records_app-2.3.0/tests/rest/providers/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/rest/providers/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.605512 core_linked_records_app-2.3.0/tests/rest/providers/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/rest/providers/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8187 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/rest/providers/views/test_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17141 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/rest/providers/views/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.638936 core_linked_records_app-2.3.0/tests/rest/query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/rest/query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1800 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/rest/query/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.652699 core_linked_records_app-2.3.0/tests/system/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/system/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.685107 core_linked_records_app-2.3.0/tests/system/api/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/system/api/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    20646 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/system/api/test_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2144 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/test_settings.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      458 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/test_urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.702196 core_linked_records_app-2.3.0/tests/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/utils/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.815261 core_linked_records_app-2.3.0/tests/utils/blob/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/utils/blob/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      421 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/utils/blob/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.852419 core_linked_records_app-2.3.0/tests/utils/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/utils/data/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      421 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/utils/data/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.888752 core_linked_records_app-2.3.0/tests/utils/dict/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/utils/dict/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4213 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/utils/dict/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.927013 core_linked_records_app-2.3.0/tests/utils/path/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/utils/path/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      378 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/utils/path/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.961397 core_linked_records_app-2.3.0/tests/utils/pid/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/utils/pid/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2298 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/utils/pid/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.980514 core_linked_records_app-2.3.0/tests/utils/providers/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/utils/providers/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:28.021821 core_linked_records_app-2.3.0/tests/utils/providers/handle_net/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/utils/providers/handle_net/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3952 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/utils/providers/handle_net/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:28.057372 core_linked_records_app-2.3.0/tests/utils/providers/local/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/utils/providers/local/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12238 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/utils/providers/local/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:28.092097 core_linked_records_app-2.3.0/tests/utils/query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/utils/query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9314 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/utils/query/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:28.122598 core_linked_records_app-2.3.0/tests/utils/xml/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/utils/xml/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1454 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/utils/xml/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:28.142178 core_linked_records_app-2.3.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:28.160730 core_linked_records_app-2.3.0/tests/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:22.000000 core_linked_records_app-2.3.0/tests/views/admin/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:28.204247 core_linked_records_app-2.3.0/tests/views/admin/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:22.000000 core_linked_records_app-2.3.0/tests/views/admin/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6799 2023-05-02 19:39:22.000000 core_linked_records_app-2.3.0/tests/views/admin/views/test_unit.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `core_linked_records_app-2.2.0/PKG-INFO` & `core_linked_records_app-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_linked_records_app
-Version: 2.2.0
+Version: 2.3.0
 Summary: Linked records for the core project
 Home-page: https://github.com/usnistgov/core_linked_records_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =======================
         core_linked_records_app
```

### Comparing `core_linked_records_app-2.2.0/README.rst` & `core_linked_records_app-2.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/core_linked_records_app/admin.py` & `core_linked_records_app-2.3.0/core_linked_records_app/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 )
 from core_linked_records_app.components.pid_xpath.models import PidXpath
 from core_linked_records_app.views.admin import views as admin_views
 from core_main_app.admin import core_admin_site
 
 admin_urls = [
     re_path(
-        r"^settings/$",
+        r"^pid/settings/$",
         staff_member_required(admin_views.PidSettingsView.as_view()),
         name="core_linked_records_app_admin_settings",
     ),
 ]
 
 admin.site.register(LocalId, CustomLocalIdAdmin)
 admin.site.register(PidSettings, CustomPidSettingsAdmin)
```

### Comparing `core_linked_records_app-2.2.0/core_linked_records_app/apps.py` & `core_linked_records_app-2.3.0/core_linked_records_app/apps.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/core_linked_records_app/components/blob/api.py` & `core_linked_records_app-2.3.0/core_linked_records_app/components/blob/api.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/core_linked_records_app/components/blob/watch.py` & `core_linked_records_app-2.3.0/core_linked_records_app/components/blob/watch.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 """ Signals to trigger after Blob save
 """
 import json
 from logging import getLogger
 
-from django.db.models.signals import post_save
+from django.db.models.signals import post_save, post_delete
 from django.urls import reverse
 
 from core_linked_records_app import settings
 from core_linked_records_app.components.blob import api as blob_api
 from core_linked_records_app.components.pid_settings import (
     api as pid_settings_api,
 )
+from core_linked_records_app.system import api as system_api
 from core_main_app.commons.exceptions import CoreError, DoesNotExist
 from core_main_app.components.blob.models import Blob
 from core_main_app.utils.requests_utils.requests_utils import send_post_request
 
 logger = getLogger(__name__)
 
 
 def init():
     """Connect to Blob object events."""
     post_save.connect(set_blob_pid, sender=Blob)
+    post_delete.connect(delete_blob_pid, sender=Blob)
 
 
-def set_blob_pid(sender, instance, **kwargs):
+def set_blob_pid(sender, instance: Blob, **kwargs):
     """set_blob_pid
 
     Args:
         sender:
         instance:
 
     Returns:
@@ -57,7 +59,26 @@
     except Exception as exc:
         error_message = (
             f"An error occurred while setting a PID for blob '{instance.pk}'"
         )
 
         logger.error("%s: %s", error_message, str(exc))
         raise CoreError(f"{error_message}.")
+
+
+def delete_blob_pid(sender, instance: Blob, **kwargs):
+    """Delete a PID assigned to a Blob
+
+    Args:
+        sender:
+        instance:
+        kwargs:
+    """
+    try:
+        system_api.delete_pid_for_blob(instance)
+    except Exception as exc:
+        logger.warning(
+            "Trying to delete PID for blob %d (%s) but an error occurred: %s",
+            instance.pk,
+            instance.filename,
+            str(exc),
+        )
```

### Comparing `core_linked_records_app-2.2.0/core_linked_records_app/components/data/api.py` & `core_linked_records_app-2.3.0/core_linked_records_app/components/data/api.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/core_linked_records_app/components/data/watch.py` & `core_linked_records_app-2.3.0/core_linked_records_app/components/data/watch.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """ Signals to trigger before Data save
 """
 import logging
 from os.path import join
 
-from django.db.models.signals import pre_save
+from django.db.models.signals import pre_save, post_delete
 
 from core_linked_records_app import settings
 from core_linked_records_app.components.pid_settings import (
     api as pid_settings_api,
 )
 from core_linked_records_app.system import api as system_api
 from core_linked_records_app.utils import data as data_utils
@@ -20,14 +20,15 @@
 
 logger = logging.getLogger(__name__)
 
 
 def init():
     """Connect to Data object events."""
     pre_save.connect(set_data_pid, sender=Data)
+    post_delete.connect(delete_data_pid, sender=Data)
 
 
 def set_data_pid(sender, instance, **kwargs):
     """Set the PID in the XML field specified in the settings. If the PID
     already exists and is valid, it is not reset.
 
     Params:
@@ -106,7 +107,25 @@
 
         error_message = (
             f"An error occurred while assigning PID to {data_definition}"
         )
 
         logger.error("%s: %s", error_message, str(exc))
         raise exceptions.CoreError(f"{error_message}.")
+
+
+def delete_data_pid(sender, instance, **kwargs):
+    """Delete a PID assigned to a Data
+
+    Args:
+        sender:
+        instance:
+        kwargs:
+    """
+    try:
+        system_api.delete_pid_for_data(instance)
+    except Exception as exc:
+        logger.warning(
+            "Trying to delete PID for data %d but an error occurred: %s",
+            instance.pk,
+            str(exc),
+        )
```

### Comparing `core_linked_records_app-2.2.0/core_linked_records_app/components/local_id/api.py` & `core_linked_records_app-2.3.0/core_linked_records_app/components/local_id/api.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/core_linked_records_app/components/local_id/models.py` & `core_linked_records_app-2.3.0/core_linked_records_app/components/local_id/models.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/core_linked_records_app/components/oai_record/api.py` & `core_linked_records_app-2.3.0/core_linked_records_app/components/oai_record/api.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/core_linked_records_app/components/pid_settings/api.py` & `core_linked_records_app-2.3.0/core_linked_records_app/components/pid_settings/api.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/core_linked_records_app/components/pid_settings/models.py` & `core_linked_records_app-2.3.0/core_linked_records_app/components/pid_settings/models.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/core_linked_records_app/components/pid_settings/watch.py` & `core_linked_records_app-2.3.0/core_linked_records_app/components/pid_settings/watch.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/core_linked_records_app/components/pid_xpath/api.py` & `core_linked_records_app-2.3.0/core_linked_records_app/components/pid_xpath/api.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/core_linked_records_app/components/pid_xpath/models.py` & `core_linked_records_app-2.3.0/core_linked_records_app/components/pid_xpath/models.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/core_linked_records_app/migrations/0001_initial.py` & `core_linked_records_app-2.3.0/core_linked_records_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/core_linked_records_app/rest/blob/views.py` & `core_linked_records_app-2.3.0/core_linked_records_app/rest/blob/views.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/core_linked_records_app/rest/data/renderers/data_html_user_renderer.py` & `core_linked_records_app-2.3.0/core_linked_records_app/rest/data/renderers/data_html_user_renderer.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/core_linked_records_app/rest/data/renderers/data_xml_renderer.py` & `core_linked_records_app-2.3.0/core_linked_records_app/rest/data/renderers/data_xml_renderer.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/core_linked_records_app/rest/pid/views.py` & `core_linked_records_app-2.3.0/core_linked_records_app/rest/pid/views.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,72 +1,81 @@
 """ Ajax views accessible by users.
 """
 import json
 from urllib.parse import urljoin
 
-from django.http import JsonResponse
 from django.urls import reverse
 from django.utils import timezone
 from rest_framework import status
+from rest_framework.response import Response
 from rest_framework.views import APIView
 
+from core_explore_common_app.commons.exceptions import ExploreRequestError
 from core_explore_common_app.components.query import api as query_api
+from core_explore_common_app.utils.oaipmh import oaipmh as oaipmh_utils
+from core_explore_common_app.utils.query import query as query_utils
 from core_explore_common_app.utils.protocols.oauth2 import (
     send_post_request as oauth2_post_request,
     send_get_request as oauth2_get_request,
 )
 from core_linked_records_app import settings
 from core_linked_records_app.components.blob import api as blob_api
 from core_linked_records_app.components.data import api as data_api
-from core_main_app.utils.requests_utils.requests_utils import (
-    send_get_request,
-)
+from core_linked_records_app.utils.query import execute_local_pid_query
+
+if (
+    "core_oaipmh_harvester_app" in settings.INSTALLED_APPS
+    and "core_explore_oaipmh_app" in settings.INSTALLED_APPS
+):  # Import OAI-PMH pid views if packages are present.
+    from core_linked_records_app.utils.query import (
+        execute_oaipmh_pid_query,
+    )
 
 
 class RetrieveDataPIDView(APIView):
     """Retrieve PIDs for a given data IDs."""
 
     def get(self, request):
         """get
 
         Args:
             request:
 
         Returns:
         """
         try:
-            if "data_id" in request.GET:
-                return JsonResponse(
+            if "data_id" in request.GET:  # Local data
+                return Response(
                     {
                         "pid": data_api.get_pid_for_data(
                             request.GET["data_id"], request
                         )
                     }
                 )
             if (
                 "core_oaipmh_harvester_app" in settings.INSTALLED_APPS
                 and "core_explore_oaipmh_app" in settings.INSTALLED_APPS
                 and "oai_data_id" in request.GET
-            ):
+            ):  # OAI-PMH data
                 from core_linked_records_app.components.oai_record import (
                     api as oai_record_api,
                 )
 
-                return JsonResponse(
+                return Response(
                     {
                         "pid": oai_record_api.get_pid_for_data(
                             request.GET["oai_data_id"], request
                         )
                     }
                 )
             if (
                 "core_federated_search_app" in settings.INSTALLED_APPS
                 and "fede_data_id" in request.GET
                 and "fede_origin" in request.GET
-            ):
+            ):  # Federated data
                 from core_federated_search_app.components.instance import (
                     api as instance_api,
                 )
 
                 fede_origin_keys = request.GET["fede_origin"].split("&")
                 instance_name = fede_origin_keys[1].split("=")[1]
                 instance = instance_api.get_by_name(instance_name)
@@ -76,25 +85,25 @@
                     f'{reverse_url}?data_id={request.GET["fede_data_id"]}'
                 )
 
                 data_response = oauth2_get_request(
                     urljoin(instance.endpoint, url_get_data),
                     instance.access_token,
                 )
-                return JsonResponse(json.loads(data_response.text))
+                return Response(json.loads(data_response.text))
 
-            return JsonResponse(
+            return Response(
                 {
                     "message": "Impossible to retrieve PID for data with the given "
                     "parameters"
                 },
                 status=status.HTTP_400_BAD_REQUEST,
             )
         except Exception as exc:
-            return JsonResponse(
+            return Response(
                 {
                     "message": f"An unexpected exception occurred while retrieving data "
                     f"PID: {str(exc)}"
                 },
                 status=status.HTTP_500_INTERNAL_SERVER_ERROR,
             )
 
@@ -117,53 +126,53 @@
                     "core_linked_records_provider_record",
                     kwargs={
                         "provider": settings.ID_PROVIDER_SYSTEM_NAME,
                         "record": "",
                     },
                 )
 
-                return JsonResponse(
+                return Response(
                     {
                         "pid": f"{settings.SERVER_URI}{sub_url}{blob_pid.record_name}"
                     }
                 )
             except Exception as exc:
-                return JsonResponse(
+                return Response(
                     {
                         "message": f"An unexpected exception occurred while retrieving "
                         f"blob PID: {str(exc)}"
                     },
                     status=status.HTTP_500_INTERNAL_SERVER_ERROR,
                 )
         else:
-            return JsonResponse(
+            return Response(
                 {"message": "Missing parameter 'blob_id'."},
                 status=status.HTTP_400_BAD_REQUEST,
             )
 
 
 class RetrieveListPIDView(APIView):
     """Retrieve PIDs for a given list of data IDs."""
 
     def post(self, request):
-        """get PIDs
+        """Retrieve PIDs
         Args:
             request:
 
         Returns:
 
         """
         try:
             # FIXME duplicated code with core_explore_common.utils.query.send
             query = query_api.get_by_id(
-                request.POST.get("query_id", None),
+                request.data.get("query_id", None),
                 request.user,
             )
             data_source = query.data_sources[
-                int(request.POST.get("data_source_index", 0))
+                int(request.data.get("data_source_index", 0))
             ]
 
             # Build serialized query to send to data source
             json_query = {
                 "query": query.content,
                 "templates": json.dumps(
                     [
@@ -172,54 +181,54 @@
                     ]
                 ),
                 "options": json.dumps(data_source["query_options"]),
                 "order_by_field": data_source["order_by_field"],
             }
 
             if (
-                "capabilities" in data_source.keys()
-                and "url_pid" not in data_source["capabilities"].keys()
-            ):
-                return JsonResponse(
-                    {"error": "The remote does not have PID capabilities."},
-                    status=status.HTTP_500_INTERNAL_SERVER_ERROR,
-                )
-
-            if data_source["authentication"]["auth_type"] == "session":
-                response = send_get_request(
-                    data_source["capabilities"]["url_pid"],
-                    json=json_query,
-                    cookies={
-                        "sessionid": request.session.session_key,
-                    },
-                )
-            elif data_source["authentication"]["auth_type"] == "oauth2":
+                data_source["authentication"]["auth_type"] == "session"
+            ):  # Local and OAI-PMH data sources
+                if query_utils.is_local_data_source(data_source):
+                    json_response = execute_local_pid_query(
+                        json_query, request
+                    )
+                elif oaipmh_utils.is_oai_data_source(data_source):
+
+                    json_response = execute_oaipmh_pid_query(
+                        json_query, request
+                    )
+                else:
+                    raise ExploreRequestError("Unknown data source type.")
+            elif (
+                data_source["authentication"]["auth_type"] == "oauth2"
+            ):  # Federated data sources
                 response = oauth2_post_request(
-                    data_source["capabilities"]["url_pid"],
+                    data_source["capabilities"]["query_pid"],
                     json_query,
                     data_source["authentication"]["params"]["access_token"],
                     session_time_zone=timezone.get_current_timezone(),
                 )
-            else:
-                raise Exception("Unknown authentication type.")
 
-            if response.status_code == 200:
-                return JsonResponse(
-                    {
-                        "pids": [
-                            pid for pid in response.json() if pid is not None
-                        ]
-                    },
-                    status=response.status_code,
+                if response.status_code == status.HTTP_200_OK:
+                    json_response = response.json()
+                else:
+                    return Response(
+                        {
+                            "error": f"Data source returned HTTP {response.status_code}."
+                        },
+                        status=status.HTTP_400_BAD_REQUEST,
+                    )
+            else:
+                return Response(
+                    {"error": "Unknown authentication type."},
+                    status=status.HTTP_400_BAD_REQUEST,
                 )
 
-            return JsonResponse(
-                {
-                    "error": f"Remote service answered with status code {response.status_code}."
-                },
-                status=response.status_code,
+            return Response(
+                {"pids": [pid for pid in json_response if pid is not None]},
+                status=status.HTTP_200_OK,
             )
         except Exception as exception:
-            return JsonResponse(
+            return Response(
                 {"error": str(exception)},
                 status=status.HTTP_500_INTERNAL_SERVER_ERROR,
             )
```

### Comparing `core_linked_records_app-2.2.0/core_linked_records_app/rest/pid_settings/serializers.py` & `core_linked_records_app-2.3.0/core_linked_records_app/rest/pid_settings/serializers.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/core_linked_records_app/rest/pid_settings/views.py` & `core_linked_records_app-2.3.0/core_linked_records_app/rest/pid_settings/views.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/core_linked_records_app/rest/pid_xpath/views.py` & `core_linked_records_app-2.3.0/core_linked_records_app/rest/pid_xpath/views.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/core_linked_records_app/rest/providers/views.py` & `core_linked_records_app-2.3.0/core_linked_records_app/rest/providers/views.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/core_linked_records_app/rest/urls.py` & `core_linked_records_app-2.3.0/core_linked_records_app/rest/urls.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,26 @@
 """ Url router for the core linked records app
 """
 from django.conf.urls import url
 
-from core_linked_records_app import settings
 from core_linked_records_app.rest.blob import views as blob_views
 from core_linked_records_app.rest.pid import views as pid_views
+from core_linked_records_app.rest.query import views as query_views
 from core_linked_records_app.rest.pid_settings import views as settings_views
 from core_linked_records_app.rest.pid_xpath import views as xpath_views
 from core_linked_records_app.rest.providers import views as providers_views
-from core_linked_records_app.rest.query import views as query_views
 
 urlpatterns = [
     url(
-        r"^query/local$",
-        query_views.ExecuteLocalPIDQueryView.as_view(),
-        name="core_linked_records_app_query_local",
+        r"^query$",
+        query_views.RetrieveQueryPidListView.as_view(),
+        name="core_linked_records_app_query_pid",
     ),
 ]
 
-if (
-    "core_oaipmh_harvester_app" in settings.INSTALLED_APPS
-    and "core_explore_oaipmh_app" in settings.INSTALLED_APPS
-):
-    urlpatterns.append(
-        url(
-            r"^query/oaipmh$",
-            query_views.ExecuteOaiPmhPIDQueryView.as_view(),
-            name="core_linked_records_app_query_oaipmh",
-        ),
-    )
-
 urlpatterns += [
     url(
         r"^settings$",
         settings_views.PidSettingsView.as_view(),
         name="core_linked_records_app_settings",
     ),
     url(
```

### Comparing `core_linked_records_app-2.2.0/core_linked_records_app/settings.py` & `core_linked_records_app-2.3.0/core_linked_records_app/settings.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/core_linked_records_app/static/core_linked_records_app/admin/js/pid_settings/auto_set_pid.js` & `core_linked_records_app-2.3.0/core_linked_records_app/static/core_linked_records_app/admin/js/pid_settings/auto_set_pid.js`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/common_list.js` & `core_linked_records_app-2.3.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/common_list.js`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/data_detail.js` & `core_linked_records_app-2.3.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/data_detail.js`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/explore.js` & `core_linked_records_app-2.3.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/explore.js`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/core_linked_records_app/system/api.py` & `core_linked_records_app-2.3.0/core_linked_records_app/system/api.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,20 +2,25 @@
 """
 import logging
 
 from django.conf import settings as conf_settings
 from rest_framework import status
 
 from core_linked_records_app import settings
+from core_linked_records_app.components.local_id.models import LocalId
 from core_linked_records_app.components.pid_xpath.models import PidXpath
+from core_linked_records_app.components.local_id import api as local_id_api
 from core_linked_records_app.utils.dict import get_value_from_dot_notation
+from core_linked_records_app.utils.path import get_api_path_from_object
 from core_linked_records_app.utils.providers import ProviderManager
 from core_main_app.commons.exceptions import DoesNotExist, ApiError
+from core_main_app.components.blob.models import Blob
 from core_main_app.components.data.models import Data
 from core_main_app.utils.query.mongo.prepare import sanitize_value
+from core_main_app.utils import xml as xml_utils
 
 logger = logging.getLogger(__name__)
 
 
 def is_pid_defined_for_data(pid, document_id):
     """Determine if a given PID match the document ID provided.
 
@@ -119,35 +124,14 @@
         raise DoesNotExist("PID is not attached to any data.")
     if query_result_length != 1:
         raise ApiError("PID must be unique.")
 
     return query_result[0]
 
 
-def get_pid_for_data(data_id):
-    """Retrieve PID matching the document ID provided.
-
-    Args:
-        data_id:
-
-    Returns:
-    """
-    # Retrieve the document passed as input and extra the PID field.
-    data = Data.get_by_id(data_id)
-
-    # Return PID value from the document and the PID_XPATH
-    pid_xpath_object = get_pid_xpath_by_template(data.template)
-    pid_xpath = pid_xpath_object.xpath
-
-    return get_value_from_dot_notation(
-        data.get_dict_content(),
-        pid_xpath,
-    )
-
-
 def get_pid_xpath_by_template(template):
     """Retrieve XPath associated with a specific template ID
 
     Args:
         template: Template object
 
     Returns:
@@ -157,35 +141,90 @@
 
     if pid_xpath_object is None:
         return PidXpath(template=template, xpath=settings.PID_XPATH)
 
     return pid_xpath_object
 
 
-def delete_pid_for_data(data):
+def delete_pid_from_record_name(record_name: str):
+    """Delete a PID from the provider using the record name as stored in the
+    LocalId table.
+
+    Args:
+        record_name: str - Formatted as prefix/record.
+    """
+    # Delete the given LocalID fron the default PID provider.
+    provider = ProviderManager().get()
+    previous_pid_delete_response = provider.delete(record_name)
+
+    # Log any error that happened during PID deletion.
+    if previous_pid_delete_response.status_code != status.HTTP_200_OK:
+        error_message = (
+            f"Deletion of LocalID {record_name} from provider {ProviderManager().provider_name} "
+            f"returned {previous_pid_delete_response.status_code}"
+        )
+        logger.error(error_message)
+        raise ApiError(error_message)
+
+
+def delete_pid_for_data(data: Data):
     """Deletes the PID assigned to the data passed in parameter. If no PID has
     been assigned, the function simply exits.
 
     Args:
-        data:
+        data: Data - The data for which the PID needs to be deleted.
     """
-    previous_pid = get_pid_for_data(data.pk)
+    # Retrieve the PID_XPATH associated with the data template.
+    pid_xpath_object = get_pid_xpath_by_template(data.template)
+    pid_xpath = pid_xpath_object.xpath
+
+    # Retrieve the data dict content to search for the PID_XPATH using dot notation.
+    try:  # Try to retrieve the dict content using data model
+        dict_content = data.get_dict_content()
+    except Exception:  # noqa
+        # Retrieving the dict content is not possible, convert the xml to dict
+        try:
+            dict_content = xml_utils.raw_xml_to_dict(data.xml_content)
+        except Exception as exc:  # Converting the xml to dict is not possible either
+            raise ApiError(
+                f"Impossible to retrieve the dict content for the data: {str(exc)}"
+            )
 
-    if not previous_pid:  # If there is no previous PID assigned.
+    # Return PID value from the document and the PID_XPATH
+    current_pid = get_value_from_dot_notation(
+        dict_content,
+        pid_xpath,
+    )
+
+    if not current_pid:  # If there is no previous PID assigned.
         logger.info("No PID assigned to the data %s", str(data.pk))
         return
 
-    provider = ProviderManager().get()  # Returns the default provider.
-
     # From the PID url (e.g. https://pid-system.org/prefix/record), retrieve
     # only the prefix and record (e.g. prefix/record) stored in DB.
-    pid_internal_name = "/".join(previous_pid.split("/")[-2:])
+    pid_internal_name = "/".join(current_pid.split("/")[-2:])
 
-    previous_pid_delete_response = provider.delete(pid_internal_name)
+    # Delete the PID using the internal name.
+    delete_pid_from_record_name(pid_internal_name)
 
-    # Log any error that happen during PID deletion.
-    if previous_pid_delete_response.status_code != status.HTTP_200_OK:
-        logger.warning(
-            "Deletion of PID %s returned %s",
-            previous_pid,
-            previous_pid_delete_response.status_code,
+
+def delete_pid_for_blob(blob: Blob):
+    """Deletes the PID assigned to the blob passed in parameter. If no PID has
+    been assigned, the function simply exits.
+
+    Args:
+        blob: Blob - The blob for which the PID needs to be deleted.
+    """
+    try:
+        local_id_obj: LocalId = local_id_api.get_by_class_and_id(
+            get_api_path_from_object(Blob()), blob.pk
         )
+
+        # Delete the PID using the internal name.
+        delete_pid_from_record_name(local_id_obj.record_name)
+    except DoesNotExist:  # If there is no previous PID assigned.
+        logger.info(
+            "No PID assigned to the blob %s (%s). Skipping deletion.",
+            str(blob.pk),
+            blob.filename,
+        )
+        return
```

### Comparing `core_linked_records_app-2.2.0/core_linked_records_app/templates/core_linked_records_app/admin/pid_settings/box.html` & `core_linked_records_app-2.3.0/core_linked_records_app/templates/core_linked_records_app/admin/pid_settings/box.html`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/core_linked_records_app/utils/blob.py` & `core_linked_records_app-2.3.0/core_linked_records_app/utils/blob.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/core_linked_records_app/utils/data.py` & `core_linked_records_app-2.3.0/core_linked_records_app/utils/data.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/core_linked_records_app/utils/dict.py` & `core_linked_records_app-2.3.0/core_linked_records_app/utils/dict.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/core_linked_records_app/utils/path.py` & `core_linked_records_app-2.3.0/core_linked_records_app/utils/path.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/core_linked_records_app/utils/pid.py` & `core_linked_records_app-2.3.0/core_linked_records_app/utils/pid.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/core_linked_records_app/utils/providers/__init__.py` & `core_linked_records_app-2.3.0/core_linked_records_app/utils/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/core_linked_records_app/utils/providers/handle_net.py` & `core_linked_records_app-2.3.0/core_linked_records_app/utils/providers/handle_net.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/core_linked_records_app/utils/providers/local.py` & `core_linked_records_app-2.3.0/core_linked_records_app/utils/providers/local.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/core_linked_records_app/utils/xml.py` & `core_linked_records_app-2.3.0/core_linked_records_app/utils/xml.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/core_linked_records_app/views/admin/views.py` & `core_linked_records_app-2.3.0/core_linked_records_app/views/admin/views.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/core_linked_records_app.egg-info/PKG-INFO` & `core_linked_records_app-2.3.0/core_linked_records_app.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-linked-records-app
-Version: 2.2.0
+Version: 2.3.0
 Summary: Linked records for the core project
 Home-page: https://github.com/usnistgov/core_linked_records_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =======================
         core_linked_records_app
```

### Comparing `core_linked_records_app-2.2.0/core_linked_records_app.egg-info/SOURCES.txt` & `core_linked_records_app-2.3.0/core_linked_records_app.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.md
 MANIFEST.in
 README.rst
 pyproject.toml
 requirements.core.txt
 requirements.txt
 setup.py
 core_linked_records_app/__init__.py
@@ -34,14 +35,15 @@
 core_linked_records_app/components/pid_settings/models.py
 core_linked_records_app/components/pid_settings/watch.py
 core_linked_records_app/components/pid_xpath/__init__.py
 core_linked_records_app/components/pid_xpath/admin_site.py
 core_linked_records_app/components/pid_xpath/api.py
 core_linked_records_app/components/pid_xpath/models.py
 core_linked_records_app/migrations/0001_initial.py
+core_linked_records_app/migrations/0002_alter_pidxpath_xpath.py
 core_linked_records_app/migrations/__init__.py
 core_linked_records_app/rest/__init__.py
 core_linked_records_app/rest/urls.py
 core_linked_records_app/rest/blob/__init__.py
 core_linked_records_app/rest/blob/views.py
 core_linked_records_app/rest/data/__init__.py
 core_linked_records_app/rest/data/renderers/__init__.py
@@ -84,14 +86,15 @@
 core_linked_records_app/templates/core_linked_records_app/user/sharing/explore/modal.html
 core_linked_records_app/utils/__init__.py
 core_linked_records_app/utils/blob.py
 core_linked_records_app/utils/data.py
 core_linked_records_app/utils/dict.py
 core_linked_records_app/utils/path.py
 core_linked_records_app/utils/pid.py
+core_linked_records_app/utils/query.py
 core_linked_records_app/utils/xml.py
 core_linked_records_app/utils/providers/__init__.py
 core_linked_records_app/utils/providers/handle_net.py
 core_linked_records_app/utils/providers/local.py
 core_linked_records_app/views/__init__.py
 core_linked_records_app/views/admin/__init__.py
 core_linked_records_app/views/admin/views.py
@@ -107,14 +110,16 @@
 tests/components/blob/watch/test_unit.py
 tests/components/data/__init__.py
 tests/components/data/api/__init__.py
 tests/components/data/api/test_unit.py
 tests/components/data/watch/__init__.py
 tests/components/data/watch/test_unit.py
 tests/components/local_id/__init__.py
+tests/components/local_id/admin_site/__init__.py
+tests/components/local_id/admin_site/test_unit.py
 tests/components/local_id/api/__init__.py
 tests/components/local_id/api/test_unit.py
 tests/components/local_id/models/__init__.py
 tests/components/local_id/models/test_unit.py
 tests/components/oai_record/__init__.py
 tests/components/oai_record/api/__init__.py
 tests/components/oai_record/api/test_unit.py
@@ -151,17 +156,15 @@
 tests/rest/pid_xpath/views/__init__.py
 tests/rest/pid_xpath/views/test_permissions.py
 tests/rest/providers/__init__.py
 tests/rest/providers/views/__init__.py
 tests/rest/providers/views/test_permissions.py
 tests/rest/providers/views/test_unit.py
 tests/rest/query/__init__.py
-tests/rest/query/views/__init__.py
-tests/rest/query/views/test_permissions.py
-tests/rest/query/views/test_unit.py
+tests/rest/query/test_unit.py
 tests/system/__init__.py
 tests/system/api/__init__.py
 tests/system/api/test_unit.py
 tests/utils/__init__.py
 tests/utils/blob/__init__.py
 tests/utils/blob/test_unit.py
 tests/utils/data/__init__.py
@@ -173,13 +176,15 @@
 tests/utils/pid/__init__.py
 tests/utils/pid/test_unit.py
 tests/utils/providers/__init__.py
 tests/utils/providers/handle_net/__init__.py
 tests/utils/providers/handle_net/test_unit.py
 tests/utils/providers/local/__init__.py
 tests/utils/providers/local/test_unit.py
+tests/utils/query/__init__.py
+tests/utils/query/test_unit.py
 tests/utils/xml/__init__.py
 tests/utils/xml/test_unit.py
 tests/views/__init__.py
 tests/views/admin/__init__.py
 tests/views/admin/views/__init__.py
 tests/views/admin/views/test_unit.py
```

### Comparing `core_linked_records_app-2.2.0/setup.py` & `core_linked_records_app-2.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_linked_records_app",
-    version="2.2.0",
+    version="2.3.0",
     description="Linked records for the core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_linked_records_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_linked_records_app-2.2.0/tests/components/blob/api/test_unit.py` & `core_linked_records_app-2.3.0/tests/components/blob/api/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/tests/components/blob/watch/test_unit.py` & `core_linked_records_app-2.3.0/tests/components/blob/watch/test_unit.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """ Unit tests for core_linked_records_app.components.blob.watch
 """
 import json
 from unittest import TestCase
 from unittest.mock import patch
 
 from core_linked_records_app.components.blob import api as blob_api
+from core_linked_records_app.system import api as system_api
 from core_linked_records_app.components.blob import watch as blob_watch
 from core_linked_records_app.components.pid_settings import (
     api as pid_settings_api,
 )
 from core_main_app.commons import exceptions
 from tests import mocks
 
@@ -240,7 +241,35 @@
         """test_pid_not_created_if_already_assigned"""
 
         mock_get_pid_for_blob.return_value = "mock_pid"
         mock_settings_get.return_value = mocks.MockPidSettings()
 
         blob_watch.set_blob_pid(None, self.mock_document)
         self.assertFalse(mock_set_pid_for_blob.called)
+
+
+class TestDeleteBlobPid(TestCase):
+    """Unit tests for detele_blob_pid function."""
+
+    def setUp(self) -> None:
+        """setUp"""
+        self.mock_blob = mocks.MockDocument()
+
+    @patch.object(system_api, "delete_pid_for_blob")
+    def test_delete_pid_for_blob_is_called(self, mock_delete_pid_for_blob):
+        """test_delete_pid_for_blob_is_called"""
+        blob_watch.delete_blob_pid(None, self.mock_blob)
+
+        mock_delete_pid_for_blob.assert_called_with(self.mock_blob)
+
+    @patch.object(blob_watch, "logger")
+    @patch.object(system_api, "delete_pid_for_blob")
+    def test_delete_pid_for_blob_error_raise_warning(
+        self, mock_delete_pid_for_blob, mock_logger
+    ):
+        """test_delete_pid_for_blob_error_raise_warning"""
+        mock_delete_pid_for_blob.side_effect = Exception(
+            "mock_delete_pid_for_blob_exception"
+        )
+        blob_watch.delete_blob_pid(None, self.mock_blob)
+
+        mock_logger.warning.assert_called()
```

### Comparing `core_linked_records_app-2.2.0/tests/components/data/api/test_unit.py` & `core_linked_records_app-2.3.0/tests/components/data/api/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/tests/components/data/watch/test_unit.py` & `core_linked_records_app-2.3.0/tests/components/data/watch/test_unit.py`

 * *Files 2% similar despite different names*

```diff
@@ -465,7 +465,35 @@
         mock_provider_manager_get.return_value = mocks.MockProviderManager()
         mock_is_pid_defined.return_value = True
         mock_is_pid_defined_for_data.return_value = True
         mock_register_pid_for_data_id.return_value = "mock_pid_value"
         mock_set_pid_value_for_data.return_value = None
 
         self.assertIsNone(data_watch.set_data_pid(**self.mock_kwargs))
+
+
+class TestDeleteDataPid(TestCase):
+    """Unit tests for detele_data_pid function."""
+
+    def setUp(self) -> None:
+        """setUp"""
+        self.mock_data = mocks.MockDocument()
+
+    @patch.object(system_api, "delete_pid_for_data")
+    def test_delete_pid_for_data_is_called(self, mock_delete_pid_for_data):
+        """test_delete_pid_for_data_is_called"""
+        data_watch.delete_data_pid(None, self.mock_data)
+
+        mock_delete_pid_for_data.assert_called_with(self.mock_data)
+
+    @patch.object(data_watch, "logger")
+    @patch.object(system_api, "delete_pid_for_data")
+    def test_delete_pid_for_data_error_raise_warning(
+        self, mock_delete_pid_for_data, mock_logger
+    ):
+        """test_delete_pid_for_data_error_raise_warning"""
+        mock_delete_pid_for_data.side_effect = Exception(
+            "mock_delete_pid_for_data_exception"
+        )
+        data_watch.delete_data_pid(None, self.mock_data)
+
+        mock_logger.warning.assert_called()
```

### Comparing `core_linked_records_app-2.2.0/tests/components/local_id/api/test_unit.py` & `core_linked_records_app-2.3.0/tests/components/local_id/api/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/tests/components/local_id/models/test_unit.py` & `core_linked_records_app-2.3.0/tests/components/local_id/models/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/tests/components/oai_record/api/test_unit.py` & `core_linked_records_app-2.3.0/tests/components/oai_record/api/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/tests/components/pid_settings/api/test_unit.py` & `core_linked_records_app-2.3.0/tests/components/pid_settings/api/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/tests/components/pid_settings/models/test_unit.py` & `core_linked_records_app-2.3.0/tests/components/pid_settings/models/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/tests/components/pid_settings/watch/test_unit.py` & `core_linked_records_app-2.3.0/tests/components/pid_settings/watch/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/tests/components/pid_xpath/admin_site/test_unit.py` & `core_linked_records_app-2.3.0/tests/components/pid_xpath/admin_site/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/tests/components/pid_xpath/api/test_unit.py` & `core_linked_records_app-2.3.0/tests/components/pid_xpath/api/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/tests/components/pid_xpath/models/test_unit.py` & `core_linked_records_app-2.3.0/tests/components/pid_xpath/models/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/tests/menus/test_unit.py` & `core_linked_records_app-2.3.0/tests/menus/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/tests/mocks.py` & `core_linked_records_app-2.3.0/tests/mocks.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,15 @@
     order_by_field = ""
     capabilities = {}
 
 
 class MockAuthentication(Mock):
     """Mock Authentication"""
 
-    type = ""
+    auth_type = ""
 
 
 class MockSerializer(Mock):
     """Mock Serializer"""
 
     data = {}
     is_valid_exc = None
```

### Comparing `core_linked_records_app-2.2.0/tests/rest/blob/views/test_permissions.py` & `core_linked_records_app-2.3.0/tests/rest/blob/views/test_permissions.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/tests/rest/blob/views/test_unit.py` & `core_linked_records_app-2.3.0/tests/rest/blob/views/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/tests/rest/pid/views/test_permissions.py` & `core_linked_records_app-2.3.0/tests/rest/pid/views/test_permissions.py`

 * *Files 6% similar despite different names*

```diff
@@ -121,68 +121,66 @@
         self.mock_data_source = dict(
             query_options={},
             order_by_field="",
             authentication=dict(
                 auth_type="oauth2",
                 params={"access_token": "mock_access_token"},
             ),
-            capabilities={"url_pid": True},
+            capabilities={"query_pid": "mock_url_pid_list"},
         )
 
-    def send_post_request(
-        self, mock_query_get_by_id, mock_send_get_request, user
-    ):
+    def send_oauth_request(self, mock_query_get_by_id, mock_request, user):
         """send_post_request"""
 
         mock_query_get_by_id.return_value = mocks.MockQuery(
             data_sources=[self.mock_data_source]
         )
-        mock_send_get_request.return_value = mocks.MockResponse(
-            json_data=[None]
+        mock_request.return_value = mocks.MockResponse(
+            json_data={"pids": ["mock_pid"]}
         )
 
         return RequestMock.do_request_post(
             pid_views.RetrieveListPIDView.as_view(),
             user,
             data={"query_id": "mock_query_id", "data_source_index": "0"},
             content_type=None,
         )
 
     @patch.object(pid_views, "oauth2_post_request")
     @patch.object(query_api, "get_by_id")
     def test_anonymous_returns_200(
-        self, mock_query_get_by_id, mock_send_get_request
+        self, mock_query_get_by_id, mock_oauth2_post_request
     ):
         """test_anonymous_returns_200"""
 
-        response = self.send_post_request(
-            mock_query_get_by_id, mock_send_get_request, None
+        response = self.send_oauth_request(
+            mock_query_get_by_id, mock_oauth2_post_request, None
         )
         self.assertEqual(response.status_code, status.HTTP_200_OK)
 
     @patch.object(pid_views, "oauth2_post_request")
     @patch.object(query_api, "get_by_id")
     def test_authenticated_returns_200(
-        self, mock_query_get_by_id, mock_send_get_request
+        self, mock_query_get_by_id, mock_oauth2_post_request
     ):
         """test_authenticated_returns_200"""
 
         mock_user = create_mock_user("1")
 
-        response = self.send_post_request(
-            mock_query_get_by_id, mock_send_get_request, mock_user
+        response = self.send_oauth_request(
+            mock_query_get_by_id, mock_oauth2_post_request, mock_user
         )
         self.assertEqual(response.status_code, status.HTTP_200_OK)
 
     @patch.object(pid_views, "oauth2_post_request")
     @patch.object(query_api, "get_by_id")
     def test_staff_returns_200(
-        self, mock_query_get_by_id, mock_send_get_request
+        self, mock_query_get_by_id, mock_oauth2_post_request
     ):
         """test_staff_returns_200"""
 
         mock_user = create_mock_user("1", is_staff=True)
 
-        response = self.send_post_request(
-            mock_query_get_by_id, mock_send_get_request, mock_user
+        response = self.send_oauth_request(
+            mock_query_get_by_id, mock_oauth2_post_request, mock_user
         )
         self.assertEqual(response.status_code, status.HTTP_200_OK)
```

### Comparing `core_linked_records_app-2.2.0/tests/rest/pid/views/test_unit.py` & `core_linked_records_app-2.3.0/tests/rest/pid/views/test_unit.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 """ Unit tests for core_linked_records_app.rest.pid.views
 """
 import json
 from unittest import TestCase
 from unittest.mock import patch
 
 from core_explore_common_app.components.query import api as query_api
+from core_explore_common_app.utils.oaipmh import oaipmh as oaipmh_utils
+from core_explore_common_app.utils.query import query as query_utils
 from core_federated_search_app.components.instance import (
     api as instance_api,
 )
 from core_linked_records_app.components.blob import api as blob_api
 from core_linked_records_app.components.data import api as data_api
+from core_linked_records_app.components.oai_record import (
+    api as oai_record_api,
+)
 from core_linked_records_app.rest.pid import views as pid_views
 from tests import mocks
 
 
 class TestRetrieveDataPidGet(TestCase):
     """Test Retrieve Data Pid Get"""
 
@@ -45,20 +50,39 @@
         mock_get_pid_for_data.return_value = "mock_data_id"
 
         test_view = pid_views.RetrieveDataPIDView()
         response = test_view.get(self.mock_request)
 
         self.assertEqual(response.status_code, 200)
 
-    # FIXME cannot import oai_pmh_harvester in INSTALLED_APPS
-    # def test_oai_record_api_get_pid_for_data_fails_returns_500(self):
-    #     pass
-    #
-    # def test_oai_record_api_success_returns_200(self):
-    #     pass
+    @patch.object(oai_record_api, "get_pid_for_data")
+    def test_oai_record_api_get_pid_for_data_fails_returns_500(
+        self, mock_get_pid_for_data
+    ):
+        """test_oai_record_api_get_pid_for_data_fails_returns_500"""
+        self.mock_request.GET["oai_data_id"] = "mock_data_id"
+        mock_get_pid_for_data.side_effect = Exception(
+            "mock_get_pid_for_data_exception"
+        )
+
+        test_view = pid_views.RetrieveDataPIDView()
+        response = test_view.get(self.mock_request)
+
+        self.assertEqual(response.status_code, 500)
+
+    @patch.object(oai_record_api, "get_pid_for_data")
+    def test_oai_record_api_success_returns_200(self, mock_get_pid_for_data):
+        """test_oai_record_api_success_returns_200"""
+        self.mock_request.GET["oai_data_id"] = "mock_data_id"
+        mock_get_pid_for_data.return_value = "mock_data_id"
+
+        test_view = pid_views.RetrieveDataPIDView()
+        response = test_view.get(self.mock_request)
+
+        self.assertEqual(response.status_code, 200)
 
     @patch.object(instance_api, "get_by_name")
     def test_instance_api_get_by_name_fails_returns_500(
         self, mock_get_by_name
     ):
         """test_instance_api_get_by_name_fails_returns_500"""
 
@@ -161,105 +185,266 @@
 
 
 class TestRetrieveListPidPost(TestCase):
     """Test Retrieve List Pid Post"""
 
     def setUp(self) -> None:
         self.mock_request = mocks.MockRequest(
-            POST={"query_id": "mock_query_id"}
+            data={"query_id": "mock_query_id"}
         )
 
     @patch.object(query_api, "get_by_id")
     def test_get_by_id_fails_returns_500(self, mock_get_by_id):
         """test_get_by_id_fails_returns_500"""
 
         mock_get_by_id.side_effect = Exception("mock_get_by_id_exception")
 
         test_view = pid_views.RetrieveListPIDView()
         response = test_view.post(self.mock_request)
 
         self.assertEqual(response.status_code, 500)
 
     @patch.object(query_api, "get_by_id")
-    def test_data_source_no_pid_url_capabilities_returns_500(
-        self, mock_get_by_id
-    ):
-        """test_data_source_no_pid_url_capabilities_returns_500"""
+    def test_data_source_invalid_returns_500(self, mock_get_by_id):
+        """test_data_source_invalid_returns_500"""
+        mock_get_by_id.return_value = mocks.MockQuery(data_sources=[])
+
+        test_view = pid_views.RetrieveListPIDView()
+        response = test_view.post(self.mock_request)
+
+        self.assertEqual(response.status_code, 500)
+
+    @patch.object(query_api, "get_by_id")
+    def test_unknown_datasource_authtype_returns_400(self, mock_get_by_id):
+        """test_unknown_auth_returns_500"""
+
+        mock_get_by_id.return_value = mocks.MockQuery(
+            data_sources=[
+                dict(
+                    query_options={},
+                    order_by_field="",
+                    capabilities={},
+                    authentication=dict(
+                        auth_type="invalid_auth_type",
+                    ),
+                )
+            ]
+        )
+
+        test_view = pid_views.RetrieveListPIDView()
+        response = test_view.post(self.mock_request)
+
+        self.assertEqual(response.status_code, 400)
+
+    @patch.object(query_api, "get_by_id")
+    def test_invalid_datasource_auth_type_returns_500(self, mock_get_by_id):
+        """test_unknown_auth_returns_500"""
 
         mock_get_by_id.return_value = mocks.MockQuery(
-            data_sources=[mocks.MockDataSource()]
+            data_sources=[
+                dict(
+                    query_options={},
+                    order_by_field="",
+                    capabilities={},
+                    authentication={},
+                )
+            ]
         )
 
         test_view = pid_views.RetrieveListPIDView()
         response = test_view.post(self.mock_request)
 
         self.assertEqual(response.status_code, 500)
 
-    @patch.object(pid_views, "send_get_request")
+    @patch.object(oaipmh_utils, "is_oai_data_source")
+    @patch.object(query_utils, "is_local_data_source")
     @patch.object(query_api, "get_by_id")
-    def test_send_get_request_fails_returns_500(
-        self, mock_get_by_id, mock_send_get_request
+    def test_invalid_session_datasource_returns_500(
+        self,
+        mock_get_by_id,
+        mock_is_local_data_source,
+        mock_is_oai_data_source,
     ):
-        """test_send_get_request_fails_returns_500"""
-
         mock_get_by_id.return_value = mocks.MockQuery(
             data_sources=[
-                mocks.MockDataSource(
-                    capabilities={"url_pid": "mock_url_pid"},
-                    authentication=mocks.MockAuthentication(type="session"),
+                dict(
+                    query_options={},
+                    order_by_field="",
+                    capabilities={},
+                    authentication=dict(
+                        auth_type="session",
+                    ),
                 )
             ]
         )
-        mock_send_get_request.side_effect = Exception(
-            "mock_send_get_request_exception"
-        )
+        mock_is_local_data_source.return_value = False
+        mock_is_oai_data_source.return_value = False
 
         test_view = pid_views.RetrieveListPIDView()
         response = test_view.post(self.mock_request)
 
         self.assertEqual(response.status_code, 500)
 
-    @patch.object(pid_views, "oauth2_post_request")
+    @patch.object(pid_views, "execute_local_pid_query")
+    @patch.object(oaipmh_utils, "is_oai_data_source")
+    @patch.object(query_utils, "is_local_data_source")
     @patch.object(query_api, "get_by_id")
-    def test_oauth2_post_request_fails_returns_500(
-        self, mock_get_by_id, mock_oauth2_post_request
+    def test_local_datasource_returns_200(
+        self,
+        mock_get_by_id,
+        mock_is_local_data_source,
+        mock_is_oai_data_source,
+        mock_execute_local_pid_query,
     ):
-        """test_oauth2_post_request_fails_returns_500"""
+        mock_get_by_id.return_value = mocks.MockQuery(
+            data_sources=[
+                dict(
+                    query_options={},
+                    order_by_field="",
+                    capabilities={},
+                    authentication=dict(
+                        auth_type="session",
+                    ),
+                )
+            ]
+        )
+        mock_is_local_data_source.return_value = True
+        mock_is_oai_data_source.return_value = False
+        mock_execute_local_pid_query.return_value = []
 
+        test_view = pid_views.RetrieveListPIDView()
+        response = test_view.post(self.mock_request)
+
+        self.assertEqual(response.status_code, 200)
+
+    @patch.object(pid_views, "execute_local_pid_query")
+    @patch.object(oaipmh_utils, "is_oai_data_source")
+    @patch.object(query_utils, "is_local_data_source")
+    @patch.object(query_api, "get_by_id")
+    def test_local_datasource_returns_local_pid_query(
+        self,
+        mock_get_by_id,
+        mock_is_local_data_source,
+        mock_is_oai_data_source,
+        mock_execute_local_pid_query,
+    ):
         mock_get_by_id.return_value = mocks.MockQuery(
             data_sources=[
-                mocks.MockDataSource(
-                    capabilities={"url_pid": "mock_url_pid"},
-                    authentication=mocks.MockAuthentication(
-                        type="oauth2",
-                        params={"access_token": "mock_access_token"},
+                dict(
+                    query_options={},
+                    order_by_field="",
+                    capabilities={},
+                    authentication=dict(
+                        auth_type="session",
                     ),
                 )
             ]
         )
-        mock_oauth2_post_request.side_effect = Exception(
-            "mock_oauth2_post_request_exception"
+        mock_is_local_data_source.return_value = True
+        mock_is_oai_data_source.return_value = False
+
+        expected_result = ["mock_pid" for _ in range(5)]
+        mock_execute_local_pid_query.return_value = expected_result
+
+        test_view = pid_views.RetrieveListPIDView()
+        response = test_view.post(self.mock_request)
+        result = response.data["pids"]
+
+        self.assertEqual(result, expected_result)
+
+    @patch.object(pid_views, "execute_oaipmh_pid_query")
+    @patch.object(oaipmh_utils, "is_oai_data_source")
+    @patch.object(query_utils, "is_local_data_source")
+    @patch.object(query_api, "get_by_id")
+    def test_oaipmh_datasource_returns_200(
+        self,
+        mock_get_by_id,
+        mock_is_local_data_source,
+        mock_is_oai_data_source,
+        mock_execute_oaipmh_pid_query,
+    ):
+        mock_get_by_id.return_value = mocks.MockQuery(
+            data_sources=[
+                dict(
+                    query_options={},
+                    order_by_field="",
+                    capabilities={},
+                    authentication=dict(
+                        auth_type="session",
+                    ),
+                )
+            ]
         )
+        mock_is_local_data_source.return_value = False
+        mock_is_oai_data_source.return_value = True
+        mock_execute_oaipmh_pid_query.return_value = []
 
         test_view = pid_views.RetrieveListPIDView()
         response = test_view.post(self.mock_request)
 
-        self.assertEqual(response.status_code, 500)
+        self.assertEqual(response.status_code, 200)
 
+    @patch.object(pid_views, "execute_oaipmh_pid_query")
+    @patch.object(oaipmh_utils, "is_oai_data_source")
+    @patch.object(query_utils, "is_local_data_source")
     @patch.object(query_api, "get_by_id")
-    def test_unknown_auth_returns_500(self, mock_get_by_id):
-        """test_unknown_auth_returns_500"""
+    def test_oaipmh_datasource_returns_oaipmh_pid_query(
+        self,
+        mock_get_by_id,
+        mock_is_local_data_source,
+        mock_is_oai_data_source,
+        mock_execute_oaipmh_pid_query,
+    ):
+        mock_get_by_id.return_value = mocks.MockQuery(
+            data_sources=[
+                dict(
+                    query_options={},
+                    order_by_field="",
+                    capabilities={},
+                    authentication=dict(
+                        auth_type="session",
+                    ),
+                )
+            ]
+        )
+        mock_is_local_data_source.return_value = False
+        mock_is_oai_data_source.return_value = True
+        expected_result = ["mock_pid" for _ in range(5)]
+        mock_execute_oaipmh_pid_query.return_value = expected_result
+
+        test_view = pid_views.RetrieveListPIDView()
+        response = test_view.post(self.mock_request)
+        result = response.data["pids"]
+
+        self.assertEqual(result, expected_result)
+
+    # FIXME need federation fixing first
+    @patch.object(pid_views, "oauth2_post_request")
+    @patch.object(query_api, "get_by_id")
+    def test_oauth2_post_request_fails_returns_500(
+        self, mock_get_by_id, mock_oauth2_post_request
+    ):
+        """test_oauth2_post_request_fails_returns_500"""
 
         mock_get_by_id.return_value = mocks.MockQuery(
             data_sources=[
-                mocks.MockDataSource(
-                    authentication=mocks.MockAuthentication(type="mock_auth")
+                dict(
+                    query_options={},
+                    order_by_field="",
+                    capabilities={"query_pid": "mock_url_pid"},
+                    authentication=dict(
+                        auth_type="oauth2",
+                        params={"access_token": "mock_access_token"},
+                    ),
                 )
             ]
         )
+        mock_oauth2_post_request.side_effect = Exception(
+            "mock_oauth2_post_request_exception"
+        )
 
         test_view = pid_views.RetrieveListPIDView()
         response = test_view.post(self.mock_request)
 
         self.assertEqual(response.status_code, 500)
 
     @patch.object(pid_views, "oauth2_post_request")
@@ -270,24 +455,24 @@
         """test_status_200_returns_200"""
 
         mock_get_by_id.return_value = mocks.MockQuery(
             data_sources=[
                 dict(
                     query_options={},
                     order_by_field="",
-                    capabilities={"url_pid": "mock_url_pid"},
+                    capabilities={"query_pid": "mock_url_pid"},
                     authentication=dict(
                         auth_type="oauth2",
                         params={"access_token": "mock_access_token"},
                     ),
                 )
             ]
         )
         mock_oauth2_post_request.return_value = mocks.MockResponse(
-            json_data=[]
+            json_data={"pids": []}
         )
 
         test_view = pid_views.RetrieveListPIDView()
         response = test_view.post(self.mock_request)
 
         self.assertEqual(response.status_code, 200)
 
@@ -299,15 +484,15 @@
         """test_status_400_returns_400"""
 
         mock_get_by_id.return_value = mocks.MockQuery(
             data_sources=[
                 dict(
                     query_options={},
                     order_by_field="",
-                    capabilities={"url_pid": "mock_url_pid"},
+                    capabilities={"query_pid": "mock_url_pid"},
                     authentication=dict(
                         auth_type="oauth2",
                         params={"access_token": "mock_access_token"},
                     ),
                 )
             ],
         )
```

### Comparing `core_linked_records_app-2.2.0/tests/rest/pid_settings/views/test_permissions.py` & `core_linked_records_app-2.3.0/tests/rest/pid_settings/views/test_permissions.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/tests/rest/pid_settings/views/test_unit.py` & `core_linked_records_app-2.3.0/tests/rest/pid_settings/views/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/tests/rest/pid_xpath/views/test_permissions.py` & `core_linked_records_app-2.3.0/tests/rest/pid_xpath/views/test_permissions.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/tests/rest/providers/views/test_permissions.py` & `core_linked_records_app-2.3.0/tests/rest/providers/views/test_permissions.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/tests/rest/providers/views/test_unit.py` & `core_linked_records_app-2.3.0/tests/rest/providers/views/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/tests/system/api/test_unit.py` & `core_linked_records_app-2.3.0/tests/system/api/test_unit.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """ Unit tests for core_linked_records_app.system.api
 """
 from unittest import TestCase
 from unittest.mock import patch, Mock, MagicMock
+
 from django.test import tag, override_settings
 
+from core_linked_records_app.components.local_id.models import LocalId
 from core_linked_records_app.components.pid_xpath.models import PidXpath
-from core_linked_records_app.system.api import (
-    delete_pid_for_data,
-    get_pid_xpath_by_template,
-    is_pid_defined_for_data,
-    get_data_by_pid,
-)
+from core_linked_records_app.components.local_id import api as local_id_api
+from core_linked_records_app.system import api as system_api
+from core_linked_records_app.utils.path import get_api_path_from_object
 from core_linked_records_app.utils.providers import AbstractIdProvider
 from core_main_app.commons.exceptions import DoesNotExist, ApiError
+from core_main_app.components.blob.models import Blob
 from core_main_app.components.data.models import Data
 from tests.mocks import MockResponse
 
 
 class TestIsPidDefinedForDocumentPsql(TestCase):
     """Test Is Pid Defined For Document"""
 
     @patch("core_linked_records_app.system.api.Data.get_by_id")
     def test_wrong_document_id_raise_error(self, mock_data_get_by_id):
         """test_wrong_document_id_raise_error"""
         mock_data_get_by_id.side_effect = DoesNotExist("mock_does_not_exist")
 
         with self.assertRaises(Exception):
-            is_pid_defined_for_data("mock_pid", "mock_document_id")
+            system_api.is_pid_defined_for_data("mock_pid", "mock_document_id")
 
     @override_settings(MONGODB_INDEXING=False)
     @patch("core_linked_records_app.system.api.Data.execute_query")
     @patch("core_linked_records_app.system.api.get_pid_xpath_by_template")
     @patch("core_linked_records_app.system.api.Data.get_by_id")
     def test_undefined_pid_returns_false(
         self,
@@ -40,15 +40,15 @@
     ):
         """test_undefined_pid_returns_false"""
         mock_data_get_by_id.return_value = MagicMock()
         mock_get_pid_xpath_by_template.return_value = MagicMock()
         mock_data_execute_query.return_value = []
 
         self.assertFalse(
-            is_pid_defined_for_data("mock_pid", "mock_document_id")
+            system_api.is_pid_defined_for_data("mock_pid", "mock_document_id")
         )
 
     @override_settings(MONGODB_INDEXING=False)
     @patch("core_linked_records_app.system.api.Data.execute_query")
     @patch("core_linked_records_app.system.api.get_pid_xpath_by_template")
     @patch("core_linked_records_app.system.api.Data.get_by_id")
     def test_duplicate_pid_returns_false(
@@ -59,15 +59,15 @@
     ):
         """test_duplicate_pid_returns_false"""
         mock_data_get_by_id.return_value = MagicMock()
         mock_get_pid_xpath_by_template.return_value = MagicMock()
         mock_data_execute_query.return_value = [MagicMock(), MagicMock()]
 
         self.assertFalse(
-            is_pid_defined_for_data("mock_pid", "mock_document_id")
+            system_api.is_pid_defined_for_data("mock_pid", "mock_document_id")
         )
 
     @override_settings(MONGODB_INDEXING=False)
     @patch("core_linked_records_app.system.api.Data.execute_query")
     @patch("core_linked_records_app.system.api.get_pid_xpath_by_template")
     @patch("core_linked_records_app.system.api.Data.get_by_id")
     def test_defined_pid_for_other_document_returns_false(
@@ -80,15 +80,15 @@
         mock_data_get_by_id.return_value = MagicMock()
         mock_get_pid_xpath_by_template.return_value = MagicMock()
         mock_result = MagicMock()
         mock_result.pk = "mock_document_id_other"
         mock_data_execute_query.return_value = [mock_result]
 
         self.assertFalse(
-            is_pid_defined_for_data("mock_pid", "mock_document_id")
+            system_api.is_pid_defined_for_data("mock_pid", "mock_document_id")
         )
 
     @override_settings(MONGODB_INDEXING=False)
     @patch("core_linked_records_app.system.api.Data.execute_query")
     @patch("core_linked_records_app.system.api.get_pid_xpath_by_template")
     @patch("core_linked_records_app.system.api.Data.get_by_id")
     def test_defined_pid_for_current_document_returns_true(
@@ -101,15 +101,15 @@
         mock_data_get_by_id.return_value = MagicMock()
         mock_get_pid_xpath_by_template.return_value = MagicMock()
         mock_result = MagicMock()
         mock_result.pk = "mock_document_id"
         mock_data_execute_query.return_value = [mock_result]
 
         self.assertTrue(
-            is_pid_defined_for_data("mock_pid", "mock_document_id")
+            system_api.is_pid_defined_for_data("mock_pid", "mock_document_id")
         )
 
 
 class TestIsPidDefinedForDocumentMongo(TestCase):
     """Test Is Pid Defined For Document"""
 
     @tag("mongodb")
@@ -125,15 +125,15 @@
     ):
         """test_undefined_pid_returns_false"""
         mock_data_get_by_id.return_value = MagicMock()
         mock_get_pid_xpath_by_template.return_value = MagicMock()
         mock_data_execute_query.return_value = []
 
         self.assertFalse(
-            is_pid_defined_for_data("mock_pid", "mock_document_id")
+            system_api.is_pid_defined_for_data("mock_pid", "mock_document_id")
         )
 
     @tag("mongodb")
     @override_settings(MONGODB_INDEXING=True)
     @patch("core_main_app.components.mongo.models.MongoData.execute_query")
     @patch("core_linked_records_app.system.api.get_pid_xpath_by_template")
     @patch("core_linked_records_app.system.api.Data.get_by_id")
@@ -145,15 +145,15 @@
     ):
         """test_duplicate_pid_returns_false"""
         mock_data_get_by_id.return_value = MagicMock()
         mock_get_pid_xpath_by_template.return_value = MagicMock()
         mock_data_execute_query.return_value = [MagicMock(), MagicMock()]
 
         self.assertFalse(
-            is_pid_defined_for_data("mock_pid", "mock_document_id")
+            system_api.is_pid_defined_for_data("mock_pid", "mock_document_id")
         )
 
     @tag("mongodb")
     @override_settings(MONGODB_INDEXING=True)
     @patch("core_main_app.components.mongo.models.MongoData.execute_query")
     @patch("core_linked_records_app.system.api.get_pid_xpath_by_template")
     @patch("core_linked_records_app.system.api.Data.get_by_id")
@@ -167,15 +167,15 @@
         mock_data_get_by_id.return_value = MagicMock()
         mock_get_pid_xpath_by_template.return_value = MagicMock()
         mock_result = MagicMock()
         mock_result.pk = "mock_document_id_other"
         mock_data_execute_query.return_value = [mock_result]
 
         self.assertFalse(
-            is_pid_defined_for_data("mock_pid", "mock_document_id")
+            system_api.is_pid_defined_for_data("mock_pid", "mock_document_id")
         )
 
     @tag("mongodb")
     @override_settings(MONGODB_INDEXING=True)
     @patch("core_main_app.components.mongo.models.MongoData.execute_query")
     @patch("core_linked_records_app.system.api.get_pid_xpath_by_template")
     @patch("core_linked_records_app.system.api.Data.get_by_id")
@@ -189,15 +189,15 @@
         mock_data_get_by_id.return_value = MagicMock()
         mock_get_pid_xpath_by_template.return_value = MagicMock()
         mock_result = MagicMock()
         mock_result.pk = "mock_document_id"
         mock_data_execute_query.return_value = [mock_result]
 
         self.assertTrue(
-            is_pid_defined_for_data("mock_pid", "mock_document_id")
+            system_api.is_pid_defined_for_data("mock_pid", "mock_document_id")
         )
 
 
 class TestIsPidDefined(TestCase):
     """Test Is Pid Defined"""
 
     def test_get_data_by_pid_fails_with_unexpected_error_raises_error(self):
@@ -228,45 +228,45 @@
         """test_query_returns_no_results_raises_error"""
         mock_pid_xpath_get_all.return_value = [MagicMock()]
         mock_queryset = MagicMock()
         mock_queryset.count.return_value = 0
         mock_execute_query.return_value = mock_queryset
 
         with self.assertRaises(DoesNotExist):
-            get_data_by_pid("mock_pid")
+            system_api.get_data_by_pid("mock_pid")
 
     @override_settings(MONGODB_INDEXING=False)
     @patch("core_linked_records_app.system.api.Data.execute_query")
     @patch("core_linked_records_app.system.api.PidXpath.get_all")
     def test_query_returns_several_results_raises_error(
         self, mock_pid_xpath_get_all, mock_execute_query
     ):
         """test_query_returns_several_results_raises_error"""
         mock_pid_xpath_get_all.return_value = [MagicMock()]
         mock_queryset = MagicMock()
         mock_queryset.count.return_value = 2
         mock_execute_query.return_value = mock_queryset
 
         with self.assertRaises(ApiError):
-            get_data_by_pid("mock_pid")
+            system_api.get_data_by_pid("mock_pid")
 
     @override_settings(MONGODB_INDEXING=False)
     @patch("core_linked_records_app.system.api.Data.execute_query")
     @patch("core_linked_records_app.system.api.PidXpath.get_all")
     def test_query_returns_single_result_returns_result(
         self, mock_pid_xpath_get_all, mock_execute_query
     ):
         """test_query_returns_single_result_returns_result"""
         mock_pid_xpath_get_all.return_value = [MagicMock()]
         mock_queryset = MagicMock()
         mock_queryset.count.return_value = 1
         mock_queryset.__getitem__.return_value = "mock_data"
         mock_execute_query.return_value = mock_queryset
 
-        self.assertEquals(get_data_by_pid("mock_pid"), "mock_data")
+        self.assertEquals(system_api.get_data_by_pid("mock_pid"), "mock_data")
 
 
 class TestGetDataByPidMongo(TestCase):
     """Test Get Data By Pid"""
 
     @tag("mongodb")
     @override_settings(MONGODB_INDEXING=True)
@@ -278,15 +278,15 @@
         """test_query_returns_no_results_raises_error"""
         mock_pid_xpath_get_all.return_value = [MagicMock()]
         mock_queryset = MagicMock()
         mock_queryset.count.return_value = 0
         mock_execute_query.return_value = mock_queryset
 
         with self.assertRaises(DoesNotExist):
-            get_data_by_pid("mock_pid")
+            system_api.get_data_by_pid("mock_pid")
 
     @tag("mongodb")
     @override_settings(MONGODB_INDEXING=True)
     @patch("core_main_app.components.mongo.models.MongoData.execute_query")
     @patch("core_linked_records_app.system.api.PidXpath.get_all")
     def test_query_returns_several_results_raises_error(
         self, mock_pid_xpath_get_all, mock_execute_query
@@ -294,15 +294,15 @@
         """test_query_returns_several_results_raises_error"""
         mock_pid_xpath_get_all.return_value = [MagicMock()]
         mock_queryset = MagicMock()
         mock_queryset.count.return_value = 2
         mock_execute_query.return_value = mock_queryset
 
         with self.assertRaises(ApiError):
-            get_data_by_pid("mock_pid")
+            system_api.get_data_by_pid("mock_pid")
 
     @tag("mongodb")
     @override_settings(MONGODB_INDEXING=True)
     @patch("core_main_app.components.mongo.models.MongoData.execute_query")
     @patch("core_linked_records_app.system.api.PidXpath.get_all")
     def test_query_returns_single_result_returns_result(
         self, mock_pid_xpath_get_all, mock_execute_query
@@ -310,122 +310,204 @@
         """test_query_returns_single_result_returns_result"""
         mock_pid_xpath_get_all.return_value = [MagicMock()]
         mock_queryset = MagicMock()
         mock_queryset.count.return_value = 1
         mock_queryset.__getitem__.return_value = "mock_data"
         mock_execute_query.return_value = mock_queryset
 
-        self.assertEquals(get_data_by_pid("mock_pid"), "mock_data")
-
-
-class TestGetPidForData(TestCase):
-    """Test Get Pid For Data"""
-
-    def test_not_existing_pid_returns_none(self):
-        """test_not_existing_pid_returns_none"""
-
-        pass
-
-    def test_existing_pid_returns_pid(self):
-        """test_existing_pid_returns_pid"""
-
-        pass
+        self.assertEquals(system_api.get_data_by_pid("mock_pid"), "mock_data")
 
 
 class TestGetPidXpathByTemplate(TestCase):
     """Test get_pid_xpath_by_template method"""
 
     @patch("core_linked_records_app.system.api.PidXpath.get_by_template")
     def test_get_by_template_is_called(self, mock_get_by_template):
         """Test get_by_template is called"""
         mock_template = "mock_template"
 
-        get_pid_xpath_by_template(mock_template)
+        system_api.get_pid_xpath_by_template(mock_template)
         mock_get_by_template.assert_called_with(mock_template)
 
     @patch("core_linked_records_app.system.api.PidXpath.__new__")
     @patch("core_linked_records_app.system.api.PidXpath.get_by_template")
     def test_get_by_template_none_returns_pid_xpath(
         self, mock_get_by_template, mock_pid_xpath
     ):
         """If get_by_template returns None, the PidXpath returned is the default one."""
         expected_result = Mock(spec=PidXpath)
         mock_get_by_template.return_value = None
         mock_pid_xpath.return_value = expected_result
 
-        result = get_pid_xpath_by_template("mock_template")
+        result = system_api.get_pid_xpath_by_template("mock_template")
         self.assertEqual(result, expected_result)
 
     @patch("core_linked_records_app.system.api.PidXpath.get_by_template")
     def test_returns_get_by_template_if_not_none(self, mock_get_by_template):
         """If get_by_template is not None, the PidXpath returned is get_by_template."""
         expected_result = "mock_result"
         mock_get_by_template.return_value = expected_result
 
-        result = get_pid_xpath_by_template("mock_template")
+        result = system_api.get_pid_xpath_by_template("mock_template")
         self.assertEqual(result, expected_result)
 
 
+class TestDeletePidFromRecordName(TestCase):
+    """Test delete_pid_from_record_name"""
+
+    @patch.object(system_api, "ProviderManager")
+    def test_provider_delete_is_called(self, mock_provider_manager):
+        """test_provider_delete_is_called"""
+        mock_provider = Mock()
+        mock_record = "mock_record"
+
+        mock_provider_manager().get.return_value = mock_provider
+        mock_provider.delete.return_value = MockResponse()
+
+        system_api.delete_pid_from_record_name(mock_record)
+        mock_provider.delete.assert_called_with(mock_record)
+
+    @patch.object(system_api, "logger")
+    @patch.object(system_api, "ProviderManager")
+    def test_provider_delete_failure_raises_api_error(
+        self, mock_provider_manager, mock_logger
+    ):
+        """test_provider_delete_failure_is_logged"""
+        mock_provider = Mock()
+        mock_provider.delete.return_value = MockResponse(status_code=500)
+        mock_record = "mock_record"
+
+        mock_provider_manager().get.return_value = mock_provider
+
+        with self.assertRaises(ApiError):
+            system_api.delete_pid_from_record_name(mock_record)
+
+
 class TestDeletePidForData(TestCase):
     """Test delete_pid_for_data"""
 
     @classmethod
     def setUpClass(cls) -> None:
         mock_data = Mock(spec=Data)
         mock_data.pk = "mock_pk"
 
         cls.mock_data = mock_data
 
         cls.mock_provider = Mock(spec=AbstractIdProvider)
 
-    @patch("core_linked_records_app.utils.providers.ProviderManager.get")
-    @patch("core_linked_records_app.system.api.get_pid_for_data")
+    @patch("core_linked_records_app.system.api.delete_pid_from_record_name")
+    @patch("core_linked_records_app.system.api.get_value_from_dot_notation")
+    @patch("core_linked_records_app.system.api.xml_utils.raw_xml_to_dict")
+    @patch("core_linked_records_app.system.api.get_pid_xpath_by_template")
+    def test_get_dict_content_failure_calls_raw_xml_to_dict_utils(
+        self,
+        mock_get_pid_xpath_by_template,
+        mock_raw_xml_to_dict,
+        mock_get_value_from_dot_notation,
+        mock_delete_pid_from_record_name,
+    ):
+        """test_get_dict_content_failure_calls_raw_xml_to_dict_utils"""
+        self.mock_data.get_dict_content.side_effect = Exception(
+            "mock_get_dict_content_exception"
+        )
+        mock_get_value_from_dot_notation.return_value = None
+
+        system_api.delete_pid_for_data(self.mock_data)
+        mock_raw_xml_to_dict.assert_called()
+
+    @patch("core_linked_records_app.system.api.delete_pid_from_record_name")
+    @patch("core_linked_records_app.system.api.get_value_from_dot_notation")
+    @patch("core_linked_records_app.system.api.xml_utils.raw_xml_to_dict")
+    @patch("core_linked_records_app.system.api.get_pid_xpath_by_template")
+    def test_raw_xml_to_dict_failure_raises_api_error(
+        self,
+        mock_get_pid_xpath_by_template,
+        mock_raw_xml_to_dict,
+        mock_get_value_from_dot_notation,
+        mock_delete_pid_from_record_name,
+    ):
+        """test_raw_xml_to_dict_failure_raises_api_error"""
+        self.mock_data.get_dict_content.side_effect = Exception(
+            "mock_get_dict_content_exception"
+        )
+        mock_raw_xml_to_dict.side_effect = Exception(
+            "mock_raw_xml_to_dict_exception"
+        )
+        mock_get_value_from_dot_notation.return_value = None
+
+        with self.assertRaises(ApiError):
+            system_api.delete_pid_for_data(self.mock_data)
+
+    @patch("core_linked_records_app.system.api.delete_pid_from_record_name")
+    @patch("core_linked_records_app.system.api.get_value_from_dot_notation")
+    @patch("core_linked_records_app.system.api.get_pid_xpath_by_template")
     def test_empty_pid_is_not_deleted(
-        self, mock_get_pid_for_data, mock_provider_manager_get
+        self,
+        mock_get_pid_xpath_by_template,
+        mock_get_value_from_dot_notation,
+        mock_delete_pid_from_record_name,
     ):
         """test_empty_pid_is_not_deleted"""
-        mock_get_pid_for_data.return_value = None
-        mock_provider_manager_get.return_value = self.mock_provider
+        mock_get_value_from_dot_notation.return_value = None
 
-        delete_pid_for_data(self.mock_data)
-        self.mock_provider.delete.assert_not_called()
+        system_api.delete_pid_for_data(self.mock_data)
+        mock_delete_pid_from_record_name.assert_not_called()
 
-    @patch("core_linked_records_app.utils.providers.ProviderManager.get")
-    @patch("core_linked_records_app.system.api.get_pid_for_data")
-    def test_provider_delete_called(
-        self, mock_get_pid_for_data, mock_provider_manager_get
+    @patch("core_linked_records_app.system.api.delete_pid_from_record_name")
+    @patch("core_linked_records_app.system.api.get_value_from_dot_notation")
+    @patch("core_linked_records_app.system.api.get_pid_xpath_by_template")
+    def test_delete_pid_from_record_called_when_pid_exists(
+        self,
+        mock_get_pid_xpath_by_template,
+        mock_get_value_from_dot_notation,
+        mock_delete_pid_from_record_name,
     ):
-        """test_provider_delete_called"""
+        """test_delete_pid_from_record_called"""
         mock_pid = "mock_pid"
-        mock_get_pid_for_data.return_value = mock_pid
-        mock_provider_manager_get.return_value = self.mock_provider
+        mock_get_value_from_dot_notation.return_value = mock_pid
 
-        delete_pid_for_data(self.mock_data)
-        self.mock_provider.delete.assert_called_with(mock_pid)
+        system_api.delete_pid_for_data(self.mock_data)
+        mock_delete_pid_from_record_name.assert_called_with(mock_pid)
 
-    @patch("core_linked_records_app.utils.providers.ProviderManager.get")
-    @patch("core_linked_records_app.system.api.get_pid_for_data")
-    def test_pid_delete_failure_exits(
-        self, mock_get_pid_for_data, mock_provider_manager_get
-    ):
-        """test_pid_delete_failure_exits"""
-        mock_pid = "mock_pid"
-        mock_get_pid_for_data.return_value = mock_pid
-        mock_provider_manager_get.return_value = self.mock_provider
 
-        self.mock_provider.delete.return_value = MockResponse(status_code=500)
+class TestDeletePidForBlob(TestCase):
+    """Test delete_pid_for_blob"""
 
-        delete_pid_for_data(self.mock_data)
+    def setUp(self) -> None:
+        self.blob = Mock(spec=Blob)
 
-    @patch("core_linked_records_app.utils.providers.ProviderManager.get")
-    @patch("core_linked_records_app.system.api.get_pid_for_data")
-    def test_pid_delete_success_works(
-        self, mock_get_pid_for_data, mock_provider_manager_get
+    @patch.object(system_api, "delete_pid_from_record_name")
+    @patch.object(local_id_api, "get_by_class_and_id")
+    def test_get_by_class_and_id_called(
+        self, mock_get_by_class_and_id, mock_delete_pid_from_record_name
     ):
-        """test_pid_delete_success_works"""
-        mock_pid = "mock_pid"
-        mock_get_pid_for_data.return_value = mock_pid
-        mock_provider_manager_get.return_value = self.mock_provider
+        """test_get_by_class_and_id_called"""
+        system_api.delete_pid_for_blob(self.blob)
+        mock_get_by_class_and_id.assert_called_with(
+            get_api_path_from_object(Blob()), self.blob.pk
+        )
 
-        self.mock_provider.delete.return_value = MockResponse(status_code=200)
+    @patch.object(system_api, "logger")
+    @patch.object(local_id_api, "get_by_class_and_id")
+    def test_does_not_exist_is_logged(
+        self, mock_get_by_class_and_id, mock_logger
+    ):
+        """test_does_not_exist_is_logged"""
+        mock_get_by_class_and_id.side_effect = DoesNotExist(
+            "mock_get_by_class_and_id_does_not_exist"
+        )
 
-        delete_pid_for_data(self.mock_data)
+        system_api.delete_pid_for_blob(self.blob)
+        mock_logger.info.assert_called()
+
+    @patch.object(system_api, "delete_pid_from_record_name")
+    @patch.object(local_id_api, "get_by_class_and_id")
+    def test_delete_from_record_name_called(
+        self, mock_get_by_class_and_id, mock_delete_pid_from_record_name
+    ):
+        """test_delete_from_record_name_called"""
+        mock_local_id = Mock(spec=LocalId)
+        mock_get_by_class_and_id.return_value = mock_local_id
+        system_api.delete_pid_for_blob(self.blob)
+        mock_delete_pid_from_record_name.assert_called_with(
+            mock_local_id.record_name
+        )
```

### Comparing `core_linked_records_app-2.2.0/tests/test_settings.py` & `core_linked_records_app-2.3.0/tests/test_settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -77,7 +77,9 @@
 
 PID_XPATH = "mock.pid"
 
 ID_PROVIDER_PREFIXES = ["mock_cdcs"]
 
 MONGODB_INDEXING = False
 MONGODB_ASYNC_SAVE = False
+
+ENABLE_SAML2_SSO_AUTH = False
```

### Comparing `core_linked_records_app-2.2.0/tests/utils/dict/test_unit.py` & `core_linked_records_app-2.3.0/tests/utils/dict/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/tests/utils/pid/test_unit.py` & `core_linked_records_app-2.3.0/tests/utils/pid/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/tests/utils/providers/handle_net/test_unit.py` & `core_linked_records_app-2.3.0/tests/utils/providers/handle_net/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/tests/utils/providers/local/test_unit.py` & `core_linked_records_app-2.3.0/tests/utils/providers/local/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/tests/utils/xml/test_unit.py` & `core_linked_records_app-2.3.0/tests/utils/xml/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.2.0/tests/views/admin/views/test_unit.py` & `core_linked_records_app-2.3.0/tests/views/admin/views/test_unit.py`

 * *Files identical despite different names*

