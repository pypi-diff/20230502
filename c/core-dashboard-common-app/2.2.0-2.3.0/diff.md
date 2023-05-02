# Comparing `tmp/core_dashboard_common_app-2.2.0.tar.gz` & `tmp/core_dashboard_common_app-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/core_dashboard_common_app-2.2.0.tar", last modified: Thu Feb 23 20:27:21 2023, max compression
+gzip compressed data, was "core_dashboard_common_app-2.3.0.tar", last modified: Tue May  2 19:36:25 2023, max compression
```

## Comparing `core_dashboard_common_app-2.2.0.tar` & `core_dashboard_common_app-2.3.0.tar`

### file list

```diff
@@ -1,120 +1,121 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:21.000000 core_dashboard_common_app-2.2.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      158 2023-02-23 20:27:16.000000 core_dashboard_common_app-2.2.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      865 2023-02-23 20:27:21.000000 core_dashboard_common_app-2.2.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      406 2023-02-23 20:27:16.000000 core_dashboard_common_app-2.2.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:19.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:16.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4169 2023-02-23 20:27:16.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/constants.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1250 2023-02-23 20:27:16.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:19.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:19.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:19.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:20.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      302 2023-02-23 20:27:16.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/action_dashboard.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      916 2023-02-23 20:27:16.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/admin_table.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       80 2023-02-23 20:27:16.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/admin_table.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      441 2023-02-23 20:27:16.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/count_checked.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      393 2023-02-23 20:27:16.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/get_selected_document_admin.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      407 2023-02-23 20:27:16.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/init_admin.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      237 2023-02-23 20:27:16.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/init_admin_menu.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:20.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       71 2023-02-23 20:27:16.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/list/view_record.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       68 2023-02-23 20:27:16.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/my_dashboard_tabs.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      697 2023-02-23 20:27:16.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/reset_checkbox.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      241 2023-02-23 20:27:16.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/select_all.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:19.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/common/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:20.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/common/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      117 2023-02-23 20:27:16.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/common/css/content_query.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       35 2023-02-23 20:27:16.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/common/css/list.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       65 2023-02-23 20:27:16.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/common/css/password_form.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:20.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       84 2023-02-23 20:27:16.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/init_pagination.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:20.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1034 2023-02-23 20:27:16.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/open_document.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       69 2023-02-23 20:27:16.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/open_form.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       69 2023-02-23 20:27:16.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/open_record.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:16.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/open_template.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      427 2023-02-23 20:27:16.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/view_record.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1277 2023-02-23 20:27:16.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/persistent_query_config.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:19.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:20.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/user/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      831 2023-02-23 20:27:16.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/user/css/exploreTabs.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:20.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      150 2023-02-23 20:27:16.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/get_selected_document.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      577 2023-02-23 20:27:16.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/init.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       83 2023-02-23 20:27:16.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/init.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       68 2023-02-23 20:27:16.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/init_user.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:20.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      836 2023-02-23 20:27:16.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/edit_record.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       61 2023-02-23 20:27:16.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/edit_record.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:20.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1714 2023-02-23 20:27:16.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/change_owner.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       81 2023-02-23 20:27:16.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/change_owner.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1331 2023-02-23 20:27:16.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/delete_document.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       78 2023-02-23 20:27:16.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/delete_document.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1613 2023-02-23 20:27:16.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/edit_persistent_query.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-02-23 20:27:16.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/edit_query.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       60 2023-02-23 20:27:16.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/view_record.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       56 2023-02-23 20:27:16.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/my_dashboard_tabs.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      916 2023-02-23 20:27:16.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/user_table.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       80 2023-02-23 20:27:16.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/user_table.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:19.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:20.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/templates/core_dashboard_common_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:20.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/templates/core_dashboard_common_app/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      380 2023-02-23 20:27:16.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/templates/core_dashboard_common_app/admin/dashboard.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:19.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/templates/core_dashboard_common_app/common/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:20.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/templates/core_dashboard_common_app/common/pagination/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2701 2023-02-23 20:27:16.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/templates/core_dashboard_common_app/common/pagination/data_source_pagination.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      123 2023-02-23 20:27:16.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/templates/core_dashboard_common_app/home.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:20.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:21.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      847 2023-02-23 20:27:17.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/modals/change_owner.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1186 2023-02-23 20:27:17.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/modals/delete_document.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      868 2023-02-23 20:27:17.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/modals/edit_persistent_query.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3055 2023-02-23 20:27:17.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_files_table.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2804 2023-02-23 20:27:17.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_forms_table.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4709 2023-02-23 20:27:17.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_queries_table.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      211 2023-02-23 20:27:17.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_queries_table_pagination.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3575 2023-02-23 20:27:17.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_records_table.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      222 2023-02-23 20:27:17.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_records_table_datatable.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      258 2023-02-23 20:27:17.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_records_table_pagination.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2648 2023-02-23 20:27:17.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_templates_table.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2476 2023-02-23 20:27:17.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_types_table.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3233 2023-02-23 20:27:17.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_workspaces_table.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1927 2023-02-23 20:27:17.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/templates/core_dashboard_common_app/my_dashboard.html
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     1415 2023-02-23 20:27:17.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/templates/core_dashboard_common_app/my_profile.html
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      187 2023-02-23 20:27:17.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/templates/core_dashboard_common_app/my_profile_change_password.html
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      759 2023-02-23 20:27:17.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/templates/core_dashboard_common_app/my_profile_edit.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1007 2023-02-23 20:27:17.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/templates/core_dashboard_common_app/password_change.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:21.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/templatetags/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:17.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/templatetags/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      804 2023-02-23 20:27:17.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/templatetags/draft_extras.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      453 2023-02-23 20:27:17.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/templatetags/special_plural.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:21.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:17.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:21.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/views/common/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:17.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/views/common/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    18721 2023-02-23 20:27:17.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/views/common/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1192 2023-02-23 20:27:17.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/views/common/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    56294 2023-02-23 20:27:17.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app/views/common/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:20.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      865 2023-02-23 20:27:19.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6400 2023-02-23 20:27:19.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-02-23 20:27:19.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       47 2023-02-23 20:27:19.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       37 2023-02-23 20:27:19.000000 core_dashboard_common_app-2.2.0/core_dashboard_common_app.egg-info/top_level.txt
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:21.000000 core_dashboard_common_app-2.2.0/docs/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:17.000000 core_dashboard_common_app-2.2.0/docs/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11337 2023-02-23 20:27:17.000000 core_dashboard_common_app-2.2.0/docs/conf.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-02-23 20:27:17.000000 core_dashboard_common_app-2.2.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       21 2023-02-23 20:27:17.000000 core_dashboard_common_app-2.2.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-02-23 20:27:21.000000 core_dashboard_common_app-2.2.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1093 2023-02-23 20:27:17.000000 core_dashboard_common_app-2.2.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:21.000000 core_dashboard_common_app-2.2.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:17.000000 core_dashboard_common_app-2.2.0/tests/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1753 2023-02-23 20:27:17.000000 core_dashboard_common_app-2.2.0/tests/test_settings.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1009 2023-02-23 20:27:17.000000 core_dashboard_common_app-2.2.0/tests/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:21.000000 core_dashboard_common_app-2.2.0/tests/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:27:17.000000 core_dashboard_common_app-2.2.0/tests/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2325 2023-02-23 20:27:17.000000 core_dashboard_common_app-2.2.0/tests/views/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1160 2023-02-23 20:27:17.000000 core_dashboard_common_app-2.2.0/tests/views/tests_int.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:25.677626 core_dashboard_common_app-2.3.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:36:18.000000 core_dashboard_common_app-2.3.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      158 2023-05-02 19:36:20.000000 core_dashboard_common_app-2.3.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      865 2023-05-02 19:36:25.669894 core_dashboard_common_app-2.3.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      406 2023-05-02 19:36:20.000000 core_dashboard_common_app-2.3.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:24.207888 core_dashboard_common_app-2.3.0/core_dashboard_common_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:20.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3824 2023-05-02 19:36:20.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/constants.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1250 2023-05-02 19:36:20.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:23.878860 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:23.950492 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:23.885731 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:24.420200 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      302 2023-05-02 19:36:20.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/action_dashboard.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      441 2023-05-02 19:36:20.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/count_checked.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      393 2023-05-02 19:36:20.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/get_selected_document_admin.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      237 2023-05-02 19:36:20.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/init_admin_menu.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:24.448260 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       71 2023-05-02 19:36:20.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/list/view_record.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       68 2023-05-02 19:36:20.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/my_dashboard_tabs.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      697 2023-05-02 19:36:20.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/reset_checkbox.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      241 2023-05-02 19:36:20.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/select_all.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:23.937729 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/common/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:24.535618 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/common/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      117 2023-05-02 19:36:20.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/common/css/content_query.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       35 2023-05-02 19:36:20.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/common/css/list.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       65 2023-05-02 19:36:20.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/common/css/password_form.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:24.601246 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       84 2023-05-02 19:36:20.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/init_pagination.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:24.684586 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1034 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/open_document.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       69 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/open_form.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       69 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/open_record.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/open_template.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      427 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/view_record.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1277 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/persistent_query_config.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:23.958713 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:24.706879 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/user/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      831 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/user/css/exploreTabs.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:24.829157 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      150 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/get_selected_document.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      577 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/init.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       83 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/init.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       68 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/init_user.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:24.876339 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      836 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/edit_record.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       61 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/edit_record.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:24.968684 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1714 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/change_owner.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       81 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/change_owner.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1331 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/delete_document.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       78 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/delete_document.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1613 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/edit_persistent_query.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/edit_query.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       60 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/view_record.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       56 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/my_dashboard_tabs.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:23.998946 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:25.061246 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:25.081713 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      380 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/admin/dashboard.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:24.019766 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/common/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:25.103294 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/common/pagination/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2701 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/common/pagination/data_source_pagination.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      123 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/home.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:25.292960 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:25.335120 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      847 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/modals/change_owner.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1053 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/modals/delete_document.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      868 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/modals/edit_persistent_query.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3055 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_files_table.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2804 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_forms_table.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4709 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_queries_table.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      211 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_queries_table_pagination.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3575 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_records_table.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      222 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_records_table_datatable.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      258 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_records_table_pagination.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2809 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_templates_table.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2476 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_types_table.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3233 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_workspaces_table.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1927 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/my_dashboard.html
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     1415 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/my_profile.html
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      187 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/my_profile_change_password.html
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      759 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/my_profile_edit.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1007 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/password_change.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:25.379547 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templatetags/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templatetags/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      804 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templatetags/draft_extras.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      453 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templatetags/special_plural.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:25.394954 core_dashboard_common_app-2.3.0/core_dashboard_common_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:25.458164 core_dashboard_common_app-2.3.0/core_dashboard_common_app/views/common/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/views/common/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    18721 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/views/common/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1192 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/views/common/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    56102 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/views/common/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:24.280379 core_dashboard_common_app-2.3.0/core_dashboard_common_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      865 2023-05-02 19:36:23.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6113 2023-05-02 19:36:23.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:36:23.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       47 2023-05-02 19:36:23.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       37 2023-05-02 19:36:23.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app.egg-info/top_level.txt
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:25.490801 core_dashboard_common_app-2.3.0/docs/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/docs/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11337 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/docs/conf.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       21 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:36:25.681607 core_dashboard_common_app-2.3.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1093 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:25.546076 core_dashboard_common_app-2.3.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/tests/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1783 2023-05-02 19:36:22.000000 core_dashboard_common_app-2.3.0/tests/test_settings.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      913 2023-05-02 19:36:22.000000 core_dashboard_common_app-2.3.0/tests/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:25.580177 core_dashboard_common_app-2.3.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:22.000000 core_dashboard_common_app-2.3.0/tests/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:25.596585 core_dashboard_common_app-2.3.0/tests/views/common/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:22.000000 core_dashboard_common_app-2.3.0/tests/views/common/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:25.651596 core_dashboard_common_app-2.3.0/tests/views/common/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:22.000000 core_dashboard_common_app-2.3.0/tests/views/common/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1150 2023-05-02 19:36:22.000000 core_dashboard_common_app-2.3.0/tests/views/common/views/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3808 2023-05-02 19:36:22.000000 core_dashboard_common_app-2.3.0/tests/views/common/views/tests_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2325 2023-05-02 19:36:22.000000 core_dashboard_common_app-2.3.0/tests/views/fixtures.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `core_dashboard_common_app-2.2.0/PKG-INFO` & `core_dashboard_common_app-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_dashboard_common_app
-Version: 2.2.0
+Version: 2.3.0
 Summary: Resource management via a dashboard for the curator core project
 Home-page: https://github.com/usnistgov/core_dashboard_common_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =========================
         Core Dashboard Common App
```

