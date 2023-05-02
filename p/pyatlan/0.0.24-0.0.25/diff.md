# Comparing `tmp/pyatlan-0.0.24.tar.gz` & `tmp/pyatlan-0.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyatlan-0.0.24.tar", last modified: Thu Apr 27 17:34:54 2023, max compression
+gzip compressed data, was "pyatlan-0.0.25.tar", last modified: Tue May  2 14:02:19 2023, max compression
```

## Comparing `pyatlan-0.0.24.tar` & `pyatlan-0.0.25.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:34:54.862131 pyatlan-0.0.24/
--rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-04-27 17:34:39.000000 pyatlan-0.0.24/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-27 17:34:39.000000 pyatlan-0.0.24/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-27 17:34:39.000000 pyatlan-0.0.24/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-27 17:34:54.862131 pyatlan-0.0.24/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-27 17:34:39.000000 pyatlan-0.0.24/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:34:54.854131 pyatlan-0.0.24/pyatlan/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-27 17:34:39.000000 pyatlan-0.0.24/pyatlan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:34:54.854131 pyatlan-0.0.24/pyatlan/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-27 17:34:39.000000 pyatlan-0.0.24/pyatlan/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-27 17:34:39.000000 pyatlan-0.0.24/pyatlan/cache/classification_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     9761 2023-04-27 17:34:39.000000 pyatlan-0.0.24/pyatlan/cache/custom_metadata_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-27 17:34:39.000000 pyatlan-0.0.24/pyatlan/cache/role_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:34:54.854131 pyatlan-0.0.24/pyatlan/client/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-27 17:34:39.000000 pyatlan-0.0.24/pyatlan/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20816 2023-04-27 17:34:39.000000 pyatlan-0.0.24/pyatlan/client/atlan.py
--rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-04-27 17:34:39.000000 pyatlan-0.0.24/pyatlan/client/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-04-27 17:34:39.000000 pyatlan-0.0.24/pyatlan/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-04-27 17:34:39.000000 pyatlan-0.0.24/pyatlan/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:34:54.854131 pyatlan-0.0.24/pyatlan/generator/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-27 17:34:39.000000 pyatlan-0.0.24/pyatlan/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-04-27 17:34:39.000000 pyatlan-0.0.24/pyatlan/generator/generate_from_typdefs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:34:54.854131 pyatlan-0.0.24/pyatlan/generator/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-27 17:34:39.000000 pyatlan-0.0.24/pyatlan/generator/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:34:54.858131 pyatlan-0.0.24/pyatlan/model/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-27 17:34:39.000000 pyatlan-0.0.24/pyatlan/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   756677 2023-04-27 17:34:39.000000 pyatlan-0.0.24/pyatlan/model/assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-04-27 17:34:39.000000 pyatlan-0.0.24/pyatlan/model/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-04-27 17:34:39.000000 pyatlan-0.0.24/pyatlan/model/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-27 17:34:39.000000 pyatlan-0.0.24/pyatlan/model/internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-04-27 17:34:39.000000 pyatlan-0.0.24/pyatlan/model/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-27 17:34:39.000000 pyatlan-0.0.24/pyatlan/model/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    58716 2023-04-27 17:34:39.000000 pyatlan-0.0.24/pyatlan/model/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-04-27 17:34:39.000000 pyatlan-0.0.24/pyatlan/model/structs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16433 2023-04-27 17:34:39.000000 pyatlan-0.0.24/pyatlan/model/typedef.py
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-04-27 17:34:39.000000 pyatlan-0.0.24/pyatlan/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-27 17:34:39.000000 pyatlan-0.0.24/pyatlan/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:34:54.854131 pyatlan-0.0.24/pyatlan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-27 17:34:54.000000 pyatlan-0.0.24/pyatlan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-27 17:34:54.000000 pyatlan-0.0.24/pyatlan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 17:34:54.000000 pyatlan-0.0.24/pyatlan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 17:34:54.000000 pyatlan-0.0.24/pyatlan.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-27 17:34:54.000000 pyatlan-0.0.24/pyatlan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-27 17:34:54.000000 pyatlan-0.0.24/pyatlan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 17:34:54.862131 pyatlan-0.0.24/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-27 17:34:39.000000 pyatlan-0.0.24/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:34:54.858131 pyatlan-0.0.24/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-27 17:34:39.000000 pyatlan-0.0.24/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:34:54.858131 pyatlan-0.0.24/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-27 17:34:39.000000 pyatlan-0.0.24/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-27 17:34:39.000000 pyatlan-0.0.24/tests/integration/classification_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-04-27 17:34:39.000000 pyatlan-0.0.24/tests/integration/custom_metadata_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-27 17:34:39.000000 pyatlan-0.0.24/tests/integration/role_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-27 17:34:39.000000 pyatlan-0.0.24/tests/integration/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    31444 2023-04-27 17:34:39.000000 pyatlan-0.0.24/tests/integration/test_entity_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-04-27 17:34:39.000000 pyatlan-0.0.24/tests/integration/test_index_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:34:54.862131 pyatlan-0.0.24/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-27 17:34:39.000000 pyatlan-0.0.24/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-04-27 17:34:39.000000 pyatlan-0.0.24/tests/unit/test_classification_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-04-27 17:34:39.000000 pyatlan-0.0.24/tests/unit/test_glossary_term.py
--rw-r--r--   0 runner    (1001) docker     (123)    48518 2023-04-27 17:34:39.000000 pyatlan-0.0.24/tests/unit/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    31771 2023-04-27 17:34:39.000000 pyatlan-0.0.24/tests/unit/test_search_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8483 2023-04-27 17:34:39.000000 pyatlan-0.0.24/tests/unit/test_typedef_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-27 17:34:39.000000 pyatlan-0.0.24/tests/unit/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:02:19.986967 pyatlan-0.0.25/
+-rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-05-02 14:02:05.000000 pyatlan-0.0.25/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-02 14:02:05.000000 pyatlan-0.0.25/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-02 14:02:05.000000 pyatlan-0.0.25/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-02 14:02:19.986967 pyatlan-0.0.25/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-02 14:02:05.000000 pyatlan-0.0.25/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:02:19.974967 pyatlan-0.0.25/pyatlan/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-02 14:02:05.000000 pyatlan-0.0.25/pyatlan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:02:19.974967 pyatlan-0.0.25/pyatlan/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-02 14:02:05.000000 pyatlan-0.0.25/pyatlan/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-05-02 14:02:05.000000 pyatlan-0.0.25/pyatlan/cache/classification_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9761 2023-05-02 14:02:05.000000 pyatlan-0.0.25/pyatlan/cache/custom_metadata_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-02 14:02:05.000000 pyatlan-0.0.25/pyatlan/cache/role_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:02:19.978967 pyatlan-0.0.25/pyatlan/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-02 14:02:05.000000 pyatlan-0.0.25/pyatlan/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20816 2023-05-02 14:02:05.000000 pyatlan-0.0.25/pyatlan/client/atlan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-05-02 14:02:05.000000 pyatlan-0.0.25/pyatlan/client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-05-02 14:02:05.000000 pyatlan-0.0.25/pyatlan/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-05-02 14:02:05.000000 pyatlan-0.0.25/pyatlan/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:02:19.978967 pyatlan-0.0.25/pyatlan/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-02 14:02:05.000000 pyatlan-0.0.25/pyatlan/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-05-02 14:02:05.000000 pyatlan-0.0.25/pyatlan/generator/generate_from_typdefs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:02:19.978967 pyatlan-0.0.25/pyatlan/generator/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-02 14:02:05.000000 pyatlan-0.0.25/pyatlan/generator/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:02:19.982967 pyatlan-0.0.25/pyatlan/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-02 14:02:05.000000 pyatlan-0.0.25/pyatlan/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   783914 2023-05-02 14:02:05.000000 pyatlan-0.0.25/pyatlan/model/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-05-02 14:02:05.000000 pyatlan-0.0.25/pyatlan/model/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-05-02 14:02:05.000000 pyatlan-0.0.25/pyatlan/model/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-02 14:02:05.000000 pyatlan-0.0.25/pyatlan/model/internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-05-02 14:02:05.000000 pyatlan-0.0.25/pyatlan/model/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-02 14:02:05.000000 pyatlan-0.0.25/pyatlan/model/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58716 2023-05-02 14:02:05.000000 pyatlan-0.0.25/pyatlan/model/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-05-02 14:02:05.000000 pyatlan-0.0.25/pyatlan/model/structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16433 2023-05-02 14:02:05.000000 pyatlan-0.0.25/pyatlan/model/typedef.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-05-02 14:02:05.000000 pyatlan-0.0.25/pyatlan/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-02 14:02:05.000000 pyatlan-0.0.25/pyatlan/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:02:19.974967 pyatlan-0.0.25/pyatlan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-02 14:02:19.000000 pyatlan-0.0.25/pyatlan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-02 14:02:19.000000 pyatlan-0.0.25/pyatlan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 14:02:19.000000 pyatlan-0.0.25/pyatlan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 14:02:19.000000 pyatlan-0.0.25/pyatlan.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-02 14:02:19.000000 pyatlan-0.0.25/pyatlan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-02 14:02:19.000000 pyatlan-0.0.25/pyatlan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 14:02:19.986967 pyatlan-0.0.25/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-02 14:02:05.000000 pyatlan-0.0.25/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:02:19.982967 pyatlan-0.0.25/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-02 14:02:05.000000 pyatlan-0.0.25/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:02:19.982967 pyatlan-0.0.25/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-02 14:02:05.000000 pyatlan-0.0.25/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-02 14:02:05.000000 pyatlan-0.0.25/tests/integration/classification_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-05-02 14:02:05.000000 pyatlan-0.0.25/tests/integration/custom_metadata_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-02 14:02:05.000000 pyatlan-0.0.25/tests/integration/role_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-02 14:02:05.000000 pyatlan-0.0.25/tests/integration/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32057 2023-05-02 14:02:05.000000 pyatlan-0.0.25/tests/integration/test_entity_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-05-02 14:02:05.000000 pyatlan-0.0.25/tests/integration/test_index_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:02:19.986967 pyatlan-0.0.25/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-02 14:02:05.000000 pyatlan-0.0.25/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-05-02 14:02:05.000000 pyatlan-0.0.25/tests/unit/test_classification_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-05-02 14:02:05.000000 pyatlan-0.0.25/tests/unit/test_glossary_term.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51299 2023-05-02 14:02:05.000000 pyatlan-0.0.25/tests/unit/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31771 2023-05-02 14:02:05.000000 pyatlan-0.0.25/tests/unit/test_search_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8483 2023-05-02 14:02:05.000000 pyatlan-0.0.25/tests/unit/test_typedef_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-02 14:02:05.000000 pyatlan-0.0.25/tests/unit/test_utils.py
```

### Comparing `pyatlan-0.0.24/LICENSE` & `pyatlan-0.0.25/LICENSE`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.24/PKG-INFO` & `pyatlan-0.0.25/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatlan
-Version: 0.0.24
+Version: 0.0.25
 Summary: Atlan Python Client
 Home-page: https://github.com/atlanhq/atlan-python
 Author: Atlan Technologies Pvt Ltd
 Author-email: engineering@atlan.com
 License: Apache LICENSE 2.0
 Keywords: atlan client
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyatlan-0.0.24/README.md` & `pyatlan-0.0.25/README.md`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.24/pyatlan/cache/classification_cache.py` & `pyatlan-0.0.25/pyatlan/cache/classification_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.24/pyatlan/cache/custom_metadata_cache.py` & `pyatlan-0.0.25/pyatlan/cache/custom_metadata_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.24/pyatlan/cache/role_cache.py` & `pyatlan-0.0.25/pyatlan/cache/role_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.24/pyatlan/client/atlan.py` & `pyatlan-0.0.25/pyatlan/client/atlan.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.24/pyatlan/client/constants.py` & `pyatlan-0.0.25/pyatlan/client/constants.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.24/pyatlan/error.py` & `pyatlan-0.0.25/pyatlan/error.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.24/pyatlan/exceptions.py` & `pyatlan-0.0.25/pyatlan/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.24/pyatlan/generator/generate_from_typdefs.py` & `pyatlan-0.0.25/pyatlan/generator/generate_from_typdefs.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.24/pyatlan/model/assets.py` & `pyatlan-0.0.25/pyatlan/model/assets.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # Copyright 2022 Atlan Pte. Ltd.
 # Based on original code from https://github.com/apache/atlas (under Apache-2.0 license)
 from __future__ import annotations
 
 import sys
 from datetime import datetime
 from typing import Any, ClassVar, Dict, List, Optional, TypeVar
