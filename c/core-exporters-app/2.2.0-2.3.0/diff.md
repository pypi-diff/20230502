# Comparing `tmp/core_exporters_app-2.2.0.tar.gz` & `tmp/core_exporters_app-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/core_exporters_app-2.2.0.tar", last modified: Thu Feb 23 20:29:34 2023, max compression
+gzip compressed data, was "core_exporters_app-2.3.0.tar", last modified: Tue May  2 19:38:47 2023, max compression
```

## Comparing `core_exporters_app-2.2.0.tar` & `core_exporters_app-2.3.0.tar`

### file list

```diff
@@ -1,202 +1,203 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:34.000000 core_exporters_app-2.2.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      292 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1017 2023-02-23 20:29:34.000000 core_exporters_app-2.2.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      542 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:32.000000 core_exporters_app-2.2.0/core_exporters_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       93 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:32.000000 core_exporters_app-2.2.0/core_exporters_app/access_control/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/access_control/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      931 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/access_control/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1764 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/admin.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      704 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/apps.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:32.000000 core_exporters_app-2.2.0/core_exporters_app/commons/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/commons/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      311 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/commons/constants.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:32.000000 core_exporters_app-2.2.0/core_exporters_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:32.000000 core_exporters_app-2.2.0/core_exporters_app/components/exported_compressed_file/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/components/exported_compressed_file/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      404 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/components/exported_compressed_file/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      778 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/components/exported_compressed_file/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1365 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/components/exported_compressed_file/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:32.000000 core_exporters_app-2.2.0/core_exporters_app/components/exporter/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/components/exporter/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      318 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/components/exporter/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1537 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/components/exporter/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6984 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/components/exporter/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1451 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/components/exporter/watch.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:32.000000 core_exporters_app-2.2.0/core_exporters_app/exporters/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/exporters/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:32.000000 core_exporters_app-2.2.0/core_exporters_app/exporters/blob/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/exporters/blob/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4587 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/exporters/blob/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      221 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/exporters/blob/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4576 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/exporters/discover.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5910 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/exporters/exporter.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:32.000000 core_exporters_app-2.2.0/core_exporters_app/exporters/json_exporter/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/exporters/json_exporter/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2358 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/exporters/json_exporter/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      230 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/exporters/json_exporter/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      323 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/exporters/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:32.000000 core_exporters_app-2.2.0/core_exporters_app/exporters/xml/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/exporters/xml/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1789 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/exporters/xml/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      216 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/exporters/xml/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:32.000000 core_exporters_app-2.2.0/core_exporters_app/exporters/xsl/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/exporters/xsl/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2801 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/exporters/xsl/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3358 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/exporters/xsl/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:31.000000 core_exporters_app-2.2.0/core_exporters_app/exporters/xsl/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:31.000000 core_exporters_app-2.2.0/core_exporters_app/exporters/xsl/static/xsl/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:31.000000 core_exporters_app-2.2.0/core_exporters_app/exporters/xsl/static/xsl/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:31.000000 core_exporters_app-2.2.0/core_exporters_app/exporters/xsl/static/xsl/admin/js/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:31.000000 core_exporters_app-2.2.0/core_exporters_app/exporters/xsl/static/xsl/admin/js/exporters/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:31.000000 core_exporters_app-2.2.0/core_exporters_app/exporters/xsl/static/xsl/admin/js/exporters/list/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:32.000000 core_exporters_app-2.2.0/core_exporters_app/exporters/xsl/static/xsl/admin/js/exporters/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2042 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/exporters/xsl/static/xsl/admin/js/exporters/list/modals/add.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       82 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/exporters/xsl/static/xsl/admin/js/exporters/list/modals/add.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:31.000000 core_exporters_app-2.2.0/core_exporters_app/exporters/xsl/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:31.000000 core_exporters_app-2.2.0/core_exporters_app/exporters/xsl/templates/xsl/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:31.000000 core_exporters_app-2.2.0/core_exporters_app/exporters/xsl/templates/xsl/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:31.000000 core_exporters_app-2.2.0/core_exporters_app/exporters/xsl/templates/xsl/admin/exporters/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:32.000000 core_exporters_app-2.2.0/core_exporters_app/exporters/xsl/templates/xsl/admin/exporters/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       40 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/exporters/xsl/templates/xsl/admin/exporters/list/add_base.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1864 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/exporters/xsl/templates/xsl/admin/exporters/list/list_base.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:32.000000 core_exporters_app-2.2.0/core_exporters_app/exporters/xsl/templates/xsl/admin/exporters/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      761 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/exporters/xsl/templates/xsl/admin/exporters/list/modals/add.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      336 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/exporters/xsl/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:32.000000 core_exporters_app-2.2.0/core_exporters_app/exporters/xsl/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/exporters/xsl/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:32.000000 core_exporters_app-2.2.0/core_exporters_app/exporters/xsl/views/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/exporters/xsl/views/admin/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2958 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/exporters/xsl/views/admin/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      751 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/exporters/xsl/views/admin/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      332 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/menus.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:32.000000 core_exporters_app-2.2.0/core_exporters_app/migrations/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3588 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/migrations/0001_initial.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/migrations/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:33.000000 core_exporters_app-2.2.0/core_exporters_app/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:33.000000 core_exporters_app-2.2.0/core_exporters_app/rest/export/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/rest/export/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:33.000000 core_exporters_app-2.2.0/core_exporters_app/rest/export/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/rest/export/data/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6863 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/rest/export/data/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:33.000000 core_exporters_app-2.2.0/core_exporters_app/rest/exporters/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/rest/exporters/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1967 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/rest/exporters/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8794 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/rest/exporters/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:33.000000 core_exporters_app-2.2.0/core_exporters_app/rest/exporters/xsl/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/rest/exporters/xsl/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4291 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/rest/exporters/xsl/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1516 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/rest/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      862 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:31.000000 core_exporters_app-2.2.0/core_exporters_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:31.000000 core_exporters_app-2.2.0/core_exporters_app/static/core_exporters_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:31.000000 core_exporters_app-2.2.0/core_exporters_app/static/core_exporters_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:31.000000 core_exporters_app-2.2.0/core_exporters_app/static/core_exporters_app/admin/css/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:31.000000 core_exporters_app-2.2.0/core_exporters_app/static/core_exporters_app/admin/css/exporters/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:33.000000 core_exporters_app-2.2.0/core_exporters_app/static/core_exporters_app/admin/css/exporters/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      115 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/static/core_exporters_app/admin/css/exporters/list/list_exporters.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:31.000000 core_exporters_app-2.2.0/core_exporters_app/static/core_exporters_app/admin/js/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:31.000000 core_exporters_app-2.2.0/core_exporters_app/static/core_exporters_app/admin/js/exporters/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:31.000000 core_exporters_app-2.2.0/core_exporters_app/static/core_exporters_app/admin/js/exporters/list/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:33.000000 core_exporters_app-2.2.0/core_exporters_app/static/core_exporters_app/admin/js/exporters/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2392 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/static/core_exporters_app/admin/js/exporters/list/modals/associated_templates.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      103 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/static/core_exporters_app/admin/js/exporters/list/modals/associated_templates.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:31.000000 core_exporters_app-2.2.0/core_exporters_app/static/core_exporters_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:31.000000 core_exporters_app-2.2.0/core_exporters_app/static/core_exporters_app/user/js/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:33.000000 core_exporters_app-2.2.0/core_exporters_app/static/core_exporters_app/user/js/exporter_compressed_file/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      962 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/static/core_exporters_app/user/js/exporter_compressed_file/download.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       82 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/static/core_exporters_app/user/js/exporter_compressed_file/download.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:31.000000 core_exporters_app-2.2.0/core_exporters_app/static/core_exporters_app/user/js/exporters/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:31.000000 core_exporters_app-2.2.0/core_exporters_app/static/core_exporters_app/user/js/exporters/list/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:33.000000 core_exporters_app-2.2.0/core_exporters_app/static/core_exporters_app/user/js/exporters/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5149 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/static/core_exporters_app/user/js/exporters/list/modals/list_exporters_selector.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      160 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/static/core_exporters_app/user/js/exporters/list/modals/list_exporters_selector.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:33.000000 core_exporters_app-2.2.0/core_exporters_app/system/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/system/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      561 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/system/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3990 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/tasks.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:31.000000 core_exporters_app-2.2.0/core_exporters_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:31.000000 core_exporters_app-2.2.0/core_exporters_app/templates/core_exporters_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:31.000000 core_exporters_app-2.2.0/core_exporters_app/templates/core_exporters_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:33.000000 core_exporters_app-2.2.0/core_exporters_app/templates/core_exporters_app/admin/exporters/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:33.000000 core_exporters_app-2.2.0/core_exporters_app/templates/core_exporters_app/admin/exporters/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       37 2023-02-23 20:29:27.000000 core_exporters_app-2.2.0/core_exporters_app/templates/core_exporters_app/admin/exporters/list/associated_templates_base.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1658 2023-02-23 20:29:28.000000 core_exporters_app-2.2.0/core_exporters_app/templates/core_exporters_app/admin/exporters/list/list_base.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:33.000000 core_exporters_app-2.2.0/core_exporters_app/templates/core_exporters_app/admin/exporters/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      881 2023-02-23 20:29:28.000000 core_exporters_app-2.2.0/core_exporters_app/templates/core_exporters_app/admin/exporters/list/modals/associated_templates.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      324 2023-02-23 20:29:28.000000 core_exporters_app-2.2.0/core_exporters_app/templates/core_exporters_app/admin/exporters/list_exporters.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:31.000000 core_exporters_app-2.2.0/core_exporters_app/templates/core_exporters_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:33.000000 core_exporters_app-2.2.0/core_exporters_app/templates/core_exporters_app/user/exported_compressed_file/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      265 2023-02-23 20:29:28.000000 core_exporters_app-2.2.0/core_exporters_app/templates/core_exporters_app/user/exported_compressed_file/download.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:31.000000 core_exporters_app-2.2.0/core_exporters_app/templates/core_exporters_app/user/exporters/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:33.000000 core_exporters_app-2.2.0/core_exporters_app/templates/core_exporters_app/user/exporters/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       41 2023-02-23 20:29:28.000000 core_exporters_app-2.2.0/core_exporters_app/templates/core_exporters_app/user/exporters/list/link_exporters_selector.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       27 2023-02-23 20:29:28.000000 core_exporters_app-2.2.0/core_exporters_app/templates/core_exporters_app/user/exporters/list/list_exporters_selector_base.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:33.000000 core_exporters_app-2.2.0/core_exporters_app/templates/core_exporters_app/user/exporters/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      842 2023-02-23 20:29:28.000000 core_exporters_app-2.2.0/core_exporters_app/templates/core_exporters_app/user/exporters/list/modals/list_exporters_selector.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      922 2023-02-23 20:29:28.000000 core_exporters_app-2.2.0/core_exporters_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:33.000000 core_exporters_app-2.2.0/core_exporters_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:28.000000 core_exporters_app-2.2.0/core_exporters_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:33.000000 core_exporters_app-2.2.0/core_exporters_app/views/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:28.000000 core_exporters_app-2.2.0/core_exporters_app/views/admin/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3974 2023-02-23 20:29:28.000000 core_exporters_app-2.2.0/core_exporters_app/views/admin/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1468 2023-02-23 20:29:28.000000 core_exporters_app-2.2.0/core_exporters_app/views/admin/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1787 2023-02-23 20:29:28.000000 core_exporters_app-2.2.0/core_exporters_app/views/admin/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:33.000000 core_exporters_app-2.2.0/core_exporters_app/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:28.000000 core_exporters_app-2.2.0/core_exporters_app/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7532 2023-02-23 20:29:28.000000 core_exporters_app-2.2.0/core_exporters_app/views/user/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2705 2023-02-23 20:29:28.000000 core_exporters_app-2.2.0/core_exporters_app/views/user/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2122 2023-02-23 20:29:28.000000 core_exporters_app-2.2.0/core_exporters_app/views/user/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:32.000000 core_exporters_app-2.2.0/core_exporters_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1017 2023-02-23 20:29:30.000000 core_exporters_app-2.2.0/core_exporters_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5965 2023-02-23 20:29:31.000000 core_exporters_app-2.2.0/core_exporters_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-02-23 20:29:30.000000 core_exporters_app-2.2.0/core_exporters_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      132 2023-02-23 20:29:30.000000 core_exporters_app-2.2.0/core_exporters_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       30 2023-02-23 20:29:30.000000 core_exporters_app-2.2.0/core_exporters_app.egg-info/top_level.txt
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:33.000000 core_exporters_app-2.2.0/docs/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:28.000000 core_exporters_app-2.2.0/docs/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11096 2023-02-23 20:29:28.000000 core_exporters_app-2.2.0/docs/conf.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      292 2023-02-23 20:29:28.000000 core_exporters_app-2.2.0/docs/conf_urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-02-23 20:29:28.000000 core_exporters_app-2.2.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       70 2023-02-23 20:29:28.000000 core_exporters_app-2.2.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       62 2023-02-23 20:29:28.000000 core_exporters_app-2.2.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-02-23 20:29:34.000000 core_exporters_app-2.2.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1393 2023-02-23 20:29:28.000000 core_exporters_app-2.2.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:33.000000 core_exporters_app-2.2.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:28.000000 core_exporters_app-2.2.0/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:33.000000 core_exporters_app-2.2.0/tests/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:28.000000 core_exporters_app-2.2.0/tests/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:33.000000 core_exporters_app-2.2.0/tests/components/exported_compressed_file/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:28.000000 core_exporters_app-2.2.0/tests/components/exported_compressed_file/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:33.000000 core_exporters_app-2.2.0/tests/components/exported_compressed_file/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:28.000000 core_exporters_app-2.2.0/tests/components/exported_compressed_file/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1744 2023-02-23 20:29:28.000000 core_exporters_app-2.2.0/tests/components/exported_compressed_file/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6492 2023-02-23 20:29:28.000000 core_exporters_app-2.2.0/tests/components/exported_compressed_file/tests_int.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:33.000000 core_exporters_app-2.2.0/tests/components/exporter/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:28.000000 core_exporters_app-2.2.0/tests/components/exporter/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2758 2023-02-23 20:29:28.000000 core_exporters_app-2.2.0/tests/components/exporter/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:33.000000 core_exporters_app-2.2.0/tests/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:28.000000 core_exporters_app-2.2.0/tests/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:33.000000 core_exporters_app-2.2.0/tests/rest/export/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:28.000000 core_exporters_app-2.2.0/tests/rest/export/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:33.000000 core_exporters_app-2.2.0/tests/rest/export/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:29.000000 core_exporters_app-2.2.0/tests/rest/export/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2520 2023-02-23 20:29:29.000000 core_exporters_app-2.2.0/tests/rest/export/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8736 2023-02-23 20:29:29.000000 core_exporters_app-2.2.0/tests/rest/export/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7069 2023-02-23 20:29:29.000000 core_exporters_app-2.2.0/tests/rest/export/tests_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5057 2023-02-23 20:29:29.000000 core_exporters_app-2.2.0/tests/rest/export/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:34.000000 core_exporters_app-2.2.0/tests/rest/exporter/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:29.000000 core_exporters_app-2.2.0/tests/rest/exporter/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:34.000000 core_exporters_app-2.2.0/tests/rest/exporter/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:29.000000 core_exporters_app-2.2.0/tests/rest/exporter/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      877 2023-02-23 20:29:29.000000 core_exporters_app-2.2.0/tests/rest/exporter/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4071 2023-02-23 20:29:29.000000 core_exporters_app-2.2.0/tests/rest/exporter/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8034 2023-02-23 20:29:29.000000 core_exporters_app-2.2.0/tests/rest/exporter/tests_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1051 2023-02-23 20:29:29.000000 core_exporters_app-2.2.0/tests/rest/exporter/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:34.000000 core_exporters_app-2.2.0/tests/rest/exporter/xsl/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:29:29.000000 core_exporters_app-2.2.0/tests/rest/exporter/xsl/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5101 2023-02-23 20:29:29.000000 core_exporters_app-2.2.0/tests/rest/exporter/xsl/tests_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1606 2023-02-23 20:29:29.000000 core_exporters_app-2.2.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:47.541329 core_exporters_app-2.3.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      292 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1017 2023-05-02 19:38:47.536278 core_exporters_app-2.3.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      542 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:45.467170 core_exporters_app-2.3.0/core_exporters_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       93 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:45.604812 core_exporters_app-2.3.0/core_exporters_app/access_control/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/access_control/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      931 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/access_control/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1764 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/admin.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      704 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/apps.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:45.640346 core_exporters_app-2.3.0/core_exporters_app/commons/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/commons/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      311 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/commons/constants.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:45.656939 core_exporters_app-2.3.0/core_exporters_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:45.721808 core_exporters_app-2.3.0/core_exporters_app/components/exported_compressed_file/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/components/exported_compressed_file/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      404 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/components/exported_compressed_file/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      778 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/components/exported_compressed_file/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1365 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/components/exported_compressed_file/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:45.849178 core_exporters_app-2.3.0/core_exporters_app/components/exporter/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/components/exporter/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      318 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/components/exporter/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1537 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/components/exporter/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6984 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/components/exporter/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1451 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/components/exporter/watch.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:45.945022 core_exporters_app-2.3.0/core_exporters_app/exporters/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/exporters/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.001441 core_exporters_app-2.3.0/core_exporters_app/exporters/blob/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/exporters/blob/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4587 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/exporters/blob/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      221 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/exporters/blob/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4576 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/exporters/discover.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5910 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/exporters/exporter.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.056586 core_exporters_app-2.3.0/core_exporters_app/exporters/json_exporter/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/exporters/json_exporter/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2358 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/exporters/json_exporter/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      230 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/exporters/json_exporter/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      323 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/exporters/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.098734 core_exporters_app-2.3.0/core_exporters_app/exporters/xml/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/exporters/xml/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1789 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/exporters/xml/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      216 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/exporters/xml/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.166719 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2801 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3358 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:44.887562 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:44.891345 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/static/xsl/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:44.895104 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/static/xsl/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:44.898838 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/static/xsl/admin/js/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:44.902349 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/static/xsl/admin/js/exporters/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:44.907458 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/static/xsl/admin/js/exporters/list/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.210326 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/static/xsl/admin/js/exporters/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1722 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/static/xsl/admin/js/exporters/list/modals/add.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       82 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/static/xsl/admin/js/exporters/list/modals/add.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:44.922196 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:44.925769 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/templates/xsl/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:44.929288 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/templates/xsl/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:44.933321 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/templates/xsl/admin/exporters/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.245998 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/templates/xsl/admin/exporters/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       40 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/templates/xsl/admin/exporters/list/add_base.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1864 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/templates/xsl/admin/exporters/list/list_base.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.260614 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/templates/xsl/admin/exporters/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      788 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/templates/xsl/admin/exporters/list/modals/add.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      336 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.283005 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.334304 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/views/admin/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3073 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/views/admin/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      833 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/views/admin/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      332 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/menus.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.381429 core_exporters_app-2.3.0/core_exporters_app/migrations/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3588 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/migrations/0001_initial.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/migrations/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.419491 core_exporters_app-2.3.0/core_exporters_app/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.434989 core_exporters_app-2.3.0/core_exporters_app/rest/export/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/rest/export/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.468696 core_exporters_app-2.3.0/core_exporters_app/rest/export/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/rest/export/data/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6863 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/rest/export/data/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.519034 core_exporters_app-2.3.0/core_exporters_app/rest/exporters/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/rest/exporters/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1967 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/rest/exporters/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8794 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/rest/exporters/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.551182 core_exporters_app-2.3.0/core_exporters_app/rest/exporters/xsl/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/rest/exporters/xsl/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4291 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/rest/exporters/xsl/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1516 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/rest/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      862 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:45.019615 core_exporters_app-2.3.0/core_exporters_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:45.063528 core_exporters_app-2.3.0/core_exporters_app/static/core_exporters_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:45.043445 core_exporters_app-2.3.0/core_exporters_app/static/core_exporters_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:45.030312 core_exporters_app-2.3.0/core_exporters_app/static/core_exporters_app/admin/css/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:45.033991 core_exporters_app-2.3.0/core_exporters_app/static/core_exporters_app/admin/css/exporters/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.580779 core_exporters_app-2.3.0/core_exporters_app/static/core_exporters_app/admin/css/exporters/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      115 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/static/core_exporters_app/admin/css/exporters/list/list_exporters.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:45.046948 core_exporters_app-2.3.0/core_exporters_app/static/core_exporters_app/admin/js/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:45.050518 core_exporters_app-2.3.0/core_exporters_app/static/core_exporters_app/admin/js/exporters/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:45.054447 core_exporters_app-2.3.0/core_exporters_app/static/core_exporters_app/admin/js/exporters/list/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.645516 core_exporters_app-2.3.0/core_exporters_app/static/core_exporters_app/admin/js/exporters/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2047 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/static/core_exporters_app/admin/js/exporters/list/modals/associated_templates.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      103 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/static/core_exporters_app/admin/js/exporters/list/modals/associated_templates.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:45.084905 core_exporters_app-2.3.0/core_exporters_app/static/core_exporters_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:45.097310 core_exporters_app-2.3.0/core_exporters_app/static/core_exporters_app/user/js/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.679628 core_exporters_app-2.3.0/core_exporters_app/static/core_exporters_app/user/js/exporter_compressed_file/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      962 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/static/core_exporters_app/user/js/exporter_compressed_file/download.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       82 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/static/core_exporters_app/user/js/exporter_compressed_file/download.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:45.100991 core_exporters_app-2.3.0/core_exporters_app/static/core_exporters_app/user/js/exporters/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:45.104511 core_exporters_app-2.3.0/core_exporters_app/static/core_exporters_app/user/js/exporters/list/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.723137 core_exporters_app-2.3.0/core_exporters_app/static/core_exporters_app/user/js/exporters/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5149 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/static/core_exporters_app/user/js/exporters/list/modals/list_exporters_selector.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      160 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/static/core_exporters_app/user/js/exporters/list/modals/list_exporters_selector.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.761469 core_exporters_app-2.3.0/core_exporters_app/system/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/system/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      561 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/system/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3990 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/tasks.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:45.122869 core_exporters_app-2.3.0/core_exporters_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:45.157407 core_exporters_app-2.3.0/core_exporters_app/templates/core_exporters_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:45.141570 core_exporters_app-2.3.0/core_exporters_app/templates/core_exporters_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.785796 core_exporters_app-2.3.0/core_exporters_app/templates/core_exporters_app/admin/exporters/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.814595 core_exporters_app-2.3.0/core_exporters_app/templates/core_exporters_app/admin/exporters/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       37 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/templates/core_exporters_app/admin/exporters/list/associated_templates_base.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1658 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/templates/core_exporters_app/admin/exporters/list/list_base.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.835118 core_exporters_app-2.3.0/core_exporters_app/templates/core_exporters_app/admin/exporters/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      907 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/templates/core_exporters_app/admin/exporters/list/modals/associated_templates.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      324 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/templates/core_exporters_app/admin/exporters/list_exporters.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:45.167296 core_exporters_app-2.3.0/core_exporters_app/templates/core_exporters_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.852836 core_exporters_app-2.3.0/core_exporters_app/templates/core_exporters_app/user/exported_compressed_file/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      265 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/templates/core_exporters_app/user/exported_compressed_file/download.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:45.170445 core_exporters_app-2.3.0/core_exporters_app/templates/core_exporters_app/user/exporters/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.882691 core_exporters_app-2.3.0/core_exporters_app/templates/core_exporters_app/user/exporters/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       41 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/templates/core_exporters_app/user/exporters/list/link_exporters_selector.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       27 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/templates/core_exporters_app/user/exporters/list/list_exporters_selector_base.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.900488 core_exporters_app-2.3.0/core_exporters_app/templates/core_exporters_app/user/exporters/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      842 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/templates/core_exporters_app/user/exporters/list/modals/list_exporters_selector.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      922 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.916008 core_exporters_app-2.3.0/core_exporters_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.980545 core_exporters_app-2.3.0/core_exporters_app/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/views/admin/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3974 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/views/admin/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1526 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/views/admin/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1650 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/views/admin/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:47.032514 core_exporters_app-2.3.0/core_exporters_app/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7532 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/views/user/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2705 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/views/user/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2122 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/views/user/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:45.570098 core_exporters_app-2.3.0/core_exporters_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1017 2023-05-02 19:38:41.000000 core_exporters_app-2.3.0/core_exporters_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5976 2023-05-02 19:38:42.000000 core_exporters_app-2.3.0/core_exporters_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:38:41.000000 core_exporters_app-2.3.0/core_exporters_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      132 2023-05-02 19:38:41.000000 core_exporters_app-2.3.0/core_exporters_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       30 2023-05-02 19:38:41.000000 core_exporters_app-2.3.0/core_exporters_app.egg-info/top_level.txt
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:47.071624 core_exporters_app-2.3.0/docs/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/docs/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11096 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/docs/conf.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      292 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/docs/conf_urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       70 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       62 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:38:47.543108 core_exporters_app-2.3.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1393 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:47.110095 core_exporters_app-2.3.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:47.125423 core_exporters_app-2.3.0/tests/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/tests/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:47.183111 core_exporters_app-2.3.0/tests/components/exported_compressed_file/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/tests/components/exported_compressed_file/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:47.223867 core_exporters_app-2.3.0/tests/components/exported_compressed_file/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/tests/components/exported_compressed_file/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1744 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/tests/components/exported_compressed_file/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6477 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/tests/components/exported_compressed_file/tests_int.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:47.254604 core_exporters_app-2.3.0/tests/components/exporter/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/tests/components/exporter/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2758 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/tests/components/exporter/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:47.270594 core_exporters_app-2.3.0/tests/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/tests/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:47.342202 core_exporters_app-2.3.0/tests/rest/export/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/tests/rest/export/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:47.369024 core_exporters_app-2.3.0/tests/rest/export/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/tests/rest/export/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2520 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/tests/rest/export/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8721 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/tests/rest/export/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7069 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/tests/rest/export/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5042 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/tests/rest/export/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:47.431000 core_exporters_app-2.3.0/tests/rest/exporter/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/tests/rest/exporter/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:47.466122 core_exporters_app-2.3.0/tests/rest/exporter/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/tests/rest/exporter/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      877 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/tests/rest/exporter/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4051 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/tests/rest/exporter/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8034 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/tests/rest/exporter/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1051 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/tests/rest/exporter/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:47.519763 core_exporters_app-2.3.0/tests/rest/exporter/xsl/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/tests/rest/exporter/xsl/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5101 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/tests/rest/exporter/xsl/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1606 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/tests/test_settings.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `core_exporters_app-2.2.0/PKG-INFO` & `core_exporters_app-2.3.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_exporters_app
-Version: 2.2.0
+Version: 2.3.0
 Summary: Exporters for the curator core project
 Home-page: https://github.com/usnistgov/core_exporters_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: ==================
         Core Exporters App
```

