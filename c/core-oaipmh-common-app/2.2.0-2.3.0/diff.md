# Comparing `tmp/core_oaipmh_common_app-2.2.0.tar.gz` & `tmp/core_oaipmh_common_app-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/core_oaipmh_common_app-2.2.0.tar", last modified: Thu Feb 23 20:33:18 2023, max compression
+gzip compressed data, was "core_oaipmh_common_app-2.3.0.tar", last modified: Tue May  2 19:46:58 2023, max compression
```

## Comparing `core_oaipmh_common_app-2.2.0.tar` & `core_oaipmh_common_app-2.3.0.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:18.000000 core_oaipmh_common_app-2.2.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      177 2023-02-23 20:33:15.000000 core_oaipmh_common_app-2.2.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1089 2023-02-23 20:33:18.000000 core_oaipmh_common_app-2.2.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      593 2023-02-23 20:33:15.000000 core_oaipmh_common_app-2.2.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:18.000000 core_oaipmh_common_app-2.2.0/core_oaipmh_common_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:15.000000 core_oaipmh_common_app-2.2.0/core_oaipmh_common_app/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:18.000000 core_oaipmh_common_app-2.2.0/core_oaipmh_common_app/commons/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:15.000000 core_oaipmh_common_app-2.2.0/core_oaipmh_common_app/commons/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1643 2023-02-23 20:33:15.000000 core_oaipmh_common_app-2.2.0/core_oaipmh_common_app/commons/exceptions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      798 2023-02-23 20:33:15.000000 core_oaipmh_common_app-2.2.0/core_oaipmh_common_app/commons/messages.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:18.000000 core_oaipmh_common_app-2.2.0/core_oaipmh_common_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:15.000000 core_oaipmh_common_app-2.2.0/core_oaipmh_common_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:18.000000 core_oaipmh_common_app-2.2.0/core_oaipmh_common_app/components/oai_metadata_format/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:15.000000 core_oaipmh_common_app-2.2.0/core_oaipmh_common_app/components/oai_metadata_format/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1094 2023-02-23 20:33:15.000000 core_oaipmh_common_app-2.2.0/core_oaipmh_common_app/components/oai_metadata_format/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2908 2023-02-23 20:33:15.000000 core_oaipmh_common_app-2.2.0/core_oaipmh_common_app/components/oai_metadata_format/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:18.000000 core_oaipmh_common_app-2.2.0/core_oaipmh_common_app/components/oai_set/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:15.000000 core_oaipmh_common_app-2.2.0/core_oaipmh_common_app/components/oai_set/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      795 2023-02-23 20:33:16.000000 core_oaipmh_common_app-2.2.0/core_oaipmh_common_app/components/oai_set/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2033 2023-02-23 20:33:16.000000 core_oaipmh_common_app-2.2.0/core_oaipmh_common_app/components/oai_set/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:18.000000 core_oaipmh_common_app-2.2.0/core_oaipmh_common_app/migrations/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:16.000000 core_oaipmh_common_app-2.2.0/core_oaipmh_common_app/migrations/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:18.000000 core_oaipmh_common_app-2.2.0/core_oaipmh_common_app/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      819 2023-02-23 20:33:16.000000 core_oaipmh_common_app-2.2.0/core_oaipmh_common_app/utils/UTCdatetime.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:16.000000 core_oaipmh_common_app-2.2.0/core_oaipmh_common_app/utils/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:18.000000 core_oaipmh_common_app-2.2.0/core_oaipmh_common_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1089 2023-02-23 20:33:17.000000 core_oaipmh_common_app-2.2.0/core_oaipmh_common_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1361 2023-02-23 20:33:17.000000 core_oaipmh_common_app-2.2.0/core_oaipmh_common_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-02-23 20:33:17.000000 core_oaipmh_common_app-2.2.0/core_oaipmh_common_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       63 2023-02-23 20:33:17.000000 core_oaipmh_common_app-2.2.0/core_oaipmh_common_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       29 2023-02-23 20:33:17.000000 core_oaipmh_common_app-2.2.0/core_oaipmh_common_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-02-23 20:33:16.000000 core_oaipmh_common_app-2.2.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       21 2023-02-23 20:33:16.000000 core_oaipmh_common_app-2.2.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       42 2023-02-23 20:33:16.000000 core_oaipmh_common_app-2.2.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-02-23 20:33:18.000000 core_oaipmh_common_app-2.2.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1420 2023-02-23 20:33:16.000000 core_oaipmh_common_app-2.2.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:18.000000 core_oaipmh_common_app-2.2.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:16.000000 core_oaipmh_common_app-2.2.0/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:18.000000 core_oaipmh_common_app-2.2.0/tests/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:16.000000 core_oaipmh_common_app-2.2.0/tests/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:18.000000 core_oaipmh_common_app-2.2.0/tests/components/oai_metadata_format/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:16.000000 core_oaipmh_common_app-2.2.0/tests/components/oai_metadata_format/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6179 2023-02-23 20:33:16.000000 core_oaipmh_common_app-2.2.0/tests/components/oai_metadata_format/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:18.000000 core_oaipmh_common_app-2.2.0/tests/components/oai_set/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:16.000000 core_oaipmh_common_app-2.2.0/tests/components/oai_set/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:18.000000 core_oaipmh_common_app-2.2.0/tests/components/oai_set/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:16.000000 core_oaipmh_common_app-2.2.0/tests/components/oai_set/tests/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4771 2023-02-23 20:33:16.000000 core_oaipmh_common_app-2.2.0/tests/components/oai_set/tests/tests_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1510 2023-02-23 20:33:16.000000 core_oaipmh_common_app-2.2.0/tests/test_settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:18.000000 core_oaipmh_common_app-2.2.0/tests/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:33:16.000000 core_oaipmh_common_app-2.2.0/tests/utils/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1286 2023-02-23 20:33:16.000000 core_oaipmh_common_app-2.2.0/tests/utils/tests_iso8601_operation.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:58.567983 core_oaipmh_common_app-2.3.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:46:55.000000 core_oaipmh_common_app-2.3.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      177 2023-05-02 19:46:55.000000 core_oaipmh_common_app-2.3.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1089 2023-05-02 19:46:58.563030 core_oaipmh_common_app-2.3.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      593 2023-05-02 19:46:55.000000 core_oaipmh_common_app-2.3.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:58.107177 core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:55.000000 core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:58.218639 core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/commons/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:55.000000 core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/commons/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1643 2023-05-02 19:46:55.000000 core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/commons/exceptions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      798 2023-05-02 19:46:55.000000 core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/commons/messages.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:58.233531 core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:55.000000 core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:58.275369 core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/components/oai_metadata_format/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:55.000000 core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/components/oai_metadata_format/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1094 2023-05-02 19:46:55.000000 core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/components/oai_metadata_format/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2908 2023-05-02 19:46:55.000000 core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/components/oai_metadata_format/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:58.330635 core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/components/oai_set/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:55.000000 core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/components/oai_set/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      795 2023-05-02 19:46:55.000000 core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/components/oai_set/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2033 2023-05-02 19:46:55.000000 core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/components/oai_set/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:58.344536 core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/migrations/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:55.000000 core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/migrations/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:58.370711 core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      819 2023-05-02 19:46:55.000000 core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/utils/UTCdatetime.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:55.000000 core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/utils/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:58.176063 core_oaipmh_common_app-2.3.0/core_oaipmh_common_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1089 2023-05-02 19:46:57.000000 core_oaipmh_common_app-2.3.0/core_oaipmh_common_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1372 2023-05-02 19:46:57.000000 core_oaipmh_common_app-2.3.0/core_oaipmh_common_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:46:57.000000 core_oaipmh_common_app-2.3.0/core_oaipmh_common_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       63 2023-05-02 19:46:57.000000 core_oaipmh_common_app-2.3.0/core_oaipmh_common_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       29 2023-05-02 19:46:57.000000 core_oaipmh_common_app-2.3.0/core_oaipmh_common_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:46:56.000000 core_oaipmh_common_app-2.3.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       21 2023-05-02 19:46:56.000000 core_oaipmh_common_app-2.3.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       42 2023-05-02 19:46:56.000000 core_oaipmh_common_app-2.3.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:46:58.569823 core_oaipmh_common_app-2.3.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1420 2023-05-02 19:46:56.000000 core_oaipmh_common_app-2.3.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:58.410889 core_oaipmh_common_app-2.3.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:56.000000 core_oaipmh_common_app-2.3.0/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:58.421177 core_oaipmh_common_app-2.3.0/tests/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:56.000000 core_oaipmh_common_app-2.3.0/tests/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:58.465680 core_oaipmh_common_app-2.3.0/tests/components/oai_metadata_format/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:56.000000 core_oaipmh_common_app-2.3.0/tests/components/oai_metadata_format/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6179 2023-05-02 19:46:56.000000 core_oaipmh_common_app-2.3.0/tests/components/oai_metadata_format/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:58.489570 core_oaipmh_common_app-2.3.0/tests/components/oai_set/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:56.000000 core_oaipmh_common_app-2.3.0/tests/components/oai_set/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:58.521817 core_oaipmh_common_app-2.3.0/tests/components/oai_set/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:56.000000 core_oaipmh_common_app-2.3.0/tests/components/oai_set/tests/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4771 2023-05-02 19:46:56.000000 core_oaipmh_common_app-2.3.0/tests/components/oai_set/tests/tests_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1510 2023-05-02 19:46:56.000000 core_oaipmh_common_app-2.3.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:58.552923 core_oaipmh_common_app-2.3.0/tests/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:46:56.000000 core_oaipmh_common_app-2.3.0/tests/utils/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1286 2023-05-02 19:46:56.000000 core_oaipmh_common_app-2.3.0/tests/utils/tests_iso8601_operation.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `core_oaipmh_common_app-2.2.0/PKG-INFO` & `core_oaipmh_common_app-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_oaipmh_common_app
-Version: 2.2.0
+Version: 2.3.0
 Summary: Base OAI-PMH functions for the curator core project
 Home-page: https://github.com/usnistgov/core_oaipmh_common_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: ======================
         Core Oaipmh Common App
```