### Comparing `core_dashboard_common_app-2.2.0/core_dashboard_common_app/constants.py` & `core_dashboard_common_app-2.3.0/core_dashboard_common_app/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,28 +47,23 @@
 MODALS_COMMON_CHANGE_OWNER = (
     "core_dashboard_common_app/list/modals/change_owner.html"
 )
 
 # TODO: replace with the constants in core main app once they are done
 CSS_COMMON = [
     "core_main_app/common/css/XMLTree.css",
-    "core_main_app/libs/datatables/1.10.13/css/jquery.dataTables.css",
     "core_main_app/common/css/table.css",
     "core_dashboard_common_app/common/css/list.css",
+    "core_main_app/common/css/highlight.css",
 ]
 JS_COMMON = [
-    {
-        "path": "core_main_app/libs/datatables/1.10.13/js/jquery.dataTables.js",
-        "is_raw": True,
-    },
     {"path": "core_dashboard_common_app/user/js/init.js", "is_raw": False},
 ]
 
 JS_INIT_USER = "core_dashboard_common_app/user/js/init_user.js"
-JS_USER_TABLE = "core_dashboard_common_app/user/js/user_table.js"
 JS_USER_SELECTED_ELEMENT = (
     "core_dashboard_common_app/user/js/get_selected_document.js"
 )
 JS_COMMON_FUNCTION_DELETE = (
     "core_dashboard_common_app/user/js/list/modals/delete_document.js"
 )
 JS_COMMON_FUNCTION_CHANGE_OWNER = (
@@ -87,19 +82,17 @@
     "core_dashboard_common_app/admin/js/reset_checkbox.js"
 )
 JS_ADMIN_SELECT_ALL = "core_dashboard_common_app/admin/js/select_all.js"
 JS_ADMIN_SELETED_ELEMENT = (
     "core_dashboard_common_app/admin/js/get_selected_document_admin.js"
 )
 JS_ADMIN_INIT_MENU = "core_dashboard_common_app/admin/js/init_admin_menu.js"
