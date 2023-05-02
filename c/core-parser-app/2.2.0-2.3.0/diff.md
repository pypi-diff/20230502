# Comparing `tmp/core_parser_app-2.2.0.tar.gz` & `tmp/core_parser_app-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/core_parser_app-2.2.0.tar", last modified: Thu Feb 23 20:34:21 2023, max compression
+gzip compressed data, was "core_parser_app-2.3.0.tar", last modified: Tue May  2 19:48:03 2023, max compression
```

## Comparing `core_parser_app-2.2.0.tar` & `core_parser_app-2.3.0.tar`

### file list

```diff
@@ -1,248 +1,249 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:21.000000 core_parser_app-2.2.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      395 2023-02-23 20:34:10.000000 core_parser_app-2.2.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2332 2023-02-23 20:34:21.000000 core_parser_app-2.2.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1696 2023-02-23 20:34:10.000000 core_parser_app-2.2.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:18.000000 core_parser_app-2.2.0/core_parser_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       64 2023-02-23 20:34:10.000000 core_parser_app-2.2.0/core_parser_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4397 2023-02-23 20:34:10.000000 core_parser_app-2.2.0/core_parser_app/access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1411 2023-02-23 20:34:10.000000 core_parser_app-2.2.0/core_parser_app/admin.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      205 2023-02-23 20:34:10.000000 core_parser_app-2.2.0/core_parser_app/apps.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:18.000000 core_parser_app-2.2.0/core_parser_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:10.000000 core_parser_app-2.2.0/core_parser_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:18.000000 core_parser_app-2.2.0/core_parser_app/components/data_structure/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:10.000000 core_parser_app-2.2.0/core_parser_app/components/data_structure/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      376 2023-02-23 20:34:10.000000 core_parser_app-2.2.0/core_parser_app/components/data_structure/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      304 2023-02-23 20:34:10.000000 core_parser_app-2.2.0/core_parser_app/components/data_structure/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6887 2023-02-23 20:34:10.000000 core_parser_app-2.2.0/core_parser_app/components/data_structure/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:18.000000 core_parser_app-2.2.0/core_parser_app/components/data_structure_element/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:10.000000 core_parser_app-2.2.0/core_parser_app/components/data_structure_element/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      398 2023-02-23 20:34:10.000000 core_parser_app-2.2.0/core_parser_app/components/data_structure_element/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2871 2023-02-23 20:34:10.000000 core_parser_app-2.2.0/core_parser_app/components/data_structure_element/api.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:18.000000 core_parser_app-2.2.0/core_parser_app/components/module/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:10.000000 core_parser_app-2.2.0/core_parser_app/components/module/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      353 2023-02-23 20:34:10.000000 core_parser_app-2.2.0/core_parser_app/components/module/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1862 2023-02-23 20:34:10.000000 core_parser_app-2.2.0/core_parser_app/components/module/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1887 2023-02-23 20:34:10.000000 core_parser_app-2.2.0/core_parser_app/components/module/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:18.000000 core_parser_app-2.2.0/core_parser_app/migrations/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3972 2023-02-23 20:34:10.000000 core_parser_app-2.2.0/core_parser_app/migrations/0001_initial.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:10.000000 core_parser_app-2.2.0/core_parser_app/migrations/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      811 2023-02-23 20:34:10.000000 core_parser_app-2.2.0/core_parser_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:18.000000 core_parser_app-2.2.0/core_parser_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:18.000000 core_parser_app-2.2.0/core_parser_app/static/core_parser_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:18.000000 core_parser_app-2.2.0/core_parser_app/static/core_parser_app/common/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:19.000000 core_parser_app-2.2.0/core_parser_app/static/core_parser_app/common/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       89 2023-02-23 20:34:10.000000 core_parser_app-2.2.0/core_parser_app/static/core_parser_app/common/css/modules.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:19.000000 core_parser_app-2.2.0/core_parser_app/static/core_parser_app/common/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3620 2023-02-23 20:34:10.000000 core_parser_app-2.2.0/core_parser_app/static/core_parser_app/common/js/module_manager.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      169 2023-02-23 20:34:10.000000 core_parser_app-2.2.0/core_parser_app/static/core_parser_app/common/js/module_manager.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:19.000000 core_parser_app-2.2.0/core_parser_app/static/core_parser_app/common/xsd/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2306 2023-02-23 20:34:10.000000 core_parser_app-2.2.0/core_parser_app/static/core_parser_app/common/xsd/annotations.xsd
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      996 2023-02-23 20:34:10.000000 core_parser_app-2.2.0/core_parser_app/static/core_parser_app/common/xsd/boolean.xsd
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      996 2023-02-23 20:34:10.000000 core_parser_app-2.2.0/core_parser_app/static/core_parser_app/common/xsd/date.xsd
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:19.000000 core_parser_app-2.2.0/core_parser_app/system/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:10.000000 core_parser_app-2.2.0/core_parser_app/system/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      533 2023-02-23 20:34:10.000000 core_parser_app-2.2.0/core_parser_app/system/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      346 2023-02-23 20:34:10.000000 core_parser_app-2.2.0/core_parser_app/tasks.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:18.000000 core_parser_app-2.2.0/core_parser_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:18.000000 core_parser_app-2.2.0/core_parser_app/templates/core_parser_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:19.000000 core_parser_app-2.2.0/core_parser_app/templates/core_parser_app/common/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:19.000000 core_parser_app-2.2.0/core_parser_app/templates/core_parser_app/common/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      968 2023-02-23 20:34:10.000000 core_parser_app-2.2.0/core_parser_app/templates/core_parser_app/common/modals/add_module.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      268 2023-02-23 20:34:10.000000 core_parser_app-2.2.0/core_parser_app/templates/core_parser_app/common/module_manager.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      695 2023-02-23 20:34:10.000000 core_parser_app-2.2.0/core_parser_app/templates/core_parser_app/common/module_manager_box.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      473 2023-02-23 20:34:10.000000 core_parser_app-2.2.0/core_parser_app/templates/core_parser_app/common/modules.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:19.000000 core_parser_app-2.2.0/core_parser_app/tools/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:10.000000 core_parser_app-2.2.0/core_parser_app/tools/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:19.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:10.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2823 2023-02-23 20:34:10.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/discover.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      182 2023-02-23 20:34:10.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/exceptions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1825 2023-02-23 20:34:10.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/sanitize.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:18.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:18.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/static/core_parser_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:18.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/static/core_parser_app/css/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:19.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/static/core_parser_app/css/builtin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       86 2023-02-23 20:34:10.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/static/core_parser_app/css/builtin/checkboxes.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      128 2023-02-23 20:34:10.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/static/core_parser_app/css/builtin/textarea.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:19.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/static/core_parser_app/js/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:19.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/static/core_parser_app/js/builtin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      128 2023-02-23 20:34:10.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/static/core_parser_app/js/builtin/autocomplete.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      412 2023-02-23 20:34:10.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/static/core_parser_app/js/builtin/checkboxes.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      265 2023-02-23 20:34:10.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/static/core_parser_app/js/builtin/input.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      227 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/static/core_parser_app/js/builtin/options.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1379 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/static/core_parser_app/js/builtin/popup.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      240 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/static/core_parser_app/js/builtin/sync_input.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      229 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/static/core_parser_app/js/builtin/textarea.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:19.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/static/core_parser_app/js/commons/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      512 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/static/core_parser_app/js/commons/file_uploader.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3135 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/static/core_parser_app/js/modules.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       75 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/static/core_parser_app/js/modules.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:19.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/static/core_parser_app/xsl/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6048 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/static/core_parser_app/xsl/xsd2html4modules.xsl
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:18.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:19.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/templates/core_parser_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:19.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/templates/core_parser_app/builtin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      142 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/templates/core_parser_app/builtin/autocomplete.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      303 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/templates/core_parser_app/builtin/checkboxes.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      255 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/templates/core_parser_app/builtin/input.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      149 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/templates/core_parser_app/builtin/input_button.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      465 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/templates/core_parser_app/builtin/modal_wrapper.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      237 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/templates/core_parser_app/builtin/options.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      267 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/templates/core_parser_app/builtin/popup.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      254 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/templates/core_parser_app/builtin/sync_input.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      126 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/templates/core_parser_app/builtin/textarea.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:19.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/templates/core_parser_app/commons/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      236 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/templates/core_parser_app/commons/file_uploader.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      264 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/templates/core_parser_app/module.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      352 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:19.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:19.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/views/builtin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/views/builtin/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1022 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/views/builtin/autocomplete_module.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3012 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/views/builtin/checkboxes_module.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1253 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/views/builtin/input_button_module.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1533 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/views/builtin/input_module.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1882 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/views/builtin/options_module.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1300 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/views/builtin/popup_module.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1627 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/views/builtin/sync_input_module.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1011 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/views/builtin/textarea_module.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7675 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/views/module.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4172 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/views/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3201 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/modules/xpathaccessor.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:19.000000 core_parser_app-2.2.0/core_parser_app/tools/parser/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/parser/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      326 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/parser/exceptions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)   117420 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/parser/parser.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:20.000000 core_parser_app-2.2.0/core_parser_app/tools/parser/renderer/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8336 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/parser/renderer/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      901 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/parser/renderer/checkbox.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    27098 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/parser/renderer/list.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10019 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/parser/renderer/table.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    24119 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/parser/renderer/xml.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:18.000000 core_parser_app-2.2.0/core_parser_app/tools/parser/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:18.000000 core_parser_app-2.2.0/core_parser_app/tools/parser/static/core_parser_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:20.000000 core_parser_app-2.2.0/core_parser_app/tools/parser/static/core_parser_app/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      958 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/parser/static/core_parser_app/css/use.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:20.000000 core_parser_app-2.2.0/core_parser_app/tools/parser/static/core_parser_app/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      934 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/parser/static/core_parser_app/js/autosave.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       89 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/parser/static/core_parser_app/js/autosave.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      882 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/parser/static/core_parser_app/js/autosave_checkbox.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4673 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/parser/static/core_parser_app/js/buttons.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5179 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/parser/static/core_parser_app/js/choice.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:18.000000 core_parser_app-2.2.0/core_parser_app/tools/parser/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:18.000000 core_parser_app-2.2.0/core_parser_app/tools/parser/templates/renderer/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:20.000000 core_parser_app-2.2.0/core_parser_app/tools/parser/templates/renderer/default/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:20.000000 core_parser_app-2.2.0/core_parser_app/tools/parser/templates/renderer/default/buttons/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       98 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/parser/templates/renderer/default/buttons/add.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       81 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/parser/templates/renderer/default/buttons/collapse.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      104 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/parser/templates/renderer/default/buttons/delete.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      110 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/parser/templates/renderer/default/form-error.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:20.000000 core_parser_app-2.2.0/core_parser_app/tools/parser/templates/renderer/default/inputs/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      346 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/parser/templates/renderer/default/inputs/boolean.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       76 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/parser/templates/renderer/default/inputs/checkbox.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      397 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/parser/templates/renderer/default/inputs/date.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      438 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/parser/templates/renderer/default/inputs/input.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      446 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/parser/templates/renderer/default/inputs/select.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:20.000000 core_parser_app-2.2.0/core_parser_app/tools/parser/templates/renderer/default/test/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       44 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/parser/templates/renderer/default/test/sample_no_data.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       52 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/parser/templates/renderer/default/test/sample_with_data.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       83 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/parser/templates/renderer/default/ul.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       86 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/parser/templates/renderer/default/warning.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:20.000000 core_parser_app-2.2.0/core_parser_app/tools/parser/templates/renderer/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      149 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/parser/templates/renderer/list/attributes.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       75 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/parser/templates/renderer/list/li.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      131 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/parser/templates/renderer/list/ul.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:20.000000 core_parser_app-2.2.0/core_parser_app/tools/parser/templates/renderer/table/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       99 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/parser/templates/renderer/table/table.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       75 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/parser/templates/renderer/table/tr.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       41 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/parser/templates/renderer/table/wrap.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:20.000000 core_parser_app-2.2.0/core_parser_app/tools/parser/templates/renderer/xml/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       99 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/parser/templates/renderer/xml/element.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:20.000000 core_parser_app-2.2.0/core_parser_app/tools/parser/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/parser/utils/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      278 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/parser/utils/rendering.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3519 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/tools/parser/utils/xml.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1075 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:20.000000 core_parser_app-2.2.0/core_parser_app/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/utils/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2190 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/utils/xml.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:20.000000 core_parser_app-2.2.0/core_parser_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:20.000000 core_parser_app-2.2.0/core_parser_app/views/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/views/admin/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1592 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/views/admin/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:20.000000 core_parser_app-2.2.0/core_parser_app/views/common/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/views/common/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1808 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/views/common/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3275 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/views/common/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:21.000000 core_parser_app-2.2.0/core_parser_app/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2477 2023-02-23 20:34:11.000000 core_parser_app-2.2.0/core_parser_app/views/user/ajax.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:18.000000 core_parser_app-2.2.0/core_parser_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2332 2023-02-23 20:34:17.000000 core_parser_app-2.2.0/core_parser_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9033 2023-02-23 20:34:18.000000 core_parser_app-2.2.0/core_parser_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-02-23 20:34:17.000000 core_parser_app-2.2.0/core_parser_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       85 2023-02-23 20:34:17.000000 core_parser_app-2.2.0/core_parser_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       22 2023-02-23 20:34:17.000000 core_parser_app-2.2.0/core_parser_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-02-23 20:34:12.000000 core_parser_app-2.2.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       39 2023-02-23 20:34:12.000000 core_parser_app-2.2.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       46 2023-02-23 20:34:12.000000 core_parser_app-2.2.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-02-23 20:34:21.000000 core_parser_app-2.2.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1441 2023-02-23 20:34:12.000000 core_parser_app-2.2.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:21.000000 core_parser_app-2.2.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:12.000000 core_parser_app-2.2.0/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:21.000000 core_parser_app-2.2.0/tests/access_control/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:12.000000 core_parser_app-2.2.0/tests/access_control/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2180 2023-02-23 20:34:12.000000 core_parser_app-2.2.0/tests/access_control/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:21.000000 core_parser_app-2.2.0/tests/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:12.000000 core_parser_app-2.2.0/tests/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:21.000000 core_parser_app-2.2.0/tests/components/data_structure/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:12.000000 core_parser_app-2.2.0/tests/components/data_structure/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:12.000000 core_parser_app-2.2.0/tests/components/data_structure/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1619 2023-02-23 20:34:12.000000 core_parser_app-2.2.0/tests/components/data_structure/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:21.000000 core_parser_app-2.2.0/tests/components/data_structure_element/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:12.000000 core_parser_app-2.2.0/tests/components/data_structure_element/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:21.000000 core_parser_app-2.2.0/tests/components/data_structure_element/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:12.000000 core_parser_app-2.2.0/tests/components/data_structure_element/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6725 2023-02-23 20:34:12.000000 core_parser_app-2.2.0/tests/components/data_structure_element/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    20139 2023-02-23 20:34:12.000000 core_parser_app-2.2.0/tests/components/data_structure_element/test_int_access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5889 2023-02-23 20:34:12.000000 core_parser_app-2.2.0/tests/components/data_structure_element/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4901 2023-02-23 20:34:12.000000 core_parser_app-2.2.0/tests/components/data_structure_element/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:21.000000 core_parser_app-2.2.0/tests/components/module/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:12.000000 core_parser_app-2.2.0/tests/components/module/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4771 2023-02-23 20:34:12.000000 core_parser_app-2.2.0/tests/components/module/tests_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1093 2023-02-23 20:34:12.000000 core_parser_app-2.2.0/tests/fixtures_utils.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      646 2023-02-23 20:34:12.000000 core_parser_app-2.2.0/tests/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      185 2023-02-23 20:34:12.000000 core_parser_app-2.2.0/tests/rights.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      998 2023-02-23 20:34:12.000000 core_parser_app-2.2.0/tests/test_settings.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2714 2023-02-23 20:34:12.000000 core_parser_app-2.2.0/tests/test_utils.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:21.000000 core_parser_app-2.2.0/tests/tools/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:12.000000 core_parser_app-2.2.0/tests/tools/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:21.000000 core_parser_app-2.2.0/tests/tools/modules/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:12.000000 core_parser_app-2.2.0/tests/tools/modules/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:21.000000 core_parser_app-2.2.0/tests/tools/modules/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:12.000000 core_parser_app-2.2.0/tests/tools/modules/tests/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2950 2023-02-23 20:34:12.000000 core_parser_app-2.2.0/tests/tools/modules/tests/tests_unit_checkboxes_module.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9401 2023-02-23 20:34:12.000000 core_parser_app-2.2.0/tests/tools/modules/tests/tests_unit_module.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2292 2023-02-23 20:34:12.000000 core_parser_app-2.2.0/tests/tools/modules/tests/tests_unit_sanitize.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:21.000000 core_parser_app-2.2.0/tests/tools/parser/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:12.000000 core_parser_app-2.2.0/tests/tools/parser/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:21.000000 core_parser_app-2.2.0/tests/tools/parser/parser/
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:15.000000 core_parser_app-2.2.0/tests/tools/parser/parser/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7131 2023-02-23 20:34:15.000000 core_parser_app-2.2.0/tests/tools/parser/parser/test_choice.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5010 2023-02-23 20:34:15.000000 core_parser_app-2.2.0/tests/tools/parser/parser/test_complex_content.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10789 2023-02-23 20:34:15.000000 core_parser_app-2.2.0/tests/tools/parser/parser/test_complex_type.py
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)    11082 2023-02-23 20:34:15.000000 core_parser_app-2.2.0/tests/tools/parser/parser/test_element.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8882 2023-02-23 20:34:15.000000 core_parser_app-2.2.0/tests/tools/parser/parser/test_extension.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      876 2023-02-23 20:34:15.000000 core_parser_app-2.2.0/tests/tools/parser/parser/test_parser.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3811 2023-02-23 20:34:15.000000 core_parser_app-2.2.0/tests/tools/parser/parser/test_restriction.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7071 2023-02-23 20:34:15.000000 core_parser_app-2.2.0/tests/tools/parser/parser/test_sequence.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:21.000000 core_parser_app-2.2.0/tests/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:15.000000 core_parser_app-2.2.0/tests/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:21.000000 core_parser_app-2.2.0/tests/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:15.000000 core_parser_app-2.2.0/tests/views/user/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:21.000000 core_parser_app-2.2.0/tests/views/user/ajax/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:15.000000 core_parser_app-2.2.0/tests/views/user/ajax/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1979 2023-02-23 20:34:15.000000 core_parser_app-2.2.0/tests/views/user/ajax/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5140 2023-02-23 20:34:15.000000 core_parser_app-2.2.0/tests/views/user/ajax/test_int_access_control.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:03.105097 core_parser_app-2.3.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:47:47.000000 core_parser_app-2.3.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      395 2023-05-02 19:47:47.000000 core_parser_app-2.3.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2332 2023-05-02 19:48:03.099934 core_parser_app-2.3.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1696 2023-05-02 19:47:47.000000 core_parser_app-2.3.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:00.057565 core_parser_app-2.3.0/core_parser_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       64 2023-05-02 19:47:47.000000 core_parser_app-2.3.0/core_parser_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4397 2023-05-02 19:47:47.000000 core_parser_app-2.3.0/core_parser_app/access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1411 2023-05-02 19:47:47.000000 core_parser_app-2.3.0/core_parser_app/admin.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      205 2023-05-02 19:47:47.000000 core_parser_app-2.3.0/core_parser_app/apps.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:00.141469 core_parser_app-2.3.0/core_parser_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:47.000000 core_parser_app-2.3.0/core_parser_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:00.206597 core_parser_app-2.3.0/core_parser_app/components/data_structure/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:47.000000 core_parser_app-2.3.0/core_parser_app/components/data_structure/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      376 2023-05-02 19:47:47.000000 core_parser_app-2.3.0/core_parser_app/components/data_structure/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      304 2023-05-02 19:47:47.000000 core_parser_app-2.3.0/core_parser_app/components/data_structure/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6887 2023-05-02 19:47:47.000000 core_parser_app-2.3.0/core_parser_app/components/data_structure/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:00.265717 core_parser_app-2.3.0/core_parser_app/components/data_structure_element/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:47.000000 core_parser_app-2.3.0/core_parser_app/components/data_structure_element/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      398 2023-05-02 19:47:47.000000 core_parser_app-2.3.0/core_parser_app/components/data_structure_element/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2871 2023-05-02 19:47:47.000000 core_parser_app-2.3.0/core_parser_app/components/data_structure_element/api.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:00.337338 core_parser_app-2.3.0/core_parser_app/components/module/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:47.000000 core_parser_app-2.3.0/core_parser_app/components/module/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      353 2023-05-02 19:47:47.000000 core_parser_app-2.3.0/core_parser_app/components/module/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1862 2023-05-02 19:47:47.000000 core_parser_app-2.3.0/core_parser_app/components/module/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1887 2023-05-02 19:47:47.000000 core_parser_app-2.3.0/core_parser_app/components/module/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:00.363780 core_parser_app-2.3.0/core_parser_app/migrations/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3972 2023-05-02 19:47:47.000000 core_parser_app-2.3.0/core_parser_app/migrations/0001_initial.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:47.000000 core_parser_app-2.3.0/core_parser_app/migrations/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      811 2023-05-02 19:47:47.000000 core_parser_app-2.3.0/core_parser_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:59.449626 core_parser_app-2.3.0/core_parser_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:59.453575 core_parser_app-2.3.0/core_parser_app/static/core_parser_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:59.497725 core_parser_app-2.3.0/core_parser_app/static/core_parser_app/common/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:00.394367 core_parser_app-2.3.0/core_parser_app/static/core_parser_app/common/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       89 2023-05-02 19:47:47.000000 core_parser_app-2.3.0/core_parser_app/static/core_parser_app/common/css/modules.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:00.425525 core_parser_app-2.3.0/core_parser_app/static/core_parser_app/common/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3620 2023-05-02 19:47:47.000000 core_parser_app-2.3.0/core_parser_app/static/core_parser_app/common/js/module_manager.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      169 2023-05-02 19:47:48.000000 core_parser_app-2.3.0/core_parser_app/static/core_parser_app/common/js/module_manager.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:00.473099 core_parser_app-2.3.0/core_parser_app/static/core_parser_app/common/xsd/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2306 2023-05-02 19:47:48.000000 core_parser_app-2.3.0/core_parser_app/static/core_parser_app/common/xsd/annotations.xsd
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      996 2023-05-02 19:47:48.000000 core_parser_app-2.3.0/core_parser_app/static/core_parser_app/common/xsd/boolean.xsd
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      996 2023-05-02 19:47:48.000000 core_parser_app-2.3.0/core_parser_app/static/core_parser_app/common/xsd/date.xsd
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:00.507577 core_parser_app-2.3.0/core_parser_app/system/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:48.000000 core_parser_app-2.3.0/core_parser_app/system/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      533 2023-05-02 19:47:48.000000 core_parser_app-2.3.0/core_parser_app/system/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      346 2023-05-02 19:47:48.000000 core_parser_app-2.3.0/core_parser_app/tasks.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:59.514796 core_parser_app-2.3.0/core_parser_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:59.517765 core_parser_app-2.3.0/core_parser_app/templates/core_parser_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:00.560709 core_parser_app-2.3.0/core_parser_app/templates/core_parser_app/common/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:00.577638 core_parser_app-2.3.0/core_parser_app/templates/core_parser_app/common/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      968 2023-05-02 19:47:48.000000 core_parser_app-2.3.0/core_parser_app/templates/core_parser_app/common/modals/add_module.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      268 2023-05-02 19:47:48.000000 core_parser_app-2.3.0/core_parser_app/templates/core_parser_app/common/module_manager.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      695 2023-05-02 19:47:48.000000 core_parser_app-2.3.0/core_parser_app/templates/core_parser_app/common/module_manager_box.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      473 2023-05-02 19:47:48.000000 core_parser_app-2.3.0/core_parser_app/templates/core_parser_app/common/modules.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:00.596759 core_parser_app-2.3.0/core_parser_app/tools/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:48.000000 core_parser_app-2.3.0/core_parser_app/tools/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:00.693035 core_parser_app-2.3.0/core_parser_app/tools/modules/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:48.000000 core_parser_app-2.3.0/core_parser_app/tools/modules/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2823 2023-05-02 19:47:48.000000 core_parser_app-2.3.0/core_parser_app/tools/modules/discover.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      182 2023-05-02 19:47:48.000000 core_parser_app-2.3.0/core_parser_app/tools/modules/exceptions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1825 2023-05-02 19:47:48.000000 core_parser_app-2.3.0/core_parser_app/tools/modules/sanitize.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:59.558232 core_parser_app-2.3.0/core_parser_app/tools/modules/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:59.585102 core_parser_app-2.3.0/core_parser_app/tools/modules/static/core_parser_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:59.565083 core_parser_app-2.3.0/core_parser_app/tools/modules/static/core_parser_app/css/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:00.736205 core_parser_app-2.3.0/core_parser_app/tools/modules/static/core_parser_app/css/builtin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       86 2023-05-02 19:47:48.000000 core_parser_app-2.3.0/core_parser_app/tools/modules/static/core_parser_app/css/builtin/checkboxes.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      128 2023-05-02 19:47:48.000000 core_parser_app-2.3.0/core_parser_app/tools/modules/static/core_parser_app/css/builtin/textarea.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:00.879015 core_parser_app-2.3.0/core_parser_app/tools/modules/static/core_parser_app/js/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:00.982368 core_parser_app-2.3.0/core_parser_app/tools/modules/static/core_parser_app/js/builtin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      128 2023-05-02 19:47:49.000000 core_parser_app-2.3.0/core_parser_app/tools/modules/static/core_parser_app/js/builtin/autocomplete.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      412 2023-05-02 19:47:49.000000 core_parser_app-2.3.0/core_parser_app/tools/modules/static/core_parser_app/js/builtin/checkboxes.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      265 2023-05-02 19:47:49.000000 core_parser_app-2.3.0/core_parser_app/tools/modules/static/core_parser_app/js/builtin/input.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      227 2023-05-02 19:47:49.000000 core_parser_app-2.3.0/core_parser_app/tools/modules/static/core_parser_app/js/builtin/options.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1379 2023-05-02 19:47:49.000000 core_parser_app-2.3.0/core_parser_app/tools/modules/static/core_parser_app/js/builtin/popup.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      240 2023-05-02 19:47:49.000000 core_parser_app-2.3.0/core_parser_app/tools/modules/static/core_parser_app/js/builtin/sync_input.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      229 2023-05-02 19:47:49.000000 core_parser_app-2.3.0/core_parser_app/tools/modules/static/core_parser_app/js/builtin/textarea.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:00.999752 core_parser_app-2.3.0/core_parser_app/tools/modules/static/core_parser_app/js/commons/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      512 2023-05-02 19:47:49.000000 core_parser_app-2.3.0/core_parser_app/tools/modules/static/core_parser_app/js/commons/file_uploader.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3135 2023-05-02 19:47:49.000000 core_parser_app-2.3.0/core_parser_app/tools/modules/static/core_parser_app/js/modules.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       75 2023-05-02 19:47:49.000000 core_parser_app-2.3.0/core_parser_app/tools/modules/static/core_parser_app/js/modules.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:01.015776 core_parser_app-2.3.0/core_parser_app/tools/modules/static/core_parser_app/xsl/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6048 2023-05-02 19:47:49.000000 core_parser_app-2.3.0/core_parser_app/tools/modules/static/core_parser_app/xsl/xsd2html4modules.xsl
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:59.594653 core_parser_app-2.3.0/core_parser_app/tools/modules/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:01.068269 core_parser_app-2.3.0/core_parser_app/tools/modules/templates/core_parser_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:01.215126 core_parser_app-2.3.0/core_parser_app/tools/modules/templates/core_parser_app/builtin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      142 2023-05-02 19:47:51.000000 core_parser_app-2.3.0/core_parser_app/tools/modules/templates/core_parser_app/builtin/autocomplete.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      303 2023-05-02 19:47:51.000000 core_parser_app-2.3.0/core_parser_app/tools/modules/templates/core_parser_app/builtin/checkboxes.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      255 2023-05-02 19:47:51.000000 core_parser_app-2.3.0/core_parser_app/tools/modules/templates/core_parser_app/builtin/input.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      149 2023-05-02 19:47:51.000000 core_parser_app-2.3.0/core_parser_app/tools/modules/templates/core_parser_app/builtin/input_button.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      465 2023-05-02 19:47:51.000000 core_parser_app-2.3.0/core_parser_app/tools/modules/templates/core_parser_app/builtin/modal_wrapper.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      237 2023-05-02 19:47:51.000000 core_parser_app-2.3.0/core_parser_app/tools/modules/templates/core_parser_app/builtin/options.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      267 2023-05-02 19:47:51.000000 core_parser_app-2.3.0/core_parser_app/tools/modules/templates/core_parser_app/builtin/popup.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      254 2023-05-02 19:47:51.000000 core_parser_app-2.3.0/core_parser_app/tools/modules/templates/core_parser_app/builtin/sync_input.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      126 2023-05-02 19:47:51.000000 core_parser_app-2.3.0/core_parser_app/tools/modules/templates/core_parser_app/builtin/textarea.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:01.232491 core_parser_app-2.3.0/core_parser_app/tools/modules/templates/core_parser_app/commons/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      236 2023-05-02 19:47:51.000000 core_parser_app-2.3.0/core_parser_app/tools/modules/templates/core_parser_app/commons/file_uploader.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      264 2023-05-02 19:47:51.000000 core_parser_app-2.3.0/core_parser_app/tools/modules/templates/core_parser_app/module.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      352 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/tools/modules/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:01.282775 core_parser_app-2.3.0/core_parser_app/tools/modules/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/tools/modules/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:01.437101 core_parser_app-2.3.0/core_parser_app/tools/modules/views/builtin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/tools/modules/views/builtin/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1022 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/tools/modules/views/builtin/autocomplete_module.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3012 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/tools/modules/views/builtin/checkboxes_module.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1253 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/tools/modules/views/builtin/input_button_module.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1533 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/tools/modules/views/builtin/input_module.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1882 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/tools/modules/views/builtin/options_module.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1300 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/tools/modules/views/builtin/popup_module.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1627 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/tools/modules/views/builtin/sync_input_module.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1011 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/tools/modules/views/builtin/textarea_module.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7675 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/tools/modules/views/module.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4172 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/tools/modules/views/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3201 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/tools/modules/xpathaccessor.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:01.491055 core_parser_app-2.3.0/core_parser_app/tools/parser/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/tools/parser/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      326 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/tools/parser/exceptions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)   117420 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/tools/parser/parser.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:01.570282 core_parser_app-2.3.0/core_parser_app/tools/parser/renderer/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8336 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/tools/parser/renderer/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      901 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/tools/parser/renderer/checkbox.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    27098 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/tools/parser/renderer/list.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10019 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/tools/parser/renderer/table.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    24119 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/tools/parser/renderer/xml.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:59.636277 core_parser_app-2.3.0/core_parser_app/tools/parser/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:59.645598 core_parser_app-2.3.0/core_parser_app/tools/parser/static/core_parser_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:01.594715 core_parser_app-2.3.0/core_parser_app/tools/parser/static/core_parser_app/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      958 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/tools/parser/static/core_parser_app/css/use.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:01.684582 core_parser_app-2.3.0/core_parser_app/tools/parser/static/core_parser_app/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      934 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/tools/parser/static/core_parser_app/js/autosave.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       89 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/tools/parser/static/core_parser_app/js/autosave.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      882 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/tools/parser/static/core_parser_app/js/autosave_checkbox.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4673 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/tools/parser/static/core_parser_app/js/buttons.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5179 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/tools/parser/static/core_parser_app/js/choice.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:59.664408 core_parser_app-2.3.0/core_parser_app/tools/parser/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:59.714064 core_parser_app-2.3.0/core_parser_app/tools/parser/templates/renderer/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:01.736634 core_parser_app-2.3.0/core_parser_app/tools/parser/templates/renderer/default/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:01.783382 core_parser_app-2.3.0/core_parser_app/tools/parser/templates/renderer/default/buttons/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       98 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/tools/parser/templates/renderer/default/buttons/add.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       81 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/tools/parser/templates/renderer/default/buttons/collapse.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      104 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/tools/parser/templates/renderer/default/buttons/delete.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      110 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/tools/parser/templates/renderer/default/form-error.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:01.852715 core_parser_app-2.3.0/core_parser_app/tools/parser/templates/renderer/default/inputs/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      346 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/tools/parser/templates/renderer/default/inputs/boolean.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       76 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/tools/parser/templates/renderer/default/inputs/checkbox.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      397 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/tools/parser/templates/renderer/default/inputs/date.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      438 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/tools/parser/templates/renderer/default/inputs/input.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      446 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/tools/parser/templates/renderer/default/inputs/select.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:01.884400 core_parser_app-2.3.0/core_parser_app/tools/parser/templates/renderer/default/test/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       44 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/tools/parser/templates/renderer/default/test/sample_no_data.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       52 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/tools/parser/templates/renderer/default/test/sample_with_data.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       83 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/tools/parser/templates/renderer/default/ul.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       86 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/tools/parser/templates/renderer/default/warning.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:01.927219 core_parser_app-2.3.0/core_parser_app/tools/parser/templates/renderer/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      149 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/tools/parser/templates/renderer/list/attributes.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       75 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/tools/parser/templates/renderer/list/li.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      131 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/tools/parser/templates/renderer/list/ul.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:01.973124 core_parser_app-2.3.0/core_parser_app/tools/parser/templates/renderer/table/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       99 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/tools/parser/templates/renderer/table/table.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       75 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/tools/parser/templates/renderer/table/tr.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       41 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/tools/parser/templates/renderer/table/wrap.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:02.001768 core_parser_app-2.3.0/core_parser_app/tools/parser/templates/renderer/xml/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       99 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/tools/parser/templates/renderer/xml/element.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:02.049676 core_parser_app-2.3.0/core_parser_app/tools/parser/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/tools/parser/utils/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      278 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/tools/parser/utils/rendering.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3519 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/tools/parser/utils/xml.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1075 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:02.099554 core_parser_app-2.3.0/core_parser_app/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/utils/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2190 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/utils/xml.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:02.115645 core_parser_app-2.3.0/core_parser_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:02.161593 core_parser_app-2.3.0/core_parser_app/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/views/admin/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1592 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/views/admin/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:02.261014 core_parser_app-2.3.0/core_parser_app/views/common/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/views/common/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1808 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/views/common/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3275 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/views/common/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:02.298389 core_parser_app-2.3.0/core_parser_app/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2477 2023-05-02 19:47:52.000000 core_parser_app-2.3.0/core_parser_app/views/user/ajax.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:00.125735 core_parser_app-2.3.0/core_parser_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2332 2023-05-02 19:47:58.000000 core_parser_app-2.3.0/core_parser_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9044 2023-05-02 19:47:59.000000 core_parser_app-2.3.0/core_parser_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:47:58.000000 core_parser_app-2.3.0/core_parser_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       85 2023-05-02 19:47:58.000000 core_parser_app-2.3.0/core_parser_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       22 2023-05-02 19:47:58.000000 core_parser_app-2.3.0/core_parser_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:47:53.000000 core_parser_app-2.3.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       39 2023-05-02 19:47:53.000000 core_parser_app-2.3.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       46 2023-05-02 19:47:53.000000 core_parser_app-2.3.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:48:03.106705 core_parser_app-2.3.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1441 2023-05-02 19:47:53.000000 core_parser_app-2.3.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:02.418741 core_parser_app-2.3.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:53.000000 core_parser_app-2.3.0/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:02.466874 core_parser_app-2.3.0/tests/access_control/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:53.000000 core_parser_app-2.3.0/tests/access_control/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2180 2023-05-02 19:47:53.000000 core_parser_app-2.3.0/tests/access_control/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:02.483995 core_parser_app-2.3.0/tests/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:53.000000 core_parser_app-2.3.0/tests/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:02.544577 core_parser_app-2.3.0/tests/components/data_structure/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:53.000000 core_parser_app-2.3.0/tests/components/data_structure/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:53.000000 core_parser_app-2.3.0/tests/components/data_structure/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1619 2023-05-02 19:47:53.000000 core_parser_app-2.3.0/tests/components/data_structure/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:02.639546 core_parser_app-2.3.0/tests/components/data_structure_element/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:53.000000 core_parser_app-2.3.0/tests/components/data_structure_element/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:02.674227 core_parser_app-2.3.0/tests/components/data_structure_element/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:53.000000 core_parser_app-2.3.0/tests/components/data_structure_element/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6725 2023-05-02 19:47:53.000000 core_parser_app-2.3.0/tests/components/data_structure_element/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    20077 2023-05-02 19:47:53.000000 core_parser_app-2.3.0/tests/components/data_structure_element/test_int_access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5869 2023-05-02 19:47:53.000000 core_parser_app-2.3.0/tests/components/data_structure_element/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4901 2023-05-02 19:47:53.000000 core_parser_app-2.3.0/tests/components/data_structure_element/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:02.718156 core_parser_app-2.3.0/tests/components/module/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:53.000000 core_parser_app-2.3.0/tests/components/module/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4771 2023-05-02 19:47:53.000000 core_parser_app-2.3.0/tests/components/module/tests_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1093 2023-05-02 19:47:53.000000 core_parser_app-2.3.0/tests/fixtures_utils.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      646 2023-05-02 19:47:53.000000 core_parser_app-2.3.0/tests/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      185 2023-05-02 19:47:53.000000 core_parser_app-2.3.0/tests/rights.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      998 2023-05-02 19:47:53.000000 core_parser_app-2.3.0/tests/test_settings.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2714 2023-05-02 19:47:53.000000 core_parser_app-2.3.0/tests/test_utils.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:02.733622 core_parser_app-2.3.0/tests/tools/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:54.000000 core_parser_app-2.3.0/tests/tools/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:02.753528 core_parser_app-2.3.0/tests/tools/modules/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:54.000000 core_parser_app-2.3.0/tests/tools/modules/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:02.816721 core_parser_app-2.3.0/tests/tools/modules/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:54.000000 core_parser_app-2.3.0/tests/tools/modules/tests/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2950 2023-05-02 19:47:54.000000 core_parser_app-2.3.0/tests/tools/modules/tests/tests_unit_checkboxes_module.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9401 2023-05-02 19:47:54.000000 core_parser_app-2.3.0/tests/tools/modules/tests/tests_unit_module.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2292 2023-05-02 19:47:54.000000 core_parser_app-2.3.0/tests/tools/modules/tests/tests_unit_sanitize.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:02.833698 core_parser_app-2.3.0/tests/tools/parser/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:54.000000 core_parser_app-2.3.0/tests/tools/parser/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:02.991529 core_parser_app-2.3.0/tests/tools/parser/parser/
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:56.000000 core_parser_app-2.3.0/tests/tools/parser/parser/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7131 2023-05-02 19:47:56.000000 core_parser_app-2.3.0/tests/tools/parser/parser/test_choice.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5010 2023-05-02 19:47:56.000000 core_parser_app-2.3.0/tests/tools/parser/parser/test_complex_content.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10789 2023-05-02 19:47:56.000000 core_parser_app-2.3.0/tests/tools/parser/parser/test_complex_type.py
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)    11082 2023-05-02 19:47:56.000000 core_parser_app-2.3.0/tests/tools/parser/parser/test_element.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8882 2023-05-02 19:47:56.000000 core_parser_app-2.3.0/tests/tools/parser/parser/test_extension.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      876 2023-05-02 19:47:56.000000 core_parser_app-2.3.0/tests/tools/parser/parser/test_parser.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3811 2023-05-02 19:47:56.000000 core_parser_app-2.3.0/tests/tools/parser/parser/test_restriction.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7071 2023-05-02 19:47:56.000000 core_parser_app-2.3.0/tests/tools/parser/parser/test_sequence.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:03.009735 core_parser_app-2.3.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:56.000000 core_parser_app-2.3.0/tests/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:03.031226 core_parser_app-2.3.0/tests/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:56.000000 core_parser_app-2.3.0/tests/views/user/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:03.083304 core_parser_app-2.3.0/tests/views/user/ajax/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:56.000000 core_parser_app-2.3.0/tests/views/user/ajax/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1979 2023-05-02 19:47:56.000000 core_parser_app-2.3.0/tests/views/user/ajax/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5125 2023-05-02 19:47:56.000000 core_parser_app-2.3.0/tests/views/user/ajax/test_int_access_control.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `core_parser_app-2.2.0/PKG-INFO` & `core_parser_app-2.3.0/core_parser_app.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
-Name: core_parser_app
-Version: 2.2.0
+Name: core-parser-app
+Version: 2.3.0
 Summary: XSD parser tools for the curator core project
 Home-page: https://github.com/usnistgov/core_parser_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: ===============
         Core Parser App
```