### Comparing `core_exporters_app-2.2.0/README.rst` & `core_exporters_app-2.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.2.0/core_exporters_app/access_control/api.py` & `core_exporters_app-2.3.0/core_exporters_app/access_control/api.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.2.0/core_exporters_app/admin.py` & `core_exporters_app-2.3.0/core_exporters_app/admin.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.2.0/core_exporters_app/apps.py` & `core_exporters_app-2.3.0/core_exporters_app/apps.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.2.0/core_exporters_app/components/exported_compressed_file/api.py` & `core_exporters_app-2.3.0/core_exporters_app/components/exported_compressed_file/api.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.2.0/core_exporters_app/components/exported_compressed_file/models.py` & `core_exporters_app-2.3.0/core_exporters_app/components/exported_compressed_file/models.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.2.0/core_exporters_app/components/exporter/api.py` & `core_exporters_app-2.3.0/core_exporters_app/components/exporter/api.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.2.0/core_exporters_app/components/exporter/models.py` & `core_exporters_app-2.3.0/core_exporters_app/components/exporter/models.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.2.0/core_exporters_app/components/exporter/watch.py` & `core_exporters_app-2.3.0/core_exporters_app/components/exporter/watch.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.2.0/core_exporters_app/exporters/blob/models.py` & `core_exporters_app-2.3.0/core_exporters_app/exporters/blob/models.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.2.0/core_exporters_app/exporters/discover.py` & `core_exporters_app-2.3.0/core_exporters_app/exporters/discover.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.2.0/core_exporters_app/exporters/exporter.py` & `core_exporters_app-2.3.0/core_exporters_app/exporters/exporter.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.2.0/core_exporters_app/exporters/json_exporter/models.py` & `core_exporters_app-2.3.0/core_exporters_app/exporters/json_exporter/models.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.2.0/core_exporters_app/exporters/xml/models.py` & `core_exporters_app-2.3.0/core_exporters_app/exporters/xml/models.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.2.0/core_exporters_app/exporters/xsl/api.py` & `core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/api.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.2.0/core_exporters_app/exporters/xsl/models.py` & `core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/models.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.2.0/core_exporters_app/exporters/xsl/static/xsl/admin/js/exporters/list/modals/add.js` & `core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/static/xsl/admin/js/exporters/list/modals/add.js`

 * *Files 25% similar despite different names*