-JS_INIT_ADMIN = "core_dashboard_common_app/admin/js/init_admin.js"
 JS_ADMIN_ACTION_DASHBOARD = (
     "core_dashboard_common_app/admin/js/action_dashboard.js"
 )
-JS_ADMIN_TABLE = "core_dashboard_common_app/admin/js/admin_table.js"
 ADMIN_VIEW_RECORD_RAW = (
     "core_dashboard_common_app/admin/js/list/view_record.raw.js"
 )
 
 FUNCTIONAL_OBJECT_ENUM = Enum(
     "FUNCTIONAL_OBJECT_ENUM",
     {
```

### Comparing `core_dashboard_common_app-2.2.0/core_dashboard_common_app/settings.py` & `core_dashboard_common_app-2.3.0/core_dashboard_common_app/settings.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/reset_checkbox.js` & `core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/reset_checkbox.js`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/open_document.js` & `core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/open_document.js`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/persistent_query_config.js` & `core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/persistent_query_config.js`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/user/css/exploreTabs.css` & `core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/user/css/exploreTabs.css`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/init.js` & `core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/init.js`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/edit_record.js` & `core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/edit_record.js`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/change_owner.js` & `core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/change_owner.js`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/delete_document.js` & `core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/delete_document.js`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.2.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/edit_persistent_query.js` & `core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/edit_persistent_query.js`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.2.0/core_dashboard_common_app/templates/core_dashboard_common_app/common/pagination/data_source_pagination.html` & `core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/common/pagination/data_source_pagination.html`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.2.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/modals/change_owner.html` & `core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/modals/change_owner.html`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.2.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/modals/delete_document.html` & `core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/modals/delete_document.html`

 * *Files 9% similar despite different names*

```diff
@@ -6,17 +6,14 @@
 {% block modal_body %}
 <div class="alert alert-danger" id="delete_banner_errors" style="display: none;">
         <a href="#" class="close" data-hide="alert" aria-label="close">&times;</a>
      	<h4><i class="fas fa-exclamation-circle"></i> Error</h4>
         <div id="delete_document_errors"></div>
 </div>
 <input type="hidden" class="{{data.document}}-id"/>
-<p>
-    The {% if data.administration %} {{data.document|special_plural}}{% else %}{{data.document}}{% endif %} will be erased.
-</p>
 <p>Are you sure you want to delete the {% if data.administration %}{{data.document|special_plural}}{% else %}{{data.document}}{% endif %} ?</p>
 {% endblock %}
 
 {% block modal_footer %}
 <button class="btn btn-secondary pull-left" data-dismiss="modal"><i class="fas fa-times"></i> No</button>
 <button id="delete-document-yes" class="btn btn-danger"><i class="fas fa-check"></i> Yes</button>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,12 +1,10 @@
 {% extends 'core_main_app/_render/admin/theme/tools/modal.html' %} {% load
 special_plural %} {% block modal_id %}delete-result-modal{% endblock %} {%
 block modal_title %}Delete {% if data.administration %}{
 {data.document|special_plural}}{% else %}{{data.document}}{% endif %}{%
 endblock %} {% block modal_body %}
 ×
  Error
-The {% if data.administration %} {{data.document|special_plural}}{% else %}{
-{data.document}}{% endif %} will be erased.
 Are you sure you want to delete the {% if data.administration %}{
 {data.document|special_plural}}{% else %}{{data.document}}{% endif %} ?
 {% endblock %} {% block modal_footer %}  No  Yes {% endblock %}
```

### Comparing `core_dashboard_common_app-2.2.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/modals/edit_persistent_query.html` & `core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/modals/edit_persistent_query.html`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.2.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_files_table.html` & `core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_files_table.html`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.2.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_forms_table.html` & `core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_forms_table.html`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -42,20 +42,20 @@
                         </a>
                     {% else %}
                         <a class="btn btn-secondary view-form-btn"
                            href="{% url 'core_curate_view_form' data_loaded.form.id %}">
                             <i class="fas fa-file-alt"></i> View
                         </a>
                     {% endif %}
-                    <a class="btn btn-secondary open-form-btn">
-                        <i class="fas fa-code"></i> Open
-                    </a>
                     <a class="btn btn-secondary edit-form-btn" href="{% url 'core_curate_enter_data' data_loaded.form.id %}">
                         <i class="fas fa-edit"></i> Edit
                     </a>
+                    <a class="btn btn-secondary open-form-btn">
+                        <i class="fas fa-code"></i> Open
+                    </a>
                     <a class="btn btn-secondary change-owner-btn">
                         <i class="fas fa-user-circle"></i> Change Owner
                     </a>
                     <button class="btn btn-danger delete-document-btn">
                         <i class="fas fa-trash"></i> Delete
                     </button>
                 </td>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
                                                                                          {% if
                                                                                          come_from_admin
                                                                                          %}
                                                                                           View
   {                     {                                      {% with                    {% else %}
   {                     {                                      key=data_loaded.form.user  View
 �data_loaded.form.name data_loaded.form.template.display_name %} {{ data.usernames|get:  {% endif %}
-  }}                    }}                                     key }} {% endwith %}       Open
+  }}                    }}                                     key }} {% endwith %}       Edit
 