### Comparing `core_parser_app-2.2.0/README.rst` & `core_parser_app-2.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/core_parser_app/access_control.py` & `core_parser_app-2.3.0/core_parser_app/access_control.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/core_parser_app/admin.py` & `core_parser_app-2.3.0/core_parser_app/admin.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/core_parser_app/components/data_structure/models.py` & `core_parser_app-2.3.0/core_parser_app/components/data_structure/models.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/core_parser_app/components/data_structure_element/api.py` & `core_parser_app-2.3.0/core_parser_app/components/data_structure_element/api.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/core_parser_app/components/module/api.py` & `core_parser_app-2.3.0/core_parser_app/components/module/api.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/core_parser_app/components/module/models.py` & `core_parser_app-2.3.0/core_parser_app/components/module/models.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/core_parser_app/migrations/0001_initial.py` & `core_parser_app-2.3.0/core_parser_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/core_parser_app/settings.py` & `core_parser_app-2.3.0/core_parser_app/settings.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/core_parser_app/static/core_parser_app/common/js/module_manager.js` & `core_parser_app-2.3.0/core_parser_app/static/core_parser_app/common/js/module_manager.js`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/core_parser_app/static/core_parser_app/common/xsd/annotations.xsd` & `core_parser_app-2.3.0/core_parser_app/static/core_parser_app/common/xsd/annotations.xsd`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/core_parser_app/static/core_parser_app/common/xsd/boolean.xsd` & `core_parser_app-2.3.0/core_parser_app/static/core_parser_app/common/xsd/boolean.xsd`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/core_parser_app/static/core_parser_app/common/xsd/date.xsd` & `core_parser_app-2.3.0/core_parser_app/static/core_parser_app/common/xsd/date.xsd`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/core_parser_app/system/api.py` & `core_parser_app-2.3.0/core_parser_app/system/api.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/core_parser_app/templates/core_parser_app/common/modals/add_module.html` & `core_parser_app-2.3.0/core_parser_app/templates/core_parser_app/common/modals/add_module.html`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/core_parser_app/templates/core_parser_app/common/module_manager_box.html` & `core_parser_app-2.3.0/core_parser_app/templates/core_parser_app/common/module_manager_box.html`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/core_parser_app/tools/modules/discover.py` & `core_parser_app-2.3.0/core_parser_app/tools/modules/discover.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/core_parser_app/tools/modules/sanitize.py` & `core_parser_app-2.3.0/core_parser_app/tools/modules/sanitize.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/core_parser_app/tools/modules/static/core_parser_app/js/builtin/popup.js` & `core_parser_app-2.3.0/core_parser_app/tools/modules/static/core_parser_app/js/builtin/popup.js`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/core_parser_app/tools/modules/static/core_parser_app/js/commons/file_uploader.js` & `core_parser_app-2.3.0/core_parser_app/tools/modules/static/core_parser_app/js/commons/file_uploader.js`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/core_parser_app/tools/modules/static/core_parser_app/js/modules.js` & `core_parser_app-2.3.0/core_parser_app/tools/modules/static/core_parser_app/js/modules.js`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/core_parser_app/tools/modules/static/core_parser_app/xsl/xsd2html4modules.xsl` & `core_parser_app-2.3.0/core_parser_app/tools/modules/static/core_parser_app/xsl/xsd2html4modules.xsl`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/core_parser_app/tools/modules/views/builtin/autocomplete_module.py` & `core_parser_app-2.3.0/core_parser_app/tools/modules/views/builtin/autocomplete_module.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/core_parser_app/tools/modules/views/builtin/checkboxes_module.py` & `core_parser_app-2.3.0/core_parser_app/tools/modules/views/builtin/checkboxes_module.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/core_parser_app/tools/modules/views/builtin/input_button_module.py` & `core_parser_app-2.3.0/core_parser_app/tools/modules/views/builtin/input_button_module.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/core_parser_app/tools/modules/views/builtin/input_module.py` & `core_parser_app-2.3.0/core_parser_app/tools/modules/views/builtin/input_module.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/core_parser_app/tools/modules/views/builtin/options_module.py` & `core_parser_app-2.3.0/core_parser_app/tools/modules/views/builtin/options_module.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/core_parser_app/tools/modules/views/builtin/popup_module.py` & `core_parser_app-2.3.0/core_parser_app/tools/modules/views/builtin/popup_module.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/core_parser_app/tools/modules/views/builtin/sync_input_module.py` & `core_parser_app-2.3.0/core_parser_app/tools/modules/views/builtin/sync_input_module.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/core_parser_app/tools/modules/views/builtin/textarea_module.py` & `core_parser_app-2.3.0/core_parser_app/tools/modules/views/builtin/textarea_module.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/core_parser_app/tools/modules/views/module.py` & `core_parser_app-2.3.0/core_parser_app/tools/modules/views/module.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/core_parser_app/tools/modules/views/views.py` & `core_parser_app-2.3.0/core_parser_app/tools/modules/views/views.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/core_parser_app/tools/modules/xpathaccessor.py` & `core_parser_app-2.3.0/core_parser_app/tools/modules/xpathaccessor.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/core_parser_app/tools/parser/parser.py` & `core_parser_app-2.3.0/core_parser_app/tools/parser/parser.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/core_parser_app/tools/parser/renderer/__init__.py` & `core_parser_app-2.3.0/core_parser_app/tools/parser/renderer/__init__.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/core_parser_app/tools/parser/renderer/checkbox.py` & `core_parser_app-2.3.0/core_parser_app/tools/parser/renderer/checkbox.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/core_parser_app/tools/parser/renderer/list.py` & `core_parser_app-2.3.0/core_parser_app/tools/parser/renderer/list.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/core_parser_app/tools/parser/renderer/table.py` & `core_parser_app-2.3.0/core_parser_app/tools/parser/renderer/table.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/core_parser_app/tools/parser/renderer/xml.py` & `core_parser_app-2.3.0/core_parser_app/tools/parser/renderer/xml.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/core_parser_app/tools/parser/static/core_parser_app/css/use.css` & `core_parser_app-2.3.0/core_parser_app/tools/parser/static/core_parser_app/css/use.css`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/core_parser_app/tools/parser/static/core_parser_app/js/autosave.js` & `core_parser_app-2.3.0/core_parser_app/tools/parser/static/core_parser_app/js/autosave.js`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/core_parser_app/tools/parser/static/core_parser_app/js/autosave_checkbox.js` & `core_parser_app-2.3.0/core_parser_app/tools/parser/static/core_parser_app/js/autosave_checkbox.js`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/core_parser_app/tools/parser/static/core_parser_app/js/buttons.js` & `core_parser_app-2.3.0/core_parser_app/tools/parser/static/core_parser_app/js/buttons.js`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/core_parser_app/tools/parser/static/core_parser_app/js/choice.js` & `core_parser_app-2.3.0/core_parser_app/tools/parser/static/core_parser_app/js/choice.js`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/core_parser_app/tools/parser/utils/xml.py` & `core_parser_app-2.3.0/core_parser_app/tools/parser/utils/xml.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/core_parser_app/urls.py` & `core_parser_app-2.3.0/core_parser_app/urls.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/core_parser_app/utils/xml.py` & `core_parser_app-2.3.0/core_parser_app/utils/xml.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/core_parser_app/views/admin/views.py` & `core_parser_app-2.3.0/core_parser_app/views/admin/views.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/core_parser_app/views/common/ajax.py` & `core_parser_app-2.3.0/core_parser_app/views/common/ajax.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/core_parser_app/views/common/views.py` & `core_parser_app-2.3.0/core_parser_app/views/common/views.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/core_parser_app/views/user/ajax.py` & `core_parser_app-2.3.0/core_parser_app/views/user/ajax.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/core_parser_app.egg-info/PKG-INFO` & `core_parser_app-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
-Name: core-parser-app
-Version: 2.2.0
+Name: core_parser_app
+Version: 2.3.0
 Summary: XSD parser tools for the curator core project
 Home-page: https://github.com/usnistgov/core_parser_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: ===============
         Core Parser App