#### js-beautify {}

```diff
@@ -21,15 +21,14 @@
     $.ajax({
         url: addXsltUrl,
         type: "GET",
         dataType: "json",
         success: function(data) {
             $("#banner_errors").hide();
             $("#form-add-xslt-content").html(data.template);
-            InitSelectMultipleXslt();
         },
         error: function(data) {
             if (data.responseText != "") {
                 $("#add-xslt-errors").html(data.responseText);
                 $("#banner_errors").show(500);
                 return (false);
             }
@@ -59,21 +58,8 @@
                 $("#form_associated_templates_errors").html(data.responseText);
                 $("#banner_errors").show(500);
                 return (false);
             }
             return (true);
         }
     });
-};
-
-/**
- * Init the drop down list of XSLT
- */
-InitSelectMultipleXslt = function() {
-    $('#id_xslt_list').fSelect({
-        placeholder: 'Select XSLT',
-        numDisplayed: 500,
-        overflowText: '{n} selected',
-        searchText: 'Search',
-        showSearch: true
-    });
 };
```

### Comparing `core_exporters_app-2.2.0/core_exporters_app/exporters/xsl/templates/xsl/admin/exporters/list/list_base.html` & `core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/templates/xsl/admin/exporters/list/list_base.html`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.2.0/core_exporters_app/exporters/xsl/templates/xsl/admin/exporters/list/modals/add.html` & `core_exporters_app-2.3.0/core_exporters_app/templates/core_exporters_app/user/exporters/list/modals/list_exporters_selector.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 {% extends 'core_main_app/_render/admin/theme/tools/modal.html' %}
 