-                                                                                          Edit
+                                                                                          Open
 
                                                                                           Change Owner
                                                                                             Delete
 {% include 'core_main_app/common/pagination/data_source_pagination.html' with
 pagination=data.pagination%}
```

### Comparing `core_dashboard_common_app-2.2.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_queries_table.html` & `core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_queries_table.html`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.2.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_records_table.html` & `core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_records_table.html`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.2.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_templates_table.html` & `core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_types_table.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,50 @@
 {% load dict_key_extras %}
 {% load get_attribute %}
 <table class="table table-bordered table-striped table-hover fixed-table
         {% if come_from_admin %}table-col-4{% else %}table-col-3{% endif %}">
     <thead>
-        <th>Template name</th>
+        <th>Type name</th>
         <th>Filename</th>
         {% if come_from_admin %}
             <th>User</th>
         {% endif %}
         <th>Actions</th>
     </thead>
     <tbody>
         {% for object in objects %}
-            <tr object-id="{{object.template_version.id}}" draggable="true" ondragstart="start()"  ondragover="dragover()">
+            <tr class="{{ rowcolors }}" objectid="{{object.type_version.id}}">
                 <td>{{ object.title }}</td>
-                <td>{{ object.template.filename }}</td>
+                <td>{{ object.type.filename }}</td>
                 {% if come_from_admin %}
                     <td>
                         {{object.user}}
                     </td>
                 {% endif %}
                 <td>
-                    {% if object.template_version|get_attribute:'is_disabled' %}
-                    <a class="btn btn-secondary restore-{{data.document}}-btn" objectid="{{ object.template_version.id }}">
+                    {% if object.type_version|get_attribute:'is_disabled' %}
+                    <a class="btn btn-secondary restore-template-btn" objectid="{{ object.type_version.id }}">
                         <i class="fas fa-undo"></i> Restore
                     </a>
                     {% else %}
                         {% if come_from_admin %}
-                            <a class="btn btn-secondary view-{{data.document}}-btn" href="{% url 'core-admin:core_main_app_manage_template_versions' object.template_version.id %}">
+                            <a class="btn btn-secondary view-{{data.document}}-btn" href="{% url 'core-admin:core_composer_app_manage_type_versions' object.type_version.id %}">
                                 <i class="fas fa-list"></i> Versions
                             </a>
