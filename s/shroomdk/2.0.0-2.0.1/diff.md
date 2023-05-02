# Comparing `tmp/shroomdk-2.0.0.tar.gz` & `tmp/shroomdk-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shroomdk-2.0.0.tar", last modified: Tue May  2 18:11:50 2023, max compression
+gzip compressed data, was "shroomdk-2.0.1.tar", last modified: Tue May  2 18:20:09 2023, max compression
```

## Comparing `shroomdk-2.0.0.tar` & `shroomdk-2.0.1.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.142986 shroomdk-2.0.0/
--rw-r--r--   0 jim        (501) staff       (20)     1073 2022-07-25 21:42:15.000000 shroomdk-2.0.0/LICENSE.txt
--rw-r--r--   0 jim        (501) staff       (20)       69 2022-07-25 21:42:15.000000 shroomdk-2.0.0/MANIFEST.in
--rw-r--r--   0 jim        (501) staff       (20)     1436 2023-05-02 18:11:50.143086 shroomdk-2.0.0/PKG-INFO
--rw-r--r--   0 jim        (501) staff       (20)      635 2023-05-02 18:10:35.000000 shroomdk-2.0.0/README.md
--rw-r--r--   0 jim        (501) staff       (20)        5 2023-05-02 18:10:35.000000 shroomdk-2.0.0/VERSION
--rw-r--r--   0 jim        (501) staff       (20)       30 2022-07-25 21:42:15.000000 shroomdk-2.0.0/requirements-dev.txt
--rw-r--r--   0 jim        (501) staff       (20)       33 2023-05-02 18:10:35.000000 shroomdk-2.0.0/requirements.txt
--rw-r--r--   0 jim        (501) staff       (20)       79 2023-05-02 18:11:50.143613 shroomdk-2.0.0/setup.cfg
--rw-r--r--   0 jim        (501) staff       (20)     1557 2023-05-02 18:10:35.000000 shroomdk-2.0.0/setup.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.127922 shroomdk-2.0.0/shroomdk/
--rw-r--r--   0 jim        (501) staff       (20)      147 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.129475 shroomdk-2.0.0/shroomdk/errors/
--rw-r--r--   0 jim        (501) staff       (20)      336 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/errors/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     1583 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/errors/api_error.py
--rw-r--r--   0 jim        (501) staff       (20)      121 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/errors/base_error.py
--rw-r--r--   0 jim        (501) staff       (20)     2077 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/errors/query_run_errors.py
--rw-r--r--   0 jim        (501) staff       (20)      262 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/errors/sdk_error.py
--rw-r--r--   0 jim        (501) staff       (20)      361 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/errors/server_error.py
--rw-r--r--   0 jim        (501) staff       (20)     2766 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/flipside.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.129595 shroomdk-2.0.0/shroomdk/integrations/
--rw-r--r--   0 jim        (501) staff       (20)       69 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/integrations/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.130340 shroomdk-2.0.0/shroomdk/integrations/query_integration/
--rw-r--r--   0 jim        (501) staff       (20)       77 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/integrations/query_integration/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     9884 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/integrations/query_integration/compass_query_integration.py
--rw-r--r--   0 jim        (501) staff       (20)      237 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/integrations/query_integration/defaults.py
--rw-r--r--   0 jim        (501) staff       (20)     3570 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/integrations/query_integration/query_result_set_builder.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.131169 shroomdk-2.0.0/shroomdk/models/
--rw-r--r--   0 jim        (501) staff       (20)      365 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/models/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.131981 shroomdk-2.0.0/shroomdk/models/compass/
--rw-r--r--   0 jim        (501) staff       (20)       50 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/models/compass/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      571 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/models/compass/cancel_query_run.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.133335 shroomdk-2.0.0/shroomdk/models/compass/core/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/models/compass/core/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      187 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/models/compass/core/column_metadata.py
--rw-r--r--   0 jim        (501) staff       (20)      117 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/models/compass/core/page.py
--rw-r--r--   0 jim        (501) staff       (20)      183 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/models/compass/core/page_stats.py
--rw-r--r--   0 jim        (501) staff       (20)      358 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/models/compass/core/query_request.py
--rw-r--r--   0 jim        (501) staff       (20)      807 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/models/compass/core/query_run.py
--rw-r--r--   0 jim        (501) staff       (20)       89 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/models/compass/core/result_format.py
--rw-r--r--   0 jim        (501) staff       (20)      149 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/models/compass/core/rpc_error.py
--rw-r--r--   0 jim        (501) staff       (20)      198 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/models/compass/core/rpc_request.py
--rw-r--r--   0 jim        (501) staff       (20)      252 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/models/compass/core/rpc_response.py
--rw-r--r--   0 jim        (501) staff       (20)      340 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/models/compass/core/sql_statement.py
--rw-r--r--   0 jim        (501) staff       (20)      221 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/models/compass/core/tags.py
--rw-r--r--   0 jim        (501) staff       (20)      845 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/models/compass/create_query_run.py
--rw-r--r--   0 jim        (501) staff       (20)      639 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/models/compass/get_query_run.py
--rw-r--r--   0 jim        (501) staff       (20)     2026 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/models/compass/get_query_run_results.py
--rw-r--r--   0 jim        (501) staff       (20)      582 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/models/compass/get_sql_statement.py
--rw-r--r--   0 jim        (501) staff       (20)      852 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/models/compass/query_results.py
--rw-r--r--   0 jim        (501) staff       (20)     1422 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/models/query.py
--rw-r--r--   0 jim        (501) staff       (20)      836 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/models/query_defaults.py
--rw-r--r--   0 jim        (501) staff       (20)     1031 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/models/query_result_set.py
--rw-r--r--   0 jim        (501) staff       (20)     1658 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/models/query_run_stats.py
--rw-r--r--   0 jim        (501) staff       (20)      544 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/models/query_status.py
--rw-r--r--   0 jim        (501) staff       (20)      194 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/models/sleep_config.py
--rw-r--r--   0 jim        (501) staff       (20)     5708 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/rpc.py
--rw-r--r--   0 jim        (501) staff       (20)       68 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/shroomdk.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.133592 shroomdk-2.0.0/shroomdk/tests/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/tests/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.133906 shroomdk-2.0.0/shroomdk/tests/integrations/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/tests/integrations/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.134391 shroomdk-2.0.0/shroomdk/tests/integrations/query_integration/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/tests/integrations/query_integration/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     8712 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/tests/integrations/query_integration/test_query_compass_integration.py
--rw-r--r--   0 jim        (501) staff       (20)     3438 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/tests/integrations/query_integration/test_query_result_set_builder.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.134868 shroomdk-2.0.0/shroomdk/tests/models/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/tests/models/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      931 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/tests/models/test_query_status.py
--rw-r--r--   0 jim        (501) staff       (20)     5218 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/tests/test_rpc.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.135163 shroomdk-2.0.0/shroomdk/tests/utils/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/tests/utils/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     2242 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/tests/utils/test_sleep.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.135437 shroomdk-2.0.0/shroomdk/utils/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/utils/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     1966 2023-05-02 18:11:49.000000 shroomdk-2.0.0/shroomdk/utils/sleep.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.128507 shroomdk-2.0.0/shroomdk.egg-info/
--rw-r--r--   0 jim        (501) staff       (20)     1436 2023-05-02 18:11:50.000000 shroomdk-2.0.0/shroomdk.egg-info/PKG-INFO
--rw-r--r--   0 jim        (501) staff       (20)     4101 2023-05-02 18:11:50.000000 shroomdk-2.0.0/shroomdk.egg-info/SOURCES.txt
--rw-r--r--   0 jim        (501) staff       (20)        1 2023-05-02 18:11:50.000000 shroomdk-2.0.0/shroomdk.egg-info/dependency_links.txt
--rw-r--r--   0 jim        (501) staff       (20)       34 2023-05-02 18:11:50.000000 shroomdk-2.0.0/shroomdk.egg-info/requires.txt
--rw-r--r--   0 jim        (501) staff       (20)       13 2023-05-02 18:11:50.000000 shroomdk-2.0.0/shroomdk.egg-info/top_level.txt
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.125538 shroomdk-2.0.0/src/
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.136359 shroomdk-2.0.0/src/errors/
--rw-r--r--   0 jim        (501) staff       (20)      336 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/errors/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     1583 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/errors/api_error.py
--rw-r--r--   0 jim        (501) staff       (20)      121 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/errors/base_error.py
--rw-r--r--   0 jim        (501) staff       (20)     2077 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/errors/query_run_errors.py
--rw-r--r--   0 jim        (501) staff       (20)      262 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/errors/sdk_error.py
--rw-r--r--   0 jim        (501) staff       (20)      361 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/errors/server_error.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.136502 shroomdk-2.0.0/src/integrations/
--rw-r--r--   0 jim        (501) staff       (20)       69 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/integrations/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.137086 shroomdk-2.0.0/src/integrations/query_integration/
--rw-r--r--   0 jim        (501) staff       (20)       77 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/integrations/query_integration/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     9884 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/integrations/query_integration/compass_query_integration.py
--rw-r--r--   0 jim        (501) staff       (20)      237 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/integrations/query_integration/defaults.py
--rw-r--r--   0 jim        (501) staff       (20)     3570 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/integrations/query_integration/query_result_set_builder.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.138332 shroomdk-2.0.0/src/models/
--rw-r--r--   0 jim        (501) staff       (20)      365 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/models/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.139429 shroomdk-2.0.0/src/models/compass/
--rw-r--r--   0 jim        (501) staff       (20)       50 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/models/compass/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      571 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/models/compass/cancel_query_run.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.140852 shroomdk-2.0.0/src/models/compass/core/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/models/compass/core/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      187 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/models/compass/core/column_metadata.py
--rw-r--r--   0 jim        (501) staff       (20)      117 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/models/compass/core/page.py
--rw-r--r--   0 jim        (501) staff       (20)      183 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/models/compass/core/page_stats.py
--rw-r--r--   0 jim        (501) staff       (20)      358 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/models/compass/core/query_request.py
--rw-r--r--   0 jim        (501) staff       (20)      807 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/models/compass/core/query_run.py
--rw-r--r--   0 jim        (501) staff       (20)       89 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/models/compass/core/result_format.py
--rw-r--r--   0 jim        (501) staff       (20)      149 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/models/compass/core/rpc_error.py
--rw-r--r--   0 jim        (501) staff       (20)      198 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/models/compass/core/rpc_request.py
--rw-r--r--   0 jim        (501) staff       (20)      252 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/models/compass/core/rpc_response.py
--rw-r--r--   0 jim        (501) staff       (20)      340 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/models/compass/core/sql_statement.py
--rw-r--r--   0 jim        (501) staff       (20)      221 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/models/compass/core/tags.py
--rw-r--r--   0 jim        (501) staff       (20)      845 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/models/compass/create_query_run.py
--rw-r--r--   0 jim        (501) staff       (20)      639 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/models/compass/get_query_run.py
--rw-r--r--   0 jim        (501) staff       (20)     2026 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/models/compass/get_query_run_results.py
--rw-r--r--   0 jim        (501) staff       (20)      582 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/models/compass/get_sql_statement.py
--rw-r--r--   0 jim        (501) staff       (20)      852 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/models/compass/query_results.py
--rw-r--r--   0 jim        (501) staff       (20)     1422 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/models/query.py
--rw-r--r--   0 jim        (501) staff       (20)      836 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/models/query_defaults.py
--rw-r--r--   0 jim        (501) staff       (20)     1031 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/models/query_result_set.py
--rw-r--r--   0 jim        (501) staff       (20)     1658 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/models/query_run_stats.py
--rw-r--r--   0 jim        (501) staff       (20)      544 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/models/query_status.py
--rw-r--r--   0 jim        (501) staff       (20)      194 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/models/sleep_config.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.141086 shroomdk-2.0.0/src/tests/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/tests/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.141224 shroomdk-2.0.0/src/tests/integrations/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/tests/integrations/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.141553 shroomdk-2.0.0/src/tests/integrations/query_integration/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/tests/integrations/query_integration/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     8712 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/tests/integrations/query_integration/test_query_compass_integration.py
--rw-r--r--   0 jim        (501) staff       (20)     3438 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/tests/integrations/query_integration/test_query_result_set_builder.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.141960 shroomdk-2.0.0/src/tests/models/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/tests/models/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      931 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/tests/models/test_query_status.py
--rw-r--r--   0 jim        (501) staff       (20)     5218 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/tests/test_rpc.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.142324 shroomdk-2.0.0/src/tests/utils/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/tests/utils/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     2242 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/tests/utils/test_sleep.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:50.142690 shroomdk-2.0.0/src/utils/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/utils/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     1966 2023-05-02 18:10:35.000000 shroomdk-2.0.0/src/utils/sleep.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:20:09.579887 shroomdk-2.0.1/
+-rw-r--r--   0 jim        (501) staff       (20)     1073 2022-07-25 21:42:15.000000 shroomdk-2.0.1/LICENSE.txt
+-rw-r--r--   0 jim        (501) staff       (20)       69 2022-07-25 21:42:15.000000 shroomdk-2.0.1/MANIFEST.in
+-rw-r--r--   0 jim        (501) staff       (20)     1510 2023-05-02 18:20:09.579975 shroomdk-2.0.1/PKG-INFO
+-rw-r--r--   0 jim        (501) staff       (20)      709 2023-05-02 18:18:58.000000 shroomdk-2.0.1/README.md
+-rw-r--r--   0 jim        (501) staff       (20)        5 2023-05-02 18:19:19.000000 shroomdk-2.0.1/VERSION
+-rw-r--r--   0 jim        (501) staff       (20)       30 2022-07-25 21:42:15.000000 shroomdk-2.0.1/requirements-dev.txt
+-rw-r--r--   0 jim        (501) staff       (20)       33 2023-05-02 18:10:35.000000 shroomdk-2.0.1/requirements.txt
+-rw-r--r--   0 jim        (501) staff       (20)       79 2023-05-02 18:20:09.580357 shroomdk-2.0.1/setup.cfg
+-rw-r--r--   0 jim        (501) staff       (20)     1557 2023-05-02 18:10:35.000000 shroomdk-2.0.1/setup.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:20:09.563139 shroomdk-2.0.1/shroomdk/
+-rw-r--r--   0 jim        (501) staff       (20)      147 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:20:09.564782 shroomdk-2.0.1/shroomdk/errors/
+-rw-r--r--   0 jim        (501) staff       (20)      336 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk/errors/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     1583 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk/errors/api_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      121 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk/errors/base_error.py
+-rw-r--r--   0 jim        (501) staff       (20)     2077 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk/errors/query_run_errors.py
+-rw-r--r--   0 jim        (501) staff       (20)      262 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk/errors/sdk_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      361 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk/errors/server_error.py
+-rw-r--r--   0 jim        (501) staff       (20)     2766 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk/flipside.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:20:09.564955 shroomdk-2.0.1/shroomdk/integrations/
+-rw-r--r--   0 jim        (501) staff       (20)       69 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk/integrations/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:20:09.565559 shroomdk-2.0.1/shroomdk/integrations/query_integration/
+-rw-r--r--   0 jim        (501) staff       (20)       77 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk/integrations/query_integration/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     9884 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk/integrations/query_integration/compass_query_integration.py
+-rw-r--r--   0 jim        (501) staff       (20)      237 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk/integrations/query_integration/defaults.py
+-rw-r--r--   0 jim        (501) staff       (20)     3570 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk/integrations/query_integration/query_result_set_builder.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:20:09.567013 shroomdk-2.0.1/shroomdk/models/
+-rw-r--r--   0 jim        (501) staff       (20)      365 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk/models/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:20:09.568326 shroomdk-2.0.1/shroomdk/models/compass/
+-rw-r--r--   0 jim        (501) staff       (20)       50 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk/models/compass/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      571 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk/models/compass/cancel_query_run.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:20:09.570894 shroomdk-2.0.1/shroomdk/models/compass/core/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk/models/compass/core/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      187 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk/models/compass/core/column_metadata.py
+-rw-r--r--   0 jim        (501) staff       (20)      117 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk/models/compass/core/page.py
+-rw-r--r--   0 jim        (501) staff       (20)      183 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk/models/compass/core/page_stats.py
+-rw-r--r--   0 jim        (501) staff       (20)      358 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk/models/compass/core/query_request.py
+-rw-r--r--   0 jim        (501) staff       (20)      807 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk/models/compass/core/query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)       89 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk/models/compass/core/result_format.py
+-rw-r--r--   0 jim        (501) staff       (20)      149 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk/models/compass/core/rpc_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      198 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk/models/compass/core/rpc_request.py
+-rw-r--r--   0 jim        (501) staff       (20)      252 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk/models/compass/core/rpc_response.py
+-rw-r--r--   0 jim        (501) staff       (20)      340 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk/models/compass/core/sql_statement.py
+-rw-r--r--   0 jim        (501) staff       (20)      221 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk/models/compass/core/tags.py
+-rw-r--r--   0 jim        (501) staff       (20)      845 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk/models/compass/create_query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)      639 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk/models/compass/get_query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)     2026 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk/models/compass/get_query_run_results.py
+-rw-r--r--   0 jim        (501) staff       (20)      582 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk/models/compass/get_sql_statement.py
+-rw-r--r--   0 jim        (501) staff       (20)      852 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk/models/compass/query_results.py
+-rw-r--r--   0 jim        (501) staff       (20)     1422 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk/models/query.py
+-rw-r--r--   0 jim        (501) staff       (20)      836 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk/models/query_defaults.py
+-rw-r--r--   0 jim        (501) staff       (20)     1031 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk/models/query_result_set.py
+-rw-r--r--   0 jim        (501) staff       (20)     1658 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk/models/query_run_stats.py
+-rw-r--r--   0 jim        (501) staff       (20)      544 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk/models/query_status.py
+-rw-r--r--   0 jim        (501) staff       (20)      194 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk/models/sleep_config.py
+-rw-r--r--   0 jim        (501) staff       (20)     5708 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk/rpc.py
+-rw-r--r--   0 jim        (501) staff       (20)       68 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk/shroomdk.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:20:09.571168 shroomdk-2.0.1/shroomdk/tests/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk/tests/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:20:09.571440 shroomdk-2.0.1/shroomdk/tests/integrations/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk/tests/integrations/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:20:09.571862 shroomdk-2.0.1/shroomdk/tests/integrations/query_integration/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk/tests/integrations/query_integration/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     8712 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk/tests/integrations/query_integration/test_query_compass_integration.py
+-rw-r--r--   0 jim        (501) staff       (20)     3438 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk/tests/integrations/query_integration/test_query_result_set_builder.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:20:09.572350 shroomdk-2.0.1/shroomdk/tests/models/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk/tests/models/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      931 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk/tests/models/test_query_status.py
+-rw-r--r--   0 jim        (501) staff       (20)     5218 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk/tests/test_rpc.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:20:09.572659 shroomdk-2.0.1/shroomdk/tests/utils/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk/tests/utils/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     2242 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk/tests/utils/test_sleep.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:20:09.573163 shroomdk-2.0.1/shroomdk/utils/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk/utils/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     1966 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk/utils/sleep.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:20:09.563841 shroomdk-2.0.1/shroomdk.egg-info/
+-rw-r--r--   0 jim        (501) staff       (20)     1510 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk.egg-info/PKG-INFO
+-rw-r--r--   0 jim        (501) staff       (20)     4101 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk.egg-info/SOURCES.txt
+-rw-r--r--   0 jim        (501) staff       (20)        1 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk.egg-info/dependency_links.txt
+-rw-r--r--   0 jim        (501) staff       (20)       34 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk.egg-info/requires.txt
+-rw-r--r--   0 jim        (501) staff       (20)       13 2023-05-02 18:20:09.000000 shroomdk-2.0.1/shroomdk.egg-info/top_level.txt
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:20:09.561337 shroomdk-2.0.1/src/
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:20:09.574065 shroomdk-2.0.1/src/errors/
+-rw-r--r--   0 jim        (501) staff       (20)      336 2023-05-02 18:10:35.000000 shroomdk-2.0.1/src/errors/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     1583 2023-05-02 18:10:35.000000 shroomdk-2.0.1/src/errors/api_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      121 2023-05-02 18:10:35.000000 shroomdk-2.0.1/src/errors/base_error.py
+-rw-r--r--   0 jim        (501) staff       (20)     2077 2023-05-02 18:10:35.000000 shroomdk-2.0.1/src/errors/query_run_errors.py
+-rw-r--r--   0 jim        (501) staff       (20)      262 2023-05-02 18:10:35.000000 shroomdk-2.0.1/src/errors/sdk_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      361 2023-05-02 18:10:35.000000 shroomdk-2.0.1/src/errors/server_error.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:20:09.574196 shroomdk-2.0.1/src/integrations/
+-rw-r--r--   0 jim        (501) staff       (20)       69 2023-05-02 18:10:35.000000 shroomdk-2.0.1/src/integrations/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:20:09.574781 shroomdk-2.0.1/src/integrations/query_integration/
+-rw-r--r--   0 jim        (501) staff       (20)       77 2023-05-02 18:10:35.000000 shroomdk-2.0.1/src/integrations/query_integration/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     9884 2023-05-02 18:10:35.000000 shroomdk-2.0.1/src/integrations/query_integration/compass_query_integration.py
+-rw-r--r--   0 jim        (501) staff       (20)      237 2023-05-02 18:10:35.000000 shroomdk-2.0.1/src/integrations/query_integration/defaults.py
+-rw-r--r--   0 jim        (501) staff       (20)     3570 2023-05-02 18:10:35.000000 shroomdk-2.0.1/src/integrations/query_integration/query_result_set_builder.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:20:09.575947 shroomdk-2.0.1/src/models/
+-rw-r--r--   0 jim        (501) staff       (20)      365 2023-05-02 18:10:35.000000 shroomdk-2.0.1/src/models/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:20:09.577011 shroomdk-2.0.1/src/models/compass/
+-rw-r--r--   0 jim        (501) staff       (20)       50 2023-05-02 18:10:35.000000 shroomdk-2.0.1/src/models/compass/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      571 2023-05-02 18:10:35.000000 shroomdk-2.0.1/src/models/compass/cancel_query_run.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:20:09.578400 shroomdk-2.0.1/src/models/compass/core/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.1/src/models/compass/core/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      187 2023-05-02 18:10:35.000000 shroomdk-2.0.1/src/models/compass/core/column_metadata.py
+-rw-r--r--   0 jim        (501) staff       (20)      117 2023-05-02 18:10:35.000000 shroomdk-2.0.1/src/models/compass/core/page.py
+-rw-r--r--   0 jim        (501) staff       (20)      183 2023-05-02 18:10:35.000000 shroomdk-2.0.1/src/models/compass/core/page_stats.py
+-rw-r--r--   0 jim        (501) staff       (20)      358 2023-05-02 18:10:35.000000 shroomdk-2.0.1/src/models/compass/core/query_request.py
+-rw-r--r--   0 jim        (501) staff       (20)      807 2023-05-02 18:10:35.000000 shroomdk-2.0.1/src/models/compass/core/query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)       89 2023-05-02 18:10:35.000000 shroomdk-2.0.1/src/models/compass/core/result_format.py
+-rw-r--r--   0 jim        (501) staff       (20)      149 2023-05-02 18:10:35.000000 shroomdk-2.0.1/src/models/compass/core/rpc_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      198 2023-05-02 18:10:35.000000 shroomdk-2.0.1/src/models/compass/core/rpc_request.py
+-rw-r--r--   0 jim        (501) staff       (20)      252 2023-05-02 18:10:35.000000 shroomdk-2.0.1/src/models/compass/core/rpc_response.py
+-rw-r--r--   0 jim        (501) staff       (20)      340 2023-05-02 18:10:35.000000 shroomdk-2.0.1/src/models/compass/core/sql_statement.py
+-rw-r--r--   0 jim        (501) staff       (20)      221 2023-05-02 18:10:35.000000 shroomdk-2.0.1/src/models/compass/core/tags.py
+-rw-r--r--   0 jim        (501) staff       (20)      845 2023-05-02 18:10:35.000000 shroomdk-2.0.1/src/models/compass/create_query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)      639 2023-05-02 18:10:35.000000 shroomdk-2.0.1/src/models/compass/get_query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)     2026 2023-05-02 18:10:35.000000 shroomdk-2.0.1/src/models/compass/get_query_run_results.py
+-rw-r--r--   0 jim        (501) staff       (20)      582 2023-05-02 18:10:35.000000 shroomdk-2.0.1/src/models/compass/get_sql_statement.py
+-rw-r--r--   0 jim        (501) staff       (20)      852 2023-05-02 18:10:35.000000 shroomdk-2.0.1/src/models/compass/query_results.py
+-rw-r--r--   0 jim        (501) staff       (20)     1422 2023-05-02 18:10:35.000000 shroomdk-2.0.1/src/models/query.py
+-rw-r--r--   0 jim        (501) staff       (20)      836 2023-05-02 18:10:35.000000 shroomdk-2.0.1/src/models/query_defaults.py
+-rw-r--r--   0 jim        (501) staff       (20)     1031 2023-05-02 18:10:35.000000 shroomdk-2.0.1/src/models/query_result_set.py
+-rw-r--r--   0 jim        (501) staff       (20)     1658 2023-05-02 18:10:35.000000 shroomdk-2.0.1/src/models/query_run_stats.py
+-rw-r--r--   0 jim        (501) staff       (20)      544 2023-05-02 18:10:35.000000 shroomdk-2.0.1/src/models/query_status.py
+-rw-r--r--   0 jim        (501) staff       (20)      194 2023-05-02 18:10:35.000000 shroomdk-2.0.1/src/models/sleep_config.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:20:09.578589 shroomdk-2.0.1/src/tests/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.1/src/tests/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:20:09.578722 shroomdk-2.0.1/src/tests/integrations/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.1/src/tests/integrations/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:20:09.579065 shroomdk-2.0.1/src/tests/integrations/query_integration/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.1/src/tests/integrations/query_integration/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     8712 2023-05-02 18:10:35.000000 shroomdk-2.0.1/src/tests/integrations/query_integration/test_query_compass_integration.py
+-rw-r--r--   0 jim        (501) staff       (20)     3438 2023-05-02 18:10:35.000000 shroomdk-2.0.1/src/tests/integrations/query_integration/test_query_result_set_builder.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:20:09.579310 shroomdk-2.0.1/src/tests/models/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.1/src/tests/models/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      931 2023-05-02 18:10:35.000000 shroomdk-2.0.1/src/tests/models/test_query_status.py
+-rw-r--r--   0 jim        (501) staff       (20)     5218 2023-05-02 18:10:35.000000 shroomdk-2.0.1/src/tests/test_rpc.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:20:09.579534 shroomdk-2.0.1/src/tests/utils/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.1/src/tests/utils/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     2242 2023-05-02 18:10:35.000000 shroomdk-2.0.1/src/tests/utils/test_sleep.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:20:09.579754 shroomdk-2.0.1/src/utils/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.1/src/utils/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     1966 2023-05-02 18:10:35.000000 shroomdk-2.0.1/src/utils/sleep.py
```

### Comparing `shroomdk-2.0.0/LICENSE.txt` & `shroomdk-2.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.0/PKG-INFO` & `shroomdk-2.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shroomdk
-Version: 2.0.0
+Version: 2.0.1
 Summary: SDK by Flipside Crypto: Query the most reliable & comprehensive blockchain data in crypto
 Home-page: https://github.com/FlipsideCrypto/sdk/python
 Author: dev@flipsidecrypto.com
 Author-email: dev@flipsidecrypto.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,15 +19,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Python SDK for the Flipside API, by Flipside Crypto
 
 [![Python Continuous Testing](https://github.com/FlipsideCrypto/sdk/actions/workflows/ci_python.yml/badge.svg)](https://github.com/FlipsideCrypto/sdk/actions/workflows/ci_python.yml)
 
-SDK, by Flipside Crypto gives you programmatic query access to the most reliable & comprehensive blockchain data sets in Web3, for free. More details on the SDK/API [here](https://data.flipsidecrypto.xyz).🥳
+The Python SDK, by Flipside Crypto gives you programmatic query access to the most reliable & comprehensive blockchain data sets in Web3, for free. More details on the SDK/API [here](https://docs.flipsidecrypto.com/flipside-api/get-started).
 
 ## Get Started
-Get started by checking out the docs on our [Gitbook here](https://docs.flipsidecrypto.xyz/sdk/python):
+Get started by checking out the docs on our [Gitbook here](https://docs.flipsidecrypto.com/flipside-api/get-started/python):
 
-[📖 Official Docs](https://docs.flipsidecrypto.xyz/sdk/python)
+[📖 Official Docs](https://docs.flipsidecrypto.com/flipside-api/get-started/python)
```

### Comparing `shroomdk-2.0.0/README.md` & `shroomdk-2.0.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Python SDK for the Flipside API, by Flipside Crypto
 
 [![Python Continuous Testing](https://github.com/FlipsideCrypto/sdk/actions/workflows/ci_python.yml/badge.svg)](https://github.com/FlipsideCrypto/sdk/actions/workflows/ci_python.yml)
 
-SDK, by Flipside Crypto gives you programmatic query access to the most reliable & comprehensive blockchain data sets in Web3, for free. More details on the SDK/API [here](https://data.flipsidecrypto.xyz).🥳
+The Python SDK, by Flipside Crypto gives you programmatic query access to the most reliable & comprehensive blockchain data sets in Web3, for free. More details on the SDK/API [here](https://docs.flipsidecrypto.com/flipside-api/get-started).
 
 ## Get Started
-Get started by checking out the docs on our [Gitbook here](https://docs.flipsidecrypto.xyz/sdk/python):
+Get started by checking out the docs on our [Gitbook here](https://docs.flipsidecrypto.com/flipside-api/get-started/python):
 
-[📖 Official Docs](https://docs.flipsidecrypto.xyz/sdk/python)
+[📖 Official Docs](https://docs.flipsidecrypto.com/flipside-api/get-started/python)
```

### Comparing `shroomdk-2.0.0/setup.py` & `shroomdk-2.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.0/shroomdk/errors/api_error.py` & `shroomdk-2.0.1/shroomdk/errors/api_error.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.0/shroomdk/errors/query_run_errors.py` & `shroomdk-2.0.1/shroomdk/errors/query_run_errors.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.0/shroomdk/flipside.py` & `shroomdk-2.0.1/shroomdk/flipside.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.0/shroomdk/integrations/query_integration/compass_query_integration.py` & `shroomdk-2.0.1/shroomdk/integrations/query_integration/compass_query_integration.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.0/shroomdk/integrations/query_integration/query_result_set_builder.py` & `shroomdk-2.0.1/shroomdk/integrations/query_integration/query_result_set_builder.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.0/shroomdk/models/compass/cancel_query_run.py` & `shroomdk-2.0.1/shroomdk/models/compass/cancel_query_run.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.0/shroomdk/models/compass/core/query_run.py` & `shroomdk-2.0.1/shroomdk/models/compass/core/query_run.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.0/shroomdk/models/compass/create_query_run.py` & `shroomdk-2.0.1/shroomdk/models/compass/create_query_run.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.0/shroomdk/models/compass/get_query_run.py` & `shroomdk-2.0.1/shroomdk/models/compass/get_query_run.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.0/shroomdk/models/compass/get_query_run_results.py` & `shroomdk-2.0.1/shroomdk/models/compass/get_query_run_results.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.0/shroomdk/models/compass/get_sql_statement.py` & `shroomdk-2.0.1/shroomdk/models/compass/get_sql_statement.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.0/shroomdk/models/compass/query_results.py` & `shroomdk-2.0.1/shroomdk/models/compass/query_results.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.0/shroomdk/models/query.py` & `shroomdk-2.0.1/shroomdk/models/query.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.0/shroomdk/models/query_defaults.py` & `shroomdk-2.0.1/shroomdk/models/query_defaults.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.0/shroomdk/models/query_result_set.py` & `shroomdk-2.0.1/shroomdk/models/query_result_set.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.0/shroomdk/models/query_run_stats.py` & `shroomdk-2.0.1/shroomdk/models/query_run_stats.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.0/shroomdk/models/query_status.py` & `shroomdk-2.0.1/shroomdk/models/query_status.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.0/shroomdk/rpc.py` & `shroomdk-2.0.1/shroomdk/rpc.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.0/shroomdk/tests/integrations/query_integration/test_query_compass_integration.py` & `shroomdk-2.0.1/shroomdk/tests/integrations/query_integration/test_query_compass_integration.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.0/shroomdk/tests/integrations/query_integration/test_query_result_set_builder.py` & `shroomdk-2.0.1/shroomdk/tests/integrations/query_integration/test_query_result_set_builder.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.0/shroomdk/tests/models/test_query_status.py` & `shroomdk-2.0.1/shroomdk/tests/models/test_query_status.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.0/shroomdk/tests/test_rpc.py` & `shroomdk-2.0.1/shroomdk/tests/test_rpc.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.0/shroomdk/tests/utils/test_sleep.py` & `shroomdk-2.0.1/shroomdk/tests/utils/test_sleep.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.0/shroomdk/utils/sleep.py` & `shroomdk-2.0.1/shroomdk/utils/sleep.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.0/shroomdk.egg-info/PKG-INFO` & `shroomdk-2.0.1/shroomdk.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shroomdk
-Version: 2.0.0
+Version: 2.0.1
 Summary: SDK by Flipside Crypto: Query the most reliable & comprehensive blockchain data in crypto
 Home-page: https://github.com/FlipsideCrypto/sdk/python
 Author: dev@flipsidecrypto.com
 Author-email: dev@flipsidecrypto.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,15 +19,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Python SDK for the Flipside API, by Flipside Crypto
 
 [![Python Continuous Testing](https://github.com/FlipsideCrypto/sdk/actions/workflows/ci_python.yml/badge.svg)](https://github.com/FlipsideCrypto/sdk/actions/workflows/ci_python.yml)
 
-SDK, by Flipside Crypto gives you programmatic query access to the most reliable & comprehensive blockchain data sets in Web3, for free. More details on the SDK/API [here](https://data.flipsidecrypto.xyz).🥳
+The Python SDK, by Flipside Crypto gives you programmatic query access to the most reliable & comprehensive blockchain data sets in Web3, for free. More details on the SDK/API [here](https://docs.flipsidecrypto.com/flipside-api/get-started).
 
 ## Get Started
-Get started by checking out the docs on our [Gitbook here](https://docs.flipsidecrypto.xyz/sdk/python):
+Get started by checking out the docs on our [Gitbook here](https://docs.flipsidecrypto.com/flipside-api/get-started/python):
 
-[📖 Official Docs](https://docs.flipsidecrypto.xyz/sdk/python)
+[📖 Official Docs](https://docs.flipsidecrypto.com/flipside-api/get-started/python)
```

### Comparing `shroomdk-2.0.0/shroomdk.egg-info/SOURCES.txt` & `shroomdk-2.0.1/shroomdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.0/src/errors/api_error.py` & `shroomdk-2.0.1/src/errors/api_error.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.0/src/errors/query_run_errors.py` & `shroomdk-2.0.1/src/errors/query_run_errors.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.0/src/integrations/query_integration/compass_query_integration.py` & `shroomdk-2.0.1/src/integrations/query_integration/compass_query_integration.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.0/src/integrations/query_integration/query_result_set_builder.py` & `shroomdk-2.0.1/src/integrations/query_integration/query_result_set_builder.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.0/src/models/compass/cancel_query_run.py` & `shroomdk-2.0.1/src/models/compass/cancel_query_run.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.0/src/models/compass/core/query_run.py` & `shroomdk-2.0.1/src/models/compass/core/query_run.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.0/src/models/compass/create_query_run.py` & `shroomdk-2.0.1/src/models/compass/create_query_run.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.0/src/models/compass/get_query_run.py` & `shroomdk-2.0.1/src/models/compass/get_query_run.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.0/src/models/compass/get_query_run_results.py` & `shroomdk-2.0.1/src/models/compass/get_query_run_results.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.0/src/models/compass/get_sql_statement.py` & `shroomdk-2.0.1/src/models/compass/get_sql_statement.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.0/src/models/compass/query_results.py` & `shroomdk-2.0.1/src/models/compass/query_results.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.0/src/models/query.py` & `shroomdk-2.0.1/src/models/query.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.0/src/models/query_defaults.py` & `shroomdk-2.0.1/src/models/query_defaults.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.0/src/models/query_result_set.py` & `shroomdk-2.0.1/src/models/query_result_set.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.0/src/models/query_run_stats.py` & `shroomdk-2.0.1/src/models/query_run_stats.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.0/src/models/query_status.py` & `shroomdk-2.0.1/src/models/query_status.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.0/src/tests/integrations/query_integration/test_query_compass_integration.py` & `shroomdk-2.0.1/src/tests/integrations/query_integration/test_query_compass_integration.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.0/src/tests/integrations/query_integration/test_query_result_set_builder.py` & `shroomdk-2.0.1/src/tests/integrations/query_integration/test_query_result_set_builder.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.0/src/tests/models/test_query_status.py` & `shroomdk-2.0.1/src/tests/models/test_query_status.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.0/src/tests/test_rpc.py` & `shroomdk-2.0.1/src/tests/test_rpc.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.0/src/tests/utils/test_sleep.py` & `shroomdk-2.0.1/src/tests/utils/test_sleep.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.0/src/utils/sleep.py` & `shroomdk-2.0.1/src/utils/sleep.py`

 * *Files identical despite different names*