-{% block modal_id %}add-xslt-exporter-modal{% endblock %}
-{% block modal_title %}Add XSLT{% endblock %}
+{% block modal_id %}select-exporters-modal{% endblock %}
+{% block modal_title %}Exporter selection{% endblock %}
 
 {% block modal_body %}
-<div class="alert alert-danger hidden" id="banner_errors">
+<div class="alert alert-danger" id="banner_errors" style="display: none;">
         <a href="#" class="close" data-hide="alert" aria-label="close">&times;</a>
      	<h4><i class="fas fa-exclamation-circle"></i> Error</h4>
-        <div id="add-xslt-errors"></div>
+        <div id="form-exporter-selection-errors">
 </div>
-<form id="form-add-xslt-content" method="post">
+</div>
+<form id="form-exporter-selection" method="post">
+
 </form>
 {% endblock %}
 
 {% block modal_footer %}
-<a class="btn btn-secondary pull-left" data-dismiss="modal" href="#"><i class="fas fa-times"></i> Cancel</a>
-<button id="btn-add-xslt" class="btn btn-primary"><i class="fas fa-save"></i> Save</button>
+<a class="btn btn-secondary pull-left" data-dismiss="modal" href="#">
+    <i class="fas fa-times"></i> Cancel
+</a>
+<button id="btn-exporter-selection-save" class="btn btn-secondary">
+    <i class="fas fa-download"></i> Download
+</button>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
 {% extends 'core_main_app/_render/admin/theme/tools/modal.html' %} {% block
-modal_id %}add-xslt-exporter-modal{% endblock %} {% block modal_title %}Add
-XSLT{% endblock %} {% block modal_body %}
+modal_id %}select-exporters-modal{% endblock %} {% block modal_title %}Exporter
+selection{% endblock %} {% block modal_body %}
 ×
  Error
 {% endblock %} {% block modal_footer %}
  Cancel
