# Comparing `tmp/core_curate_app-2.2.0.tar.gz` & `tmp/core_curate_app-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/core_curate_app-2.2.0.tar", last modified: Thu Feb 23 20:26:49 2023, max compression
+gzip compressed data, was "core_curate_app-2.3.0.tar", last modified: Tue May  2 19:35:41 2023, max compression
```

## Comparing `core_curate_app-2.2.0.tar` & `core_curate_app-2.3.0.tar`

### file list

```diff
@@ -1,144 +1,146 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:49.000000 core_curate_app-2.2.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1016 2023-02-23 20:26:49.000000 core_curate_app-2.2.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      532 2023-02-23 20:26:43.000000 core_curate_app-2.2.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:47.000000 core_curate_app-2.2.0/core_curate_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       73 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:47.000000 core_curate_app-2.2.0/core_curate_app/access_control/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/access_control/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2987 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/access_control/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1017 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/admin.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      478 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/apps.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:47.000000 core_curate_app-2.2.0/core_curate_app/common/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/common/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      207 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/common/exceptions.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:47.000000 core_curate_app-2.2.0/core_curate_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:47.000000 core_curate_app-2.2.0/core_curate_app/components/curate_data_structure/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/components/curate_data_structure/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      464 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/components/curate_data_structure/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4953 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/components/curate_data_structure/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5888 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/components/curate_data_structure/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      233 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/menus.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:47.000000 core_curate_app-2.2.0/core_curate_app/migrations/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2186 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/migrations/0001_initial.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/migrations/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      738 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:47.000000 core_curate_app-2.2.0/core_curate_app/permissions/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/permissions/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1306 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/permissions/discover.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      221 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/permissions/rights.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:47.000000 core_curate_app-2.2.0/core_curate_app/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:48.000000 core_curate_app-2.2.0/core_curate_app/rest/curate_data_structure/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/rest/curate_data_structure/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1396 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/rest/curate_data_structure/admin_serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2131 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/rest/curate_data_structure/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11996 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/rest/curate_data_structure/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      668 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/rest/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1174 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:47.000000 core_curate_app-2.2.0/core_curate_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:47.000000 core_curate_app-2.2.0/core_curate_app/static/core_curate_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:47.000000 core_curate_app-2.2.0/core_curate_app/static/core_curate_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:48.000000 core_curate_app-2.2.0/core_curate_app/static/core_curate_app/user/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      481 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/static/core_curate_app/user/css/common.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2033 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/static/core_curate_app/user/css/style.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      683 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/static/core_curate_app/user/css/xsd_form.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:48.000000 core_curate_app-2.2.0/core_curate_app/static/core_curate_app/user/img/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      246 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/static/core_curate_app/user/img/collapse.png
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      253 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/static/core_curate_app/user/img/expand.png
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:48.000000 core_curate_app-2.2.0/core_curate_app/static/core_curate_app/user/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      157 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/static/core_curate_app/user/js/buttons.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       89 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/static/core_curate_app/user/js/choice.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      168 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/static/core_curate_app/user/js/download.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9748 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/static/core_curate_app/user/js/enter_data.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      357 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/static/core_curate_app/user/js/enter_data.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6638 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/static/core_curate_app/user/js/select_template.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      121 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/static/core_curate_app/user/js/select_template.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       81 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/static/core_curate_app/user/js/text_editor.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1083 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/static/core_curate_app/user/js/view_data.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      108 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/static/core_curate_app/user/js/view_data.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3595 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/static/core_curate_app/user/js/xml_entities_tooltip.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:47.000000 core_curate_app-2.2.0/core_curate_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:47.000000 core_curate_app-2.2.0/core_curate_app/templates/core_curate_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:48.000000 core_curate_app-2.2.0/core_curate_app/templates/core_curate_app/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      366 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/templates/core_curate_app/admin/detail.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      348 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/templates/core_curate_app/admin/view_curate_data_structure.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:48.000000 core_curate_app-2.2.0/core_curate_app/templates/core_curate_app/common/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      167 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/templates/core_curate_app/common/detail_curate_data_structure.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      173 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/templates/core_curate_app/common/tools_curate_data_structure.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:48.000000 core_curate_app-2.2.0/core_curate_app/templates/core_curate_app/user/
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     1266 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/templates/core_curate_app/user/curate.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1191 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/templates/core_curate_app/user/curate_full_start.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      628 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/templates/core_curate_app/user/curate_start.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:48.000000 core_curate_app-2.2.0/core_curate_app/templates/core_curate_app/user/data-entry/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1854 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/templates/core_curate_app/user/data-entry/enter_data.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:48.000000 core_curate_app-2.2.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      575 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/cancel-changes.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      671 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/cancel-form.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      579 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/clear-fields.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1137 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/download-options.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      549 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/save-form.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      857 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/use-validation.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      361 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/validation-warning.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      383 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/xml-error.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      702 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/xml-valid.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:48.000000 core_curate_app-2.2.0/core_curate_app/templates/core_curate_app/user/data-review/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:48.000000 core_curate_app-2.2.0/core_curate_app/templates/core_curate_app/user/data-review/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      376 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/templates/core_curate_app/user/data-review/modals/save-error.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      973 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/templates/core_curate_app/user/data-review/view_data.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      318 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/templates/core_curate_app/user/detail.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       32 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/templates/core_curate_app/user/errors.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:48.000000 core_curate_app-2.2.0/core_curate_app/templates/core_curate_app/user/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      207 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/templates/core_curate_app/user/list/list.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3391 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:48.000000 core_curate_app-2.2.0/core_curate_app/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/utils/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      764 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/utils/parser.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:48.000000 core_curate_app-2.2.0/core_curate_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:48.000000 core_curate_app-2.2.0/core_curate_app/views/common/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/views/common/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7151 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/views/common/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:48.000000 core_curate_app-2.2.0/core_curate_app/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    19505 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/views/user/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2923 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/views/user/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    19931 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/core_curate_app/views/user/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:47.000000 core_curate_app-2.2.0/core_curate_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1016 2023-02-23 20:26:46.000000 core_curate_app-2.2.0/core_curate_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5052 2023-02-23 20:26:47.000000 core_curate_app-2.2.0/core_curate_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-02-23 20:26:46.000000 core_curate_app-2.2.0/core_curate_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       88 2023-02-23 20:26:46.000000 core_curate_app-2.2.0/core_curate_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       27 2023-02-23 20:26:46.000000 core_curate_app-2.2.0/core_curate_app.egg-info/top_level.txt
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:48.000000 core_curate_app-2.2.0/docs/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/docs/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11286 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/docs/conf.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      283 2023-02-23 20:26:44.000000 core_curate_app-2.2.0/docs/conf_urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-02-23 20:26:45.000000 core_curate_app-2.2.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       62 2023-02-23 20:26:45.000000 core_curate_app-2.2.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-02-23 20:26:49.000000 core_curate_app-2.2.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1508 2023-02-23 20:26:45.000000 core_curate_app-2.2.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:49.000000 core_curate_app-2.2.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:45.000000 core_curate_app-2.2.0/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:49.000000 core_curate_app-2.2.0/tests/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:45.000000 core_curate_app-2.2.0/tests/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:49.000000 core_curate_app-2.2.0/tests/components/curate_data_structure/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:45.000000 core_curate_app-2.2.0/tests/components/curate_data_structure/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:49.000000 core_curate_app-2.2.0/tests/components/curate_data_structure/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:45.000000 core_curate_app-2.2.0/tests/components/curate_data_structure/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2541 2023-02-23 20:26:45.000000 core_curate_app-2.2.0/tests/components/curate_data_structure/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    19351 2023-02-23 20:26:45.000000 core_curate_app-2.2.0/tests/components/curate_data_structure/tests_int_access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11642 2023-02-23 20:26:45.000000 core_curate_app-2.2.0/tests/components/curate_data_structure/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:49.000000 core_curate_app-2.2.0/tests/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:45.000000 core_curate_app-2.2.0/tests/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:49.000000 core_curate_app-2.2.0/tests/rest/curate_data_structure/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:45.000000 core_curate_app-2.2.0/tests/rest/curate_data_structure/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11307 2023-02-23 20:26:45.000000 core_curate_app-2.2.0/tests/rest/curate_data_structure/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    13049 2023-02-23 20:26:45.000000 core_curate_app-2.2.0/tests/rest/curate_data_structure/tests_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1687 2023-02-23 20:26:45.000000 core_curate_app-2.2.0/tests/test_settings.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3653 2023-02-23 20:26:45.000000 core_curate_app-2.2.0/tests/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:49.000000 core_curate_app-2.2.0/tests/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:26:45.000000 core_curate_app-2.2.0/tests/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1046 2023-02-23 20:26:45.000000 core_curate_app-2.2.0/tests/views/test_forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9676 2023-02-23 20:26:45.000000 core_curate_app-2.2.0/tests/views/tests_int_access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2995 2023-02-23 20:26:45.000000 core_curate_app-2.2.0/tests/views/tests_views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:41.925579 core_curate_app-2.3.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      138 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1016 2023-05-02 19:35:41.921128 core_curate_app-2.3.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      532 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:40.131051 core_curate_app-2.3.0/core_curate_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       73 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:40.228402 core_curate_app-2.3.0/core_curate_app/access_control/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/access_control/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2987 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/access_control/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1017 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/admin.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      478 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/apps.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:40.258601 core_curate_app-2.3.0/core_curate_app/common/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/common/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      207 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/common/exceptions.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:40.274563 core_curate_app-2.3.0/core_curate_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:40.333337 core_curate_app-2.3.0/core_curate_app/components/curate_data_structure/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/components/curate_data_structure/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      464 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/components/curate_data_structure/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4953 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/components/curate_data_structure/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5888 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/components/curate_data_structure/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      233 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/menus.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:40.363319 core_curate_app-2.3.0/core_curate_app/migrations/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2186 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/migrations/0001_initial.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/migrations/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      738 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:40.416331 core_curate_app-2.3.0/core_curate_app/permissions/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/permissions/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1306 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/permissions/discover.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      221 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/permissions/rights.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:40.452454 core_curate_app-2.3.0/core_curate_app/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:40.517094 core_curate_app-2.3.0/core_curate_app/rest/curate_data_structure/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/rest/curate_data_structure/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1396 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/rest/curate_data_structure/admin_serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2131 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/rest/curate_data_structure/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11996 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/rest/curate_data_structure/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      668 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/rest/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1174 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:39.767322 core_curate_app-2.3.0/core_curate_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:39.770696 core_curate_app-2.3.0/core_curate_app/static/core_curate_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:39.784551 core_curate_app-2.3.0/core_curate_app/static/core_curate_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:40.673718 core_curate_app-2.3.0/core_curate_app/static/core_curate_app/user/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      481 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/static/core_curate_app/user/css/common.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2033 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/static/core_curate_app/user/css/style.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      683 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/static/core_curate_app/user/css/xsd_form.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:40.710049 core_curate_app-2.3.0/core_curate_app/static/core_curate_app/user/img/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      246 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/static/core_curate_app/user/img/collapse.png
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      253 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/static/core_curate_app/user/img/expand.png
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:40.974284 core_curate_app-2.3.0/core_curate_app/static/core_curate_app/user/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      157 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/static/core_curate_app/user/js/buttons.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       89 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/static/core_curate_app/user/js/choice.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      168 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/static/core_curate_app/user/js/download.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9748 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/static/core_curate_app/user/js/enter_data.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      357 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/static/core_curate_app/user/js/enter_data.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6638 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/static/core_curate_app/user/js/select_template.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      121 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/static/core_curate_app/user/js/select_template.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       81 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/static/core_curate_app/user/js/text_editor.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1083 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/static/core_curate_app/user/js/view_data.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      108 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/static/core_curate_app/user/js/view_data.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3595 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/static/core_curate_app/user/js/xml_entities_tooltip.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:39.795538 core_curate_app-2.3.0/core_curate_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:39.809405 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:41.010326 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      366 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/admin/detail.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      348 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/admin/view_curate_data_structure.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:41.045981 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/common/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      167 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/common/detail_curate_data_structure.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      173 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/common/tools_curate_data_structure.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:41.147903 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     1266 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/curate.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1191 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/curate_full_start.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      628 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/curate_start.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:41.171407 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/data-entry/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1854 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/data-entry/enter_data.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:41.314778 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      575 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/cancel-changes.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      671 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/cancel-form.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      579 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/clear-fields.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1137 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/download-options.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      549 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/save-form.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      857 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/use-validation.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      361 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/validation-warning.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      383 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/xml-error.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      702 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/xml-valid.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:41.330408 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/data-review/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:41.346074 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/data-review/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      376 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/data-review/modals/save-error.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      973 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/data-review/view_data.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      318 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/detail.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       32 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/errors.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:41.362487 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      207 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/list/list.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3259 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/core_curate_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:41.397655 core_curate_app-2.3.0/core_curate_app/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/core_curate_app/utils/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      764 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/core_curate_app/utils/parser.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:41.419642 core_curate_app-2.3.0/core_curate_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/core_curate_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:41.462331 core_curate_app-2.3.0/core_curate_app/views/common/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/core_curate_app/views/common/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7151 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/core_curate_app/views/common/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:41.535393 core_curate_app-2.3.0/core_curate_app/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/core_curate_app/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    19505 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/core_curate_app/views/user/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2923 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/core_curate_app/views/user/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    19644 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/core_curate_app/views/user/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:40.200031 core_curate_app-2.3.0/core_curate_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1016 2023-05-02 19:35:39.000000 core_curate_app-2.3.0/core_curate_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5075 2023-05-02 19:35:39.000000 core_curate_app-2.3.0/core_curate_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:35:39.000000 core_curate_app-2.3.0/core_curate_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       88 2023-05-02 19:35:39.000000 core_curate_app-2.3.0/core_curate_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       27 2023-05-02 19:35:39.000000 core_curate_app-2.3.0/core_curate_app.egg-info/top_level.txt
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:41.583020 core_curate_app-2.3.0/docs/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/docs/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11286 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/docs/conf.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      283 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/docs/conf_urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       62 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:35:41.927206 core_curate_app-2.3.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1508 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:41.631082 core_curate_app-2.3.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:41.647068 core_curate_app-2.3.0/tests/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/tests/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:41.704787 core_curate_app-2.3.0/tests/components/curate_data_structure/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/tests/components/curate_data_structure/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:41.755722 core_curate_app-2.3.0/tests/components/curate_data_structure/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/tests/components/curate_data_structure/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2541 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/tests/components/curate_data_structure/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    19295 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/tests/components/curate_data_structure/tests_int_access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11642 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/tests/components/curate_data_structure/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:41.782599 core_curate_app-2.3.0/tests/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/tests/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:41.835129 core_curate_app-2.3.0/tests/rest/curate_data_structure/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/tests/rest/curate_data_structure/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11287 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/tests/rest/curate_data_structure/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    13049 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/tests/rest/curate_data_structure/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1687 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/tests/test_settings.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3522 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/tests/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:41.896044 core_curate_app-2.3.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/tests/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1046 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/tests/views/test_forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9661 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/tests/views/tests_int_access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2995 2023-05-02 19:35:38.000000 core_curate_app-2.3.0/tests/views/tests_views.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `core_curate_app-2.2.0/PKG-INFO` & `core_curate_app-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_curate_app
-Version: 2.2.0
+Version: 2.3.0
 Summary: Curation functionalities for the curator core project
 Home-page: https://github.com/usnistgov/core_curate_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: ===============
         Core Curate App
```

