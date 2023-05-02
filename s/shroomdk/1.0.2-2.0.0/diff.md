# Comparing `tmp/shroomdk-1.0.2.tar.gz` & `tmp/shroomdk-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shroomdk-1.0.2.tar", last modified: Mon Oct 31 18:44:47 2022, max compression
+gzip compressed data, was "shroomdk-2.0.0.tar", last modified: Tue May  2 18:11:50 2023, max compression
```

## Comparing `shroomdk-1.0.2.tar` & `shroomdk-2.0.0.tar`

### file list

```diff
@@ -1,64 +1,144 @@
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2022-10-31 18:44:47.129064 shroomdk-1.0.2/
--rw-r--r--   0 jim        (501) staff       (20)     1073 2022-07-25 21:42:15.000000 shroomdk-1.0.2/LICENSE.txt
--rw-r--r--   0 jim        (501) staff       (20)       69 2022-07-25 21:42:15.000000 shroomdk-1.0.2/MANIFEST.in
--rw-r--r--   0 jim        (501) staff       (20)    11123 2022-10-31 18:44:47.129161 shroomdk-1.0.2/PKG-INFO
--rw-r--r--   0 jim        (501) staff       (20)    10322 2022-07-25 22:56:45.000000 shroomdk-1.0.2/README.md
--rw-r--r--   0 jim        (501) staff       (20)        5 2022-10-31 18:41:14.000000 shroomdk-1.0.2/VERSION
--rw-r--r--   0 jim        (501) staff       (20)       30 2022-07-25 21:42:15.000000 shroomdk-1.0.2/requirements-dev.txt
--rw-r--r--   0 jim        (501) staff       (20)       50 2022-07-27 13:44:04.000000 shroomdk-1.0.2/requirements.txt
--rw-r--r--   0 jim        (501) staff       (20)       79 2022-10-31 18:44:47.129485 shroomdk-1.0.2/setup.cfg
--rw-r--r--   0 jim        (501) staff       (20)     1418 2022-07-25 21:48:33.000000 shroomdk-1.0.2/setup.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2022-10-31 18:44:47.124793 shroomdk-1.0.2/shroomdk/
--rw-r--r--   0 jim        (501) staff       (20)       80 2022-07-25 21:42:15.000000 shroomdk-1.0.2/shroomdk/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     3212 2022-07-25 21:42:15.000000 shroomdk-1.0.2/shroomdk/api.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2022-10-31 18:44:47.126095 shroomdk-1.0.2/shroomdk/errors/
--rw-r--r--   0 jim        (501) staff       (20)      276 2022-07-25 21:42:15.000000 shroomdk-1.0.2/shroomdk/errors/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      121 2022-07-25 21:42:15.000000 shroomdk-1.0.2/shroomdk/errors/base_error.py
--rw-r--r--   0 jim        (501) staff       (20)      950 2022-07-25 21:42:15.000000 shroomdk-1.0.2/shroomdk/errors/query_run_errors.py
--rw-r--r--   0 jim        (501) staff       (20)      262 2022-07-25 21:42:15.000000 shroomdk-1.0.2/shroomdk/errors/sdk_error.py
--rw-r--r--   0 jim        (501) staff       (20)      361 2022-07-25 21:42:15.000000 shroomdk-1.0.2/shroomdk/errors/server_error.py
--rw-r--r--   0 jim        (501) staff       (20)      344 2022-07-25 21:42:15.000000 shroomdk-1.0.2/shroomdk/errors/user_error.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2022-10-31 18:44:47.126198 shroomdk-1.0.2/shroomdk/integrations/
--rw-r--r--   0 jim        (501) staff       (20)       62 2022-07-25 21:42:15.000000 shroomdk-1.0.2/shroomdk/integrations/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2022-10-31 18:44:47.126547 shroomdk-1.0.2/shroomdk/integrations/query_integration/
--rw-r--r--   0 jim        (501) staff       (20)       77 2022-07-25 21:42:15.000000 shroomdk-1.0.2/shroomdk/integrations/query_integration/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     4418 2022-07-25 21:42:15.000000 shroomdk-1.0.2/shroomdk/integrations/query_integration/query_integration.py
--rw-r--r--   0 jim        (501) staff       (20)     2005 2022-07-25 21:42:15.000000 shroomdk-1.0.2/shroomdk/integrations/query_integration/query_result_set_builder.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2022-10-31 18:44:47.127313 shroomdk-1.0.2/shroomdk/models/
--rw-r--r--   0 jim        (501) staff       (20)      315 2022-07-25 21:42:15.000000 shroomdk-1.0.2/shroomdk/models/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2022-10-31 18:44:47.127759 shroomdk-1.0.2/shroomdk/models/api/
--rw-r--r--   0 jim        (501) staff       (20)      208 2022-07-25 21:42:15.000000 shroomdk-1.0.2/shroomdk/models/api/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      207 2022-07-25 21:42:15.000000 shroomdk-1.0.2/shroomdk/models/api/api_response.py
--rw-r--r--   0 jim        (501) staff       (20)      527 2022-07-25 21:42:15.000000 shroomdk-1.0.2/shroomdk/models/api/create_query_resp.py
--rw-r--r--   0 jim        (501) staff       (20)      548 2022-07-25 21:42:15.000000 shroomdk-1.0.2/shroomdk/models/api/query_result_resp.py
--rw-r--r--   0 jim        (501) staff       (20)     1079 2022-10-31 18:41:14.000000 shroomdk-1.0.2/shroomdk/models/query.py
--rw-r--r--   0 jim        (501) staff       (20)      641 2022-07-25 21:42:15.000000 shroomdk-1.0.2/shroomdk/models/query_defaults.py
--rw-r--r--   0 jim        (501) staff       (20)     1030 2022-07-28 15:19:00.000000 shroomdk-1.0.2/shroomdk/models/query_result_set.py
--rw-r--r--   0 jim        (501) staff       (20)      509 2022-07-25 21:42:15.000000 shroomdk-1.0.2/shroomdk/models/query_run_stats.py
--rw-r--r--   0 jim        (501) staff       (20)      232 2022-07-25 21:42:15.000000 shroomdk-1.0.2/shroomdk/models/query_status.py
--rw-r--r--   0 jim        (501) staff       (20)      194 2022-07-25 21:42:15.000000 shroomdk-1.0.2/shroomdk/models/sleep_config.py
--rw-r--r--   0 jim        (501) staff       (20)     1065 2022-10-31 18:41:14.000000 shroomdk-1.0.2/shroomdk/shroomdk.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2022-10-31 18:44:47.127958 shroomdk-1.0.2/shroomdk/tests/
--rw-r--r--   0 jim        (501) staff       (20)        0 2022-07-25 21:42:15.000000 shroomdk-1.0.2/shroomdk/tests/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2022-10-31 18:44:47.128086 shroomdk-1.0.2/shroomdk/tests/integrations/
--rw-r--r--   0 jim        (501) staff       (20)        0 2022-07-25 21:42:15.000000 shroomdk-1.0.2/shroomdk/tests/integrations/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2022-10-31 18:44:47.128378 shroomdk-1.0.2/shroomdk/tests/integrations/query_integration/
--rw-r--r--   0 jim        (501) staff       (20)        0 2022-07-25 21:42:15.000000 shroomdk-1.0.2/shroomdk/tests/integrations/query_integration/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     7233 2022-10-31 18:41:14.000000 shroomdk-1.0.2/shroomdk/tests/integrations/query_integration/test_query_integration.py
--rw-r--r--   0 jim        (501) staff       (20)     2949 2022-07-25 21:42:15.000000 shroomdk-1.0.2/shroomdk/tests/integrations/query_integration/test_query_result_set_builder.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2022-10-31 18:44:47.128587 shroomdk-1.0.2/shroomdk/tests/models/
--rw-r--r--   0 jim        (501) staff       (20)        0 2022-07-25 21:42:15.000000 shroomdk-1.0.2/shroomdk/tests/models/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      418 2022-07-25 21:42:15.000000 shroomdk-1.0.2/shroomdk/tests/models/test_query_status.py
--rw-r--r--   0 jim        (501) staff       (20)     4213 2022-07-25 21:42:15.000000 shroomdk-1.0.2/shroomdk/tests/test_api.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2022-10-31 18:44:47.128772 shroomdk-1.0.2/shroomdk/tests/utils/
--rw-r--r--   0 jim        (501) staff       (20)        0 2022-07-25 21:42:15.000000 shroomdk-1.0.2/shroomdk/tests/utils/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     2254 2022-07-25 21:42:15.000000 shroomdk-1.0.2/shroomdk/tests/utils/test_sleep.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2022-10-31 18:44:47.128955 shroomdk-1.0.2/shroomdk/utils/
--rw-r--r--   0 jim        (501) staff       (20)        0 2022-07-25 21:42:15.000000 shroomdk-1.0.2/shroomdk/utils/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     1967 2022-07-25 21:42:15.000000 shroomdk-1.0.2/shroomdk/utils/sleep.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2022-10-31 18:44:47.125421 shroomdk-1.0.2/shroomdk.egg-info/
--rw-r--r--   0 jim        (501) staff       (20)    11123 2022-10-31 18:44:47.000000 shroomdk-1.0.2/shroomdk.egg-info/PKG-INFO
--rw-r--r--   0 jim        (501) staff       (20)     1586 2022-10-31 18:44:47.000000 shroomdk-1.0.2/shroomdk.egg-info/SOURCES.txt
--rw-r--r--   0 jim        (501) staff       (20)        1 2022-10-31 18:44:47.000000 shroomdk-1.0.2/shroomdk.egg-info/dependency_links.txt
--rw-r--r--   0 jim        (501) staff       (20)       50 2022-10-31 18:44:47.000000 shroomdk-1.0.2/shroomdk.egg-info/requires.txt
--rw-r--r--   0 jim        (501) staff       (20)        9 2022-10-31 18:44:47.000000 shroomdk-1.0.2/shroomdk.egg-info/top_level.txt
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.142986 shroomdk-2.0.0/
+-rw-r--r--   0 jim        (501) staff       (20)     1073 2022-07-25 21:42:15.000000 shroomdk-2.0.0/LICENSE.txt
+-rw-r--r--   0 jim        (501) staff       (20)       69 2022-07-25 21:42:15.000000 shroomdk-2.0.0/MANIFEST.in
+-rw-r--r--   0 jim        (501) staff       (20)     1436 2023-05-02 18:11:50.143086 shroomdk-2.0.0/PKG-INFO
+-rw-r--r--   0 jim        (501) staff       (20)      635 2023-05-02 18:10:35.000000 shroomdk-2.0.0/README.md
+-rw-r--r--   0 jim        (501) staff       (20)        5 2023-05-02 18:10:35.000000 shroomdk-2.0.0/VERSION
+-rw-r--r--   0 jim        (501) staff       (20)       30 2022-07-25 21:42:15.000000 shroomdk-2.0.0/requirements-dev.txt
+-rw-r--r--   0 jim        (501) staff       (20)       33 2023-05-02 18:10:35.000000 shroomdk-2.0.0/requirements.txt
+-rw-r--r--   0 jim        (501) staff       (20)       79 2023-05-02 18:11:50.143613 shroomdk-2.0.0/setup.cfg
+-rw-r--r--   0 jim        (501) staff       (20)     1557 2023-05-02 18:10:35.000000 shroomdk-2.0.0/setup.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.127922 shroomdk-2.0.0/shroomdk/
+-rw-r--r--   0 jim        (501) staff       (20)      147 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.129475 shroomdk-2.0.0/shroomdk/errors/
+-rw-r--r--   0 jim        (501) staff       (20)      336 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/errors/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     1583 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/errors/api_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      121 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/errors/base_error.py
+-rw-r--r--   0 jim        (501) staff       (20)     2077 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/errors/query_run_errors.py
+-rw-r--r--   0 jim        (501) staff       (20)      262 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/errors/sdk_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      361 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/errors/server_error.py
+-rw-r--r--   0 jim        (501) staff       (20)     2766 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/flipside.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.129595 shroomdk-2.0.0/shroomdk/integrations/
+-rw-r--r--   0 jim        (501) staff       (20)       69 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/integrations/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.130340 shroomdk-2.0.0/shroomdk/integrations/query_integration/
+-rw-r--r--   0 jim        (501) staff       (20)       77 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/integrations/query_integration/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     9884 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/integrations/query_integration/compass_query_integration.py
+-rw-r--r--   0 jim        (501) staff       (20)      237 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/integrations/query_integration/defaults.py
+-rw-r--r--   0 jim        (501) staff       (20)     3570 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/integrations/query_integration/query_result_set_builder.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.131169 shroomdk-2.0.0/shroomdk/models/
+-rw-r--r--   0 jim        (501) staff       (20)      365 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/models/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.131981 shroomdk-2.0.0/shroomdk/models/compass/
+-rw-r--r--   0 jim        (501) staff       (20)       50 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/models/compass/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      571 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/models/compass/cancel_query_run.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.133335 shroomdk-2.0.0/shroomdk/models/compass/core/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/models/compass/core/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      187 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/models/compass/core/column_metadata.py
+-rw-r--r--   0 jim        (501) staff       (20)      117 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/models/compass/core/page.py
+-rw-r--r--   0 jim        (501) staff       (20)      183 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/models/compass/core/page_stats.py
+-rw-r--r--   0 jim        (501) staff       (20)      358 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/models/compass/core/query_request.py
+-rw-r--r--   0 jim        (501) staff       (20)      807 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/models/compass/core/query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)       89 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/models/compass/core/result_format.py
+-rw-r--r--   0 jim        (501) staff       (20)      149 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/models/compass/core/rpc_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      198 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/models/compass/core/rpc_request.py
+-rw-r--r--   0 jim        (501) staff       (20)      252 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/models/compass/core/rpc_response.py
+-rw-r--r--   0 jim        (501) staff       (20)      340 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/models/compass/core/sql_statement.py
+-rw-r--r--   0 jim        (501) staff       (20)      221 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/models/compass/core/tags.py
+-rw-r--r--   0 jim        (501) staff       (20)      845 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/models/compass/create_query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)      639 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/models/compass/get_query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)     2026 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/models/compass/get_query_run_results.py
+-rw-r--r--   0 jim        (501) staff       (20)      582 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/models/compass/get_sql_statement.py
+-rw-r--r--   0 jim        (501) staff       (20)      852 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/models/compass/query_results.py
+-rw-r--r--   0 jim        (501) staff       (20)     1422 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/models/query.py
+-rw-r--r--   0 jim        (501) staff       (20)      836 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/models/query_defaults.py
+-rw-r--r--   0 jim        (501) staff       (20)     1031 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/models/query_result_set.py
+-rw-r--r--   0 jim        (501) staff       (20)     1658 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/models/query_run_stats.py
+-rw-r--r--   0 jim        (501) staff       (20)      544 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/models/query_status.py
+-rw-r--r--   0 jim        (501) staff       (20)      194 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/models/sleep_config.py
+-rw-r--r--   0 jim        (501) staff       (20)     5708 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/rpc.py
+-rw-r--r--   0 jim        (501) staff       (20)       68 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/shroomdk.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.133592 shroomdk-2.0.0/shroomdk/tests/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/tests/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.133906 shroomdk-2.0.0/shroomdk/tests/integrations/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/tests/integrations/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.134391 shroomdk-2.0.0/shroomdk/tests/integrations/query_integration/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/tests/integrations/query_integration/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     8712 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/tests/integrations/query_integration/test_query_compass_integration.py
+-rw-r--r--   0 jim        (501) staff       (20)     3438 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/tests/integrations/query_integration/test_query_result_set_builder.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.134868 shroomdk-2.0.0/shroomdk/tests/models/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/tests/models/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      931 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/tests/models/test_query_status.py
+-rw-r--r--   0 jim        (501) staff       (20)     5218 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/tests/test_rpc.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.135163 shroomdk-2.0.0/shroomdk/tests/utils/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/tests/utils/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     2242 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/tests/utils/test_sleep.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.135437 shroomdk-2.0.0/shroomdk/utils/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/utils/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     1966 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/utils/sleep.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.128507 shroomdk-2.0.0/shroomdk.egg-info/
+-rw-r--r--   0 jim        (501) staff       (20)     1436 2023-05-02 18:11:50.000000 shroomdk-2.0.0/shroomdk.egg-info/PKG-INFO
+-rw-r--r--   0 jim        (501) staff       (20)     4101 2023-05-02 18:11:50.000000 shroomdk-2.0.0/shroomdk.egg-info/SOURCES.txt
+-rw-r--r--   0 jim        (501) staff       (20)        1 2023-05-02 18:11:50.000000 shroomdk-2.0.0/shroomdk.egg-info/dependency_links.txt
+-rw-r--r--   0 jim        (501) staff       (20)       34 2023-05-02 18:11:50.000000 shroomdk-2.0.0/shroomdk.egg-info/requires.txt
+-rw-r--r--   0 jim        (501) staff       (20)       13 2023-05-02 18:11:50.000000 shroomdk-2.0.0/shroomdk.egg-info/top_level.txt
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.125538 shroomdk-2.0.0/src/
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.136359 shroomdk-2.0.0/src/errors/
+-rw-r--r--   0 jim        (501) staff       (20)      336 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/errors/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     1583 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/errors/api_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      121 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/errors/base_error.py
+-rw-r--r--   0 jim        (501) staff       (20)     2077 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/errors/query_run_errors.py
+-rw-r--r--   0 jim        (501) staff       (20)      262 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/errors/sdk_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      361 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/errors/server_error.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.136502 shroomdk-2.0.0/src/integrations/
+-rw-r--r--   0 jim        (501) staff       (20)       69 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/integrations/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.137086 shroomdk-2.0.0/src/integrations/query_integration/
+-rw-r--r--   0 jim        (501) staff       (20)       77 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/integrations/query_integration/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     9884 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/integrations/query_integration/compass_query_integration.py
+-rw-r--r--   0 jim        (501) staff       (20)      237 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/integrations/query_integration/defaults.py
+-rw-r--r--   0 jim        (501) staff       (20)     3570 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/integrations/query_integration/query_result_set_builder.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.138332 shroomdk-2.0.0/src/models/
+-rw-r--r--   0 jim        (501) staff       (20)      365 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/models/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.139429 shroomdk-2.0.0/src/models/compass/
+-rw-r--r--   0 jim        (501) staff       (20)       50 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/models/compass/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      571 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/models/compass/cancel_query_run.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.140852 shroomdk-2.0.0/src/models/compass/core/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/models/compass/core/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      187 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/models/compass/core/column_metadata.py
+-rw-r--r--   0 jim        (501) staff       (20)      117 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/models/compass/core/page.py
+-rw-r--r--   0 jim        (501) staff       (20)      183 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/models/compass/core/page_stats.py
+-rw-r--r--   0 jim        (501) staff       (20)      358 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/models/compass/core/query_request.py
+-rw-r--r--   0 jim        (501) staff       (20)      807 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/models/compass/core/query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)       89 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/models/compass/core/result_format.py
+-rw-r--r--   0 jim        (501) staff       (20)      149 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/models/compass/core/rpc_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      198 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/models/compass/core/rpc_request.py
+-rw-r--r--   0 jim        (501) staff       (20)      252 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/models/compass/core/rpc_response.py
+-rw-r--r--   0 jim        (501) staff       (20)      340 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/models/compass/core/sql_statement.py
+-rw-r--r--   0 jim        (501) staff       (20)      221 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/models/compass/core/tags.py
+-rw-r--r--   0 jim        (501) staff       (20)      845 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/models/compass/create_query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)      639 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/models/compass/get_query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)     2026 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/models/compass/get_query_run_results.py
+-rw-r--r--   0 jim        (501) staff       (20)      582 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/models/compass/get_sql_statement.py
+-rw-r--r--   0 jim        (501) staff       (20)      852 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/models/compass/query_results.py
+-rw-r--r--   0 jim        (501) staff       (20)     1422 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/models/query.py
+-rw-r--r--   0 jim        (501) staff       (20)      836 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/models/query_defaults.py
+-rw-r--r--   0 jim        (501) staff       (20)     1031 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/models/query_result_set.py
+-rw-r--r--   0 jim        (501) staff       (20)     1658 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/models/query_run_stats.py
+-rw-r--r--   0 jim        (501) staff       (20)      544 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/models/query_status.py
+-rw-r--r--   0 jim        (501) staff       (20)      194 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/models/sleep_config.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.141086 shroomdk-2.0.0/src/tests/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/tests/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.141224 shroomdk-2.0.0/src/tests/integrations/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/tests/integrations/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.141553 shroomdk-2.0.0/src/tests/integrations/query_integration/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/tests/integrations/query_integration/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     8712 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/tests/integrations/query_integration/test_query_compass_integration.py
+-rw-r--r--   0 jim        (501) staff       (20)     3438 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/tests/integrations/query_integration/test_query_result_set_builder.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.141960 shroomdk-2.0.0/src/tests/models/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/tests/models/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      931 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/tests/models/test_query_status.py
+-rw-r--r--   0 jim        (501) staff       (20)     5218 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/tests/test_rpc.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.142324 shroomdk-2.0.0/src/tests/utils/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/tests/utils/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     2242 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/tests/utils/test_sleep.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.142690 shroomdk-2.0.0/src/utils/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/utils/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     1966 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/utils/sleep.py
```

### Comparing `shroomdk-1.0.2/LICENSE.txt` & `shroomdk-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shroomdk-1.0.2/setup.py` & `shroomdk-2.0.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,25 +8,28 @@
     version = f.read().strip()
 
 
 with open("requirements.txt", "r") as fh:
     requirements = fh.readlines()
 
 