+from urllib.parse import quote, unquote
 
 from pydantic import Field, StrictStr, root_validator, validator
 
 from pyatlan.model.core import (
     Announcement,
     AtlanObject,
     Classification,
@@ -2063,14 +2064,34 @@
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "DataSet":
             raise ValueError("must be DataSet")
         return v
 
+    class Attributes(Asset.Attributes):
+        links: Optional[list[Link]] = Field(
+            None, description="", alias="links"
+        )  # relationship
+        metrics: Optional[list[Metric]] = Field(
+            None, description="", alias="metrics"
+        )  # relationship
+        readme: Optional[Readme] = Field(
+            None, description="", alias="readme"
+        )  # relationship
+        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="meanings"
+        )  # relationship
+
+    attributes: "DataSet.Attributes" = Field(
+        None,
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
 
 class ProcessExecution(Asset, type_name="ProcessExecution"):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in ProcessExecution._convience_properties:
             return object.__setattr__(self, name, value)
@@ -2082,14 +2103,34 @@
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "ProcessExecution":
             raise ValueError("must be ProcessExecution")
         return v
 
+    class Attributes(Asset.Attributes):
+        links: Optional[list[Link]] = Field(
+            None, description="", alias="links"
+        )  # relationship
+        metrics: Optional[list[Metric]] = Field(
+            None, description="", alias="metrics"
+        )  # relationship
+        readme: Optional[Readme] = Field(
+            None, description="", alias="readme"
+        )  # relationship
+        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="meanings"
+        )  # relationship
+
+    attributes: "ProcessExecution.Attributes" = Field(
+        None,
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
 
 class AtlasGlossaryTerm(Asset, type_name="AtlasGlossaryTerm"):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in AtlasGlossaryTerm._convience_properties:
             return object.__setattr__(self, name, value)
@@ -2347,14 +2388,34 @@
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Cloud":
             raise ValueError("must be Cloud")
         return v
 
+    class Attributes(Asset.Attributes):
+        links: Optional[list[Link]] = Field(
+            None, description="", alias="links"
+        )  # relationship
+        metrics: Optional[list[Metric]] = Field(
+            None, description="", alias="metrics"
+        )  # relationship
+        readme: Optional[Readme] = Field(
+            None, description="", alias="readme"
+        )  # relationship
+        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="meanings"
+        )  # relationship
+
+    attributes: "Cloud.Attributes" = Field(
+        None,
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
 
 class Infrastructure(Asset, type_name="Infrastructure"):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in Infrastructure._convience_properties:
             return object.__setattr__(self, name, value)
@@ -2366,14 +2427,34 @@
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Infrastructure":
             raise ValueError("must be Infrastructure")
         return v
 
+    class Attributes(Asset.Attributes):
+        links: Optional[list[Link]] = Field(
+            None, description="", alias="links"
+        )  # relationship
+        metrics: Optional[list[Metric]] = Field(
+            None, description="", alias="metrics"
+        )  # relationship
+        readme: Optional[Readme] = Field(
+            None, description="", alias="readme"
+        )  # relationship
+        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="meanings"
+        )  # relationship
+
+    attributes: "Infrastructure.Attributes" = Field(
+        None,
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
 
 class Connection(Asset, type_name="Connection"):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in Connection._convience_properties:
             return object.__setattr__(self, name, value)
@@ -3092,14 +3173,40 @@
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Namespace":
             raise ValueError("must be Namespace")
         return v
 
+    class Attributes(Asset.Attributes):
+        children_queries: Optional[list[Query]] = Field(
+            None, description="", alias="childrenQueries"
+        )  # relationship
+        links: Optional[list[Link]] = Field(
+            None, description="", alias="links"
+        )  # relationship
+        children_folders: Optional[list[Folder]] = Field(
+            None, description="", alias="childrenFolders"
+        )  # relationship
+        metrics: Optional[list[Metric]] = Field(
+            None, description="", alias="metrics"
+        )  # relationship
+        readme: Optional[Readme] = Field(
+            None, description="", alias="readme"
+        )  # relationship
+        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="meanings"
+        )  # relationship
+
+    attributes: "Namespace.Attributes" = Field(
+        None,
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
 
 class Catalog(Asset, type_name="Catalog"):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in Catalog._convience_properties:
             return object.__setattr__(self, name, value)
@@ -3111,14 +3218,40 @@
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Catalog":
             raise ValueError("must be Catalog")
         return v
 
+    class Attributes(Asset.Attributes):
+        input_to_processes: Optional[list[Process]] = Field(
+            None, description="", alias="inputToProcesses"
+        )  # relationship
+        links: Optional[list[Link]] = Field(
+            None, description="", alias="links"
+        )  # relationship
+        metrics: Optional[list[Metric]] = Field(
+            None, description="", alias="metrics"
+        )  # relationship
+        readme: Optional[Readme] = Field(
+            None, description="", alias="readme"
+        )  # relationship
+        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="meanings"
+        )  # relationship
+        output_from_processes: Optional[list[Process]] = Field(
+            None, description="", alias="outputFromProcesses"
+        )  # relationship
+
+    attributes: "Catalog.Attributes" = Field(
+        None,
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
 
 class Google(Cloud):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in Google._convience_properties:
             return object.__setattr__(self, name, value)
@@ -3536,14 +3669,43 @@
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "BIProcess":
             raise ValueError("must be BIProcess")
         return v
 
+    class Attributes(Process.Attributes):
+        outputs: Optional[list[Catalog]] = Field(
+            None, description="", alias="outputs"
+        )  # relationship
+        inputs: Optional[list[Catalog]] = Field(
+            None, description="", alias="inputs"
+        )  # relationship
+        links: Optional[list[Link]] = Field(
+            None, description="", alias="links"
+        )  # relationship
+        metrics: Optional[list[Metric]] = Field(
+            None, description="", alias="metrics"
+        )  # relationship
+        readme: Optional[Readme] = Field(
+            None, description="", alias="readme"
+        )  # relationship
+        column_processes: Optional[list[ColumnProcess]] = Field(
+            None, description="", alias="columnProcesses"
+        )  # relationship
+        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="meanings"
+        )  # relationship
+
+    attributes: "BIProcess.Attributes" = Field(
+        None,
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
 
 class ColumnProcess(Process):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in ColumnProcess._convience_properties:
             return object.__setattr__(self, name, value)
@@ -3555,14 +3717,46 @@
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "ColumnProcess":
             raise ValueError("must be ColumnProcess")
         return v
 
+    class Attributes(Process.Attributes):
+        outputs: Optional[list[Catalog]] = Field(
+            None, description="", alias="outputs"
+        )  # relationship
+        process: Optional[Process] = Field(
+            None, description="", alias="process"
+        )  # relationship
+        inputs: Optional[list[Catalog]] = Field(
+            None, description="", alias="inputs"
+        )  # relationship
+        links: Optional[list[Link]] = Field(
+            None, description="", alias="links"
+        )  # relationship
+        metrics: Optional[list[Metric]] = Field(
+            None, description="", alias="metrics"
+        )  # relationship
+        readme: Optional[Readme] = Field(
+            None, description="", alias="readme"
+        )  # relationship
+        column_processes: Optional[list[ColumnProcess]] = Field(
+            None, description="", alias="columnProcesses"
+        )  # relationship
+        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="meanings"
+        )  # relationship
+
+    attributes: "ColumnProcess.Attributes" = Field(
+        None,
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
 
 class Collection(Namespace):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in Collection._convience_properties:
             return object.__setattr__(self, name, value)
@@ -3719,14 +3913,40 @@
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "EventStore":
             raise ValueError("must be EventStore")
         return v
 
+    class Attributes(Catalog.Attributes):
+        input_to_processes: Optional[list[Process]] = Field(
+            None, description="", alias="inputToProcesses"
+        )  # relationship
+        links: Optional[list[Link]] = Field(
+            None, description="", alias="links"
+        )  # relationship
+        metrics: Optional[list[Metric]] = Field(
+            None, description="", alias="metrics"
+        )  # relationship
+        readme: Optional[Readme] = Field(
+            None, description="", alias="readme"
+        )  # relationship
+        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="meanings"
+        )  # relationship
+        output_from_processes: Optional[list[Process]] = Field(
+            None, description="", alias="outputFromProcesses"
+        )  # relationship
+
+    attributes: "EventStore.Attributes" = Field(
+        None,
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
 
 class ObjectStore(Catalog):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in ObjectStore._convience_properties:
             return object.__setattr__(self, name, value)
@@ -3738,14 +3958,40 @@
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "ObjectStore":
             raise ValueError("must be ObjectStore")
         return v
 
+    class Attributes(Catalog.Attributes):
+        input_to_processes: Optional[list[Process]] = Field(
+            None, description="", alias="inputToProcesses"
+        )  # relationship
+        links: Optional[list[Link]] = Field(
+            None, description="", alias="links"
+        )  # relationship
+        metrics: Optional[list[Metric]] = Field(
+            None, description="", alias="metrics"
+        )  # relationship
+        readme: Optional[Readme] = Field(
+            None, description="", alias="readme"
+        )  # relationship
+        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="meanings"
+        )  # relationship
+        output_from_processes: Optional[list[Process]] = Field(
+            None, description="", alias="outputFromProcesses"
+        )  # relationship
+
+    attributes: "ObjectStore.Attributes" = Field(
+        None,
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
 
 class DataQuality(Catalog):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in DataQuality._convience_properties:
             return object.__setattr__(self, name, value)
@@ -3757,14 +4003,40 @@
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "DataQuality":
             raise ValueError("must be DataQuality")
         return v
 
+    class Attributes(Catalog.Attributes):
+        input_to_processes: Optional[list[Process]] = Field(
+            None, description="", alias="inputToProcesses"
+        )  # relationship
+        links: Optional[list[Link]] = Field(
+            None, description="", alias="links"
+        )  # relationship
+        metrics: Optional[list[Metric]] = Field(
+            None, description="", alias="metrics"
+        )  # relationship
+        readme: Optional[Readme] = Field(
+            None, description="", alias="readme"
+        )  # relationship
+        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="meanings"
+        )  # relationship
+        output_from_processes: Optional[list[Process]] = Field(
+            None, description="", alias="outputFromProcesses"
+        )  # relationship
+
+    attributes: "DataQuality.Attributes" = Field(
+        None,
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
 
 class BI(Catalog):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in BI._convience_properties:
             return object.__setattr__(self, name, value)
@@ -3776,14 +4048,40 @@
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "BI":
             raise ValueError("must be BI")
         return v
 
+    class Attributes(Catalog.Attributes):
+        input_to_processes: Optional[list[Process]] = Field(
+            None, description="", alias="inputToProcesses"
+        )  # relationship
+        links: Optional[list[Link]] = Field(
+            None, description="", alias="links"
+        )  # relationship
+        metrics: Optional[list[Metric]] = Field(
+            None, description="", alias="metrics"
+        )  # relationship
+        readme: Optional[Readme] = Field(
+            None, description="", alias="readme"
+        )  # relationship
+        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="meanings"
+        )  # relationship
+        output_from_processes: Optional[list[Process]] = Field(
+            None, description="", alias="outputFromProcesses"
+        )  # relationship
+
+    attributes: "BI.Attributes" = Field(
+        None,
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
 
 class SaaS(Catalog):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in SaaS._convience_properties:
             return object.__setattr__(self, name, value)
@@ -3795,14 +4093,40 @@
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "SaaS":
             raise ValueError("must be SaaS")
         return v
 
+    class Attributes(Catalog.Attributes):
+        input_to_processes: Optional[list[Process]] = Field(
+            None, description="", alias="inputToProcesses"
+        )  # relationship
+        links: Optional[list[Link]] = Field(
+            None, description="", alias="links"
+        )  # relationship
+        metrics: Optional[list[Metric]] = Field(
+            None, description="", alias="metrics"
+        )  # relationship
+        readme: Optional[Readme] = Field(
+            None, description="", alias="readme"
+        )  # relationship
+        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="meanings"
+        )  # relationship
+        output_from_processes: Optional[list[Process]] = Field(
+            None, description="", alias="outputFromProcesses"
+        )  # relationship
+
+    attributes: "SaaS.Attributes" = Field(
+        None,
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
 
 class Dbt(Catalog):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in Dbt._convience_properties:
             return object.__setattr__(self, name, value)
@@ -4202,14 +4526,40 @@
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Insight":
             raise ValueError("must be Insight")
         return v
 
+    class Attributes(Catalog.Attributes):
+        input_to_processes: Optional[list[Process]] = Field(
+            None, description="", alias="inputToProcesses"
+        )  # relationship
+        links: Optional[list[Link]] = Field(
+            None, description="", alias="links"
+        )  # relationship
+        metrics: Optional[list[Metric]] = Field(
+            None, description="", alias="metrics"
+        )  # relationship
+        readme: Optional[Readme] = Field(
+            None, description="", alias="readme"
+        )  # relationship
+        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="meanings"
+        )  # relationship
+        output_from_processes: Optional[list[Process]] = Field(
+            None, description="", alias="outputFromProcesses"
+        )  # relationship
+
+    attributes: "Insight.Attributes" = Field(
+        None,
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
 
 class API(Catalog):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in API._convience_properties:
             return object.__setattr__(self, name, value)
@@ -5883,14 +6233,40 @@
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Kafka":
             raise ValueError("must be Kafka")
         return v
 
+    class Attributes(EventStore.Attributes):
+        input_to_processes: Optional[list[Process]] = Field(
+            None, description="", alias="inputToProcesses"
+        )  # relationship
+        links: Optional[list[Link]] = Field(
+            None, description="", alias="links"
+        )  # relationship
+        metrics: Optional[list[Metric]] = Field(
+            None, description="", alias="metrics"
+        )  # relationship
+        readme: Optional[Readme] = Field(
+            None, description="", alias="readme"
+        )  # relationship
+        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="meanings"
+        )  # relationship
+        output_from_processes: Optional[list[Process]] = Field(
+            None, description="", alias="outputFromProcesses"
+        )  # relationship
+
+    attributes: "Kafka.Attributes" = Field(
+        None,
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
 
 class Metric(DataQuality):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in Metric._convience_properties:
             return object.__setattr__(self, name, value)
@@ -6919,14 +7295,40 @@
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Tableau":
             raise ValueError("must be Tableau")
         return v
 
+    class Attributes(BI.Attributes):
+        input_to_processes: Optional[list[Process]] = Field(
+            None, description="", alias="inputToProcesses"
+        )  # relationship
+        links: Optional[list[Link]] = Field(
+            None, description="", alias="links"
+        )  # relationship
+        metrics: Optional[list[Metric]] = Field(
+            None, description="", alias="metrics"
+        )  # relationship
+        readme: Optional[Readme] = Field(
+            None, description="", alias="readme"
+        )  # relationship
+        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="meanings"
+        )  # relationship
+        output_from_processes: Optional[list[Process]] = Field(
+            None, description="", alias="outputFromProcesses"
+        )  # relationship
+
+    attributes: "Tableau.Attributes" = Field(
+        None,
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
 
 class Looker(BI):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in Looker._convience_properties:
             return object.__setattr__(self, name, value)
@@ -6938,14 +7340,40 @@
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Looker":
             raise ValueError("must be Looker")
         return v
 
+    class Attributes(BI.Attributes):
+        input_to_processes: Optional[list[Process]] = Field(
+            None, description="", alias="inputToProcesses"
+        )  # relationship
+        links: Optional[list[Link]] = Field(
+            None, description="", alias="links"
+        )  # relationship
+        metrics: Optional[list[Metric]] = Field(
+            None, description="", alias="metrics"
+        )  # relationship
+        readme: Optional[Readme] = Field(
+            None, description="", alias="readme"
+        )  # relationship
+        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="meanings"
+        )  # relationship
+        output_from_processes: Optional[list[Process]] = Field(
+            None, description="", alias="outputFromProcesses"
+        )  # relationship
+
+    attributes: "Looker.Attributes" = Field(
+        None,
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
 
 class Salesforce(SaaS):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in Salesforce._convience_properties:
             return object.__setattr__(self, name, value)
@@ -8260,22 +8688,95 @@
     def validate_type_name(cls, v):
         if v != "Readme":
             raise ValueError("must be Readme")
         return v
 
     @classmethod
     # @validate_arguments()
-    def create(cls, asset: Asset) -> Readme:
+    def create(
+        cls, *, asset: Asset, content: str, asset_name: Optional[str] = None
+    ) -> Readme:
         return Readme(
-            attributes=Readme.Attributes(
-                qualified_name=f"{asset.guid}/readme",
-                name=f"{asset.attributes.name} Readme",
-            ),
+            attributes=Readme.Attributes.create(
+                asset=asset, content=content, asset_name=asset_name
+            )
+        )
+
+    @property
+    def description(self) -> Optional[str]:
+        ret_value = self.attributes.description
+        return unquote(ret_value) if ret_value is not None else ret_value
+
+    @description.setter
+    def description(self, description: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.description = (
+            quote(description) if description is not None else description
         )
 
+    class Attributes(Resource.Attributes):
+        input_to_processes: Optional[list[Process]] = Field(
+            None, description="", alias="inputToProcesses"
+        )  # relationship
+        internal: Optional[Internal] = Field(
+            None, description="", alias="__internal"
+        )  # relationship
+        links: Optional[list[Link]] = Field(
+            None, description="", alias="links"
+        )  # relationship
+        metrics: Optional[list[Metric]] = Field(
+            None, description="", alias="metrics"
+        )  # relationship
+        readme: Optional[Readme] = Field(
+            None, description="", alias="readme"
+        )  # relationship
+        asset: Optional[Asset] = Field(
+            None, description="", alias="asset"
+        )  # relationship
+        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="meanings"
+        )  # relationship
+        see_also: Optional[list[Readme]] = Field(
+            None, description="", alias="seeAlso"
+        )  # relationship
+        output_from_processes: Optional[list[Process]] = Field(
+            None, description="", alias="outputFromProcesses"
+        )  # relationship
+
+        @classmethod
+        # @validate_arguments()
+        def create(
+            cls, *, asset: Asset, content: str, asset_name: Optional[str] = None
+        ) -> Readme.Attributes:
+            validate_required_fields(["asset", "content"], [asset, content])
+            if not asset.name:
+                if not asset_name:
+                    raise ValueError(
+                        "asset_name is required when name is not available from asset"
+                    )
+            elif asset_name:
+                raise ValueError(
+                    "asset_name can not be given when name is available from asset"
+                )
+            else:
+                asset_name = asset.name
+            return Readme.Attributes(
+                qualified_name=f"{asset.guid}/readme",
+                name=f"{asset_name} Readme",
+                asset=asset,
+                description=quote(content),
+            )
+
+    attributes: "Readme.Attributes" = Field(
+        None,
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
 
 class Link(Resource):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in Link._convience_properties:
             return object.__setattr__(self, name, value)
@@ -13782,14 +14283,43 @@
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "ThoughtspotLiveboard":
             raise ValueError("must be ThoughtspotLiveboard")
         return v
 
+    class Attributes(Thoughtspot.Attributes):
+        input_to_processes: Optional[list[Process]] = Field(
+            None, description="", alias="inputToProcesses"
+        )  # relationship
+        thoughtspot_dashlets: Optional[list[ThoughtspotDashlet]] = Field(
+            None, description="", alias="thoughtspotDashlets"
+        )  # relationship
+        links: Optional[list[Link]] = Field(
+            None, description="", alias="links"
+        )  # relationship
+        metrics: Optional[list[Metric]] = Field(
+            None, description="", alias="metrics"
+        )  # relationship
+        readme: Optional[Readme] = Field(
+            None, description="", alias="readme"
+        )  # relationship
+        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="meanings"
+        )  # relationship
+        output_from_processes: Optional[list[Process]] = Field(
+            None, description="", alias="outputFromProcesses"
+        )  # relationship
+
+    attributes: "ThoughtspotLiveboard.Attributes" = Field(
+        None,
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
 
 class ThoughtspotDashlet(Thoughtspot):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in ThoughtspotDashlet._convience_properties:
             return object.__setattr__(self, name, value)
@@ -13882,14 +14412,40 @@
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "ThoughtspotAnswer":
             raise ValueError("must be ThoughtspotAnswer")
         return v
 
+    class Attributes(Thoughtspot.Attributes):
+        input_to_processes: Optional[list[Process]] = Field(
+            None, description="", alias="inputToProcesses"
+        )  # relationship
+        links: Optional[list[Link]] = Field(
+            None, description="", alias="links"
+        )  # relationship
+        metrics: Optional[list[Metric]] = Field(
+            None, description="", alias="metrics"
+        )  # relationship
+        readme: Optional[Readme] = Field(
+            None, description="", alias="readme"
+        )  # relationship
+        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="meanings"
+        )  # relationship
+        output_from_processes: Optional[list[Process]] = Field(
+            None, description="", alias="outputFromProcesses"
+        )  # relationship
+
+    attributes: "ThoughtspotAnswer.Attributes" = Field(
+        None,
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
 
 class PowerBIReport(PowerBI):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in PowerBIReport._convience_properties:
             return object.__setattr__(self, name, value)
@@ -17726,14 +18282,43 @@
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "TableauSite":
             raise ValueError("must be TableauSite")
         return v
 
+    class Attributes(Tableau.Attributes):
+        input_to_processes: Optional[list[Process]] = Field(
+            None, description="", alias="inputToProcesses"
+        )  # relationship
+        projects: Optional[list[TableauProject]] = Field(
+            None, description="", alias="projects"
+        )  # relationship
+        links: Optional[list[Link]] = Field(
+            None, description="", alias="links"
+        )  # relationship
+        metrics: Optional[list[Metric]] = Field(
+            None, description="", alias="metrics"
+        )  # relationship
+        readme: Optional[Readme] = Field(
+            None, description="", alias="readme"
+        )  # relationship
+        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="meanings"
+        )  # relationship
+        output_from_processes: Optional[list[Process]] = Field(
+            None, description="", alias="outputFromProcesses"
+        )  # relationship
+
+    attributes: "TableauSite.Attributes" = Field(
+        None,
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
 
 class TableauDatasource(Tableau):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in TableauDatasource._convience_properties:
             return object.__setattr__(self, name, value)
@@ -19170,14 +19755,52 @@
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "LookerProject":
             raise ValueError("must be LookerProject")
         return v
 
+    class Attributes(Looker.Attributes):
+        input_to_processes: Optional[list[Process]] = Field(
+            None, description="", alias="inputToProcesses"
+        )  # relationship
+        models: Optional[list[LookerModel]] = Field(
+            None, description="", alias="models"
+        )  # relationship
+        explores: Optional[list[LookerExplore]] = Field(
+            None, description="", alias="explores"
+        )  # relationship
+        links: Optional[list[Link]] = Field(
+            None, description="", alias="links"
+        )  # relationship
+        metrics: Optional[list[Metric]] = Field(
+            None, description="", alias="metrics"
+        )  # relationship
+        readme: Optional[Readme] = Field(
+            None, description="", alias="readme"
+        )  # relationship
+        fields: Optional[list[LookerField]] = Field(
+            None, description="", alias="fields"
+        )  # relationship
+        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="meanings"
+        )  # relationship
+        views: Optional[list[LookerView]] = Field(
+            None, description="", alias="views"
+        )  # relationship
+        output_from_processes: Optional[list[Process]] = Field(
+            None, description="", alias="outputFromProcesses"
+        )  # relationship
+
+    attributes: "LookerProject.Attributes" = Field(
+        None,
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
 
 class LookerQuery(Looker):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in LookerQuery._convience_properties:
             return object.__setattr__(self, name, value)
@@ -20128,14 +20751,46 @@
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "QlikStream":
             raise ValueError("must be QlikStream")
         return v
 
+    class Attributes(QlikSpace.Attributes):
+        input_to_processes: Optional[list[Process]] = Field(
+            None, description="", alias="inputToProcesses"
+        )  # relationship
+        qlik_datasets: Optional[list[QlikDataset]] = Field(
+            None, description="", alias="qlikDatasets"
+        )  # relationship
+        links: Optional[list[Link]] = Field(
+            None, description="", alias="links"
+        )  # relationship
+        qlik_apps: Optional[list[QlikApp]] = Field(
+            None, description="", alias="qlikApps"
+        )  # relationship
+        metrics: Optional[list[Metric]] = Field(
+            None, description="", alias="metrics"
+        )  # relationship
+        readme: Optional[Readme] = Field(
+            None, description="", alias="readme"
+        )  # relationship
+        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="meanings"
+        )  # relationship
+        output_from_processes: Optional[list[Process]] = Field(
+            None, description="", alias="outputFromProcesses"
+        )  # relationship
+
+    attributes: "QlikStream.Attributes" = Field(
+        None,
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
 
 Referenceable.update_forward_refs()
 AtlasGlossary.update_forward_refs()
 
 Referenceable.Attributes.update_forward_refs()
 
 Asset.Attributes.update_forward_refs()
```

### Comparing `pyatlan-0.0.24/pyatlan/model/core.py` & `pyatlan-0.0.25/pyatlan/model/core.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.24/pyatlan/model/enums.py` & `pyatlan-0.0.25/pyatlan/model/enums.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.24/pyatlan/model/response.py` & `pyatlan-0.0.25/pyatlan/model/response.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.24/pyatlan/model/role.py` & `pyatlan-0.0.25/pyatlan/model/role.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.24/pyatlan/model/search.py` & `pyatlan-0.0.25/pyatlan/model/search.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.24/pyatlan/model/structs.py` & `pyatlan-0.0.25/pyatlan/model/structs.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.24/pyatlan/model/typedef.py` & `pyatlan-0.0.25/pyatlan/model/typedef.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.24/pyatlan/utils.py` & `pyatlan-0.0.25/pyatlan/utils.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.24/pyatlan.egg-info/PKG-INFO` & `pyatlan-0.0.25/pyatlan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatlan
-Version: 0.0.24
+Version: 0.0.25
 Summary: Atlan Python Client
 Home-page: https://github.com/atlanhq/atlan-python
 Author: Atlan Technologies Pvt Ltd
 Author-email: engineering@atlan.com
 License: Apache LICENSE 2.0
 Keywords: atlan client
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyatlan-0.0.24/pyatlan.egg-info/SOURCES.txt` & `pyatlan-0.0.25/pyatlan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.24/setup.py` & `pyatlan-0.0.25/setup.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.24/tests/integration/classification_test.py` & `pyatlan-0.0.25/tests/integration/classification_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.24/tests/integration/custom_metadata_test.py` & `pyatlan-0.0.25/tests/integration/custom_metadata_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.24/tests/integration/role_test.py` & `pyatlan-0.0.25/tests/integration/role_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.24/tests/integration/test_entity_model.py` & `pyatlan-0.0.25/tests/integration/test_entity_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     Asset,
     AtlasGlossary,
     AtlasGlossaryCategory,
     AtlasGlossaryTerm,
     Column,
     Connection,
     Database,
+    Readme,
     Schema,
     Table,
     View,
 )
 from pyatlan.model.core import Announcement
 from pyatlan.model.enums import AnnouncementType, AtlanConnectorType, CertificateStatus
 
@@ -184,14 +185,15 @@
         "AtlasGlossary",
         "Table",
         "Schema",
         "Database",
         "Connection",
         "View",
         "Column",
+        "Readme",
     ]
     for type_name in type_names:
         print()
         delete_assets(atlan_host, headers, type_name)
     yield
     for type_name in type_names:
         delete_assets(atlan_host, headers, type_name)