-  Save {% endblock %}
+   Download  {% endblock %}
```

### Comparing `core_exporters_app-2.2.0/core_exporters_app/exporters/xsl/views/admin/ajax.py` & `core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/views/admin/ajax.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,12 +93,18 @@
         # set the list as data for pre selection
         xslt_form = XsltSelectionForm(data_form)
         context_params["xslt_selection_form"] = xslt_form
         context = {}
         context.update(request)
         context.update(context_params)
         return HttpResponse(
-            json.dumps({"template": templates_selector.render(context)}),
+            json.dumps(
+                {
+                    "template": templates_selector.render(
+                        context,
+                    )
+                }
+            ),
             content_type="application/javascript",
         )
     except Exception:
         raise Exception("Error occurred during the form display")
```

### Comparing `core_exporters_app-2.2.0/core_exporters_app/exporters/xsl/views/admin/forms.py` & `core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/views/admin/forms.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,15 +5,19 @@
 import core_main_app.components.xsl_transformation.api as xsl_api
 
 
 class XsltSelectionForm(forms.Form):
     """Xslt selection form"""
 
     xslt_list = forms.MultipleChoiceField(
-        label="", widget=forms.SelectMultiple(), required=False
+        label="",
+        widget=forms.CheckboxSelectMultiple(
+            attrs={"class": "multiple-columns"}
+        ),
+        required=False,
     )
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.fields["xslt_list"].choices = _get_xsl()
```

### Comparing `core_exporters_app-2.2.0/core_exporters_app/migrations/0001_initial.py` & `core_exporters_app-2.3.0/core_exporters_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.2.0/core_exporters_app/rest/export/data/views.py` & `core_exporters_app-2.3.0/core_exporters_app/rest/export/data/views.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.2.0/core_exporters_app/rest/exporters/serializers.py` & `core_exporters_app-2.3.0/core_exporters_app/rest/exporters/serializers.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.2.0/core_exporters_app/rest/exporters/views.py` & `core_exporters_app-2.3.0/core_exporters_app/rest/exporters/views.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.2.0/core_exporters_app/rest/exporters/xsl/views.py` & `core_exporters_app-2.3.0/core_exporters_app/rest/exporters/xsl/views.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.2.0/core_exporters_app/rest/urls.py` & `core_exporters_app-2.3.0/core_exporters_app/rest/urls.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.2.0/core_exporters_app/settings.py` & `core_exporters_app-2.3.0/core_exporters_app/settings.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.2.0/core_exporters_app/static/core_exporters_app/admin/js/exporters/list/modals/associated_templates.js` & `core_exporters_app-2.3.0/core_exporters_app/static/core_exporters_app/admin/js/exporters/list/modals/associated_templates.js`

 * *Files 26% similar despite different names*

#### js-beautify {}

```diff
@@ -25,15 +25,14 @@
         dataType: "json",
         data: {
             'exporter_id': exporterId
         },
         success: function(data) {
             $("#banner_errors").hide();
             $("#form-associated-template-content").html(data.template);
-            InitSelectMultipleTemplates();
         },
         error: function(data) {
             if (data.responseText != "") {
                 $("#form_associated_templates_errors").html(data.responseText);
                 $("#banner_errors").show(500);
                 return (false);
             }
@@ -63,21 +62,8 @@
                 $("#form_associated_templates_errors").html(data.responseText);
                 $("#banner_errors").show(500);
                 return (false);
             }
             return (true);
         }
     });