### Comparing `core_oaipmh_common_app-2.2.0/README.rst` & `core_oaipmh_common_app-2.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_oaipmh_common_app-2.2.0/core_oaipmh_common_app/commons/exceptions.py` & `core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/commons/exceptions.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_common_app-2.2.0/core_oaipmh_common_app/commons/messages.py` & `core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/commons/messages.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_common_app-2.2.0/core_oaipmh_common_app/components/oai_metadata_format/api.py` & `core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/components/oai_metadata_format/api.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_common_app-2.2.0/core_oaipmh_common_app/components/oai_metadata_format/models.py` & `core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/components/oai_metadata_format/models.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_common_app-2.2.0/core_oaipmh_common_app/components/oai_set/api.py` & `core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/components/oai_set/api.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_common_app-2.2.0/core_oaipmh_common_app/components/oai_set/models.py` & `core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/components/oai_set/models.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_common_app-2.2.0/core_oaipmh_common_app/utils/UTCdatetime.py` & `core_oaipmh_common_app-2.3.0/core_oaipmh_common_app/utils/UTCdatetime.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_common_app-2.2.0/core_oaipmh_common_app.egg-info/PKG-INFO` & `core_oaipmh_common_app-2.3.0/core_oaipmh_common_app.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-oaipmh-common-app
-Version: 2.2.0
+Version: 2.3.0
 Summary: Base OAI-PMH functions for the curator core project
 Home-page: https://github.com/usnistgov/core_oaipmh_common_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: ======================
         Core Oaipmh Common App
```

### Comparing `core_oaipmh_common_app-2.2.0/core_oaipmh_common_app.egg-info/SOURCES.txt` & `core_oaipmh_common_app-2.3.0/core_oaipmh_common_app.egg-info/SOURCES.txt`

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
 core_oaipmh_common_app/__init__.py
```

### Comparing `core_oaipmh_common_app-2.2.0/setup.py` & `core_oaipmh_common_app-2.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_oaipmh_common_app",
-    version="2.2.0",
+    version="2.3.0",
     description="Base OAI-PMH functions for the curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_oaipmh_common_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_oaipmh_common_app-2.2.0/tests/components/oai_metadata_format/tests_unit.py` & `core_oaipmh_common_app-2.3.0/tests/components/oai_metadata_format/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_common_app-2.2.0/tests/components/oai_set/tests/tests_unit.py` & `core_oaipmh_common_app-2.3.0/tests/components/oai_set/tests/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_common_app-2.2.0/tests/test_settings.py` & `core_oaipmh_common_app-2.3.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_common_app-2.2.0/tests/utils/tests_iso8601_operation.py` & `core_oaipmh_common_app-2.3.0/tests/utils/tests_iso8601_operation.py`

 * *Files identical despite different names*