```

### Comparing `core_parser_app-2.2.0/core_parser_app.egg-info/SOURCES.txt` & `core_parser_app-2.3.0/core_parser_app.egg-info/SOURCES.txt`

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
 core_parser_app/__init__.py
```

### Comparing `core_parser_app-2.2.0/setup.py` & `core_parser_app-2.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 chdir(normpath(join(abspath(__file__), pardir)))
 
 dep_links = [r for r in required if r.startswith("https://")]
 required = [req_link(r) if r.startswith("https://") else r for r in required]
 
 setup(
     name="core_parser_app",
-    version="2.2.0",
+    version="2.3.0",
     description="XSD parser tools for the curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_parser_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_parser_app-2.2.0/tests/access_control/test_unit.py` & `core_parser_app-2.3.0/tests/access_control/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/tests/components/data_structure/tests_unit.py` & `core_parser_app-2.3.0/tests/components/data_structure/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/tests/components/data_structure_element/fixtures/fixtures.py` & `core_parser_app-2.3.0/tests/components/data_structure_element/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/tests/components/data_structure_element/test_int_access_control.py` & `core_parser_app-2.3.0/tests/components/data_structure_element/test_int_access_control.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from django.contrib.auth.models import AnonymousUser
 from django.http import HttpRequest
 
 from core_main_app.access_control.exceptions import AccessControlError
 from core_main_app.commons.exceptions import DoesNotExist
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 from core_parser_app.access_control import (
     _check_data_structure_elements_access,
 )
 from core_parser_app.components.data_structure.models import (
     DataStructureElement,
 )
@@ -21,15 +21,15 @@
 )
 from tests.components.data_structure_element.fixtures.fixtures import (
     DataStructureElementFixtures,
 )
 from tests.fixtures_utils import MockAnonDataStructure
 
 