### Comparing `core_curate_app-2.2.0/README.rst` & `core_curate_app-2.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.2.0/core_curate_app/access_control/api.py` & `core_curate_app-2.3.0/core_curate_app/access_control/api.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.2.0/core_curate_app/admin.py` & `core_curate_app-2.3.0/core_curate_app/admin.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.2.0/core_curate_app/components/curate_data_structure/api.py` & `core_curate_app-2.3.0/core_curate_app/components/curate_data_structure/api.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.2.0/core_curate_app/components/curate_data_structure/models.py` & `core_curate_app-2.3.0/core_curate_app/components/curate_data_structure/models.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.2.0/core_curate_app/migrations/0001_initial.py` & `core_curate_app-2.3.0/core_curate_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.2.0/core_curate_app/models.py` & `core_curate_app-2.3.0/core_curate_app/models.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.2.0/core_curate_app/permissions/discover.py` & `core_curate_app-2.3.0/core_curate_app/permissions/discover.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.2.0/core_curate_app/rest/curate_data_structure/admin_serializers.py` & `core_curate_app-2.3.0/core_curate_app/rest/curate_data_structure/admin_serializers.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.2.0/core_curate_app/rest/curate_data_structure/serializers.py` & `core_curate_app-2.3.0/core_curate_app/rest/curate_data_structure/serializers.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.2.0/core_curate_app/rest/curate_data_structure/views.py` & `core_curate_app-2.3.0/core_curate_app/rest/curate_data_structure/views.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.2.0/core_curate_app/rest/urls.py` & `core_curate_app-2.3.0/core_curate_app/rest/urls.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.2.0/core_curate_app/settings.py` & `core_curate_app-2.3.0/core_curate_app/settings.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.2.0/core_curate_app/static/core_curate_app/user/css/style.css` & `core_curate_app-2.3.0/core_curate_app/static/core_curate_app/user/css/style.css`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.2.0/core_curate_app/static/core_curate_app/user/css/xsd_form.css` & `core_curate_app-2.3.0/core_curate_app/static/core_curate_app/user/css/xsd_form.css`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.2.0/core_curate_app/static/core_curate_app/user/js/enter_data.js` & `core_curate_app-2.3.0/core_curate_app/static/core_curate_app/user/js/enter_data.js`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.2.0/core_curate_app/static/core_curate_app/user/js/select_template.js` & `core_curate_app-2.3.0/core_curate_app/static/core_curate_app/user/js/select_template.js`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.2.0/core_curate_app/static/core_curate_app/user/js/view_data.js` & `core_curate_app-2.3.0/core_curate_app/static/core_curate_app/user/js/view_data.js`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.2.0/core_curate_app/static/core_curate_app/user/js/xml_entities_tooltip.js` & `core_curate_app-2.3.0/core_curate_app/static/core_curate_app/user/js/xml_entities_tooltip.js`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.2.0/core_curate_app/templates/core_curate_app/user/curate.html` & `core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/curate.html`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.2.0/core_curate_app/templates/core_curate_app/user/curate_full_start.html` & `core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/curate_full_start.html`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.2.0/core_curate_app/templates/core_curate_app/user/curate_start.html` & `core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/curate_start.html`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.2.0/core_curate_app/templates/core_curate_app/user/data-entry/enter_data.html` & `core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/data-entry/enter_data.html`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.2.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/cancel-changes.html` & `core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/cancel-changes.html`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.2.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/cancel-form.html` & `core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/cancel-form.html`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.2.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/clear-fields.html` & `core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/clear-fields.html`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.2.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/download-options.html` & `core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/download-options.html`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.2.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/save-form.html` & `core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/save-form.html`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.2.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/use-validation.html` & `core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/use-validation.html`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.2.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/xml-valid.html` & `core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/xml-valid.html`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.2.0/core_curate_app/templates/core_curate_app/user/data-review/view_data.html` & `core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/data-review/view_data.html`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.2.0/core_curate_app/urls.py` & `core_curate_app-2.3.0/core_curate_app/urls.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """ Url router for the curate application
 """
 from django.conf.urls import include
-from django.urls import re_path, reverse_lazy
-from core_main_app.utils.decorators import permission_required
-from core_curate_app.permissions import rights
+from django.urls import re_path
+
 import core_curate_app.views.user.ajax as user_ajax
 import core_curate_app.views.user.views as user_views
+from core_curate_app.permissions import rights
 from core_curate_app.views.common import views as common_views
-
+from core_main_app.utils.decorators import permission_required
 
 urlpatterns = [
     re_path(r"^$", user_views.index, name="core_curate_index"),
     re_path(
         r"^start_curate$", user_ajax.start_curate, name="core_curate_start"
     ),
     re_path(
@@ -70,15 +70,14 @@
         r"^cancel-form$", user_ajax.cancel_form, name="core_curate_cancel_form"
     ),
     re_path(
         r"^xml-editor/form",
         permission_required(
             content_type=rights.CURATE_CONTENT_TYPE,
             permission=rights.CURATE_DATA_STRUCTURE_ACCESS,
-            login_url=reverse_lazy("core_main_app_login"),
         )(common_views.DraftContentEditor.as_view()),
         name="core_curate_app_xml_text_editor_view",
     ),
     re_path(r"^save-form$", user_ajax.save_form, name="core_curate_save_form"),
     re_path(r"^save-data$", user_ajax.save_data, name="core_curate_save_data"),
     re_path(
         r"^validate-form$",
@@ -86,13 +85,12 @@
         name="core_curate_validate_form",
     ),
     re_path(
         r"^view-form/(?P<curate_data_structure_id>\w+)$",
         permission_required(
             content_type=rights.CURATE_CONTENT_TYPE,
             permission=rights.CURATE_ACCESS,
-            login_url=reverse_lazy("core_main_app_login"),
         )(common_views.FormView.as_view()),
         name="core_curate_view_form",
     ),
     re_path(r"^rest/", include("core_curate_app.rest.urls")),
 ]
```

### Comparing `core_curate_app-2.2.0/core_curate_app/utils/parser.py` & `core_curate_app-2.3.0/core_curate_app/utils/parser.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.2.0/core_curate_app/views/common/views.py` & `core_curate_app-2.3.0/core_curate_app/views/common/views.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.2.0/core_curate_app/views/user/ajax.py` & `core_curate_app-2.3.0/core_curate_app/views/user/ajax.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.2.0/core_curate_app/views/user/forms.py` & `core_curate_app-2.3.0/core_curate_app/views/user/forms.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.2.0/core_curate_app/views/user/views.py` & `core_curate_app-2.3.0/core_curate_app/views/user/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,61 +2,58 @@
 """
 import logging
 from builtins import any
 from typing import Dict, List
 
 from django.contrib import messages
 from django.http import HttpResponseRedirect
