# Comparing `tmp/core_oaipmh_provider_app-2.2.0.tar.gz` & `tmp/core_oaipmh_provider_app-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/core_oaipmh_provider_app-2.2.0.tar", last modified: Thu Feb 23 20:33:55 2023, max compression
+gzip compressed data, was "core_oaipmh_provider_app-2.3.0.tar", last modified: Tue May  2 19:47:36 2023, max compression
```

## Comparing `core_oaipmh_provider_app-2.2.0.tar` & `core_oaipmh_provider_app-2.3.0.tar`

### file list

```diff
@@ -1,217 +1,209 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:55.000000 core_oaipmh_provider_app-2.2.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      156 2023-02-23 20:33:47.000000 core_oaipmh_provider_app-2.2.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1118 2023-02-23 20:33:55.000000 core_oaipmh_provider_app-2.2.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      611 2023-02-23 20:33:47.000000 core_oaipmh_provider_app-2.2.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:52.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       97 2023-02-23 20:33:47.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4465 2023-02-23 20:33:47.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/admin.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2593 2023-02-23 20:33:47.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/apps.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:52.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/commons/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:47.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/commons/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      150 2023-02-23 20:33:47.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/commons/constants.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3064 2023-02-23 20:33:47.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/commons/exceptions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       54 2023-02-23 20:33:47.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/commons/status.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:52.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:47.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:53.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/components/oai_data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:47.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/components/oai_data/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3741 2023-02-23 20:33:47.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/components/oai_data/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5466 2023-02-23 20:33:47.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/components/oai_data/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1535 2023-02-23 20:33:47.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/components/oai_data/watch.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:53.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/components/oai_provider_metadata_format/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:47.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/components/oai_provider_metadata_format/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10750 2023-02-23 20:33:47.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/components/oai_provider_metadata_format/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2310 2023-02-23 20:33:47.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/components/oai_provider_metadata_format/discover.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4113 2023-02-23 20:33:47.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/components/oai_provider_metadata_format/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:53.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/components/oai_provider_set/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:47.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/components/oai_provider_set/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2308 2023-02-23 20:33:47.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/components/oai_provider_set/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2579 2023-02-23 20:33:47.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/components/oai_provider_set/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:53.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/components/oai_request_page/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:47.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/components/oai_request_page/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1637 2023-02-23 20:33:47.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/components/oai_request_page/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1408 2023-02-23 20:33:47.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/components/oai_request_page/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:53.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/components/oai_settings/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:47.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/components/oai_settings/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      465 2023-02-23 20:33:47.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/components/oai_settings/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1651 2023-02-23 20:33:47.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/components/oai_settings/discover.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1017 2023-02-23 20:33:47.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/components/oai_settings/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:53.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/components/oai_xsl_template/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:47.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/components/oai_xsl_template/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2595 2023-02-23 20:33:47.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/components/oai_xsl_template/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3598 2023-02-23 20:33:47.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/components/oai_xsl_template/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      584 2023-02-23 20:33:47.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/menus.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:53.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/migrations/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7245 2023-02-23 20:33:47.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/migrations/0001_initial.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      900 2023-02-23 20:33:47.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/migrations/0002_oai_data_on_delete.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      527 2023-02-23 20:33:47.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/migrations/0003_oai_data_bulk_delete.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/migrations/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:53.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:53.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/rest/oai_provider_metadata_format/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/rest/oai_provider_metadata_format/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14117 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/rest/oai_provider_metadata_format/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:53.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/rest/oai_provider_set/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/rest/oai_provider_set/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7772 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/rest/oai_provider_set/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:53.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/rest/oai_settings/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/rest/oai_settings/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4347 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/rest/oai_settings/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7797 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/rest/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1759 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/rest/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1568 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:52.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:52.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:52.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:52.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:52.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/registry/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:53.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/registry/identity/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      584 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/registry/identity/table_info.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:53.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/registry/metadata_formats/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      183 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/registry/metadata_formats/page.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:53.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/registry/sets/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       63 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/registry/sets/add_set.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:52.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/js/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:52.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/js/registry/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:53.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/js/registry/identity/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1082 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/js/registry/identity/check_registry.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       91 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/js/registry/identity/check_registry.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:52.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/js/registry/sets/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:53.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/js/registry/sets/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      557 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/js/registry/sets/modals/init_select.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:52.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/libs/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:52.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/libs/fSelect/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:53.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/libs/fSelect/css/
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     2719 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/libs/fSelect/css/fSelect.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:53.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/libs/fSelect/js/
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)    12656 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/libs/fSelect/js/fSelect.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:53.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/xsd/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1444 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/xsd/oai_dc.xsd
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3029 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/xsd/simpledc20021212.xsd
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:53.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/system/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/system/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      490 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/system/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1976 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/tasks.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:52.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:52.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:52.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:53.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:53.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/identity/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2016 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/identity/table.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      259 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/identity.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:53.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/metadata_formats/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1408 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/metadata_formats/table_default.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2232 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/metadata_formats/table_metadata_formats.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2013 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/metadata_formats/table_template_metadata_formats.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      502 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/metadata_formats.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:53.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/sets/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1799 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/sets/table.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      251 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/sets.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:53.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/xsl_template/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1877 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/xsl_template/table.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      382 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/xsl_template.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:52.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:53.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      717 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/base.html
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      201 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/error.html
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      635 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/get_record.html
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      254 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/header.html
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     1118 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/identify.html
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      374 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/list_identifiers.html
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      407 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/list_metadata_formats.html
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      577 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/list_records.html
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     1030 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/list_sets.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      298 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/resumption_token.xml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      566 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:54.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/utils/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5850 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/utils/request_checker.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:54.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:54.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/views/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/views/admin/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11317 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/views/admin/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7727 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/views/admin/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7639 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/views/admin/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:54.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    24356 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/views/user/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:52.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1118 2023-02-23 20:33:51.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7929 2023-02-23 20:33:52.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-02-23 20:33:51.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      131 2023-02-23 20:33:51.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       36 2023-02-23 20:33:51.000000 core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app.egg-info/top_level.txt
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:54.000000 core_oaipmh_provider_app-2.2.0/docs/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/docs/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11332 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/docs/conf.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      311 2023-02-23 20:33:48.000000 core_oaipmh_provider_app-2.2.0/docs/conf_urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-02-23 20:33:49.000000 core_oaipmh_provider_app-2.2.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       69 2023-02-23 20:33:49.000000 core_oaipmh_provider_app-2.2.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-02-23 20:33:55.000000 core_oaipmh_provider_app-2.2.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1481 2023-02-23 20:33:49.000000 core_oaipmh_provider_app-2.2.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:54.000000 core_oaipmh_provider_app-2.2.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:49.000000 core_oaipmh_provider_app-2.2.0/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:54.000000 core_oaipmh_provider_app-2.2.0/tests/apps/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:49.000000 core_oaipmh_provider_app-2.2.0/tests/apps/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1799 2023-02-23 20:33:49.000000 core_oaipmh_provider_app-2.2.0/tests/apps/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:54.000000 core_oaipmh_provider_app-2.2.0/tests/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:49.000000 core_oaipmh_provider_app-2.2.0/tests/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:54.000000 core_oaipmh_provider_app-2.2.0/tests/components/oai_data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1527 2023-02-23 20:33:49.000000 core_oaipmh_provider_app-2.2.0/tests/components/oai_data/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:54.000000 core_oaipmh_provider_app-2.2.0/tests/components/oai_data/api/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:49.000000 core_oaipmh_provider_app-2.2.0/tests/components/oai_data/api/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2287 2023-02-23 20:33:49.000000 core_oaipmh_provider_app-2.2.0/tests/components/oai_data/api/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9480 2023-02-23 20:33:49.000000 core_oaipmh_provider_app-2.2.0/tests/components/oai_data/api/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:54.000000 core_oaipmh_provider_app-2.2.0/tests/components/oai_data/models/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:49.000000 core_oaipmh_provider_app-2.2.0/tests/components/oai_data/models/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1336 2023-02-23 20:33:49.000000 core_oaipmh_provider_app-2.2.0/tests/components/oai_data/models/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7942 2023-02-23 20:33:49.000000 core_oaipmh_provider_app-2.2.0/tests/components/oai_data/models/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:54.000000 core_oaipmh_provider_app-2.2.0/tests/components/oai_data/watch/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:49.000000 core_oaipmh_provider_app-2.2.0/tests/components/oai_data/watch/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1098 2023-02-23 20:33:49.000000 core_oaipmh_provider_app-2.2.0/tests/components/oai_data/watch/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:54.000000 core_oaipmh_provider_app-2.2.0/tests/components/oai_provider_metadata_format/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:49.000000 core_oaipmh_provider_app-2.2.0/tests/components/oai_provider_metadata_format/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    13665 2023-02-23 20:33:49.000000 core_oaipmh_provider_app-2.2.0/tests/components/oai_provider_metadata_format/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:54.000000 core_oaipmh_provider_app-2.2.0/tests/components/oai_provider_set/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:49.000000 core_oaipmh_provider_app-2.2.0/tests/components/oai_provider_set/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9462 2023-02-23 20:33:49.000000 core_oaipmh_provider_app-2.2.0/tests/components/oai_provider_set/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:54.000000 core_oaipmh_provider_app-2.2.0/tests/components/oai_settings/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:49.000000 core_oaipmh_provider_app-2.2.0/tests/components/oai_settings/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2770 2023-02-23 20:33:49.000000 core_oaipmh_provider_app-2.2.0/tests/components/oai_settings/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:54.000000 core_oaipmh_provider_app-2.2.0/tests/components/oai_xsl_template/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:49.000000 core_oaipmh_provider_app-2.2.0/tests/components/oai_xsl_template/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9663 2023-02-23 20:33:49.000000 core_oaipmh_provider_app-2.2.0/tests/components/oai_xsl_template/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:54.000000 core_oaipmh_provider_app-2.2.0/tests/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:49.000000 core_oaipmh_provider_app-2.2.0/tests/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:54.000000 core_oaipmh_provider_app-2.2.0/tests/rest/oai_provider_metadata_format/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:49.000000 core_oaipmh_provider_app-2.2.0/tests/rest/oai_provider_metadata_format/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7022 2023-02-23 20:33:49.000000 core_oaipmh_provider_app-2.2.0/tests/rest/oai_provider_metadata_format/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    16462 2023-02-23 20:33:49.000000 core_oaipmh_provider_app-2.2.0/tests/rest/oai_provider_metadata_format/tests_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17947 2023-02-23 20:33:49.000000 core_oaipmh_provider_app-2.2.0/tests/rest/oai_provider_metadata_format/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:54.000000 core_oaipmh_provider_app-2.2.0/tests/rest/oai_provider_set/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:49.000000 core_oaipmh_provider_app-2.2.0/tests/rest/oai_provider_set/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5359 2023-02-23 20:33:49.000000 core_oaipmh_provider_app-2.2.0/tests/rest/oai_provider_set/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8591 2023-02-23 20:33:49.000000 core_oaipmh_provider_app-2.2.0/tests/rest/oai_provider_set/tests_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5925 2023-02-23 20:33:49.000000 core_oaipmh_provider_app-2.2.0/tests/rest/oai_provider_set/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:54.000000 core_oaipmh_provider_app-2.2.0/tests/rest/oai_settings/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:49.000000 core_oaipmh_provider_app-2.2.0/tests/rest/oai_settings/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2633 2023-02-23 20:33:49.000000 core_oaipmh_provider_app-2.2.0/tests/rest/oai_settings/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4840 2023-02-23 20:33:49.000000 core_oaipmh_provider_app-2.2.0/tests/rest/oai_settings/tests_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3149 2023-02-23 20:33:49.000000 core_oaipmh_provider_app-2.2.0/tests/rest/oai_settings/tests_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1894 2023-02-23 20:33:49.000000 core_oaipmh_provider_app-2.2.0/tests/test_settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:54.000000 core_oaipmh_provider_app-2.2.0/tests/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:49.000000 core_oaipmh_provider_app-2.2.0/tests/utils/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:55.000000 core_oaipmh_provider_app-2.2.0/tests/utils/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:49.000000 core_oaipmh_provider_app-2.2.0/tests/utils/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12394 2023-02-23 20:33:49.000000 core_oaipmh_provider_app-2.2.0/tests/utils/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      539 2023-02-23 20:33:49.000000 core_oaipmh_provider_app-2.2.0/tests/utils/mocks.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1299 2023-02-23 20:33:49.000000 core_oaipmh_provider_app-2.2.0/tests/utils/test_oai_pmh_suite.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:55.000000 core_oaipmh_provider_app-2.2.0/tests/utils/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:49.000000 core_oaipmh_provider_app-2.2.0/tests/utils/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:55.000000 core_oaipmh_provider_app-2.2.0/tests/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:49.000000 core_oaipmh_provider_app-2.2.0/tests/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:55.000000 core_oaipmh_provider_app-2.2.0/tests/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:49.000000 core_oaipmh_provider_app-2.2.0/tests/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5622 2023-02-23 20:33:49.000000 core_oaipmh_provider_app-2.2.0/tests/views/user/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    45422 2023-02-23 20:33:49.000000 core_oaipmh_provider_app-2.2.0/tests/views/user/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:36.357797 core_oaipmh_provider_app-2.3.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      156 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1118 2023-05-02 19:47:36.352805 core_oaipmh_provider_app-2.3.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      611 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:34.014911 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       97 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4465 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/admin.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2593 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/apps.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:34.191938 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/commons/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/commons/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      150 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/commons/constants.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3064 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/commons/exceptions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       54 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/commons/status.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:34.210087 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:34.276342 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_data/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3741 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_data/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5466 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_data/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1535 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_data/watch.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:34.331434 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_provider_metadata_format/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_provider_metadata_format/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10750 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_provider_metadata_format/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2310 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_provider_metadata_format/discover.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4113 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_provider_metadata_format/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:34.376352 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_provider_set/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_provider_set/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2308 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_provider_set/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2579 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_provider_set/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:34.421787 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_request_page/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_request_page/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1637 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_request_page/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1408 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_request_page/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:34.476907 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_settings/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_settings/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      465 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_settings/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1651 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_settings/discover.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1017 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_settings/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:34.525511 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_xsl_template/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_xsl_template/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2595 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_xsl_template/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3598 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_xsl_template/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      584 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/menus.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:34.574761 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/migrations/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7245 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/migrations/0001_initial.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      900 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/migrations/0002_oai_data_on_delete.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      527 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/migrations/0003_oai_data_bulk_delete.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/migrations/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:34.620583 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:34.657695 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/rest/oai_provider_metadata_format/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/rest/oai_provider_metadata_format/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14117 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/rest/oai_provider_metadata_format/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:34.692253 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/rest/oai_provider_set/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/rest/oai_provider_set/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7772 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/rest/oai_provider_set/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:34.743776 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/rest/oai_settings/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/rest/oai_settings/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4347 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/rest/oai_settings/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7797 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/rest/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1759 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/rest/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1568 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:33.482442 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:33.561710 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:33.530994 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:33.493589 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:33.513690 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/registry/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:34.772426 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/registry/identity/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      584 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/registry/identity/table_info.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:34.789927 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/registry/metadata_formats/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      183 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/registry/metadata_formats/page.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:34.807505 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/registry/sets/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       63 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/registry/sets/add_set.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:33.534470 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/js/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:33.537794 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/js/registry/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:34.844033 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/js/registry/identity/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1082 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/js/registry/identity/check_registry.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       91 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/js/registry/identity/check_registry.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:34.872195 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/xsd/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1444 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/xsd/oai_dc.xsd
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3029 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/xsd/simpledc20021212.xsd
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:34.907192 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/system/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/system/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      490 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/system/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1976 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/tasks.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:33.602504 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:33.638078 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:33.610512 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:34.979847 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:34.996293 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/identity/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2016 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/identity/table.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      259 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/identity.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:35.043552 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/metadata_formats/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1408 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/metadata_formats/table_default.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2232 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/metadata_formats/table_metadata_formats.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2013 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/metadata_formats/table_template_metadata_formats.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      502 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/metadata_formats.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:35.059590 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/sets/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1799 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/sets/table.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      251 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/sets.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:35.075751 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/xsl_template/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1877 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/xsl_template/table.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      382 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/xsl_template.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:33.647604 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:35.244524 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      717 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/base.html
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      201 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/error.html
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      635 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/get_record.html
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      254 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/header.html
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     1118 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/identify.html
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      374 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/list_identifiers.html
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      407 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/list_metadata_formats.html
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      577 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/list_records.html
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     1030 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/list_sets.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      298 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/resumption_token.xml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      566 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:35.276029 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/utils/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5850 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/utils/request_checker.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:35.293151 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:35.347323 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/views/admin/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11317 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/views/admin/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7785 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/views/admin/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7309 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/views/admin/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:35.375686 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    24356 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/views/user/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:34.106797 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1118 2023-05-02 19:47:32.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7656 2023-05-02 19:47:33.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:47:32.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      131 2023-05-02 19:47:32.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       36 2023-05-02 19:47:32.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app.egg-info/top_level.txt
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:35.450021 core_oaipmh_provider_app-2.3.0/docs/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/docs/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11332 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/docs/conf.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      311 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/docs/conf_urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       69 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:47:36.360168 core_oaipmh_provider_app-2.3.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1481 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:35.494883 core_oaipmh_provider_app-2.3.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:35.520025 core_oaipmh_provider_app-2.3.0/tests/apps/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/apps/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1799 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/apps/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:35.534071 core_oaipmh_provider_app-2.3.0/tests/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:35.551826 core_oaipmh_provider_app-2.3.0/tests/components/oai_data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1527 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/components/oai_data/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:35.599741 core_oaipmh_provider_app-2.3.0/tests/components/oai_data/api/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/components/oai_data/api/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2277 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/components/oai_data/api/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9480 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/components/oai_data/api/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:35.647009 core_oaipmh_provider_app-2.3.0/tests/components/oai_data/models/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/components/oai_data/models/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1315 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/components/oai_data/models/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7942 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/components/oai_data/models/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:35.682212 core_oaipmh_provider_app-2.3.0/tests/components/oai_data/watch/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/components/oai_data/watch/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1098 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/components/oai_data/watch/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:35.719308 core_oaipmh_provider_app-2.3.0/tests/components/oai_provider_metadata_format/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/components/oai_provider_metadata_format/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    13665 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/components/oai_provider_metadata_format/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:35.754989 core_oaipmh_provider_app-2.3.0/tests/components/oai_provider_set/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/components/oai_provider_set/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9462 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/components/oai_provider_set/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:35.804848 core_oaipmh_provider_app-2.3.0/tests/components/oai_settings/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/components/oai_settings/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2770 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/components/oai_settings/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:35.853458 core_oaipmh_provider_app-2.3.0/tests/components/oai_xsl_template/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/components/oai_xsl_template/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9663 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/components/oai_xsl_template/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:35.870952 core_oaipmh_provider_app-2.3.0/tests/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:35.937357 core_oaipmh_provider_app-2.3.0/tests/rest/oai_provider_metadata_format/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/rest/oai_provider_metadata_format/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6987 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/rest/oai_provider_metadata_format/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    16462 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/rest/oai_provider_metadata_format/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17947 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/rest/oai_provider_metadata_format/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:36.036130 core_oaipmh_provider_app-2.3.0/tests/rest/oai_provider_set/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/rest/oai_provider_set/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5329 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/rest/oai_provider_set/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8591 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/rest/oai_provider_set/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5925 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/rest/oai_provider_set/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:36.099854 core_oaipmh_provider_app-2.3.0/tests/rest/oai_settings/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/rest/oai_settings/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2618 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/rest/oai_settings/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4840 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/rest/oai_settings/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3149 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/rest/oai_settings/tests_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1924 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:36.173611 core_oaipmh_provider_app-2.3.0/tests/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/utils/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:36.208734 core_oaipmh_provider_app-2.3.0/tests/utils/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/utils/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12394 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/utils/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      539 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/utils/mocks.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1299 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/utils/test_oai_pmh_suite.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:36.223141 core_oaipmh_provider_app-2.3.0/tests/utils/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/utils/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:36.275453 core_oaipmh_provider_app-2.3.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:31.000000 core_oaipmh_provider_app-2.3.0/tests/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:36.336074 core_oaipmh_provider_app-2.3.0/tests/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:31.000000 core_oaipmh_provider_app-2.3.0/tests/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5607 2023-05-02 19:47:31.000000 core_oaipmh_provider_app-2.3.0/tests/views/user/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    45422 2023-05-02 19:47:31.000000 core_oaipmh_provider_app-2.3.0/tests/views/user/tests_unit.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `core_oaipmh_provider_app-2.2.0/PKG-INFO` & `core_oaipmh_provider_app-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_oaipmh_provider_app
-Version: 2.2.0
+Version: 2.3.0
 Summary: OAI-PMH provider capabilities for the curator core project
 Home-page: https://github.com/usnistgov/core_oaipmh_provider_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: ========================
         Core Oaipmh Provider App
```