@@ -744,15 +746,15 @@
     assert len(glossary_term.classifications) == 1
     classification = glossary_term.classifications[0]
     assert str(classification.type_name) == classification_name
     client.remove_classification(AtlasGlossaryTerm, qualified_name, classification_name)
     glossary_term = client.get_asset_by_guid(
         glossary_term.guid, asset_type=AtlasGlossaryTerm
     )
-    assert glossary_term.classifications is None
+    assert not glossary_term.classifications
 
 
 def test_create_for_modification(client: AtlanClient):
     qualified_name = (
         "default/snowflake/1669038939/GREENE_HOMES_DEMO/STAGE/CONTRACT_STATUS"
     )
     classification_name = "TEST"
@@ -807,7 +809,19 @@
     asset = client.remove_announcement(
         asset_type=AtlasGlossary,
         qualified_name=glossary.qualified_name,
         name=glossary.name,
     )
     assert asset is not None
     assert asset.get_announcment() is None
+
+
+def test_create_readme(client: AtlanClient):
+    glossary = AtlasGlossary.create(name="Integration Readme Test")
+    glossary.attributes.user_description = "This is a description of the glossary"
+    glossary = client.upsert(glossary).assets_created(AtlasGlossary)[0]
+    readme = Readme.create(asset=glossary, content="<h1>Important</h1>")
+    response = client.upsert(readme)
+    assert (reaadmes := response.assets_created(asset_type=Readme))
+    assert len(reaadmes) == 1
+    assert (glossaries := response.assets_updated(asset_type=AtlasGlossary))
+    assert len(glossaries) == 1
```

### Comparing `pyatlan-0.0.24/tests/integration/test_index_search.py` & `pyatlan-0.0.25/tests/integration/test_index_search.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.24/tests/unit/test_classification_name.py` & `pyatlan-0.0.25/tests/unit/test_classification_name.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.24/tests/unit/test_glossary_term.py` & `pyatlan-0.0.25/tests/unit/test_glossary_term.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.24/tests/unit/test_model.py` & `pyatlan-0.0.25/tests/unit/test_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     Connection,
     Database,
     DbtMetricFilter,
     GoogleLabel,
     GoogleTag,
     Histogram,
     PopularityInsights,