-};
-
-/**
- * Init the drop down list of templates
- */
-InitSelectMultipleTemplates = function() {
-    $('#id_templates_manager').fSelect({
-        placeholder: 'Select templates',
-        numDisplayed: 3,
-        overflowText: '{n} selected',
-        searchText: 'Search',
-        showSearch: true
-    });
 };
```

### Comparing `core_exporters_app-2.2.0/core_exporters_app/static/core_exporters_app/user/js/exporter_compressed_file/download.js` & `core_exporters_app-2.3.0/core_exporters_app/static/core_exporters_app/user/js/exporter_compressed_file/download.js`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.2.0/core_exporters_app/static/core_exporters_app/user/js/exporters/list/modals/list_exporters_selector.js` & `core_exporters_app-2.3.0/core_exporters_app/static/core_exporters_app/user/js/exporters/list/modals/list_exporters_selector.js`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.2.0/core_exporters_app/system/api.py` & `core_exporters_app-2.3.0/core_exporters_app/system/api.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.2.0/core_exporters_app/tasks.py` & `core_exporters_app-2.3.0/core_exporters_app/tasks.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.2.0/core_exporters_app/templates/core_exporters_app/admin/exporters/list/list_base.html` & `core_exporters_app-2.3.0/core_exporters_app/templates/core_exporters_app/admin/exporters/list/list_base.html`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.2.0/core_exporters_app/templates/core_exporters_app/admin/exporters/list/modals/associated_templates.html` & `core_exporters_app-2.3.0/core_exporters_app/templates/core_exporters_app/admin/exporters/list/modals/associated_templates.html`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 {% block modal_body %}
 <div class="alert alert-danger" id="banner_errors" style="display: none;">
         <a href="#" class="close" data-hide="alert" aria-label="close">&times;</a>
      	<h4><i class="fas fa-exclamation-circle"></i> Error</h4>
         <div id="form_associated_templates_errors">
 </div>
 </div>
-<div class="clearer"></div>
+<div class="clearer"><h5>Select templates:</h5></div>
 <form id="form-associated-template-content" method="post">
 </form>
 {% endblock %}
 
 {% block modal_footer %}
 <a class="btn btn-secondary pull-left" data-dismiss="modal" href="#"><i class="fas fa-times"></i> Cancel</a>
 <button id="btn-associated-templates-save" class="btn btn-primary"><i class="fas fa-save"></i> Save</button>
```

#### html2text {}

```diff
@@ -1,8 +1,9 @@
 {% extends 'core_main_app/_render/admin/theme/tools/modal.html' %} {% block
 modal_id %}select-associated-template-modal{% endblock %} {% block modal_title
 %}Associated template selection{% endblock %} {% block modal_body %}
 ×
  Error