-class TestUpsert(MongoIntegrationBaseTestCase):
+class TestUpsert(IntegrationBaseTestCase):
     """Test Upsert"""
 
     def setUp(self):
         """setUp"""
 
         self.fixtures = DataStructureElementFixtures()
         self.fixtures.insert_data(user=self.fixtures.default_owner_with_perm)
@@ -116,15 +116,15 @@
             data_structure_element_api.get_by_id(
                 self.mock_data_structure_element.id, self.mock_request
             ),
             self.mock_data_structure_element,
         )
 
 
-class TestGetById(MongoIntegrationBaseTestCase):
+class TestGetById(IntegrationBaseTestCase):
     """Test Get By Id"""
 
     def setUp(self):
         """setUp"""
 
         self.fixtures = DataStructureElementFixtures()
         self.fixtures.insert_data(user=self.fixtures.default_owner_with_perm)
@@ -183,15 +183,15 @@
             self.mock_request,
         )
         self.assertEqual(
             result, self.fixtures.data_structure_element_collection["root"]
         )
 
 
-class TestGetByXPath(MongoIntegrationBaseTestCase):
+class TestGetByXPath(IntegrationBaseTestCase):
     """Test Get By XPath"""
 
     def setUp(self):
         """setUp"""
 
         self.fixtures = DataStructureElementFixtures()
         self.fixtures.insert_data(user=self.fixtures.default_owner_with_perm)