+    Readme,
     S3Bucket,
     S3Object,
     Schema,
     Table,
     View,
     validate_single_required_field,
 )
@@ -63,14 +64,18 @@
     QuickSightFolderType,
     SourceCostUnitType,
 )
 from pyatlan.model.response import AssetMutationResponse
 from pyatlan.model.structs import KafkaTopicConsumption
 from pyatlan.model.typedef import TypeDefResponse
 
+SCHEMA_QUALIFIED_NAME = "default/snowflake/1646836521/ATLAN_SAMPLE_DATA/FOOD_BEVERAGE"
+
+TABLE_NAME = "MKT_EXPENSES"
+
 TABLE_URL = "POsWut55wIYsXZ5v4z3K98"
 
 FRESHNESS = "VdRC4dyNdTJHfFjCiNaKt9"
 
 MONTE_CARLO = "AFq4ctARP76ctapiTbuT92"
 
 MOON = "FAq4ctARP76ctapiTbuT92"
@@ -163,16 +168,16 @@
         announcement_type=AnnouncementType.ISSUE,
     )
 
 
 @pytest.fixture()
 def table():
     return Table.create(
-        name="MKT_EXPENSES",
-        schema_qualified_name="default/snowflake/1646836521/ATLAN_SAMPLE_DATA/FOOD_BEVERAGE",
+        name=TABLE_NAME,
+        schema_qualified_name=SCHEMA_QUALIFIED_NAME,
     )
 
 
 @pytest.fixture()
 def type_def_response():
     data = {
         "enumDefs": [],
@@ -1348,7 +1353,102 @@
 ):
     with pytest.raises(ValueError, match=message):
         validate_single_required_field(names, values)
 
 
 def test_validate_single_required_field_with_only_one_field_does_not_raise_value_error():
     validate_single_required_field(["One", "Two", "Three"], [None, None, 3])