-from django.urls import reverse_lazy, reverse
+from django.urls import reverse
 from django.utils.decorators import method_decorator
 from django.views import View
 
-import core_main_app.components.template_version_manager.api as template_version_manager_api
 import core_main_app.components.template.api as template_api
-from core_main_app.components.lock import api as lock_api
-from core_main_app.utils import decorators
+import core_main_app.components.template_version_manager.api as template_version_manager_api
+from core_curate_app.components.curate_data_structure import (
+    api as curate_data_structure_api,
+)
+from core_curate_app.permissions import rights
+from core_curate_app.settings import (
+    INSTALLED_APPS,
+    ENABLE_XML_ENTITIES_TOOLTIPS,
+)
+from core_curate_app.utils.parser import get_parser
+from core_main_app.access_control.api import check_can_write
+from core_main_app.access_control.exceptions import AccessControlError
 from core_main_app.commons.exceptions import (
     LockError,
     ModelError,
     DoesNotExist,
 )
-from core_main_app.access_control.exceptions import AccessControlError
-from core_main_app.access_control.api import check_can_write
-
+from core_main_app.components.lock import api as lock_api
+from core_main_app.utils import decorators
+from core_main_app.utils.boolean import to_bool
 from core_main_app.utils.file import get_file_http_response
 from core_main_app.utils.labels import get_form_label
 from core_main_app.utils.rendering import render
