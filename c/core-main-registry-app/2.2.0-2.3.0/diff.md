# Comparing `tmp/core_main_registry_app-2.2.0.tar.gz` & `tmp/core_main_registry_app-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/core_main_registry_app-2.2.0.tar", last modified: Thu Feb 23 20:31:30 2023, max compression
+gzip compressed data, was "core_main_registry_app-2.3.0.tar", last modified: Tue May  2 19:40:47 2023, max compression
```

## Comparing `core_main_registry_app-2.2.0.tar` & `core_main_registry_app-2.3.0.tar`

### file list

```diff
@@ -1,193 +1,194 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:30.000000 core_main_registry_app-2.2.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      177 2023-02-23 20:31:24.000000 core_main_registry_app-2.2.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2372 2023-02-23 20:31:30.000000 core_main_registry_app-2.2.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1506 2023-02-23 20:31:24.000000 core_main_registry_app-2.2.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:28.000000 core_main_registry_app-2.2.0/core_main_registry_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       99 2023-02-23 20:31:24.000000 core_main_registry_app-2.2.0/core_main_registry_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5076 2023-02-23 20:31:24.000000 core_main_registry_app-2.2.0/core_main_registry_app/admin.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      539 2023-02-23 20:31:24.000000 core_main_registry_app-2.2.0/core_main_registry_app/apps.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:28.000000 core_main_registry_app-2.2.0/core_main_registry_app/commons/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:24.000000 core_main_registry_app-2.2.0/core_main_registry_app/commons/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      168 2023-02-23 20:31:24.000000 core_main_registry_app-2.2.0/core_main_registry_app/commons/constants.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:28.000000 core_main_registry_app-2.2.0/core_main_registry_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:24.000000 core_main_registry_app-2.2.0/core_main_registry_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:28.000000 core_main_registry_app-2.2.0/core_main_registry_app/components/category/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:24.000000 core_main_registry_app-2.2.0/core_main_registry_app/components/category/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1843 2023-02-23 20:31:24.000000 core_main_registry_app-2.2.0/core_main_registry_app/components/category/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3721 2023-02-23 20:31:24.000000 core_main_registry_app-2.2.0/core_main_registry_app/components/category/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:28.000000 core_main_registry_app-2.2.0/core_main_registry_app/components/custom_resource/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:24.000000 core_main_registry_app-2.2.0/core_main_registry_app/components/custom_resource/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      478 2023-02-23 20:31:24.000000 core_main_registry_app-2.2.0/core_main_registry_app/components/custom_resource/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7731 2023-02-23 20:31:24.000000 core_main_registry_app-2.2.0/core_main_registry_app/components/custom_resource/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4505 2023-02-23 20:31:24.000000 core_main_registry_app-2.2.0/core_main_registry_app/components/custom_resource/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:28.000000 core_main_registry_app-2.2.0/core_main_registry_app/components/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:24.000000 core_main_registry_app-2.2.0/core_main_registry_app/components/data/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      515 2023-02-23 20:31:24.000000 core_main_registry_app-2.2.0/core_main_registry_app/components/data/access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3117 2023-02-23 20:31:24.000000 core_main_registry_app-2.2.0/core_main_registry_app/components/data/api.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:28.000000 core_main_registry_app-2.2.0/core_main_registry_app/components/refinement/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:24.000000 core_main_registry_app-2.2.0/core_main_registry_app/components/refinement/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1463 2023-02-23 20:31:24.000000 core_main_registry_app-2.2.0/core_main_registry_app/components/refinement/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2488 2023-02-23 20:31:24.000000 core_main_registry_app-2.2.0/core_main_registry_app/components/refinement/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:28.000000 core_main_registry_app-2.2.0/core_main_registry_app/components/template/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:24.000000 core_main_registry_app-2.2.0/core_main_registry_app/components/template/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      881 2023-02-23 20:31:24.000000 core_main_registry_app-2.2.0/core_main_registry_app/components/template/api.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:28.000000 core_main_registry_app-2.2.0/core_main_registry_app/components/version_manager/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:24.000000 core_main_registry_app-2.2.0/core_main_registry_app/components/version_manager/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      749 2023-02-23 20:31:24.000000 core_main_registry_app-2.2.0/core_main_registry_app/components/version_manager/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      360 2023-02-23 20:31:24.000000 core_main_registry_app-2.2.0/core_main_registry_app/constants.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3751 2023-02-23 20:31:24.000000 core_main_registry_app-2.2.0/core_main_registry_app/discover.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      705 2023-02-23 20:31:24.000000 core_main_registry_app-2.2.0/core_main_registry_app/menus.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:28.000000 core_main_registry_app-2.2.0/core_main_registry_app/migrations/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5740 2023-02-23 20:31:24.000000 core_main_registry_app-2.2.0/core_main_registry_app/migrations/0001_initial.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:24.000000 core_main_registry_app-2.2.0/core_main_registry_app/migrations/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       80 2023-02-23 20:31:24.000000 core_main_registry_app-2.2.0/core_main_registry_app/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:28.000000 core_main_registry_app-2.2.0/core_main_registry_app/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:24.000000 core_main_registry_app-2.2.0/core_main_registry_app/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:28.000000 core_main_registry_app-2.2.0/core_main_registry_app/rest/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:24.000000 core_main_registry_app-2.2.0/core_main_registry_app/rest/data/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3575 2023-02-23 20:31:24.000000 core_main_registry_app-2.2.0/core_main_registry_app/rest/data/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:28.000000 core_main_registry_app-2.2.0/core_main_registry_app/rest/template_version_manager/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:24.000000 core_main_registry_app-2.2.0/core_main_registry_app/rest/template_version_manager/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      784 2023-02-23 20:31:24.000000 core_main_registry_app-2.2.0/core_main_registry_app/rest/template_version_manager/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11382 2023-02-23 20:31:24.000000 core_main_registry_app-2.2.0/core_main_registry_app/rest/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1006 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:28.000000 core_main_registry_app-2.2.0/core_main_registry_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:28.000000 core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:29.000000 core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/json/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4331 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/json/custom_registry.json
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:28.000000 core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:29.000000 core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     6830 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.childcounter.js
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)    12752 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.clones.js
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     4207 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.columnview.js
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     6032 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.customtag.js
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     3737 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.debug.js
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)    19449 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.dnd.js
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)    14809 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.dnd5.js
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     8978 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.edit.js
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)    10817 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.filter.js
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)    19024 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.fixed.js
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     4031 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.glyph.js
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     5317 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.gridnav.js
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)   160231 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.js
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     4291 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.menu.js
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)    11287 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.persist.js
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)    14308 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.table.js
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     4174 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.themeroller.js
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     6509 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.wide.js
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)    15197 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jsdoc-globals.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:29.000000 core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    21971 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap/ui.fancytree.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11747 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap/ui.fancytree.less
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14470 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap/ui.fancytree.min.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      842 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap/vline-rtl.gif
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      844 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap/vline.gif
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:29.000000 core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap-n/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    18706 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap-n/ui.fancytree.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5248 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap-n/ui.fancytree.less
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11739 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap-n/ui.fancytree.min.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      842 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap-n/vline-rtl.gif
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      844 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap-n/vline.gif
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)    23637 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-common.less
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:28.000000 core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:28.000000 core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/user/css/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:29.000000 core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/user/css/fancytree/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      371 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/user/css/fancytree/fancytree.custom.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:29.000000 core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/user/css/resource_banner/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      980 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/user/css/resource_banner/resource_banner.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      327 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/user/css/resource_banner/selection.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:29.000000 core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/xsd/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)   188155 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/xsd/res-md.xsd
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:29.000000 core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/xsl/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5626 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/xsl/xml2html.xsl
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:29.000000 core_main_registry_app-2.2.0/core_main_registry_app/system/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/system/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2769 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/system/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      426 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/tasks.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:28.000000 core_main_registry_app-2.2.0/core_main_registry_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:28.000000 core_main_registry_app-2.2.0/core_main_registry_app/templates/core_main_registry_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:28.000000 core_main_registry_app-2.2.0/core_main_registry_app/templates/core_main_registry_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:29.000000 core_main_registry_app-2.2.0/core_main_registry_app/templates/core_main_registry_app/admin/custom_registry/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      338 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/templates/core_main_registry_app/admin/custom_registry/list.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      925 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/templates/core_main_registry_app/admin/custom_registry/table.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:29.000000 core_main_registry_app-2.2.0/core_main_registry_app/templates/core_main_registry_app/admin/custom_registry/upload/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       60 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/templates/core_main_registry_app/admin/custom_registry/upload/base.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      181 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/templates/core_main_registry_app/admin/custom_registry/upload.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:29.000000 core_main_registry_app-2.2.0/core_main_registry_app/templates/core_main_registry_app/admin/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      384 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/templates/core_main_registry_app/admin/data/detail.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      319 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/templates/core_main_registry_app/admin/data/view_data.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:29.000000 core_main_registry_app-2.2.0/core_main_registry_app/templates/core_main_registry_app/resource_banner/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      815 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/templates/core_main_registry_app/resource_banner/resource_banner.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5517 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:29.000000 core_main_registry_app-2.2.0/core_main_registry_app/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/utils/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:29.000000 core_main_registry_app-2.2.0/core_main_registry_app/utils/fancytree/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/utils/fancytree/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12184 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/utils/fancytree/widget.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:29.000000 core_main_registry_app-2.2.0/core_main_registry_app/utils/refinement/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/utils/refinement/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6124 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/utils/refinement/mongo_query.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2776 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/utils/refinement/refinement.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:29.000000 core_main_registry_app-2.2.0/core_main_registry_app/utils/refinement/tools/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/utils/refinement/tools/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3577 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/utils/refinement/tools/tree.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9709 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/utils/refinement/tools/xsd_refinements.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1032 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/utils/refinement/watch.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:29.000000 core_main_registry_app-2.2.0/core_main_registry_app/utils/role/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/utils/role/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      659 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/utils/role/extraction.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:29.000000 core_main_registry_app-2.2.0/core_main_registry_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:30.000000 core_main_registry_app-2.2.0/core_main_registry_app/views/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/views/admin/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      310 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/views/admin/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5354 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/core_main_registry_app/views/admin/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:28.000000 core_main_registry_app-2.2.0/core_main_registry_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2372 2023-02-23 20:31:27.000000 core_main_registry_app-2.2.0/core_main_registry_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8031 2023-02-23 20:31:27.000000 core_main_registry_app-2.2.0/core_main_registry_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-02-23 20:31:27.000000 core_main_registry_app-2.2.0/core_main_registry_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      132 2023-02-23 20:31:27.000000 core_main_registry_app-2.2.0/core_main_registry_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       29 2023-02-23 20:31:27.000000 core_main_registry_app-2.2.0/core_main_registry_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       71 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       61 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-02-23 20:31:30.000000 core_main_registry_app-2.2.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1413 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:30.000000 core_main_registry_app-2.2.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:30.000000 core_main_registry_app-2.2.0/tests/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/tests/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:30.000000 core_main_registry_app-2.2.0/tests/components/category/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/tests/components/category/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5376 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/tests/components/category/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:30.000000 core_main_registry_app-2.2.0/tests/components/custom_resource/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/tests/components/custom_resource/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:30.000000 core_main_registry_app-2.2.0/tests/components/custom_resource/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/tests/components/custom_resource/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5244 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/tests/components/custom_resource/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14400 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/tests/components/custom_resource/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14727 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/tests/components/custom_resource/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:30.000000 core_main_registry_app-2.2.0/tests/components/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/tests/components/data/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:30.000000 core_main_registry_app-2.2.0/tests/components/data/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/tests/components/data/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2996 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/tests/components/data/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4858 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/tests/components/data/tests_int.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:30.000000 core_main_registry_app-2.2.0/tests/components/refinement/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/tests/components/refinement/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4487 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/tests/components/refinement/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:30.000000 core_main_registry_app-2.2.0/tests/components/template_version_manager/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/tests/components/template_version_manager/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:30.000000 core_main_registry_app-2.2.0/tests/components/template_version_manager/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/tests/components/template_version_manager/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2178 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/tests/components/template_version_manager/fixtures/fixtures.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:30.000000 core_main_registry_app-2.2.0/tests/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/tests/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:30.000000 core_main_registry_app-2.2.0/tests/rest/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/tests/rest/data/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3421 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/tests/rest/data/tests_permissions.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:30.000000 core_main_registry_app-2.2.0/tests/rest/template_version_manager/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/tests/rest/template_version_manager/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3018 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/tests/rest/template_version_manager/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2135 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/tests/rest/template_version_manager/tests_permission.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1743 2023-02-23 20:31:25.000000 core_main_registry_app-2.2.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:47.521330 core_main_registry_app-2.3.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      177 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2372 2023-05-02 19:40:47.516137 core_main_registry_app-2.3.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1506 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:45.396858 core_main_registry_app-2.3.0/core_main_registry_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       99 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5076 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/admin.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      539 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/apps.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:45.522261 core_main_registry_app-2.3.0/core_main_registry_app/commons/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/commons/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      168 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/commons/constants.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:45.539908 core_main_registry_app-2.3.0/core_main_registry_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:45.587835 core_main_registry_app-2.3.0/core_main_registry_app/components/category/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/components/category/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1843 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/components/category/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3721 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/components/category/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:45.656624 core_main_registry_app-2.3.0/core_main_registry_app/components/custom_resource/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/components/custom_resource/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      478 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/components/custom_resource/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7731 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/components/custom_resource/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4505 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/components/custom_resource/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:45.701578 core_main_registry_app-2.3.0/core_main_registry_app/components/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/components/data/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      515 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/components/data/access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3117 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/components/data/api.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:45.759666 core_main_registry_app-2.3.0/core_main_registry_app/components/refinement/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/components/refinement/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1463 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/components/refinement/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2488 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/components/refinement/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:45.794256 core_main_registry_app-2.3.0/core_main_registry_app/components/template/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/components/template/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      881 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/components/template/api.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:45.829581 core_main_registry_app-2.3.0/core_main_registry_app/components/version_manager/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/components/version_manager/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      749 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/components/version_manager/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      360 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/constants.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3751 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/discover.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      705 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/menus.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:45.873115 core_main_registry_app-2.3.0/core_main_registry_app/migrations/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5740 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/migrations/0001_initial.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/migrations/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       80 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:45.908826 core_main_registry_app-2.3.0/core_main_registry_app/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:45.943245 core_main_registry_app-2.3.0/core_main_registry_app/rest/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/rest/data/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3575 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/rest/data/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:45.979315 core_main_registry_app-2.3.0/core_main_registry_app/rest/template_version_manager/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/rest/template_version_manager/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      784 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/rest/template_version_manager/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11382 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/rest/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1006 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:44.902290 core_main_registry_app-2.3.0/core_main_registry_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:44.976371 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:46.001756 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/json/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4331 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/json/custom_registry.json
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:44.915305 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:46.289056 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     6830 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.childcounter.js
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)    12752 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.clones.js
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     4207 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.columnview.js
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     6032 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.customtag.js
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     3737 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.debug.js
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)    19449 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.dnd.js
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)    14809 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.dnd5.js
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     8978 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.edit.js
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)    10817 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.filter.js
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)    19024 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.fixed.js
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     4031 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.glyph.js
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     5317 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.gridnav.js
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)   160231 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.js
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     4291 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.menu.js
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)    11287 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.persist.js
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)    14308 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.table.js
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     4174 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.themeroller.js
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     6509 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.wide.js
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)    15197 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jsdoc-globals.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:46.417646 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    21971 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap/ui.fancytree.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11747 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap/ui.fancytree.less
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14470 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap/ui.fancytree.min.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      842 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap/vline-rtl.gif
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      844 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap/vline.gif
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:46.500631 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap-n/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    18706 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap-n/ui.fancytree.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5248 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap-n/ui.fancytree.less
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11739 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap-n/ui.fancytree.min.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      842 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap-n/vline-rtl.gif
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      844 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap-n/vline.gif
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)    23637 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-common.less
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:44.938295 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:44.959574 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/user/css/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:46.549974 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/user/css/fancytree/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      371 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/user/css/fancytree/fancytree.custom.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:46.582321 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/user/css/resource_banner/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      980 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/user/css/resource_banner/resource_banner.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      327 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/user/css/resource_banner/selection.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:46.600056 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/xsd/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)   188155 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/xsd/res-md.xsd
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:46.622475 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/xsl/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5626 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/xsl/xml2html.xsl
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:46.660661 core_main_registry_app-2.3.0/core_main_registry_app/system/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/system/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2769 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/system/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      426 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/tasks.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:44.995075 core_main_registry_app-2.3.0/core_main_registry_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:45.013896 core_main_registry_app-2.3.0/core_main_registry_app/templates/core_main_registry_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:45.009684 core_main_registry_app-2.3.0/core_main_registry_app/templates/core_main_registry_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:46.722475 core_main_registry_app-2.3.0/core_main_registry_app/templates/core_main_registry_app/admin/custom_registry/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      338 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/templates/core_main_registry_app/admin/custom_registry/list.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      925 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/templates/core_main_registry_app/admin/custom_registry/table.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:46.740734 core_main_registry_app-2.3.0/core_main_registry_app/templates/core_main_registry_app/admin/custom_registry/upload/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       60 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/templates/core_main_registry_app/admin/custom_registry/upload/base.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      181 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/templates/core_main_registry_app/admin/custom_registry/upload.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:46.774470 core_main_registry_app-2.3.0/core_main_registry_app/templates/core_main_registry_app/admin/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      384 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/templates/core_main_registry_app/admin/data/detail.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      319 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/templates/core_main_registry_app/admin/data/view_data.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:46.791741 core_main_registry_app-2.3.0/core_main_registry_app/templates/core_main_registry_app/resource_banner/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      815 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/templates/core_main_registry_app/resource_banner/resource_banner.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4813 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:46.810940 core_main_registry_app-2.3.0/core_main_registry_app/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/utils/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:46.848753 core_main_registry_app-2.3.0/core_main_registry_app/utils/fancytree/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/utils/fancytree/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12184 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/utils/fancytree/widget.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:46.913812 core_main_registry_app-2.3.0/core_main_registry_app/utils/refinement/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/utils/refinement/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6124 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/utils/refinement/mongo_query.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2776 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/utils/refinement/refinement.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:46.954718 core_main_registry_app-2.3.0/core_main_registry_app/utils/refinement/tools/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/utils/refinement/tools/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3577 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/utils/refinement/tools/tree.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9709 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/utils/refinement/tools/xsd_refinements.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1032 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/utils/refinement/watch.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:46.985288 core_main_registry_app-2.3.0/core_main_registry_app/utils/role/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/utils/role/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      659 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/utils/role/extraction.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:47.007013 core_main_registry_app-2.3.0/core_main_registry_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:47.053312 core_main_registry_app-2.3.0/core_main_registry_app/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/views/admin/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      310 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/views/admin/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5354 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/views/admin/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:45.488279 core_main_registry_app-2.3.0/core_main_registry_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2372 2023-05-02 19:40:44.000000 core_main_registry_app-2.3.0/core_main_registry_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8042 2023-05-02 19:40:44.000000 core_main_registry_app-2.3.0/core_main_registry_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:40:44.000000 core_main_registry_app-2.3.0/core_main_registry_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      132 2023-05-02 19:40:44.000000 core_main_registry_app-2.3.0/core_main_registry_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       29 2023-05-02 19:40:44.000000 core_main_registry_app-2.3.0/core_main_registry_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       71 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       61 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:40:47.528789 core_main_registry_app-2.3.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1413 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:47.093111 core_main_registry_app-2.3.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:47.112486 core_main_registry_app-2.3.0/tests/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/tests/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:47.147660 core_main_registry_app-2.3.0/tests/components/category/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/tests/components/category/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5376 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/tests/components/category/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:47.192247 core_main_registry_app-2.3.0/tests/components/custom_resource/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/tests/components/custom_resource/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:47.230636 core_main_registry_app-2.3.0/tests/components/custom_resource/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/tests/components/custom_resource/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5244 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/tests/components/custom_resource/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14360 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/tests/components/custom_resource/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14727 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/tests/components/custom_resource/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:47.263796 core_main_registry_app-2.3.0/tests/components/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/tests/components/data/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:47.304648 core_main_registry_app-2.3.0/tests/components/data/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/tests/components/data/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2996 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/tests/components/data/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4838 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/tests/components/data/tests_int.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:47.337740 core_main_registry_app-2.3.0/tests/components/refinement/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/tests/components/refinement/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4487 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/tests/components/refinement/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:47.354321 core_main_registry_app-2.3.0/tests/components/template_version_manager/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/tests/components/template_version_manager/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:47.394074 core_main_registry_app-2.3.0/tests/components/template_version_manager/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/tests/components/template_version_manager/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2178 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/tests/components/template_version_manager/fixtures/fixtures.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:47.410911 core_main_registry_app-2.3.0/tests/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/tests/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:47.449134 core_main_registry_app-2.3.0/tests/rest/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/tests/rest/data/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3421 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/tests/rest/data/tests_permissions.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:47.500310 core_main_registry_app-2.3.0/tests/rest/template_version_manager/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/tests/rest/template_version_manager/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3008 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/tests/rest/template_version_manager/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2135 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/tests/rest/template_version_manager/tests_permission.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1773 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/tests/test_settings.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `core_main_registry_app-2.2.0/PKG-INFO` & `core_main_registry_app-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_main_registry_app
-Version: 2.2.0
+Version: 2.3.0
 Summary: Main functionalities for the registry project
 Home-page: https://github.com/usnistgov/core_main_registry_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: Core Main Registry App
         ======================
```