+
+
+@pytest.mark.parametrize(
+    "asset, content, asset_name, error, message",
+    [
+        (None, "stuff", None, ValueError, "asset is required"),
+        (table, None, None, ValueError, "content is required"),
+        (
+            Table(),
+            "stuff",
+            None,
+            AttributeError,
+            "'NoneType' object has no attribute 'name'",
+        ),
+        (
+            Table(attributes=Table.Attributes()),
+            "stuff",
+            None,
+            ValueError,
+            "asset_name is required when name is not available from asset",
+        ),
+    ],
+)
+def test_create_readme_attributes_without_required_parameters_raises_exception(
+    asset, content, asset_name, error, message
+):
+
+    with pytest.raises(error, match=message):
+        Readme.Attributes.create(asset=asset, content=content, asset_name=asset_name)
+
+
+@pytest.mark.parametrize(
+    "asset, content, asset_name, error, message",
+    [
+        (None, "stuff", None, ValueError, "asset is required"),
+        (
+            Table.create(
+                name=TABLE_NAME,
+                schema_qualified_name=SCHEMA_QUALIFIED_NAME,
+            ),
+            None,
+            None,
+            ValueError,
+            "content is required",
+        ),
+        (
+            Table(),
+            "stuff",
+            None,
+            AttributeError,
+            "'NoneType' object has no attribute 'name'",
+        ),
+        (
+            Table(attributes=Table.Attributes()),
+            "stuff",
+            None,
+            ValueError,
+            "asset_name is required when name is not available from asset",
+        ),
+    ],
+)
+def test_create_readme_without_required_parameters_raises_exception(
+    asset, content, asset_name, error, message
+):
+
+    with pytest.raises(error, match=message):
+        Readme.create(asset=asset, content=content, asset_name=asset_name)
+
+
+@pytest.mark.parametrize(
+    "asset, content, asset_name, expected_name",
+    [
+        (
+            Table.create(
+                name=TABLE_NAME,
+                schema_qualified_name=SCHEMA_QUALIFIED_NAME,
+            ),
+            "<h1>stuff</h1>",
+            None,
+            TABLE_NAME,
+        ),
+        (
+            Table(attributes=Table.Attributes()),
+            "<h1>stuff</h1>",
+            TABLE_NAME,
+            TABLE_NAME,
+        ),
+    ],
+)
+def test_create_readme(asset, content, asset_name, expected_name):
+    readme = Readme.create(asset=asset, content=content, asset_name=asset_name)
+    assert readme.qualified_name == f"{asset.guid}/readme"
+    assert readme.name == f"{expected_name} Readme"
+    assert readme.attributes.asset == asset
+    assert readme.description == content
```

### Comparing `pyatlan-0.0.24/tests/unit/test_search_model.py` & `pyatlan-0.0.25/tests/unit/test_search_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.24/tests/unit/test_typedef_model.py` & `pyatlan-0.0.25/tests/unit/test_typedef_model.py`

 * *Files identical despite different names*