-from core_main_app.utils.boolean import to_bool
 from core_main_app.utils.xml import format_content_xml
 from core_parser_app.components.data_structure_element import (
     api as data_structure_element_api,
 )
 from core_parser_app.tools.parser.exceptions import ParserError
 from core_parser_app.tools.parser.renderer.list import ListRenderer
 from core_parser_app.tools.parser.renderer.xml import XmlRenderer
 
-from core_curate_app.components.curate_data_structure import (
-    api as curate_data_structure_api,
-)
-from core_curate_app.permissions import rights
-from core_curate_app.settings import (
-    INSTALLED_APPS,
-    ENABLE_XML_ENTITIES_TOOLTIPS,
-)
-from core_curate_app.utils.parser import get_parser
-
 logger = logging.getLogger(__name__)
 
 # TODO: Add a view for the registry. Ajax code need to be refactored
 
 
 @decorators.permission_required(
     content_type=rights.CURATE_CONTENT_TYPE,
     permission=rights.CURATE_ACCESS,
-    login_url=reverse_lazy("core_main_app_login"),
 )
 def index(request):
     """Page that allows to select a template to start curating.
 
     Args:
         request:
 
@@ -223,15 +220,14 @@
             "data_structure": curate_data_structure,
         }
 
     @method_decorator(
         decorators.permission_required(
             content_type=rights.CURATE_CONTENT_TYPE,
             permission=rights.CURATE_ACCESS,
-            login_url=reverse_lazy("core_main_app_login"),
         )
     )
     def get(
         self, request, curate_data_structure_id, reload_unsaved_changes=False
     ):
         """Load view to enter data.
 