-                            {% url 'core-admin:core_dashboard_app_edit_template' object.template_version.id as edit_url %}
+                            {% url 'core-admin:core_dashboard_app_edit_type' object.type_version.id as edit_url %}
                             {% include 'core_main_app/common/buttons/edit.html' %}
                         {% else %}
-                            <a class="btn btn-secondary view-{{data.document}}-btn" href="{% url 'core_main_app_manage_template_versions' object.template_version.id %}">
+                            <a class="btn btn-secondary view-{{data.document}}-btn" href="{% url 'core_composer_app_manage_type_versions' object.type_version.id %}">
                                 <i class="fas fa-list"></i> Versions
                             </a>
-                            {% url 'core_dashboard_app_edit_template' object.template_version.id as edit_url %}
+                            {% url 'core_dashboard_app_edit_type' object.type_version.id as edit_url %}
                             {% include 'core_main_app/common/buttons/edit.html' %}
                         {% endif %}
-                        <button class="btn btn-danger disable-{{data.document}}-btn" objectid="{{ object.template_version.id }}">
+                        <button class="btn btn-danger disable-template-btn" objectid="{{ object.type_version.id }}">
                             <i class="fas fa-trash"></i> Disable
                         </button>
-
                     {% endif %}
-
                 </td>
             </tr>
         {% endfor %}
     </tbody>
 </table>
-{% include 'core_main_app/common/buttons/save_ordering.html' %}
```

#### html2text {}

```diff
@@ -1,20 +1,21 @@
 {% load dict_key_extras %} {% load get_attribute %}