### Comparing `core_oaipmh_provider_app-2.2.0/README.rst` & `core_oaipmh_provider_app-2.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/admin.py` & `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/admin.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/apps.py` & `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/apps.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/commons/exceptions.py` & `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/commons/exceptions.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/components/oai_data/api.py` & `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_data/api.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/components/oai_data/models.py` & `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_data/models.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/components/oai_data/watch.py` & `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_data/watch.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/components/oai_provider_metadata_format/api.py` & `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_provider_metadata_format/api.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/components/oai_provider_metadata_format/discover.py` & `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_provider_metadata_format/discover.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/components/oai_provider_metadata_format/models.py` & `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_provider_metadata_format/models.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/components/oai_provider_set/api.py` & `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_provider_set/api.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/components/oai_provider_set/models.py` & `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_provider_set/models.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/components/oai_request_page/api.py` & `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_request_page/api.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/components/oai_request_page/models.py` & `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_request_page/models.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/components/oai_settings/discover.py` & `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_settings/discover.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/components/oai_settings/models.py` & `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_settings/models.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/components/oai_xsl_template/api.py` & `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_xsl_template/api.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/components/oai_xsl_template/models.py` & `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_xsl_template/models.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/menus.py` & `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/menus.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/migrations/0001_initial.py` & `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/migrations/0002_oai_data_on_delete.py` & `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/migrations/0002_oai_data_on_delete.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/migrations/0003_oai_data_bulk_delete.py` & `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/migrations/0003_oai_data_bulk_delete.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/rest/oai_provider_metadata_format/views.py` & `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/rest/oai_provider_metadata_format/views.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/rest/oai_provider_set/views.py` & `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/rest/oai_provider_set/views.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/rest/oai_settings/views.py` & `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/rest/oai_settings/views.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/rest/serializers.py` & `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/rest/serializers.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/rest/urls.py` & `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/rest/urls.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/settings.py` & `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/settings.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/registry/identity/table_info.css` & `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/registry/identity/table_info.css`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/js/registry/identity/check_registry.js` & `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/js/registry/identity/check_registry.js`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/xsd/oai_dc.xsd` & `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/xsd/oai_dc.xsd`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/xsd/simpledc20021212.xsd` & `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/xsd/simpledc20021212.xsd`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/tasks.py` & `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/tasks.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/identity/table.html` & `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/identity/table.html`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/metadata_formats/table_default.html` & `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/metadata_formats/table_default.html`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/metadata_formats/table_metadata_formats.html` & `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/metadata_formats/table_metadata_formats.html`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/metadata_formats/table_template_metadata_formats.html` & `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/metadata_formats/table_template_metadata_formats.html`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/sets/table.html` & `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/sets/table.html`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/xsl_template/table.html` & `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/xsl_template/table.html`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/base.html` & `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/base.html`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/get_record.html` & `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/get_record.html`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/identify.html` & `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/identify.html`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/list_records.html` & `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/list_records.html`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/list_sets.html` & `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/list_sets.html`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/urls.py` & `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/urls.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/utils/request_checker.py` & `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/utils/request_checker.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/views/admin/ajax.py` & `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/views/admin/ajax.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/views/admin/forms.py` & `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/views/admin/forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,15 +153,17 @@
     )
     set_name = forms.CharField(
         label="Set name",
         required=True,
         widget=forms.TextInput(attrs={"class": "form-control"}),
     )
     templates_manager = forms.MultipleChoiceField(
-        label="Templates", widget=forms.SelectMultiple(), required=True
+        label="Templates",
+        widget=forms.CheckboxSelectMultiple(attrs={"class": "double-columns"}),
+        required=True,
     )
     description = forms.CharField(
         label="Description",
         required=True,
         widget=forms.Textarea(
             attrs={
                 "cols": "60",
```

### Comparing `core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/views/admin/views.py` & `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/views/admin/views.py`

 * *Files 5% similar despite different names*

```diff
@@ -145,28 +145,20 @@
         request:
 
     Returns:
 
     """
     assets = {
         "js": [
-            {
-                "path": "core_oaipmh_provider_app/admin/js/registry/sets/modals/init_select.js",
-                "is_raw": False,
-            },
-            {
-                "path": "core_oaipmh_provider_app/admin/libs/fSelect/js/fSelect.js",
-                "is_raw": False,
-            },
             AddObjectModalView.get_modal_js_path(),
             EditObjectModalView.get_modal_js_path(),
             DeleteObjectModalView.get_modal_js_path(),
         ],
         "css": [
-            "core_oaipmh_provider_app/admin/libs/fSelect/css/fSelect.css",
+            "core_main_app/common/css/select.css",
             "core_oaipmh_provider_app/admin/css/registry/sets/add_set.css",
         ],
     }
 
     modals = [
         AddObjectModalView.get_modal_html_path(),
         EditObjectModalView.get_modal_html_path(),
```

### Comparing `core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app/views/user/views.py` & `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/views/user/views.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app.egg-info/PKG-INFO` & `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-oaipmh-provider-app
-Version: 2.2.0
+Version: 2.3.0
 Summary: OAI-PMH provider capabilities for the curator core project
 Home-page: https://github.com/usnistgov/core_oaipmh_provider_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: ========================
         Core Oaipmh Provider App
```

### Comparing `core_oaipmh_provider_app-2.2.0/core_oaipmh_provider_app.egg-info/SOURCES.txt` & `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.md
 MANIFEST.in
 README.rst
 pyproject.toml
 requirements.core.txt
 setup.py
 core_oaipmh_provider_app/__init__.py
 core_oaipmh_provider_app/admin.py
@@ -55,17 +56,14 @@
 core_oaipmh_provider_app/rest/oai_settings/__init__.py
 core_oaipmh_provider_app/rest/oai_settings/views.py
 core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/registry/identity/table_info.css
 core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/registry/metadata_formats/page.css
 core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/registry/sets/add_set.css
 core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/js/registry/identity/check_registry.js
 core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/js/registry/identity/check_registry.raw.js
-core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/js/registry/sets/modals/init_select.js
-core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/libs/fSelect/css/fSelect.css
-core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/libs/fSelect/js/fSelect.js
 core_oaipmh_provider_app/static/core_oaipmh_provider_app/xsd/oai_dc.xsd
 core_oaipmh_provider_app/static/core_oaipmh_provider_app/xsd/simpledc20021212.xsd
 core_oaipmh_provider_app/system/__init__.py
 core_oaipmh_provider_app/system/api.py
 core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/identity.html
 core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/metadata_formats.html
 core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/sets.html
```

### Comparing `core_oaipmh_provider_app-2.2.0/docs/conf.py` & `core_oaipmh_provider_app-2.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/setup.py` & `core_oaipmh_provider_app-2.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_oaipmh_provider_app",
-    version="2.2.0",
+    version="2.3.0",
     description="OAI-PMH provider capabilities for the curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_oaipmh_provider_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_oaipmh_provider_app-2.2.0/tests/apps/tests_unit.py` & `core_oaipmh_provider_app-2.3.0/tests/apps/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/tests/components/oai_data/__init__.py` & `core_oaipmh_provider_app-2.3.0/tests/components/oai_data/__init__.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/tests/components/oai_data/api/tests_int.py` & `core_oaipmh_provider_app-2.3.0/tests/components/oai_data/api/tests_int.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """ Integrations testing of the OaiData API
 """
 from django.db.models import Q
 
 from core_main_app.components.data.models import Data
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 from core_oaipmh_provider_app.components.oai_data import api as oai_data_api
 from tests.utils.fixtures.fixtures import OaiPmhFixtures, OaiPmhMock
 
 
-class TestUpsertFromData(MongoIntegrationBaseTestCase):
+class TestUpsertFromData(IntegrationBaseTestCase):
     """Test upsert_from_data API call"""
 
     fixture = OaiPmhFixtures()
 
     def setUp(self):
         """setUp"""
         super().setUp()
```

### Comparing `core_oaipmh_provider_app-2.2.0/tests/components/oai_data/api/tests_unit.py` & `core_oaipmh_provider_app-2.3.0/tests/components/oai_data/api/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/tests/components/oai_data/models/tests_int.py` & `core_oaipmh_provider_app-2.3.0/tests/components/oai_data/models/tests_int.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 """ Integration testing of OaiData model
 """
 from core_main_app.system import api as system_api
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 from core_oaipmh_provider_app.components.oai_data.models import OaiData
 from tests.utils.fixtures.fixtures import OaiPmhFixtures
 
 
-class TestOaiDataGetAllByTemplateListAndTimeframe(
-    MongoIntegrationBaseTestCase
-):
+class TestOaiDataGetAllByTemplateListAndTimeframe(IntegrationBaseTestCase):
     """Test OaiData get_all_by_template_list_and_timeframe method"""
 
     fixture = OaiPmhFixtures()
 
     def test_correct_items_returned(self):
         """test_correct_items_returned"""
         template = system_api.get_template_by_id(1)
         results = OaiData.get_all_by_template_list_and_timeframe(
             [template], None, None
         )
 
         self.assertEqual(list(results), list(OaiData.objects.all()))
 
 
-class TestOaiDataGetAllByTemplateAndTimeframe(MongoIntegrationBaseTestCase):
+class TestOaiDataGetAllByTemplateAndTimeframe(IntegrationBaseTestCase):
     """Test OaiData get_all_by_template_and_timeframe method"""
 
     fixture = OaiPmhFixtures()
 
     def test_correct_items_returned(self):
         """test_correct_items_returned"""
         template = system_api.get_template_by_id(1)
```

### Comparing `core_oaipmh_provider_app-2.2.0/tests/components/oai_data/models/tests_unit.py` & `core_oaipmh_provider_app-2.3.0/tests/components/oai_data/models/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/tests/components/oai_data/watch/tests_unit.py` & `core_oaipmh_provider_app-2.3.0/tests/components/oai_data/watch/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/tests/components/oai_provider_metadata_format/tests_unit.py` & `core_oaipmh_provider_app-2.3.0/tests/components/oai_provider_metadata_format/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/tests/components/oai_provider_set/tests_unit.py` & `core_oaipmh_provider_app-2.3.0/tests/components/oai_provider_set/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/tests/components/oai_settings/tests_unit.py` & `core_oaipmh_provider_app-2.3.0/tests/components/oai_settings/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/tests/components/oai_xsl_template/tests_unit.py` & `core_oaipmh_provider_app-2.3.0/tests/components/oai_xsl_template/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/tests/rest/oai_provider_metadata_format/tests_int.py` & `core_oaipmh_provider_app-2.3.0/tests/rest/oai_provider_metadata_format/tests_int.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
 from unittest.mock import Mock, patch
 
 from requests import Response
 from rest_framework import status
 
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from core_main_app.utils.tests_tools.RequestMock import RequestMock
 from core_oaipmh_provider_app.components.oai_provider_metadata_format import (
     api as oai_provider_metadata_format_api,
 )
 from core_oaipmh_provider_app.components.oai_provider_metadata_format.models import (
@@ -18,15 +18,15 @@
 )
 from core_oaipmh_provider_app.rest.oai_provider_metadata_format import (
     views as rest_oai_provider_metadata_format,
 )
 from tests.utils.fixtures.fixtures import OaiPmhFixtures, OaiPmhMock
 
 
-class TestSelectMetadataFormat(MongoIntegrationBaseTestCase):
+class TestSelectMetadataFormat(IntegrationBaseTestCase):
     """Test Select Metadata Format"""
 
     fixture = OaiPmhFixtures()
 
     def setUp(self):
         """setUp"""
 
@@ -50,15 +50,15 @@
             param=self.param,
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_200_OK)
 
 
-class TestSelectAllMetadataFormats(MongoIntegrationBaseTestCase):
+class TestSelectAllMetadataFormats(IntegrationBaseTestCase):
     """Test Select All Metadata Formats"""
 
     fixture = OaiPmhFixtures()
 
     def setUp(self):
         """setUp"""
 
@@ -78,15 +78,15 @@
             self.data,
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_200_OK)
 
 
-class TestAddMetadataFormat(MongoIntegrationBaseTestCase):
+class TestAddMetadataFormat(IntegrationBaseTestCase):
     """Test Add Metadata Format"""
 
     fixture = OaiPmhFixtures()
 
     def setUp(self):
         """setUp"""
 
@@ -121,15 +121,15 @@
         self.assertEqual(response.status_code, status.HTTP_201_CREATED)
         self.assertEqual(
             len(OaiProviderMetadataFormat.objects.all()),
             self.nb_metadata_formats + 1,
         )
 
 
-class TestAddTemplateMetadataFormat(MongoIntegrationBaseTestCase):
+class TestAddTemplateMetadataFormat(IntegrationBaseTestCase):
     """Test Add Template Metadata Format"""
 
     fixture = OaiPmhFixtures()
 
     def setUp(self):
         """setUp"""
 
@@ -159,15 +159,15 @@
         self.assertEqual(response.status_code, status.HTTP_201_CREATED)
         self.assertEqual(
             len(OaiProviderMetadataFormat.objects.all()),
             self.nb_template_metadata_formats + 1,
         )
 
 
-class TestDeleteMetadataFormat(MongoIntegrationBaseTestCase):
+class TestDeleteMetadataFormat(IntegrationBaseTestCase):
     """Test Delete Metadata Format"""
 
     fixture = OaiPmhFixtures()
 
     def setUp(self):
         """setUp"""
 
@@ -196,15 +196,15 @@
         self.assertEqual(response.status_code, status.HTTP_204_NO_CONTENT)
         self.assertEqual(
             len(OaiProviderMetadataFormat.objects.all()),
             self.nb_metadata_formats - 1,
         )
 
 
-class TestUpdateMetadataFormat(MongoIntegrationBaseTestCase):
+class TestUpdateMetadataFormat(IntegrationBaseTestCase):
     """Test Update Metadata Format"""
 
     fixture = OaiPmhFixtures()
 
     def setUp(self):
         """setUp"""
```

### Comparing `core_oaipmh_provider_app-2.2.0/tests/rest/oai_provider_metadata_format/tests_permissions.py` & `core_oaipmh_provider_app-2.3.0/tests/rest/oai_provider_metadata_format/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/tests/rest/oai_provider_metadata_format/tests_unit.py` & `core_oaipmh_provider_app-2.3.0/tests/rest/oai_provider_metadata_format/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/tests/rest/oai_provider_set/tests_int.py` & `core_oaipmh_provider_app-2.3.0/tests/rest/oai_provider_set/tests_int.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """ Int Test Rest OaiProviderSet
 """
 
 from rest_framework import status
 
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from core_main_app.utils.tests_tools.RequestMock import RequestMock
 from core_oaipmh_provider_app.components.oai_provider_set.models import (
     OaiProviderSet,
 )
 from core_oaipmh_provider_app.rest.oai_provider_set import (
     views as rest_oai_provider_set,
 )
 from tests.utils.fixtures.fixtures import OaiPmhFixtures, OaiPmhMock
 
 
-class TestSelectSet(MongoIntegrationBaseTestCase):
+class TestSelectSet(IntegrationBaseTestCase):
     """Test Select Set"""
 
     fixture = OaiPmhFixtures()
 
     def setUp(self):
         """setUp"""
 
@@ -41,15 +41,15 @@
             param=self.param,
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_200_OK)
 
 
-class TestSelectAllSets(MongoIntegrationBaseTestCase):
+class TestSelectAllSets(IntegrationBaseTestCase):
     """Test Select All Sets"""
 
     fixture = OaiPmhFixtures()
 
     def setUp(self):
         """setUp"""
 
@@ -67,15 +67,15 @@
             rest_oai_provider_set.SetsList.as_view(), user, self.data
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_200_OK)
 
 
-class TestAddSet(MongoIntegrationBaseTestCase):
+class TestAddSet(IntegrationBaseTestCase):
     """Test Add Set"""
 
     fixture = OaiPmhFixtures()
 
     def setUp(self):
         """setUp"""
 
@@ -100,15 +100,15 @@
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_201_CREATED)
         self.assertEqual(len(OaiProviderSet.objects.all()), self.nb_sets + 1)
 
 
-class TestDeleteSet(MongoIntegrationBaseTestCase):
+class TestDeleteSet(IntegrationBaseTestCase):
     """Test Delete Set"""
 
     fixture = OaiPmhFixtures()
 
     def setUp(self):
         """setUp"""
 
@@ -128,15 +128,15 @@
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_204_NO_CONTENT)
         self.assertEqual(len(OaiProviderSet.objects.all()), self.nb_sets - 1)
 
 
-class TestUpdateSet(MongoIntegrationBaseTestCase):
+class TestUpdateSet(IntegrationBaseTestCase):
     """Test Update Set"""
 
     fixture = OaiPmhFixtures()
 
     def setUp(self):
         """setUp"""
```

### Comparing `core_oaipmh_provider_app-2.2.0/tests/rest/oai_provider_set/tests_permissions.py` & `core_oaipmh_provider_app-2.3.0/tests/rest/oai_provider_set/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/tests/rest/oai_provider_set/tests_unit.py` & `core_oaipmh_provider_app-2.3.0/tests/rest/oai_provider_set/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/tests/rest/oai_settings/tests_int.py` & `core_oaipmh_provider_app-2.3.0/tests/rest/oai_settings/tests_int.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """ Int Test Rest OaiSettings
 """
 
 from rest_framework import status
 
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from core_main_app.utils.tests_tools.RequestMock import RequestMock
 from core_oaipmh_provider_app.components.oai_settings.models import OaiSettings
 from core_oaipmh_provider_app.rest.oai_settings import (
     views as rest_oai_settings,
 )
 from tests.utils.fixtures.fixtures import OaiPmhFixtures
 
 
-class TestSelect(MongoIntegrationBaseTestCase):
+class TestSelect(IntegrationBaseTestCase):
     """Test Select"""
 
     fixture = OaiPmhFixtures()
 
     def setUp(self):
         """setUp"""
 
@@ -37,15 +37,15 @@
             rest_oai_settings.Settings.as_view(), user=user, data=self.data
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_200_OK)
 
 
-class TestUpdateSettings(MongoIntegrationBaseTestCase):
+class TestUpdateSettings(IntegrationBaseTestCase):
     """Test Update Settings"""
 
     fixture = OaiPmhFixtures()
 
     def setUp(self):
         """setUp"""
```

### Comparing `core_oaipmh_provider_app-2.2.0/tests/rest/oai_settings/tests_permissions.py` & `core_oaipmh_provider_app-2.3.0/tests/rest/oai_settings/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/tests/rest/oai_settings/tests_unit.py` & `core_oaipmh_provider_app-2.3.0/tests/rest/oai_settings/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/tests/test_settings.py` & `core_oaipmh_provider_app-2.3.0/tests/test_settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,7 +75,8 @@
 USE_TZ = True
 
 DEFAULT_AUTO_FIELD = "django.db.models.BigAutoField"
 CELERYBEAT_SCHEDULER = "django_celery_beat.schedulers:DatabaseScheduler"
 
 MONGODB_INDEXING = False
 MONGODB_ASYNC_SAVE = False
+ENABLE_SAML2_SSO_AUTH = False
```

### Comparing `core_oaipmh_provider_app-2.2.0/tests/utils/fixtures/fixtures.py` & `core_oaipmh_provider_app-2.3.0/tests/utils/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/tests/utils/mocks.py` & `core_oaipmh_provider_app-2.3.0/tests/utils/mocks.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/tests/utils/test_oai_pmh_suite.py` & `core_oaipmh_provider_app-2.3.0/tests/utils/test_oai_pmh_suite.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.2.0/tests/views/user/tests_int.py` & `core_oaipmh_provider_app-2.3.0/tests/views/user/tests_int.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 """
 from unittest.mock import patch, PropertyMock
 
 from rest_framework import status
 
 from core_main_app.components.data.models import Data
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from core_main_app.utils.tests_tools.RequestMock import RequestMock
 from core_oaipmh_provider_app.components.oai_provider_metadata_format import (
     api as oai_provider_metadata_format_api,
 )
 from core_oaipmh_provider_app.views.user.views import OAIProviderView
 from tests.utils.fixtures.fixtures import OaiPmhFixtures
 from tests.utils.test_oai_pmh_suite import TestOaiPmhSuite
 
 
-class TestVerbs(TestOaiPmhSuite, MongoIntegrationBaseTestCase):
-    """MongoIntegrationBaseTestCase"""
+class TestVerbs(TestOaiPmhSuite, IntegrationBaseTestCase):
+    """IntegrationBaseTestCase"""
 
     fixture = OaiPmhFixtures()
 
     def test_identify(self):
         """test_identify"""
 
         # Arrange
```

### Comparing `core_oaipmh_provider_app-2.2.0/tests/views/user/tests_unit.py` & `core_oaipmh_provider_app-2.3.0/tests/views/user/tests_unit.py`

 * *Files identical despite different names*