@@ -380,15 +376,14 @@
             "data_structure": curate_data_structure,
         }
 
     @method_decorator(
         decorators.permission_required(
             content_type=rights.CURATE_CONTENT_TYPE,
             permission=rights.CURATE_ACCESS,
-            login_url=reverse_lazy("core_main_app_login"),
         )
     )
     def get(self, request, curate_data_structure_id):
         """Get data view
 
         Args:
             request:
@@ -438,15 +433,14 @@
                 context={"errors": str(exception), "page_title": "Error"},
             )
 
 
 @decorators.permission_required(
     content_type=rights.CURATE_CONTENT_TYPE,
     permission=rights.CURATE_ACCESS,
-    login_url=reverse_lazy("core_main_app_login"),
 )
 def download_current_xml(request, curate_data_structure_id):
     """Make the current XML document available for download.
 
     Args:
         request:
         curate_data_structure_id:
@@ -479,15 +473,14 @@
         extension="xml",
     )
 
 
 @decorators.permission_required(
     content_type=rights.CURATE_CONTENT_TYPE,
     permission=rights.CURATE_ACCESS,
-    login_url=reverse_lazy("core_main_app_login"),
 )
 def download_xsd(request, curate_data_structure_id):
     """Make the current XSD available for download.
 
     Args:
         request:
         curate_data_structure_id:
```

### Comparing `core_curate_app-2.2.0/core_curate_app.egg-info/PKG-INFO` & `core_curate_app-2.3.0/core_curate_app.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-curate-app
-Version: 2.2.0
+Version: 2.3.0
 Summary: Curation functionalities for the curator core project
 Home-page: https://github.com/usnistgov/core_curate_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: ===============
         Core Curate App
```

### Comparing `core_curate_app-2.2.0/core_curate_app.egg-info/SOURCES.txt` & `core_curate_app-2.3.0/core_curate_app.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+LICENSE.md
+MANIFEST.in
 README.rst
 pyproject.toml
 requirements.core.txt
 setup.py
 core_curate_app/__init__.py
 core_curate_app/admin.py
 core_curate_app/apps.py
```

### Comparing `core_curate_app-2.2.0/docs/conf.py` & `core_curate_app-2.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.2.0/setup.py` & `core_curate_app-2.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 chdir(normpath(join(abspath(__file__), pardir)))
 
 dep_links = [r for r in required if r.startswith("https://")]
 required = [req_link(r) if r.startswith("https://") else r for r in required]
 
 setup(
     name="core_curate_app",
-    version="2.2.0",
+    version="2.3.0",
     description="Curation functionalities for the curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_curate_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_curate_app-2.2.0/tests/components/curate_data_structure/fixtures/fixtures.py` & `core_curate_app-2.3.0/tests/components/curate_data_structure/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.2.0/tests/components/curate_data_structure/tests_int_access_control.py` & `core_curate_app-2.3.0/tests/components/curate_data_structure/tests_int_access_control.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """ ACL Test Data Structure
 """
 from django.contrib.auth.models import AnonymousUser
 from core_main_app.access_control.exceptions import AccessControlError
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from core_parser_app.components.data_structure.models import (
     DataStructureElement,
 )
 from core_curate_app.components.curate_data_structure.models import (
     CurateDataStructure,
@@ -18,15 +18,15 @@
     DataStructureFixtures,
 )
 
 
 fixture_data_structure = DataStructureFixtures()
 
 
-class TestCurateDataStructureGetById(MongoIntegrationBaseTestCase):
+class TestCurateDataStructureGetById(IntegrationBaseTestCase):
     """
     Test Curate Data Structure Get ById
     """
 
     fixture = fixture_data_structure
 
     def test_get_by_id_as_superuser_returns_data_structure(self):
@@ -83,15 +83,15 @@
         data_structure_id = self.fixture.data_structure_1.id
         with self.assertRaises(AccessControlError):
             curate_data_structure_api.get_by_id(
                 data_structure_id, AnonymousUser()
             )
 
 
-class TestCurateDataStructureGetAll(MongoIntegrationBaseTestCase):
+class TestCurateDataStructureGetAll(IntegrationBaseTestCase):
     """
     Test Curate Data Structure Get All
     """
 
     fixture = fixture_data_structure
 
     def test_get_all_as_superuser_returns_all_data_structure(self):
@@ -126,15 +126,15 @@
 
         """
         with self.assertRaises(AccessControlError):
             curate_data_structure_api.get_all(AnonymousUser())
 
 
 class TestCurateDataStructureGetAllExceptUserIdWithNoData(
-    MongoIntegrationBaseTestCase
+    IntegrationBaseTestCase
 ):
     """
     Test Curate Data Structure Get All Except User Id With No Data
     """
 
     fixture = fixture_data_structure
 