+** Select templates: **
 {% endblock %} {% block modal_footer %}
  Cancel
   Save {% endblock %}
```

### Comparing `core_exporters_app-2.2.0/core_exporters_app/templates/core_exporters_app/user/exporters/list/modals/list_exporters_selector.html` & `core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/templates/xsl/admin/exporters/list/modals/add.html`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,20 @@
 {% extends 'core_main_app/_render/admin/theme/tools/modal.html' %}
 
-{% block modal_id %}select-exporters-modal{% endblock %}
-{% block modal_title %}Exporter selection{% endblock %}
+{% block modal_id %}add-xslt-exporter-modal{% endblock %}
+{% block modal_title %}Add XSLT{% endblock %}
 
 {% block modal_body %}
-<div class="alert alert-danger" id="banner_errors" style="display: none;">
+<div class="alert alert-danger hidden" id="banner_errors">
         <a href="#" class="close" data-hide="alert" aria-label="close">&times;</a>
      	<h4><i class="fas fa-exclamation-circle"></i> Error</h4>
-        <div id="form-exporter-selection-errors">
+        <div id="add-xslt-errors"></div>
 </div>
-</div>
-<form id="form-exporter-selection" method="post">
-
+<h5>Select templates:</h5>
+<form id="form-add-xslt-content" method="post">
 </form>
 {% endblock %}
 
 {% block modal_footer %}
-<a class="btn btn-secondary pull-left" data-dismiss="modal" href="#">
-    <i class="fas fa-times"></i> Cancel
-</a>
-<button id="btn-exporter-selection-save" class="btn btn-secondary">
-    <i class="fas fa-download"></i> Download
-</button>
+<a class="btn btn-secondary pull-left" data-dismiss="modal" href="#"><i class="fas fa-times"></i> Cancel</a>
+<button id="btn-add-xslt" class="btn btn-primary"><i class="fas fa-save"></i> Save</button>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,8 +1,9 @@
 {% extends 'core_main_app/_render/admin/theme/tools/modal.html' %} {% block
-modal_id %}select-exporters-modal{% endblock %} {% block modal_title %}Exporter
-selection{% endblock %} {% block modal_body %}
+modal_id %}add-xslt-exporter-modal{% endblock %} {% block modal_title %}Add
+XSLT{% endblock %} {% block modal_body %}
 ×
  Error
+** Select templates: **
 {% endblock %} {% block modal_footer %}
  Cancel
-   Download  {% endblock %}
+  Save {% endblock %}
```