-                                                     {% if
-                                                     object.template_version|get_attribute:
-                                                     'is_disabled' %}
-                                                      Restore
-                                                      {% else %} {% if come_from_admin %}
-                                                      Versions
-                                                      {% url 'core-admin:
-{            {                                       core_dashboard_app_edit_template'
-{            {                        {              object.template_version.id as edit_url
-object.title object.template.filename {object.user}} %} {% include 'core_main_app/common/
-}}           }}                                      buttons/edit.html' %} {% else %}
-                                                      Versions
-                                                      {% url
-                                                     'core_dashboard_app_edit_template'
-                                                     object.template_version.id as edit_url
-                                                     %} {% include 'core_main_app/common/
-                                                     buttons/edit.html' %} {% endif %}
-                                                     Disable  {% endif %}
-{% include 'core_main_app/common/buttons/save_ordering.html' %}
+                                                 {% if
+                                                 object.type_version|get_attribute:
+                                                 'is_disabled' %}
+                                                  Restore
+                                                  {% else %} {% if come_from_admin
+                                                 %}
+                                                  Versions
+                                                  {% url 'core-admin:
+{            {                                   core_dashboard_app_edit_type'
+{            {                    {              object.type_version.id as edit_url
+object.title object.type.filename {object.user}} %} {% include 'core_main_app/
+}}           }}                                  common/buttons/edit.html' %} {%
+                                                 else %}
+                                                  Versions
+                                                  {% url
+                                                 'core_dashboard_app_edit_type'
+                                                 object.type_version.id as edit_url
+                                                 %} {% include 'core_main_app/
+                                                 common/buttons/edit.html' %} {%
+                                                 endif %}   Disable  {% endif %}
```

### Comparing `core_dashboard_common_app-2.2.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_types_table.html` & `core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_workspaces_table.html`

 * *Files 21% similar despite different names*

```diff
@@ -1,50 +1,69 @@
 {% load dict_key_extras %}
-{% load get_attribute %}
-<table class="table table-bordered table-striped table-hover fixed-table
-        {% if come_from_admin %}table-col-4{% else %}table-col-3{% endif %}">
+{% load i18n %}
+
+<table class="table table-bordered table-striped table-hover">
     <thead>
-        <th>Type name</th>
-        <th>Filename</th>
-        {% if come_from_admin %}
-            <th>User</th>
-        {% endif %}
+        <th>Title</th>
+        <th>Owner</th>
+        <th>Can read</th>
+        <th>Can write</th>
+        <th>Public</th>
         <th>Actions</th>
     </thead>
     <tbody>
         {% for object in objects %}
-            <tr class="{{ rowcolors }}" objectid="{{object.type_version.id}}">
-                <td>{{ object.title }}</td>
-                <td>{{ object.type.filename }}</td>
-                {% if come_from_admin %}
-                    <td>
-                        {{object.user}}
-                    </td>
-                {% endif %}
+            <tr objectid="{{object.workspace.id}}">
+                <td>{{ object.name }}</td>
+                <td>{{ object.user }}</td>
+                <td>{{ object.can_read }}</td>
+                <td>{{ object.can_write }}</td>
+                <td>{{ object.is_public }} </td>
                 <td>
-                    {% if object.type_version|get_attribute:'is_disabled' %}
-                    <a class="btn btn-secondary restore-template-btn" objectid="{{ object.type_version.id }}">
-                        <i class="fas fa-undo"></i> Restore
-                    </a>
+                    {% if come_from_admin %}
+                        <a class="btn btn-secondary view-data-{{data.document}}-btn"
+                           objectid="{{ object.workspace.id }}"
+                           href="{% url 'core-admin:core_dashboard_workspace_list' object.workspace.id %}">
+                            <i class="fas fa-list"></i> View Content
+                        </a>
                     {% else %}
+                        <a class="btn btn-secondary view-data-{{data.document}}-btn"
+                           objectid="{{ object.workspace.id }}"
+                           href="{% url 'core_dashboard_workspace_list' object.workspace.id %}">
+                            <i class="fas fa-list"></i> View Content
+                        </a>
+                    {% endif %}
+
+                    {% if object.is_owner %}
                         {% if come_from_admin %}
-                            <a class="btn btn-secondary view-{{data.document}}-btn" href="{% url 'core-admin:core_composer_app_manage_type_versions' object.type_version.id %}">
-                                <i class="fas fa-list"></i> Versions
+                            <a class="btn btn-secondary rights-document-btn"
+                                href="{% url 'core-admin:core_main_edit_rights_workspace' object.workspace.id %}">
+                                <i class="fas fa-edit"></i> Manage Access
                             </a>
-                            {% url 'core-admin:core_dashboard_app_edit_type' object.type_version.id as edit_url %}
-                            {% include 'core_main_app/common/buttons/edit.html' %}
                         {% else %}
-                            <a class="btn btn-secondary view-{{data.document}}-btn" href="{% url 'core_composer_app_manage_type_versions' object.type_version.id %}">
-                                <i class="fas fa-list"></i> Versions
+                            <a class="btn btn-secondary rights-document-btn"
+                                href="{% url 'core_main_edit_rights_workspace' object.workspace.id %}">
+                                <i class="fas fa-edit"></i> Manage Access
                             </a>
-                            {% url 'core_dashboard_app_edit_type' object.type_version.id as edit_url %}
-                            {% include 'core_main_app/common/buttons/edit.html' %}
                         {% endif %}
-                        <button class="btn btn-danger disable-template-btn" objectid="{{ object.type_version.id }}">
-                            <i class="fas fa-trash"></i> Disable
-                        </button>
+                        {% if not object.is_global %}
+                            {% if object.is_public %}
+                                <a class="btn btn-secondary private-{{data.document}}-btn">
+                                    <i class="fas fa-user"></i> Set private
+                                </a>
+                            {% elif data.can_set_public %}
+                                <a class="btn btn-secondary public-{{data.document}}-btn">
+                                    <i class="fas fa-users"></i> Set public
+                                </a>
+                            {% endif %}
+                        {% endif %}
+                        {% if not object.is_public %}
+                            <button class="btn btn-danger delete-document-btn">
+                                <i class="fas fa-trash"></i> Delete
+                            </button>
+                        {% endif %}
                     {% endif %}
                 </td>
             </tr>
         {% endfor %}
     </tbody>
-</table>
+</table>
```

#### html2text {}

```diff
@@ -1,21 +1,28 @@
-{% load dict_key_extras %} {% load get_attribute %}
-                                                 {% if
-                                                 object.type_version|get_attribute:
-                                                 'is_disabled' %}
-                                                  Restore
-                                                  {% else %} {% if come_from_admin
-                                                 %}
-                                                  Versions
-                                                  {% url 'core-admin:
-{            {                                   core_dashboard_app_edit_type'
-{            {                    {              object.type_version.id as edit_url
-object.title object.type.filename {object.user}} %} {% include 'core_main_app/
-}}           }}                                  common/buttons/edit.html' %} {%
-                                                 else %}
-                                                  Versions
-                                                  {% url
-                                                 'core_dashboard_app_edit_type'
-                                                 object.type_version.id as edit_url
-                                                 %} {% include 'core_main_app/
-                                                 common/buttons/edit.html' %} {%
-                                                 endif %}   Disable  {% endif %}
+{% load dict_key_extras %} {% load i18n %}
+                                                                          {% if
+                                                                          come_from_admin %}
+                                                                           View_Content
+                                                                           {% else %}
+                                                                           View_Content
+                                                                           {% endif %} {% if
+                                                                          object.is_owner %}
+                                                                          {% if
+                                                                          come_from_admin %}
+                                                                           Manage_Access
+                                                                           {% else %}
+{           {           {               {                {                 Manage_Access
+{           {           {               {                {                 {% endif %} {% if
+object.name object.user object.can_read object.can_write object.is_public not
+}}          }}          }}              }}               }}               object.is_global %}
+                                                                          {% if
+                                                                          object.is_public %}
+                                                                           Set private
+                                                                           {% elif
+                                                                          data.can_set_public
+                                                                          %}
+                                                                           Set public
+                                                                           {% endif %} {%
+                                                                          endif %} {% if not
+                                                                          object.is_public %}
+                                                                          Delete  {% endif %}
+                                                                          {% endif %}
```

### Comparing `core_dashboard_common_app-2.2.0/core_dashboard_common_app/templates/core_dashboard_common_app/my_dashboard.html` & `core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/my_dashboard.html`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.2.0/core_dashboard_common_app/templates/core_dashboard_common_app/my_profile.html` & `core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/my_profile.html`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.2.0/core_dashboard_common_app/templates/core_dashboard_common_app/my_profile_edit.html` & `core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/my_profile_edit.html`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.2.0/core_dashboard_common_app/templates/core_dashboard_common_app/password_change.html` & `core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/password_change.html`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.2.0/core_dashboard_common_app/templatetags/draft_extras.py` & `core_dashboard_common_app-2.3.0/core_dashboard_common_app/templatetags/draft_extras.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.2.0/core_dashboard_common_app/views/common/ajax.py` & `core_dashboard_common_app-2.3.0/core_dashboard_common_app/views/common/ajax.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.2.0/core_dashboard_common_app/views/common/forms.py` & `core_dashboard_common_app-2.3.0/core_dashboard_common_app/views/common/forms.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.2.0/core_dashboard_common_app/views/common/views.py` & `core_dashboard_common_app-2.3.0/core_dashboard_common_app/views/common/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from django.contrib.auth import update_session_auth_hash
 from django.contrib.auth.decorators import login_required
 from django.contrib.auth.forms import PasswordChangeForm
 from django.core.exceptions import ObjectDoesNotExist
 from django.db import IntegrityError
 from django.http.response import HttpResponseRedirect
 from django.shortcuts import redirect
-from django.urls import reverse, reverse_lazy
+from django.urls import reverse
 
 import core_main_app.components.data.api as workspace_data_api
 from core_explore_common_app.components.abstract_persistent_query import (
     api as abstract_persistent_query_api,
 )
 from core_explore_common_app.components.abstract_persistent_query.models import (
     AbstractPersistentQuery,
@@ -54,15 +54,15 @@
     from core_composer_app.components.type import api as type_api
     from core_composer_app.views.user.ajax import EditTypeVersionManagerView
 from core_dashboard_common_app import constants as dashboard_constants
 from core_dashboard_common_app import settings
 from core_dashboard_common_app.views.common.forms import ActionForm, UserForm
 
 
-@login_required(login_url=reverse_lazy("core_main_app_login"))
+@login_required
 def home(request):
     """Home page.
 
     Args:
         request:
 
     Returns:
@@ -70,43 +70,45 @@
     return render(
         request,
         dashboard_constants.DASHBOARD_HOME_TEMPLATE,
         context={"page_title": "Dashboard"},
     )
 
 
-@login_required(login_url=reverse_lazy("core_main_app_login"))
+@login_required
 def my_profile(request):
     """User's profile information page.
 
     Args:
         request:
 
     Returns:
     """
     return render(
         request,
         dashboard_constants.DASHBOARD_PROFILE_TEMPLATE,
-        context={"page_title": "My Profile"},
+        context={
+            "page_title": "My Profile",
+        },
     )
 
 
-@login_required(login_url=reverse_lazy("core_main_app_login"))
+@login_required
 def my_profile_edit(request):
     """Edit the profile.
 
     Args:
         request:
 
     Returns:
     """
     if request.method == "POST":
         form = _get_edit_profile_form(
             request=request,
-            url=dashboard_constants.DASHBOARD_PROFILE_EDIT_TEMPLATE,
+            template=dashboard_constants.DASHBOARD_PROFILE_EDIT_TEMPLATE,
         )
         if form.is_valid():
             user = request.user
             user.first_name = request.POST["firstname"]
             user.last_name = request.POST["lastname"]
             user.email = request.POST["email"]
             try:
@@ -148,32 +150,32 @@
     return render(
         request,
         dashboard_constants.DASHBOARD_PROFILE_EDIT_TEMPLATE,
         context={"form": form, "page_title": "Edit Profile"},
     )
 
 
-def _get_edit_profile_form(request, url, data=None):
+def _get_edit_profile_form(request, template, data=None):
     """Edit the profile.
 
     Args:
         request
-        url
+        template
         data
 
     Returns:
     """
     data = request.POST if data is None else data
     try:
         return EditProfileForm(data)
     except Exception:
         message = "A problem with the form has occurred."
         return render(
             request,
-            url,
+            template,
             context={"action_result": message, "page_title": "Error"},
         )
 
 
 def _error_while_saving(request, form):
     """Raise exception if uncatched problems occurred while saving.
 
@@ -1297,14 +1299,24 @@
             }
         )
 
         modals = self._get_modals()
 
         assets = self._get_assets()
 
+        if self.administration and workspace.owner:
+            context.update(
+                {
+                    "owner": user_api.get_user_by_id(workspace.owner).username,
+                    "owner_change_url": reverse(
+                        "admin:auth_user_change", args=[workspace.owner]
+                    ),
+                }
+            )
+
         # Set page title
         context.update({"page_title": "Dashboard"})
 
         return self.common_render(
             request,
             self.template,
             context=context,
@@ -1571,33 +1583,22 @@
                     "path": "core_dashboard_app/common/js/my_dashboard_tabs.js",
                     "is_raw": False,
                 },
                 {
                     "path": "core_dashboard_common_app/user/js/list/modals/edit_persistent_query.js",
                     "is_raw": False,
                 },
-                {
-                    "path": "core_main_app/libs/highlight/11.0.0/js/highlight.min.js",
-                    "is_raw": False,
-                },
-                {
-                    "path": "core_main_app/libs/highlight/11.0.0/js/init_highlight.js",
-                    "is_raw": False,
-                },
             ],
         }
         assets["css"].append(
             "core_dashboard_app/common/css/my_dashboard_tabs.css"
         )
         assets["css"].append(
             "core_dashboard_common_app/common/css/content_query.css"
         )