@@ -189,15 +189,15 @@
         user_id = self.fixture.data_structure_3.user
         with self.assertRaises(AccessControlError):
             curate_data_structure_api.get_all_except_user_id_with_no_data(
                 user_id, AnonymousUser()
             )
 
 
-class TestCurateDataStructureDelete(MongoIntegrationBaseTestCase):
+class TestCurateDataStructureDelete(IntegrationBaseTestCase):
     """
     Test Curate Data Structure Delete
     """
 
     fixture = fixture_data_structure
 
     def test_delete_others_data_structure_as_superuser_deletes_data_structure(
@@ -248,17 +248,15 @@
 
         """
         data_structure = self.fixture.data_structure_3
         with self.assertRaises(AccessControlError):
             curate_data_structure_api.delete(data_structure, AnonymousUser())
 
 
-class TestCurateDataStructureUpdateDataStructureRoot(
-    MongoIntegrationBaseTestCase
-):
+class TestCurateDataStructureUpdateDataStructureRoot(IntegrationBaseTestCase):
     """
     Test Curate Data Structure Update Data Structure Root
     """
 
     fixture = fixture_data_structure
 
     def test_update_others_data_structure_root_as_superuser_updates_data_structure(
@@ -337,15 +335,15 @@
             curate_data_structure_api.update_data_structure_root(
                 data_structure,
                 new_data_structure_element_root,
                 AnonymousUser(),
             )
 
 
-class TestCurateDataStructureCreateOrUpdate(MongoIntegrationBaseTestCase):
+class TestCurateDataStructureCreateOrUpdate(IntegrationBaseTestCase):
     """
     Test Curate Data Structure Create Or Update
     """
 
     fixture = fixture_data_structure
 
     def test_upsert_others_data_structure_as_superuser_updates_data_structure(
@@ -404,15 +402,15 @@
         """
         data_structure = self.fixture.data_structure_1
         data_structure.name = "new_name_1"
         with self.assertRaises(AccessControlError):
             curate_data_structure_api.upsert(data_structure, AnonymousUser())
 
 
-class TestCurateDataStructureGetAllWithNoData(MongoIntegrationBaseTestCase):
+class TestCurateDataStructureGetAllWithNoData(IntegrationBaseTestCase):
     """
     Test Curate Data Structure Get All With No Data
     """
 
     fixture = fixture_data_structure
 
     def test_get_all_with_no_data_as_superuser_returns_all_data_structure(
@@ -449,15 +447,15 @@
         Returns:
 
         """
         with self.assertRaises(AccessControlError):
             curate_data_structure_api.get_all_with_no_data(AnonymousUser())
 
 
-class TestCurateDataStructureGetByDataId(MongoIntegrationBaseTestCase):
+class TestCurateDataStructureGetByDataId(IntegrationBaseTestCase):
     """
     Test Curate Data Structure Get ById
     """
 
     fixture = fixture_data_structure
 
     def test_get_by_data_id_as_superuser_returns_data_structure(self):
@@ -515,15 +513,15 @@
         """
         with self.assertRaises(AccessControlError):
             curate_data_structure_api.get_by_data_id(
                 self.fixture.data.id, AnonymousUser()
             )
 
 
-class TestDataStructureChangeOwner(MongoIntegrationBaseTestCase):
+class TestDataStructureChangeOwner(IntegrationBaseTestCase):
     """
     Test Data Structure Change Owner
     """
 
     fixture = fixture_data_structure
 
     def test_change_owner_from_owner_to_owner_ok(self):
```

### Comparing `core_curate_app-2.2.0/tests/components/curate_data_structure/tests_unit.py` & `core_curate_app-2.3.0/tests/components/curate_data_structure/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.2.0/tests/rest/curate_data_structure/tests_int.py` & `core_curate_app-2.3.0/tests/rest/curate_data_structure/tests_int.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """ Integration Test for Data Structure Rest API
 """
 
 from rest_framework import status
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from core_main_app.utils.tests_tools.RequestMock import RequestMock
 from tests.components.curate_data_structure.fixtures.fixtures import (
     DataStructureFixtures,
 )
@@ -15,15 +15,15 @@
     views as data_structure_rest_views,
 )
 
 
 fixture_data_structure = DataStructureFixtures()
 
 
-class TestDataStructureListAdmin(MongoIntegrationBaseTestCase):
+class TestDataStructureListAdmin(IntegrationBaseTestCase):
     """
     Test Data Structure List Admin
     """
 
     fixture = fixture_data_structure
 
     def setUp(self):
@@ -114,15 +114,15 @@
             data=self.data,
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_400_BAD_REQUEST)
 
 
-class TestDataStructureList(MongoIntegrationBaseTestCase):
+class TestDataStructureList(IntegrationBaseTestCase):
     """
     Test Data Structure List
     """
 
     fixture = fixture_data_structure
 
     def setUp(self):