### Comparing `core_exporters_app-2.2.0/core_exporters_app/urls.py` & `core_exporters_app-2.3.0/core_exporters_app/urls.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.2.0/core_exporters_app/views/admin/ajax.py` & `core_exporters_app-2.3.0/core_exporters_app/views/admin/ajax.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.2.0/core_exporters_app/views/admin/forms.py` & `core_exporters_app-2.3.0/core_exporters_app/views/admin/forms.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,17 @@
 
 
 class AssociatedTemplatesForm(forms.Form):
     """Associated Template form"""
 
     id = forms.CharField(widget=forms.HiddenInput(), required=False)
     templates_manager = forms.MultipleChoiceField(
-        label="", widget=forms.SelectMultiple(), required=False
+        label="",
+        widget=forms.CheckboxSelectMultiple(attrs={"class": "double-columns"}),
+        required=False,
     )
 
     def __init__(self, *args, **kwargs):
         request = kwargs.pop("request")
         super().__init__(*args, **kwargs)
         self.fields["templates_manager"].choices = _get_templates_versions(
             request=request
```

### Comparing `core_exporters_app-2.2.0/core_exporters_app/views/admin/views.py` & `core_exporters_app-2.3.0/core_exporters_app/views/admin/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,29 +31,25 @@
         "xsl/admin/exporters/list/modals/add.html",
         EditExporterView.get_modal_html_path(),
     ]
 
     assets = {
         "js": [
             {
-                "path": "core_main_app/libs/fSelect/js/fSelect.js",
-                "is_raw": False,
-            },
-            {
                 "path": "core_exporters_app/admin/js/exporters/list/modals/associated_templates.js",
                 "is_raw": False,
             },
             {
                 "path": "xsl/admin/js/exporters/list/modals/add.js",
                 "is_raw": False,
             },
             EditExporterView.get_modal_js_path(),
         ],
         "css": [
-            "core_main_app/libs/fSelect/css/fSelect.css",
+            "core_main_app/common/css/select.css",
             "core_exporters_app/admin/css/exporters/list/list_exporters.css",
         ],
     }
 
     return admin_render(
         request,
         "core_exporters_app/admin/exporters/list_exporters.html",
```

### Comparing `core_exporters_app-2.2.0/core_exporters_app/views/user/ajax.py` & `core_exporters_app-2.3.0/core_exporters_app/views/user/ajax.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.2.0/core_exporters_app/views/user/forms.py` & `core_exporters_app-2.3.0/core_exporters_app/views/user/forms.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.2.0/core_exporters_app/views/user/views.py` & `core_exporters_app-2.3.0/core_exporters_app/views/user/views.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.2.0/core_exporters_app.egg-info/PKG-INFO` & `core_exporters_app-2.3.0/core_exporters_app.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-exporters-app
-Version: 2.2.0
+Version: 2.3.0
 Summary: Exporters for the curator core project
 Home-page: https://github.com/usnistgov/core_exporters_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: ==================
         Core Exporters App
```

### Comparing `core_exporters_app-2.2.0/core_exporters_app.egg-info/SOURCES.txt` & `core_exporters_app-2.3.0/core_exporters_app.egg-info/SOURCES.txt`

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
 core_exporters_app/__init__.py
```

### Comparing `core_exporters_app-2.2.0/docs/conf.py` & `core_exporters_app-2.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.2.0/setup.py` & `core_exporters_app-2.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_exporters_app",
-    version="2.2.0",
+    version="2.3.0",
     description="Exporters for the curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_exporters_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_exporters_app-2.2.0/tests/components/exported_compressed_file/fixtures/fixtures.py` & `core_exporters_app-2.3.0/tests/components/exported_compressed_file/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.2.0/tests/components/exported_compressed_file/tests_int.py` & `core_exporters_app-2.3.0/tests/components/exported_compressed_file/tests_int.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
 
 from django.contrib.auth.models import AnonymousUser
 from django.test import override_settings
 
 from core_main_app.access_control.exceptions import AccessControlError
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from core_exporters_app.components.exported_compressed_file import (
     api as exported_compressed_file_api,
 )
 from core_exporters_app.components.exported_compressed_file.models import (
     ExportedCompressedFile,
@@ -18,15 +18,15 @@
 from tests.components.exported_compressed_file.fixtures.fixtures import (
     ExportedCompressedFileFixtures,
 )
 
 fixture_data = ExportedCompressedFileFixtures()
 
 
-class TestGetByExportedCompressedFile(MongoIntegrationBaseTestCase):
+class TestGetByExportedCompressedFile(IntegrationBaseTestCase):
     """Test Get By Exported Compressed File"""
 
     fixture = fixture_data
 
     def setUp(self):
         """setUp"""
 
@@ -149,15 +149,15 @@
             self.fixture.exported_compressed_file_2.id, user
         )
 
         # Assert
         self.assertEqual(result, self.fixture.exported_compressed_file_2)
 
 
-class TestUpsertExportedCompressedFile(MongoIntegrationBaseTestCase):
+class TestUpsertExportedCompressedFile(IntegrationBaseTestCase):
     """Test Upsert Exported Compressed File"""
 
     fixture = fixture_data
 
     def setUp(self):
         """setUp"""
```

### Comparing `core_exporters_app-2.2.0/tests/components/exporter/tests_unit.py` & `core_exporters_app-2.3.0/tests/components/exporter/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.2.0/tests/rest/export/fixtures/fixtures.py` & `core_exporters_app-2.3.0/tests/rest/export/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.2.0/tests/rest/export/tests_int.py` & `core_exporters_app-2.3.0/tests/rest/export/tests_int.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,27 +12,27 @@
 from core_main_app.utils.tests_tools.RequestMock import RequestMock
 import core_main_app.components.data.api as data_api
 from core_main_app.components.data.models import Data
 from core_main_app.components.xsl_transformation.models import (
     XslTransformation,
 )
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 import core_exporters_app.components.exporter.api as exporter_api
 import core_exporters_app.exporters.xsl.api as exporter_xsl_api
 import core_exporters_app.rest.export.data.views as export_data_views
 
 
 from tests.rest.export.fixtures.fixtures import ExportDataFixtures
 
 fixture_data = ExportDataFixtures()
 
 
-class TestExportDataById(MongoIntegrationBaseTestCase):
+class TestExportDataById(IntegrationBaseTestCase):
     """Test Export Data By Id"""
 
     fixture = fixture_data
 
     def setUp(self):
         """setUp"""
         super().setUp()
@@ -124,15 +124,15 @@
 
 
 if "core_linked_records_app" in settings.INSTALLED_APPS:
     from core_linked_records_app.components.data import (
         api as linked_data_api,
     )
 
-    class TestExportDataByPID(MongoIntegrationBaseTestCase):
+    class TestExportDataByPID(IntegrationBaseTestCase):
         """Test Export Data By PID"""
 
         fixture = fixture_data
 
         def setUp(self):
             """setUp"""
             super().setUp()
```

### Comparing `core_exporters_app-2.2.0/tests/rest/export/tests_permissions.py` & `core_exporters_app-2.3.0/tests/rest/export/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.2.0/tests/rest/export/tests_unit.py` & `core_exporters_app-2.3.0/tests/rest/export/tests_unit.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 from unittest.mock import patch
 from rest_framework import status
 
 
 import core_main_app.components.data.api as data_api
 from core_main_app.components.data.models import Data
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from core_main_app.utils.tests_tools.RequestMock import RequestMock
 
 import core_exporters_app.rest.export.data.views as export_data_views
 from tests.rest.export.fixtures.fixtures import ExportDataFixtures
 
 fixture_data = ExportDataFixtures()
 
 
-class TestExportDataById(MongoIntegrationBaseTestCase):
+class TestExportDataById(IntegrationBaseTestCase):
     """Test Export Data By Id"""
 
     fixture = fixture_data
 
     def setUp(self):
         """setUp"""
 
@@ -93,15 +93,15 @@
 
 
 if "core_linked_records_app" in settings.INSTALLED_APPS:
     from core_linked_records_app.components.data import (
         api as linked_data_api,
     )
 
-    class TestExportDataByPID(MongoIntegrationBaseTestCase):
+    class TestExportDataByPID(IntegrationBaseTestCase):
         """Test Export Data By PID"""
 
         fixture = fixture_data
 
         def setUp(self):
             """setUp"""
```

### Comparing `core_exporters_app-2.2.0/tests/rest/exporter/fixtures/fixtures.py` & `core_exporters_app-2.3.0/tests/rest/exporter/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.2.0/tests/rest/exporter/tests_int.py` & `core_exporters_app-2.3.0/tests/rest/exporter/tests_int.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """Integration tests for exporter rest api
 """
 
 from rest_framework import status
 
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from core_main_app.utils.tests_tools.RequestMock import RequestMock
 import core_exporters_app.rest.exporters.views as exporter_views
 from tests.rest.exporter.fixtures.fixtures import ExporterFixtures
 
 fixture_data = ExporterFixtures()
 
 
-class TestGetExportersList(MongoIntegrationBaseTestCase):
+class TestGetExportersList(IntegrationBaseTestCase):
     """Test Get Exporters List"""
 
     fixture = fixture_data
 
     def setUp(self):
         """setUp"""
         super().setUp()
@@ -33,15 +33,15 @@
             exporter_views.ExporterList.as_view(), user
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_200_OK)
 
 
-class TestGetExportersDetail(MongoIntegrationBaseTestCase):
+class TestGetExportersDetail(IntegrationBaseTestCase):
     """Test Get Exporters Detail"""
 
     fixture = fixture_data
 
     def setUp(self):
         """setUp"""
         super().setUp()
@@ -97,15 +97,15 @@
 
         # Assert
         self.assertEqual(
             response.status_code, status.HTTP_500_INTERNAL_SERVER_ERROR
         )
 
 
-class TestGetExporterDownload(MongoIntegrationBaseTestCase):
+class TestGetExporterDownload(IntegrationBaseTestCase):
     """Test Get Exporter Download"""
 
     fixture = fixture_data
 
     def setUp(self):
         """setUp"""
         super().setUp()
```

### Comparing `core_exporters_app-2.2.0/tests/rest/exporter/tests_permissions.py` & `core_exporters_app-2.3.0/tests/rest/exporter/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.2.0/tests/rest/exporter/tests_unit.py` & `core_exporters_app-2.3.0/tests/rest/exporter/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.2.0/tests/rest/exporter/xsl/tests_permissions.py` & `core_exporters_app-2.3.0/tests/rest/exporter/xsl/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.2.0/tests/test_settings.py` & `core_exporters_app-2.3.0/tests/test_settings.py`

 * *Files identical despite different names*