@@ -264,15 +264,15 @@
 
         self.assertEqual(result.count(), 1)
         self.assertEqual(
             result[0], self.fixtures.data_structure_element_collection["1121"]
         )
 
 
-class TestRemoveChild(MongoIntegrationBaseTestCase):
+class TestRemoveChild(IntegrationBaseTestCase):
     """Test Remove Child"""
 
     def setUp(self):
         """setUp"""
 
         self.fixtures = DataStructureElementFixtures()
         self.fixtures.insert_data(user=self.fixtures.default_owner_with_perm)
@@ -351,15 +351,15 @@
             self.fixtures.data_structure_element_collection[
                 "1000"
             ].children.count(),
             orig_children_count - 1,
         )
 
 
-class TestAddChild(MongoIntegrationBaseTestCase):
+class TestAddChild(IntegrationBaseTestCase):
     """Test Add Child"""
 
     def setUp(self):
         """setUp"""
 
         self.fixtures = DataStructureElementFixtures()
         self.fixtures.insert_data(user=self.fixtures.default_owner_with_perm)
@@ -445,15 +445,15 @@
             self.fixtures.data_structure_element_collection[
                 "1000"
             ].children.count(),
             orig_children_count + 1,
         )
 
 
-class TestGetRootElement(MongoIntegrationBaseTestCase):
+class TestGetRootElement(IntegrationBaseTestCase):
     """Test Get Root Element"""
 
     def setUp(self):
         """setUp"""
 
         self.fixtures = DataStructureElementFixtures()
         self.fixtures.insert_data(user=self.fixtures.default_owner_with_perm)