+with open("package_name.txt", "r") as fh:
+    package_name = fh.read().strip().lower()
+
 setup(
     install_requires=[req for req in requirements if req[:2] != "# "],
-    name="shroomdk",
+    name=package_name,
     version=version,
     author="dev@flipsidecrypto.com",
     author_email="dev@flipsidecrypto.com",
-    description="ShroomDK (SDK) by Flipside Crypto: Query the most comprehensive blockchain data in crypto",
+    description="SDK by Flipside Crypto: Query the most reliable & comprehensive blockchain data in crypto",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/FlipsideCrypto/sdk/python",
-    packages=find_packages(),
+    packages=find_packages(exclude=["src"]),  # Add the exclude parameter here
     include_package_data=True,
     classifiers=[
         "Development Status :: 5 - Production/Stable",  # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
         "Intended Audience :: Developers",  # Define that your audience are developers
         "License :: OSI Approved :: MIT License",  # Again, pick a license
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3.7",
```

### Comparing `shroomdk-1.0.2/shroomdk/models/api/query_result_resp.py` & `shroomdk-2.0.0/shroomdk/models/compass/core/query_run.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,33 @@
-from typing import Any, List, Optional, Union
+from datetime import datetime
+from typing import Any, Dict, List, Optional
 
 from pydantic import BaseModel
 
-from .api_response import ApiResponse
+from .tags import Tags
 
 
-class QueryResultJson(BaseModel):
-    queryId: Optional[str]
-    status: str
-    results: Optional[List[Any]]
+class QueryRun(BaseModel):
+    id: str
+    sqlStatementId: str
+    state: str
+    path: str
+    fileCount: Optional[int]
+    lastFileNumber: Optional[int]
+    fileNames: Optional[str]
+    errorName: Optional[str]
+    errorMessage: Optional[str]
+    errorData: Optional[Any]
+    dataSourceQueryId: Optional[str]
+    dataSourceSessionId: Optional[str]
     startedAt: Optional[str]
+    queryRunningEndedAt: Optional[str]
+    queryStreamingEndedAt: Optional[str]
     endedAt: Optional[str]
-    columnLabels: Optional[List[str]]
-    columnTypes: Optional[List[str]]
-    message: Optional[str]
-    errors: Optional[str]
-    pageNumber: Optional[int]
-    pageSize: Optional[int]
-
-
-class QueryResultResp(ApiResponse):
-    data: Union[QueryResultJson, None]
+    rowCount: Optional[int]
+    totalSize: Optional[int]
+    tags: Tags
+    dataSourceId: str
+    userId: str
+    createdAt: str
+    updatedAt: datetime
+    archivedAt: Optional[datetime]
```

### Comparing `shroomdk-1.0.2/shroomdk/models/query.py` & `shroomdk-2.0.0/shroomdk/models/query.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 
 
 class Query(BaseModel):
     sql: str = Field(None, description="SQL query to execute")
     ttl_minutes: Optional[int] = Field(
         None, description="The number of minutes to cache the query results"
     )
+    max_age_minutes: Optional[int] = Field(
+        5, description="The max age of the query results in minutes"
+    )
     timeout_minutes: Optional[int] = Field(
         None, description="The number of minutes to timeout the query"
     )
     retry_interval_seconds: Optional[Union[int, float]] = Field(
         1, description="The number of seconds to use between retries"
     )
     cached: Optional[bool] = Field(
@@ -22,7 +25,13 @@
     page_number: int = Field(None, description="The page number to return")
     sdk_package: Optional[str] = Field(
         None, description="The SDK package used for the query"
     )
     sdk_version: Optional[str] = Field(
         None, description="The SDK version used for the query"
     )
+    data_source: Optional[str] = Field(
+        None, description="The data source to execute the query against"
+    )
+    data_provider: Optional[str] = Field(
+        None, description="The owner of the data source"
+    )
```

### Comparing `shroomdk-1.0.2/shroomdk/models/query_defaults.py` & `shroomdk-2.0.0/shroomdk/models/query_defaults.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 from pydantic import BaseModel, Field
 
 
 class QueryDefaults(BaseModel):
-    ttl_minutes: int = Field(None, description="The number of minutes to cache the query results")
+    ttl_minutes: int = Field(
+        None, description="The number of minutes to cache the query results"
+    )
+    max_age_minutes: int = Field(
+        None,
+        description="The max age of query results to accept before deciding to run a query again",
+    )
     cached: bool = Field(False, description="Whether or not to cache the query results")
-    timeout_minutes: int = Field(None, description="The number of minutes to timeout the query")
-    retry_interval_seconds: float = Field(None, description="The number of seconds to wait before retrying the query")
+    timeout_minutes: int = Field(
+        None, description="The number of minutes to timeout the query"
+    )
+    retry_interval_seconds: float = Field(
+        None, description="The number of seconds to wait before retrying the query"
+    )
     page_size: int = Field(None, description="The number of results to return per page")
     page_number: int = Field(None, description="The page number to return")
```

### Comparing `shroomdk-1.0.2/shroomdk/models/query_result_set.py` & `shroomdk-2.0.0/shroomdk/models/query_result_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from pydantic import BaseModel, Field
 
 from .query_run_stats import QueryRunStats
 
 
 class QueryResultSet(BaseModel):
     query_id: Union[str, None] = Field(None, description="The server id of the query")
+
     status: str = Field(
         False, description="The status of the query (`PENDING`, `FINISHED`, `ERROR`)"
     )
     columns: Union[List[str], None] = Field(
         None, description="The names of the columns in the result set"
     )
     column_types: Union[List[str], None] = Field(
```

### Comparing `shroomdk-1.0.2/shroomdk/tests/integrations/query_integration/test_query_result_set_builder.py` & `shroomdk-2.0.0/shroomdk/tests/integrations/query_integration/test_query_result_set_builder.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,59 +1,52 @@
 from datetime import datetime
 
-from shroomdk.integrations.query_integration.query_result_set_builder import (
+from ....integrations.query_integration.query_result_set_builder import (
     QueryResultSetBuilder,
 )
-from shroomdk.models.api import QueryResultJson
-from shroomdk.models.query_status import QueryStatus
+from ....models.compass.get_query_run import GetQueryRunRpcResponse
+from ....models.compass.get_query_run_results import GetQueryRunResultsRpcResponse
+from ....models.query_status import QueryStatus
+from ...utils.mock_data.get_query_results import get_query_results_response
+from ...utils.mock_data.get_query_run import get_query_run_response
 
 
-def getQueryResultSetData(status: str) -> QueryResultJson:
-    return QueryResultJson(
-        queryId="test",
-        status=status,
-        results=[
-            [1, "0x-tx-id-0", "0xfrom-address-0", True, 0.5],
-            [2, "0x-tx-id-1", "0xfrom-address-1", False, 0.75],
-            [3, "0x-tx-id-2", "0xfrom-address-2", False, 1.75],
-            [4, "0x-tx-id-3", "0xfrom-address-3", True, 100.001],
-        ],
-        startedAt="2022-05-19T00:00:00.00Z",
-        endedAt="2022-05-19T00:01:30.00Z",
-        columnLabels=[
-            "block_id",
-            "tx_id",
-            "from_address",
-            "succeeded",
-            "amount",
-        ],
-        columnTypes=["number", "string", "string", "boolean", "number"],
-        message="",
-        errors=None,
-        pageSize=100,
-        pageNumber=0,
+def getQueryResultSetData(status: str) -> dict:
+    query_run_resp = GetQueryRunRpcResponse(**get_query_run_response(status=status))
+    query_result_resp = GetQueryRunResultsRpcResponse(
+        **get_query_results_response(status=status)
     )
+    return {
+        "query_run": query_run_resp.result.queryRun if query_run_resp.result else None,
+        "query_result": query_result_resp.result if query_result_resp.result else None,
+    }
 
 
 def test_run_stats():
-    qr = QueryResultSetBuilder(getQueryResultSetData(QueryStatus.Finished))
+    qr = QueryResultSetBuilder(**getQueryResultSetData(QueryStatus.Success))
 
     # Start/end are datetime objects?
     assert type(qr.run_stats.started_at) == datetime
     assert type(qr.run_stats.ended_at) == datetime
 
     # Elapsed seconds
-    assert qr.run_stats.elapsed_seconds == 90
+    assert qr.run_stats.elapsed_seconds == 51
+
+    # Streaming seconds
+    assert qr.run_stats.streaming_seconds == 45
+
+    # Exec Seconds
+    assert qr.run_stats.query_exec_seconds == 5
 
     # Record count
-    assert qr.run_stats.record_count == 4
+    assert qr.run_stats.record_count == 10000
 
 
 def test_records():
-    qr = QueryResultSetBuilder(getQueryResultSetData(QueryStatus.Finished))
+    qr = QueryResultSetBuilder(**getQueryResultSetData(QueryStatus.Success))
 
     # Records Length Matches Row Length?
     assert qr.records is not None
     assert qr.rows is not None
     assert qr.columns is not None
     assert len(qr.records) == len(qr.rows)
 
@@ -71,28 +64,40 @@
     # Record values match row values?
     for record, row in zip(qr.records, qr.rows):
         for column, value in zip(qr.columns, row):
             assert record[column] == value
 
 
 def test_status():
+    # Status is ready?
+    qr = QueryResultSetBuilder(**getQueryResultSetData(QueryStatus.Ready))
+    assert qr.status == QueryStatus.Ready
+
+    # Status is running?
+    qr = QueryResultSetBuilder(**getQueryResultSetData(QueryStatus.Running))
+    assert qr.status == QueryStatus.Running
+
+    # Status is streaming?
+    qr = QueryResultSetBuilder(**getQueryResultSetData(QueryStatus.StreamingResults))
+    assert qr.status == QueryStatus.StreamingResults
+
+    # Status is cancelled?
+    qr = QueryResultSetBuilder(**getQueryResultSetData(QueryStatus.Canceled))
+    assert qr.status == QueryStatus.Canceled
+
     # Status is finished?
-    qr = QueryResultSetBuilder(getQueryResultSetData(QueryStatus.Finished))
-    assert qr.status == QueryStatus.Finished
+    qr = QueryResultSetBuilder(**getQueryResultSetData(QueryStatus.Success))
+    assert qr.status == QueryStatus.Success
 
-    # Status is pending?
-    qr = QueryResultSetBuilder(getQueryResultSetData(QueryStatus.Pending))
-    assert qr.status == QueryStatus.Pending
-
-    # Status is error?
-    qr = QueryResultSetBuilder(getQueryResultSetData(QueryStatus.Error))
-    assert qr.status == QueryStatus.Error
+    # Status is failed?
+    qr = QueryResultSetBuilder(**getQueryResultSetData(QueryStatus.Failed))
+    assert qr.status == QueryStatus.Failed
 
 
 def test_query_id():
     # Query ID is set?
-    qr = QueryResultSetBuilder(getQueryResultSetData(QueryStatus.Finished))
+    qr = QueryResultSetBuilder(**getQueryResultSetData(QueryStatus.Success))
     assert qr.query_id is not None
 
     # Query ID is test
-    qr = QueryResultSetBuilder(getQueryResultSetData(QueryStatus.Finished))
-    assert qr.query_id == "test"
+    qr = QueryResultSetBuilder(**getQueryResultSetData(QueryStatus.Success))
+    assert qr.query_id == "clg44olzq00cbn60tasvob5l2"
```

### Comparing `shroomdk-1.0.2/shroomdk/tests/utils/test_sleep.py` & `shroomdk-2.0.0/shroomdk/tests/utils/test_sleep.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from shroomdk.models.sleep_config import SleepConfig
-from shroomdk.utils.sleep import (
+from ...models.sleep_config import SleepConfig
+from ...utils.sleep import (
     exp_backoff,
     get_elapsed_exp_seconds,
     get_elapsed_linear_seconds,
     get_exp_backoff_seconds,
     get_linear_backoff_seconds,
     linear_backoff,
     sec_to_ms,
```

### Comparing `shroomdk-1.0.2/shroomdk/utils/sleep.py` & `shroomdk-2.0.0/shroomdk/utils/sleep.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import time
 from typing import Union
 
-from shroomdk.models.sleep_config import SleepConfig
+from ..models.sleep_config import SleepConfig
 
 
 def sec_to_ms(sec: int):
     return sec * 1000
 
 
 def get_exp_backoff_seconds(attempts: Union[int, float]):
     return 2**attempts
 
 
-def get_linear_backoff_seconds(attempts: Union[int, float], interval_seconds: Union[int, float]):
+def get_linear_backoff_seconds(
+    attempts: Union[int, float], interval_seconds: Union[int, float]
+):
     return (attempts + 1) * interval_seconds
 
 
 def get_elapsed_exp_seconds(config: SleepConfig):
     if not config.interval_seconds:
         raise Exception("intervalSeconds is required for `get_elapsed_exp_seconds`")
```