@@ -229,15 +229,15 @@
             data=self.data,
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_400_BAD_REQUEST)
 
 
-class TestDataStructureDetail(MongoIntegrationBaseTestCase):
+class TestDataStructureDetail(IntegrationBaseTestCase):
     """
     Test Data Structure Detail
     """
 
     fixture = fixture_data_structure
 
     def test_get_returns_http_200(self):
```

### Comparing `core_curate_app-2.2.0/tests/rest/curate_data_structure/tests_permissions.py` & `core_curate_app-2.3.0/tests/rest/curate_data_structure/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.2.0/tests/test_settings.py` & `core_curate_app-2.3.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.2.0/tests/urls.py` & `core_curate_app-2.3.0/tests/urls.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """ Url router for the curate application
 """
 from django.conf.urls import include
-from django.urls import re_path, reverse_lazy
 from django.contrib.auth.decorators import login_required
-from core_main_app.utils.decorators import permission_required
-from core_curate_app.permissions import rights
+from django.urls import re_path
+
 import core_curate_app.views.user.ajax as user_ajax
 import core_curate_app.views.user.views as user_views
+from core_curate_app.permissions import rights
 from core_curate_app.views.common import views as common_views
+from core_main_app.utils.decorators import permission_required
 from core_main_app.views.user import views as main_user_views
 
 urlpatterns = [
     re_path(r"^$", user_views.index, name="core_curate_index"),
     re_path(
         r"^start_curate$", user_ajax.start_curate, name="core_curate_start"
     ),
@@ -70,15 +71,14 @@
     re_path(
         r"^cancel-form$", user_ajax.cancel_form, name="core_curate_cancel_form"
     ),
     re_path(
         r"^xml-editor/form",
         login_required(
             common_views.DraftContentEditor.as_view(),
-            login_url=reverse_lazy("core_main_app_login"),
         ),
         name="core_curate_app_xml_text_editor_view",
     ),
     re_path(r"^save-form$", user_ajax.save_form, name="core_curate_save_form"),
     re_path(r"^save-data$", user_ajax.save_data, name="core_curate_save_data"),
     re_path(
         r"^save-record$", user_ajax.save_data, name="core_dashboard_records"
@@ -89,15 +89,14 @@
         name="core_curate_validate_form",
     ),
     re_path(
         r"^view-form/(?P<curate_data_structure_id>\w+)$",
         permission_required(
             content_type=rights.CURATE_CONTENT_TYPE,
             permission=rights.CURATE_ACCESS,
-            login_url=reverse_lazy("core_main_app_login"),
         )(common_views.FormView.as_view()),
         name="core_curate_view_form",
     ),
     re_path(r"^rest/", include("core_curate_app.rest.urls")),
     re_path(r"^tz_detect/", include("tz_detect.urls")),
     re_path(
         r"^login", main_user_views.custom_login, name="core_main_app_login"
```

### Comparing `core_curate_app-2.2.0/tests/views/test_forms.py` & `core_curate_app-2.3.0/tests/views/test_forms.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.2.0/tests/views/tests_int_access_control.py` & `core_curate_app-2.3.0/tests/views/tests_int_access_control.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 from tests.components.curate_data_structure.fixtures.fixtures import (
     DataStructureFixtures,
 )
 
 from core_curate_app.views.common.views import DraftContentEditor
 from core_curate_app.views.user import ajax as curate_ajax
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 
 fixture_data_structure = DataStructureFixtures()
 
 
-class TestDraftContentEditorView(MongoIntegrationBaseTestCase):
+class TestDraftContentEditorView(IntegrationBaseTestCase):
     """Test Draft Content Editor View"""
 
     def setUp(self):
         """setUp
 
         Returns:
 
@@ -172,15 +172,15 @@
             "core_curate_app_xml_text_editor_view", data
         )
         request.user = self.user1
         response = DraftContentEditor.as_view()(request)
         self.assertEqual(response.status_code, 400)
 
 
-class TestStartCuratePost(MongoIntegrationBaseTestCase):
+class TestStartCuratePost(IntegrationBaseTestCase):
     """Test Start Curate Post"""
 
     def setUp(self):
         """setUp
 
         Returns:
```

### Comparing `core_curate_app-2.2.0/tests/views/tests_views.py` & `core_curate_app-2.3.0/tests/views/tests_views.py`

 * *Files identical despite different names*