-        assets["css"].append(
-            "core_main_app/libs/highlight/11.0.0/css/atom-one-light.css"
-        )
         assets["css"].append("core_main_app/common/css/share_link.css"),
 
         # Admin
         if self.administration:
             assets["js"].append(
                 {
                     "path": "core_dashboard_common_app/common/js/init_pagination.js",
```

### Comparing `core_dashboard_common_app-2.2.0/core_dashboard_common_app.egg-info/PKG-INFO` & `core_dashboard_common_app-2.3.0/core_dashboard_common_app.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-dashboard-common-app
-Version: 2.2.0
+Version: 2.3.0
 Summary: Resource management via a dashboard for the curator core project
 Home-page: https://github.com/usnistgov/core_dashboard_common_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =========================
         Core Dashboard Common App
```

### Comparing `core_dashboard_common_app-2.2.0/core_dashboard_common_app.egg-info/SOURCES.txt` & `core_dashboard_common_app-2.3.0/core_dashboard_common_app.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,24 @@
+LICENSE.md
 MANIFEST.in
 README.rst
 pyproject.toml
 requirements.core.txt
 setup.py
 core_dashboard_common_app/__init__.py
 core_dashboard_common_app/constants.py
 core_dashboard_common_app/settings.py
 core_dashboard_common_app.egg-info/PKG-INFO
 core_dashboard_common_app.egg-info/SOURCES.txt
 core_dashboard_common_app.egg-info/dependency_links.txt
 core_dashboard_common_app.egg-info/requires.txt
 core_dashboard_common_app.egg-info/top_level.txt
 core_dashboard_common_app/static/core_dashboard_common_app/admin/js/action_dashboard.js
-core_dashboard_common_app/static/core_dashboard_common_app/admin/js/admin_table.js
-core_dashboard_common_app/static/core_dashboard_common_app/admin/js/admin_table.raw.js
 core_dashboard_common_app/static/core_dashboard_common_app/admin/js/count_checked.js
 core_dashboard_common_app/static/core_dashboard_common_app/admin/js/get_selected_document_admin.js
-core_dashboard_common_app/static/core_dashboard_common_app/admin/js/init_admin.js
 core_dashboard_common_app/static/core_dashboard_common_app/admin/js/init_admin_menu.js
 core_dashboard_common_app/static/core_dashboard_common_app/admin/js/my_dashboard_tabs.raw.js
 core_dashboard_common_app/static/core_dashboard_common_app/admin/js/reset_checkbox.js
 core_dashboard_common_app/static/core_dashboard_common_app/admin/js/select_all.js
 core_dashboard_common_app/static/core_dashboard_common_app/admin/js/list/view_record.raw.js
 core_dashboard_common_app/static/core_dashboard_common_app/common/css/content_query.css
 core_dashboard_common_app/static/core_dashboard_common_app/common/css/list.css
@@ -34,16 +32,14 @@
 core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/view_record.js
 core_dashboard_common_app/static/core_dashboard_common_app/user/css/exploreTabs.css
 core_dashboard_common_app/static/core_dashboard_common_app/user/js/get_selected_document.js
 core_dashboard_common_app/static/core_dashboard_common_app/user/js/init.js
 core_dashboard_common_app/static/core_dashboard_common_app/user/js/init.raw.js
 core_dashboard_common_app/static/core_dashboard_common_app/user/js/init_user.js
 core_dashboard_common_app/static/core_dashboard_common_app/user/js/my_dashboard_tabs.raw.js
-core_dashboard_common_app/static/core_dashboard_common_app/user/js/user_table.js
-core_dashboard_common_app/static/core_dashboard_common_app/user/js/user_table.raw.js
 core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/edit_record.js
 core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/edit_record.raw.js
 core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/view_record.raw.js
 core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/change_owner.js
 core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/change_owner.raw.js
 core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/delete_document.js
 core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/delete_document.raw.js
@@ -81,8 +77,11 @@
 docs/__init__.py
 docs/conf.py
 tests/__init__.py
 tests/test_settings.py
 tests/urls.py
 tests/views/__init__.py
 tests/views/fixtures.py
-tests/views/tests_int.py
+tests/views/common/__init__.py
+tests/views/common/views/__init__.py
+tests/views/common/views/tests_int.py
+tests/views/common/views/tests_unit.py
```

### Comparing `core_dashboard_common_app-2.2.0/docs/conf.py` & `core_dashboard_common_app-2.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.2.0/setup.py` & `core_dashboard_common_app-2.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_dashboard_common_app",
-    version="2.2.0",
+    version="2.3.0",
     description="Resource management via a dashboard for the curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_dashboard_common_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_dashboard_common_app-2.2.0/tests/test_settings.py` & `core_dashboard_common_app-2.3.0/tests/test_settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -59,7 +59,8 @@
 ]
 
 CELERYBEAT_SCHEDULER = "django_celery_beat.schedulers:DatabaseScheduler"
 CUSTOM_NAME = "Curator"
 ROOT_URLCONF = "tests.urls"
 MONGODB_INDEXING = False
 MONGODB_ASYNC_SAVE = False
+ENABLE_SAML2_SSO_AUTH = False
```

### Comparing `core_dashboard_common_app-2.2.0/tests/urls.py` & `core_dashboard_common_app-2.3.0/tests/urls.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
     Url router for the dashboard common
 """
+from django.conf.urls import include
 from django.contrib.auth.decorators import login_required
 from django.urls import re_path
-from django.urls import reverse_lazy
-from django.conf.urls import include
 
 from core_dashboard_common_app.views.common import (
     ajax,
     views as dashboard_common_app_common_views,
 )
 
 urlpatterns = [
@@ -25,13 +24,12 @@
     re_path(
         r"^edit-record", ajax.edit_record, name="core_dashboard_edit_record"
     ),
     re_path(
         r"^forms$",
         login_required(
             dashboard_common_app_common_views.DashboardForms.as_view(),
-            login_url=reverse_lazy("core_main_app_login"),
         ),
         name="core_dashboard_common_forms",
     ),
     re_path(r"^tz_detect/", include("tz_detect.urls")),
 ]
```

### Comparing `core_dashboard_common_app-2.2.0/tests/views/fixtures.py` & `core_dashboard_common_app-2.3.0/tests/views/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.2.0/tests/views/tests_int.py` & `core_dashboard_common_app-2.3.0/tests/views/common/views/tests_int.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """ Test access to views
 """
 from django.contrib.auth.models import AnonymousUser
 from django.test import RequestFactory
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from core_dashboard_common_app.views.common.views import DashboardForms
 
 from tests.views.fixtures import (
     DataStructureFixtures,
 )
 
 
-class TestViewDashboardForms(MongoIntegrationBaseTestCase):
+class TestViewDashboardForms(IntegrationBaseTestCase):
     """Test View Dashboard Forms"""
 
     def setUp(self):
         """setUp
 
         Returns:
```