### Comparing `core_main_registry_app-2.2.0/README.rst` & `core_main_registry_app-2.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/admin.py` & `core_main_registry_app-2.3.0/core_main_registry_app/admin.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/apps.py` & `core_main_registry_app-2.3.0/core_main_registry_app/apps.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/components/category/api.py` & `core_main_registry_app-2.3.0/core_main_registry_app/components/category/api.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/components/category/models.py` & `core_main_registry_app-2.3.0/core_main_registry_app/components/category/models.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/components/custom_resource/api.py` & `core_main_registry_app-2.3.0/core_main_registry_app/components/custom_resource/api.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/components/custom_resource/models.py` & `core_main_registry_app-2.3.0/core_main_registry_app/components/custom_resource/models.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/components/data/access_control.py` & `core_main_registry_app-2.3.0/core_main_registry_app/components/data/access_control.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/components/data/api.py` & `core_main_registry_app-2.3.0/core_main_registry_app/components/data/api.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/components/refinement/api.py` & `core_main_registry_app-2.3.0/core_main_registry_app/components/refinement/api.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/components/refinement/models.py` & `core_main_registry_app-2.3.0/core_main_registry_app/components/refinement/models.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/components/template/api.py` & `core_main_registry_app-2.3.0/core_main_registry_app/components/template/api.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/components/version_manager/api.py` & `core_main_registry_app-2.3.0/core_main_registry_app/components/version_manager/api.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/discover.py` & `core_main_registry_app-2.3.0/core_main_registry_app/discover.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/menus.py` & `core_main_registry_app-2.3.0/core_main_registry_app/menus.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/migrations/0001_initial.py` & `core_main_registry_app-2.3.0/core_main_registry_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/rest/data/views.py` & `core_main_registry_app-2.3.0/core_main_registry_app/rest/data/views.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/rest/template_version_manager/views.py` & `core_main_registry_app-2.3.0/core_main_registry_app/rest/template_version_manager/views.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/rest/urls.py` & `core_main_registry_app-2.3.0/core_main_registry_app/rest/urls.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/settings.py` & `core_main_registry_app-2.3.0/core_main_registry_app/settings.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/json/custom_registry.json` & `core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/json/custom_registry.json`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.childcounter.js` & `core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.childcounter.js`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.clones.js` & `core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.clones.js`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.columnview.js` & `core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.columnview.js`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.customtag.js` & `core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.customtag.js`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.debug.js` & `core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.debug.js`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.dnd.js` & `core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.dnd.js`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.dnd5.js` & `core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.dnd5.js`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.edit.js` & `core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.edit.js`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.filter.js` & `core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.filter.js`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.fixed.js` & `core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.fixed.js`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.glyph.js` & `core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.glyph.js`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.gridnav.js` & `core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.gridnav.js`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.js` & `core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.js`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.menu.js` & `core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.menu.js`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.persist.js` & `core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.persist.js`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.table.js` & `core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.table.js`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.themeroller.js` & `core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.themeroller.js`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.wide.js` & `core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.wide.js`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jsdoc-globals.js` & `core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jsdoc-globals.js`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap/ui.fancytree.css` & `core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap/ui.fancytree.css`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap/ui.fancytree.less` & `core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap/ui.fancytree.less`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap/ui.fancytree.min.css` & `core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap/ui.fancytree.min.css`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap/vline-rtl.gif` & `core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap/vline-rtl.gif`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap/vline.gif` & `core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap/vline.gif`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap-n/ui.fancytree.css` & `core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap-n/ui.fancytree.css`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap-n/ui.fancytree.less` & `core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap-n/ui.fancytree.less`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap-n/ui.fancytree.min.css` & `core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap-n/ui.fancytree.min.css`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap-n/vline-rtl.gif` & `core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap-n/vline-rtl.gif`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap-n/vline.gif` & `core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap-n/vline.gif`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-common.less` & `core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-common.less`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/user/css/resource_banner/resource_banner.css` & `core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/user/css/resource_banner/resource_banner.css`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/xsd/res-md.xsd` & `core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/xsd/res-md.xsd`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/static/core_main_registry_app/xsl/xml2html.xsl` & `core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/xsl/xml2html.xsl`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/system/api.py` & `core_main_registry_app-2.3.0/core_main_registry_app/system/api.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/templates/core_main_registry_app/admin/custom_registry/table.html` & `core_main_registry_app-2.3.0/core_main_registry_app/templates/core_main_registry_app/admin/custom_registry/table.html`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/templates/core_main_registry_app/resource_banner/resource_banner.html` & `core_main_registry_app-2.3.0/core_main_registry_app/templates/core_main_registry_app/resource_banner/resource_banner.html`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/urls.py` & `core_main_registry_app-2.3.0/core_main_registry_app/urls.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 """ Url router for the core main registry app
 """
-from django.conf import settings
 from django.conf.urls import include
 from django.contrib.auth.decorators import login_required
 from django.urls import re_path
 from drf_yasg import openapi
 from drf_yasg.views import get_schema_view
 
 from core_main_app.components.data import api as data_api
 from core_main_app.utils.rendering import render
+from core_main_app.utils.urls import get_auth_urls
 from core_main_app.views.common import views as common_views
 from core_main_app.views.user import views as user_views, ajax as user_ajax
-
 from core_main_registry_app.settings import ENABLE_BLOB_ENDPOINTS
 
 schema_view = get_schema_view(
     openapi.Info(
         title="REST API",
         default_version="v1",
     ),
@@ -140,41 +139,15 @@
         login_required(
             common_views.DataContentEditor.as_view(),
         ),
         name="core_main_app_xml_text_editor_view",
     ),
 ]
 
-if settings.ENABLE_SAML2_SSO_AUTH:
-    from djangosaml2 import views as saml2_views
-
-    urlpatterns.append(re_path(r"saml2/", include("djangosaml2.urls")))
-    urlpatterns.append(
-        re_path(
-            r"^saml2/login",
-            saml2_views.LoginView.as_view(),
-            name="core_main_app_login",
-        )
-    )
-    urlpatterns.append(
-        re_path(
-            r"^saml2/logout",
-            saml2_views.LogoutInitView.as_view(),
-            name="core_main_app_logout",
-        )
-    )
-else:
-    urlpatterns.append(
-        re_path(r"^login", user_views.custom_login, name="core_main_app_login")
-    )
-    urlpatterns.append(
-        re_path(
-            r"^logout", user_views.custom_logout, name="core_main_app_logout"
-        )
-    )
+urlpatterns.extend(get_auth_urls())
 
 if ENABLE_BLOB_ENDPOINTS:
     from core_main_app.components.blob import api as blob_api
 
     urlpatterns.append(
         re_path(
             r"^assign-blob-workspace",
```

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/utils/fancytree/widget.py` & `core_main_registry_app-2.3.0/core_main_registry_app/utils/fancytree/widget.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/utils/refinement/mongo_query.py` & `core_main_registry_app-2.3.0/core_main_registry_app/utils/refinement/mongo_query.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/utils/refinement/refinement.py` & `core_main_registry_app-2.3.0/core_main_registry_app/utils/refinement/refinement.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/utils/refinement/tools/tree.py` & `core_main_registry_app-2.3.0/core_main_registry_app/utils/refinement/tools/tree.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/utils/refinement/tools/xsd_refinements.py` & `core_main_registry_app-2.3.0/core_main_registry_app/utils/refinement/tools/xsd_refinements.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/utils/refinement/watch.py` & `core_main_registry_app-2.3.0/core_main_registry_app/utils/refinement/watch.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/utils/role/extraction.py` & `core_main_registry_app-2.3.0/core_main_registry_app/utils/role/extraction.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app/views/admin/views.py` & `core_main_registry_app-2.3.0/core_main_registry_app/views/admin/views.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app.egg-info/PKG-INFO` & `core_main_registry_app-2.3.0/core_main_registry_app.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-main-registry-app
-Version: 2.2.0
+Version: 2.3.0
 Summary: Main functionalities for the registry project
 Home-page: https://github.com/usnistgov/core_main_registry_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: Core Main Registry App
         ======================
```

### Comparing `core_main_registry_app-2.2.0/core_main_registry_app.egg-info/SOURCES.txt` & `core_main_registry_app-2.3.0/core_main_registry_app.egg-info/SOURCES.txt`

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
 core_main_registry_app/__init__.py
```

### Comparing `core_main_registry_app-2.2.0/setup.py` & `core_main_registry_app-2.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_main_registry_app",
-    version="2.2.0",
+    version="2.3.0",
     description="Main functionalities for the registry project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_main_registry_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_main_registry_app-2.2.0/tests/components/category/tests_unit.py` & `core_main_registry_app-2.3.0/tests/components/category/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/tests/components/custom_resource/fixtures/fixtures.py` & `core_main_registry_app-2.3.0/tests/components/custom_resource/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/tests/components/custom_resource/tests_int.py` & `core_main_registry_app-2.3.0/tests/components/custom_resource/tests_int.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
 from django.core.exceptions import ValidationError
 from django.utils.text import slugify
 from unittest.mock import patch
 
 from core_main_app.commons import exceptions as exceptions
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from core_main_app.utils.tests_tools.RequestMock import create_mock_request
 from core_main_registry_app.components.custom_resource import (
     api as custom_resource_api,
 )
 from core_main_registry_app.components.custom_resource.models import (
@@ -20,15 +20,15 @@
 from tests.components.custom_resource.fixtures.fixtures import (
     CustomResourceFixtures,
 )
 
 fixtureCustomResource = CustomResourceFixtures()
 
 
-class TestCreateAndSaveCustomResource(MongoIntegrationBaseTestCase):
+class TestCreateAndSaveCustomResource(IntegrationBaseTestCase):
     """
     Test Create And Save Custom Resource
     """
 
     fixture = fixtureCustomResource
 
     def test_create_all_custom_resource_return_collection_of_custom_resource(
@@ -217,15 +217,15 @@
                 type="wrong",
                 icon="icon",
                 sort=0,
             )
             custom_resource.save()
 
 
-class TestGetAllByTemplate(MongoIntegrationBaseTestCase):
+class TestGetAllByTemplate(IntegrationBaseTestCase):
     """
     Test Get All By Template
     """
 
     fixture = fixtureCustomResource
 
     def test_get_all_by_template_return_all(self):
@@ -241,15 +241,15 @@
             self.fixture.get_dict_all_custom_resource(), template
         )
         result = custom_resource_api.get_all_by_template(template)
         # Assert
         self.assertEqual(length, len(result))
 
 
-class TestGetByRoleForCurrentTemplate(MongoIntegrationBaseTestCase):
+class TestGetByRoleForCurrentTemplate(IntegrationBaseTestCase):
     """
     Test Get By Role For Current Template
     """
 
     fixture = fixtureCustomResource
 
     @patch(
@@ -271,15 +271,15 @@
         custom_resource = custom_resource_api.get_by_role_for_current_template(
             self.fixture.custom_resource.role_choice, request=mock_request
         )
         # Assert
         self.assertTrue(isinstance(custom_resource, CustomResource))
 
 
-class TestGetByCurrentTemplateAndSlug(MongoIntegrationBaseTestCase):
+class TestGetByCurrentTemplateAndSlug(IntegrationBaseTestCase):
     """
     Test Get By Current Template And Slug
     """
 
     fixture = fixtureCustomResource
 
     @patch(
@@ -322,15 +322,15 @@
         # Act
         with self.assertRaises(exceptions.DoesNotExist):
             custom_resource_api.get_by_current_template_and_slug(
                 "incorrect slug", mock_request
             )
 
 
-class TestDeleteCustomResourcesByTemplate(MongoIntegrationBaseTestCase):
+class TestDeleteCustomResourcesByTemplate(IntegrationBaseTestCase):
     """
     Test Delete Custom Resources By Template
     """
 
     fixture = fixtureCustomResource
 
     def test_delete_custom_resources_by_template_return_0(self):
@@ -345,15 +345,15 @@
             self.fixture.template
         )
         result = custom_resource_api.get_all_by_template(self.fixture.template)
         # Assert
         self.assertEqual(0, len(result))
 
 
-class TestSaveList(MongoIntegrationBaseTestCase):
+class TestSaveList(IntegrationBaseTestCase):
     """
     Test Save List
     """
 
     fixture = fixtureCustomResource
 
     def test_save_list(self):
@@ -381,15 +381,15 @@
         list_custom = [custom_resource1, custom_resource2]
         custom_resource_api.save_list(list_custom)
         result = custom_resource_api.get_all_by_template(template)
         # Assert
         self.assertEqual(len(list_custom), len(result))
 
 
-class TestReplaceCustomResourceByTemplate(MongoIntegrationBaseTestCase):
+class TestReplaceCustomResourceByTemplate(IntegrationBaseTestCase):
     """
     Test Replace Custom Resource By Template
     """
 
     fixture = fixtureCustomResource
 
     def test_replace_custom_resources_by_template_return_ok(self):
```

### Comparing `core_main_registry_app-2.2.0/tests/components/custom_resource/tests_unit.py` & `core_main_registry_app-2.3.0/tests/components/custom_resource/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/tests/components/data/fixtures/fixtures.py` & `core_main_registry_app-2.3.0/tests/components/data/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/tests/components/data/tests_int.py` & `core_main_registry_app-2.3.0/tests/components/data/tests_int.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 from unittest.mock import patch
 
 
 from core_main_app.commons import exceptions as exceptions
 from core_main_app.components.data.models import Data
 import core_main_app.components.workspace.api as workspace_api
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from core_main_app.utils.tests_tools.RequestMock import create_mock_request
 
 import core_main_registry_app.components.data.api as data_registry_api
 from core_main_registry_app.commons.constants import DataStatus
 from tests.components.data.fixtures.fixtures import DataRegistryFixtures
 
 
 fixture_data = DataRegistryFixtures()
 
 
-class TestDataGetStatus(MongoIntegrationBaseTestCase):
+class TestDataGetStatus(IntegrationBaseTestCase):
     """Test Data Get Status"""
 
     fixture = fixture_data
 
     def test_data_get_status_return_status_from_xml_content(self):
         """test_data_get_status_return_status_from_xml_content"""
 
@@ -39,15 +39,15 @@
         """test_data_get_status_raise_model_exception_if_status_key_does_not_exist"""
 
         # Act, Assert
         with self.assertRaises(exceptions.ModelError):
             data_registry_api.get_status(self.fixture.data_2)
 
 
-class TestDataSetStatus(MongoIntegrationBaseTestCase):
+class TestDataSetStatus(IntegrationBaseTestCase):
     """Test Data Set Status"""
 
     fixture = fixture_data
 
     @patch.object(Data, "convert_to_file")
     def test_data_set_status_to_inactive_should_always_work(
         self, mock_convert_to_file
@@ -81,15 +81,15 @@
         # Act Assert
         with self.assertRaises(exceptions.ModelError):
             data_registry_api.set_status(
                 self.fixture.data_1, DataStatus.DELETED, mock_request
             )
 
 
-class TestDataPublish(MongoIntegrationBaseTestCase):
+class TestDataPublish(IntegrationBaseTestCase):
     """Test Data Publish"""
 
     fixture = fixture_data
 
     @patch.object(workspace_api, "get_global_workspace")
     def test_publish_data_without_workspace_publishes_data(
         self, get_global_workspace
```

### Comparing `core_main_registry_app-2.2.0/tests/components/refinement/tests_unit.py` & `core_main_registry_app-2.3.0/tests/components/refinement/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/tests/components/template_version_manager/fixtures/fixtures.py` & `core_main_registry_app-2.3.0/tests/components/template_version_manager/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/tests/rest/data/tests_permissions.py` & `core_main_registry_app-2.3.0/tests/rest/data/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/tests/rest/template_version_manager/tests_int.py` & `core_main_registry_app-2.3.0/tests/rest/template_version_manager/tests_int.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """ Integration Test for registry Template Version Manager Rest API
 """
 
 from rest_framework import status
 
 from core_main_app.rest.template_version_manager import views
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from core_main_app.utils.tests_tools.RequestMock import RequestMock
 from tests.components.template_version_manager.fixtures.fixtures import (
     TemplateVersionManagerFixtures,
 )
 
 fixture_template = TemplateVersionManagerFixtures()
 
 
-class TestCurrentTemplateVersion(MongoIntegrationBaseTestCase):
+class TestCurrentTemplateVersion(IntegrationBaseTestCase):
     """Test Current Template Version"""
 
     fixture = fixture_template
 
     def test_patch_returns_http_200(self):
         """test_patch_returns_http_200"""
```

### Comparing `core_main_registry_app-2.2.0/tests/rest/template_version_manager/tests_permission.py` & `core_main_registry_app-2.3.0/tests/rest/template_version_manager/tests_permission.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.2.0/tests/test_settings.py` & `core_main_registry_app-2.3.0/tests/test_settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,7 +61,8 @@
 PASSWORD_HASHERS = ("django.contrib.auth.hashers.UnsaltedMD5PasswordHasher",)
 
 USE_TZ = True
 CELERYBEAT_SCHEDULER = "django_celery_beat.schedulers:DatabaseScheduler"
 
 MONGODB_INDEXING = False
 MONGODB_ASYNC_SAVE = False
+ENABLE_SAML2_SSO_AUTH = False
```