@@ -516,17 +516,15 @@
 
         self.assertEqual(
             result,
             self.fixtures.data_structure_element_collection["root"],
         )
 
 
-class TestDataStructureElementPermissionWithOwners(
-    MongoIntegrationBaseTestCase
-):
+class TestDataStructureElementPermissionWithOwners(IntegrationBaseTestCase):
     """Test access to data structure elements when owner is set"""
 
     def setUp(self):
         """setUp"""
 
         self.fixtures = DataStructureElementFixtures()
         self.fixtures.insert_data(user=self.fixtures.default_owner_with_perm)
@@ -566,17 +564,15 @@
         with self.assertRaises(AccessControlError):
             _check_data_structure_elements_access(
                 [self.fixtures.data_structure_element_collection["root"]],
                 self.users["user"],
             )
 
 
-class TestDataStructureElementPermissionWithoutOwners(
-    MongoIntegrationBaseTestCase
-):
+class TestDataStructureElementPermissionWithoutOwners(IntegrationBaseTestCase):
     """Test access to data structure elements when owner is not set"""
 
     def setUp(self):
         """setUp"""
 
         self.fixtures = DataStructureElementFixtures(add_anon_perm=True)
         self.fixtures.insert_data(
@@ -589,15 +585,15 @@
         _check_data_structure_elements_access(
             [self.fixtures.data_structure_element_collection["root"]],
             AnonymousUser(),
         )
 
 
 class TestDataStructureElementPermissionWithoutOwnersWithoutPerm(
-    MongoIntegrationBaseTestCase
+    IntegrationBaseTestCase
 ):
     """Test access to data structure elements when owner is not set"""
 
     def setUp(self):
         """setUp"""
 
         self.fixtures = DataStructureElementFixtures(add_anon_perm=False)
```

### Comparing `core_parser_app-2.2.0/tests/components/data_structure_element/tests_int.py` & `core_parser_app-2.3.0/tests/components/data_structure_element/tests_int.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 """
 from unittest.mock import Mock
 
 from django.http import HttpRequest
 
 from core_main_app.commons import exceptions
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 from core_parser_app.components.data_structure_element import (
     api as data_structure_element_api,
 )
 from tests.components.data_structure_element.fixtures.fixtures import (
     DataStructureElementFixtures,
 )
 
 
-class TestDataStructureElementGetById(MongoIntegrationBaseTestCase):
+class TestDataStructureElementGetById(IntegrationBaseTestCase):
     """Test Data Structure Element Get By Id"""
 
     def setUp(self):
         """setUp"""
 
         self.fixtures = DataStructureElementFixtures()
         self.fixtures.insert_data()
@@ -56,15 +56,15 @@
 
         mock_request = Mock(spec=HttpRequest)
         # Act # Assert
         with self.assertRaises(Exception):
             data_structure_element_api.get_by_id("", mock_request)
 
 
-class TestDataStructureElementGetByXpath(MongoIntegrationBaseTestCase):
+class TestDataStructureElementGetByXpath(IntegrationBaseTestCase):
     """Test Data Structure Element Get By Xpath"""
 
     def setUp(self):
         """setUp"""
 
         self.fixtures = DataStructureElementFixtures()
         self.user = self.fixtures.default_owner_with_perm
@@ -93,15 +93,15 @@
         result = data_structure_element_api.get_by_xpath(
             "wrong_xpath_value", self.mock_request
         )
         # Act
         self.assertEqual(result.count(), 0)
 
 
-class TestDataStructureElementGetRootElement(MongoIntegrationBaseTestCase):
+class TestDataStructureElementGetRootElement(IntegrationBaseTestCase):
     """Test Data Structure Element Get Root Element"""
 
     def setUp(self):
         """setUp"""
 
         self.fixtures = DataStructureElementFixtures()
         self.fixtures.insert_data()
```

### Comparing `core_parser_app-2.2.0/tests/components/data_structure_element/tests_unit.py` & `core_parser_app-2.3.0/tests/components/data_structure_element/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/tests/components/module/tests_unit.py` & `core_parser_app-2.3.0/tests/components/module/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/tests/fixtures_utils.py` & `core_parser_app-2.3.0/tests/fixtures_utils.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/tests/models.py` & `core_parser_app-2.3.0/tests/models.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/tests/test_settings.py` & `core_parser_app-2.3.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/tests/test_utils.py` & `core_parser_app-2.3.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/tests/tools/modules/tests/tests_unit_checkboxes_module.py` & `core_parser_app-2.3.0/tests/tools/modules/tests/tests_unit_checkboxes_module.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/tests/tools/modules/tests/tests_unit_module.py` & `core_parser_app-2.3.0/tests/tools/modules/tests/tests_unit_module.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/tests/tools/modules/tests/tests_unit_sanitize.py` & `core_parser_app-2.3.0/tests/tools/modules/tests/tests_unit_sanitize.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/tests/tools/parser/parser/test_choice.py` & `core_parser_app-2.3.0/tests/tools/parser/parser/test_choice.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/tests/tools/parser/parser/test_complex_content.py` & `core_parser_app-2.3.0/tests/tools/parser/parser/test_complex_content.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/tests/tools/parser/parser/test_complex_type.py` & `core_parser_app-2.3.0/tests/tools/parser/parser/test_complex_type.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/tests/tools/parser/parser/test_element.py` & `core_parser_app-2.3.0/tests/tools/parser/parser/test_element.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/tests/tools/parser/parser/test_extension.py` & `core_parser_app-2.3.0/tests/tools/parser/parser/test_extension.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/tests/tools/parser/parser/test_parser.py` & `core_parser_app-2.3.0/tests/tools/parser/parser/test_parser.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/tests/tools/parser/parser/test_restriction.py` & `core_parser_app-2.3.0/tests/tools/parser/parser/test_restriction.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/tests/tools/parser/parser/test_sequence.py` & `core_parser_app-2.3.0/tests/tools/parser/parser/test_sequence.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/tests/views/user/ajax/fixtures.py` & `core_parser_app-2.3.0/tests/views/user/ajax/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.2.0/tests/views/user/ajax/test_int_access_control.py` & `core_parser_app-2.3.0/tests/views/user/ajax/test_int_access_control.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 import json
 
 from django.contrib.auth.models import AnonymousUser
 from django.test import RequestFactory
 from django.urls import reverse
 
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 from core_parser_app.components.data_structure.models import (
     DataStructureElement,
 )
 from core_parser_app.views.user.ajax import data_structure_element_value
 from tests import test_settings
 from tests.components.data_structure_element.fixtures.fixtures import (
     DataStructureElementFixtures,
 )
 from tests.views.user.ajax.fixtures import DataStructureElementFixture
 
 
-class TestGetDataStructureElementValue(MongoIntegrationBaseTestCase):
+class TestGetDataStructureElementValue(IntegrationBaseTestCase):
     """Test Get Data Structure Element Value"""
 
     def setUp(self):
         """setUp"""
 
         self.fixtures = DataStructureElementFixtures()
         self.fixtures.insert_data(user=self.fixtures.default_owner_with_perm)
@@ -93,15 +93,15 @@
                 "value": self.fixtures.data_structure_element_collection[
                     "root"
                 ].value
             },
         )
 
 
-class TestPostDataStructureElementValue(MongoIntegrationBaseTestCase):
+class TestPostDataStructureElementValue(IntegrationBaseTestCase):
     """Test Post Data Structure Element Value"""
 
     def setUp(self):
         """setUp"""
 
         self.fixtures = DataStructureElementFixtures()
         self.fixtures.insert_data(user=self.fixtures.default_owner_with_perm)
```

