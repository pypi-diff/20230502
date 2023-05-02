# Comparing `tmp/shroomdk-2.0.2.tar.gz` & `tmp/shroomdk-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shroomdk-2.0.2.tar", last modified: Tue May  2 18:42:17 2023, max compression
+gzip compressed data, was "shroomdk-2.0.3.tar", last modified: Tue May  2 20:15:21 2023, max compression
```

## Comparing `shroomdk-2.0.2.tar` & `shroomdk-2.0.3.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:42:17.905077 shroomdk-2.0.2/
--rw-r--r--   0 jim        (501) staff       (20)     1073 2022-07-25 21:42:15.000000 shroomdk-2.0.2/LICENSE.txt
--rw-r--r--   0 jim        (501) staff       (20)       69 2022-07-25 21:42:15.000000 shroomdk-2.0.2/MANIFEST.in
--rw-r--r--   0 jim        (501) staff       (20)     1510 2023-05-02 18:42:17.905163 shroomdk-2.0.2/PKG-INFO
--rw-r--r--   0 jim        (501) staff       (20)      709 2023-05-02 18:18:58.000000 shroomdk-2.0.2/README.md
--rw-r--r--   0 jim        (501) staff       (20)        5 2023-05-02 18:39:27.000000 shroomdk-2.0.2/VERSION
--rw-r--r--   0 jim        (501) staff       (20)       30 2022-07-25 21:42:15.000000 shroomdk-2.0.2/requirements-dev.txt
--rw-r--r--   0 jim        (501) staff       (20)       33 2023-05-02 18:10:35.000000 shroomdk-2.0.2/requirements.txt
--rw-r--r--   0 jim        (501) staff       (20)       79 2023-05-02 18:42:17.905565 shroomdk-2.0.2/setup.cfg
--rw-r--r--   0 jim        (501) staff       (20)     1557 2023-05-02 18:10:35.000000 shroomdk-2.0.2/setup.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:42:17.883415 shroomdk-2.0.2/shroomdk/
--rw-r--r--   0 jim        (501) staff       (20)      147 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:42:17.884685 shroomdk-2.0.2/shroomdk/errors/
--rw-r--r--   0 jim        (501) staff       (20)      336 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk/errors/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     1583 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk/errors/api_error.py
--rw-r--r--   0 jim        (501) staff       (20)      121 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk/errors/base_error.py
--rw-r--r--   0 jim        (501) staff       (20)     2077 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk/errors/query_run_errors.py
--rw-r--r--   0 jim        (501) staff       (20)      262 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk/errors/sdk_error.py
--rw-r--r--   0 jim        (501) staff       (20)      361 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk/errors/server_error.py
--rw-r--r--   0 jim        (501) staff       (20)     2766 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk/flipside.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:42:17.884797 shroomdk-2.0.2/shroomdk/integrations/
--rw-r--r--   0 jim        (501) staff       (20)       69 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk/integrations/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:42:17.885262 shroomdk-2.0.2/shroomdk/integrations/query_integration/
--rw-r--r--   0 jim        (501) staff       (20)       77 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk/integrations/query_integration/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     9884 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk/integrations/query_integration/compass_query_integration.py
--rw-r--r--   0 jim        (501) staff       (20)      237 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk/integrations/query_integration/defaults.py
--rw-r--r--   0 jim        (501) staff       (20)     3570 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk/integrations/query_integration/query_result_set_builder.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:42:17.886116 shroomdk-2.0.2/shroomdk/models/
--rw-r--r--   0 jim        (501) staff       (20)      365 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk/models/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:42:17.887387 shroomdk-2.0.2/shroomdk/models/compass/
--rw-r--r--   0 jim        (501) staff       (20)       50 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk/models/compass/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      571 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk/models/compass/cancel_query_run.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:42:17.890471 shroomdk-2.0.2/shroomdk/models/compass/core/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk/models/compass/core/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      187 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk/models/compass/core/column_metadata.py
--rw-r--r--   0 jim        (501) staff       (20)      117 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk/models/compass/core/page.py
--rw-r--r--   0 jim        (501) staff       (20)      183 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk/models/compass/core/page_stats.py
--rw-r--r--   0 jim        (501) staff       (20)      358 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk/models/compass/core/query_request.py
--rw-r--r--   0 jim        (501) staff       (20)      807 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk/models/compass/core/query_run.py
--rw-r--r--   0 jim        (501) staff       (20)       89 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk/models/compass/core/result_format.py
--rw-r--r--   0 jim        (501) staff       (20)      149 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk/models/compass/core/rpc_error.py
--rw-r--r--   0 jim        (501) staff       (20)      198 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk/models/compass/core/rpc_request.py
--rw-r--r--   0 jim        (501) staff       (20)      252 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk/models/compass/core/rpc_response.py
--rw-r--r--   0 jim        (501) staff       (20)      340 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk/models/compass/core/sql_statement.py
--rw-r--r--   0 jim        (501) staff       (20)      221 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk/models/compass/core/tags.py
--rw-r--r--   0 jim        (501) staff       (20)      845 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk/models/compass/create_query_run.py
--rw-r--r--   0 jim        (501) staff       (20)      639 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk/models/compass/get_query_run.py
--rw-r--r--   0 jim        (501) staff       (20)     2026 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk/models/compass/get_query_run_results.py
--rw-r--r--   0 jim        (501) staff       (20)      582 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk/models/compass/get_sql_statement.py
--rw-r--r--   0 jim        (501) staff       (20)      852 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk/models/compass/query_results.py
--rw-r--r--   0 jim        (501) staff       (20)     1422 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk/models/query.py
--rw-r--r--   0 jim        (501) staff       (20)      836 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk/models/query_defaults.py
--rw-r--r--   0 jim        (501) staff       (20)     1031 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk/models/query_result_set.py
--rw-r--r--   0 jim        (501) staff       (20)     1658 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk/models/query_run_stats.py
--rw-r--r--   0 jim        (501) staff       (20)      544 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk/models/query_status.py
--rw-r--r--   0 jim        (501) staff       (20)      194 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk/models/sleep_config.py
--rw-r--r--   0 jim        (501) staff       (20)     5898 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk/rpc.py
--rw-r--r--   0 jim        (501) staff       (20)       68 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk/shroomdk.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:42:17.890681 shroomdk-2.0.2/shroomdk/tests/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk/tests/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:42:17.890824 shroomdk-2.0.2/shroomdk/tests/integrations/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk/tests/integrations/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:42:17.894317 shroomdk-2.0.2/shroomdk/tests/integrations/query_integration/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk/tests/integrations/query_integration/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     8712 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk/tests/integrations/query_integration/test_query_compass_integration.py
--rw-r--r--   0 jim        (501) staff       (20)     3438 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk/tests/integrations/query_integration/test_query_result_set_builder.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:42:17.894554 shroomdk-2.0.2/shroomdk/tests/models/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk/tests/models/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      931 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk/tests/models/test_query_status.py
--rw-r--r--   0 jim        (501) staff       (20)     5218 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk/tests/test_rpc.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:42:17.894865 shroomdk-2.0.2/shroomdk/tests/utils/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk/tests/utils/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     2242 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk/tests/utils/test_sleep.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:42:17.895069 shroomdk-2.0.2/shroomdk/utils/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk/utils/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     1966 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk/utils/sleep.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:42:17.884005 shroomdk-2.0.2/shroomdk.egg-info/
--rw-r--r--   0 jim        (501) staff       (20)     1510 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk.egg-info/PKG-INFO
--rw-r--r--   0 jim        (501) staff       (20)     4101 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk.egg-info/SOURCES.txt
--rw-r--r--   0 jim        (501) staff       (20)        1 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk.egg-info/dependency_links.txt
--rw-r--r--   0 jim        (501) staff       (20)       34 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk.egg-info/requires.txt
--rw-r--r--   0 jim        (501) staff       (20)       13 2023-05-02 18:42:17.000000 shroomdk-2.0.2/shroomdk.egg-info/top_level.txt
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:42:17.880730 shroomdk-2.0.2/src/
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:42:17.896378 shroomdk-2.0.2/src/errors/
--rw-r--r--   0 jim        (501) staff       (20)      336 2023-05-02 18:10:35.000000 shroomdk-2.0.2/src/errors/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     1583 2023-05-02 18:10:35.000000 shroomdk-2.0.2/src/errors/api_error.py
--rw-r--r--   0 jim        (501) staff       (20)      121 2023-05-02 18:10:35.000000 shroomdk-2.0.2/src/errors/base_error.py
--rw-r--r--   0 jim        (501) staff       (20)     2077 2023-05-02 18:10:35.000000 shroomdk-2.0.2/src/errors/query_run_errors.py
--rw-r--r--   0 jim        (501) staff       (20)      262 2023-05-02 18:10:35.000000 shroomdk-2.0.2/src/errors/sdk_error.py
--rw-r--r--   0 jim        (501) staff       (20)      361 2023-05-02 18:10:35.000000 shroomdk-2.0.2/src/errors/server_error.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:42:17.896498 shroomdk-2.0.2/src/integrations/
--rw-r--r--   0 jim        (501) staff       (20)       69 2023-05-02 18:10:35.000000 shroomdk-2.0.2/src/integrations/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:42:17.896972 shroomdk-2.0.2/src/integrations/query_integration/
--rw-r--r--   0 jim        (501) staff       (20)       77 2023-05-02 18:10:35.000000 shroomdk-2.0.2/src/integrations/query_integration/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     9884 2023-05-02 18:10:35.000000 shroomdk-2.0.2/src/integrations/query_integration/compass_query_integration.py
--rw-r--r--   0 jim        (501) staff       (20)      237 2023-05-02 18:10:35.000000 shroomdk-2.0.2/src/integrations/query_integration/defaults.py
--rw-r--r--   0 jim        (501) staff       (20)     3570 2023-05-02 18:10:35.000000 shroomdk-2.0.2/src/integrations/query_integration/query_result_set_builder.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:42:17.897828 shroomdk-2.0.2/src/models/
--rw-r--r--   0 jim        (501) staff       (20)      365 2023-05-02 18:10:35.000000 shroomdk-2.0.2/src/models/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:42:17.898835 shroomdk-2.0.2/src/models/compass/
--rw-r--r--   0 jim        (501) staff       (20)       50 2023-05-02 18:10:35.000000 shroomdk-2.0.2/src/models/compass/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      571 2023-05-02 18:10:35.000000 shroomdk-2.0.2/src/models/compass/cancel_query_run.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:42:17.901980 shroomdk-2.0.2/src/models/compass/core/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.2/src/models/compass/core/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      187 2023-05-02 18:10:35.000000 shroomdk-2.0.2/src/models/compass/core/column_metadata.py
--rw-r--r--   0 jim        (501) staff       (20)      117 2023-05-02 18:10:35.000000 shroomdk-2.0.2/src/models/compass/core/page.py
--rw-r--r--   0 jim        (501) staff       (20)      183 2023-05-02 18:10:35.000000 shroomdk-2.0.2/src/models/compass/core/page_stats.py
--rw-r--r--   0 jim        (501) staff       (20)      358 2023-05-02 18:10:35.000000 shroomdk-2.0.2/src/models/compass/core/query_request.py
--rw-r--r--   0 jim        (501) staff       (20)      807 2023-05-02 18:10:35.000000 shroomdk-2.0.2/src/models/compass/core/query_run.py
--rw-r--r--   0 jim        (501) staff       (20)       89 2023-05-02 18:10:35.000000 shroomdk-2.0.2/src/models/compass/core/result_format.py
--rw-r--r--   0 jim        (501) staff       (20)      149 2023-05-02 18:10:35.000000 shroomdk-2.0.2/src/models/compass/core/rpc_error.py
--rw-r--r--   0 jim        (501) staff       (20)      198 2023-05-02 18:10:35.000000 shroomdk-2.0.2/src/models/compass/core/rpc_request.py
--rw-r--r--   0 jim        (501) staff       (20)      252 2023-05-02 18:10:35.000000 shroomdk-2.0.2/src/models/compass/core/rpc_response.py
--rw-r--r--   0 jim        (501) staff       (20)      340 2023-05-02 18:10:35.000000 shroomdk-2.0.2/src/models/compass/core/sql_statement.py
--rw-r--r--   0 jim        (501) staff       (20)      221 2023-05-02 18:10:35.000000 shroomdk-2.0.2/src/models/compass/core/tags.py
--rw-r--r--   0 jim        (501) staff       (20)      845 2023-05-02 18:10:35.000000 shroomdk-2.0.2/src/models/compass/create_query_run.py
--rw-r--r--   0 jim        (501) staff       (20)      639 2023-05-02 18:10:35.000000 shroomdk-2.0.2/src/models/compass/get_query_run.py
--rw-r--r--   0 jim        (501) staff       (20)     2026 2023-05-02 18:10:35.000000 shroomdk-2.0.2/src/models/compass/get_query_run_results.py
--rw-r--r--   0 jim        (501) staff       (20)      582 2023-05-02 18:10:35.000000 shroomdk-2.0.2/src/models/compass/get_sql_statement.py
--rw-r--r--   0 jim        (501) staff       (20)      852 2023-05-02 18:10:35.000000 shroomdk-2.0.2/src/models/compass/query_results.py
--rw-r--r--   0 jim        (501) staff       (20)     1422 2023-05-02 18:10:35.000000 shroomdk-2.0.2/src/models/query.py
--rw-r--r--   0 jim        (501) staff       (20)      836 2023-05-02 18:10:35.000000 shroomdk-2.0.2/src/models/query_defaults.py
--rw-r--r--   0 jim        (501) staff       (20)     1031 2023-05-02 18:10:35.000000 shroomdk-2.0.2/src/models/query_result_set.py
--rw-r--r--   0 jim        (501) staff       (20)     1658 2023-05-02 18:10:35.000000 shroomdk-2.0.2/src/models/query_run_stats.py
--rw-r--r--   0 jim        (501) staff       (20)      544 2023-05-02 18:10:35.000000 shroomdk-2.0.2/src/models/query_status.py
--rw-r--r--   0 jim        (501) staff       (20)      194 2023-05-02 18:10:35.000000 shroomdk-2.0.2/src/models/sleep_config.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:42:17.902208 shroomdk-2.0.2/src/tests/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.2/src/tests/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:42:17.902365 shroomdk-2.0.2/src/tests/integrations/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.2/src/tests/integrations/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:42:17.902665 shroomdk-2.0.2/src/tests/integrations/query_integration/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.2/src/tests/integrations/query_integration/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     8712 2023-05-02 18:10:35.000000 shroomdk-2.0.2/src/tests/integrations/query_integration/test_query_compass_integration.py
--rw-r--r--   0 jim        (501) staff       (20)     3438 2023-05-02 18:10:35.000000 shroomdk-2.0.2/src/tests/integrations/query_integration/test_query_result_set_builder.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:42:17.902874 shroomdk-2.0.2/src/tests/models/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.2/src/tests/models/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      931 2023-05-02 18:10:35.000000 shroomdk-2.0.2/src/tests/models/test_query_status.py
--rw-r--r--   0 jim        (501) staff       (20)     5218 2023-05-02 18:10:35.000000 shroomdk-2.0.2/src/tests/test_rpc.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:42:17.904568 shroomdk-2.0.2/src/tests/utils/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.2/src/tests/utils/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     2242 2023-05-02 18:10:35.000000 shroomdk-2.0.2/src/tests/utils/test_sleep.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:42:17.904931 shroomdk-2.0.2/src/utils/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.2/src/utils/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     1966 2023-05-02 18:10:35.000000 shroomdk-2.0.2/src/utils/sleep.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.212392 shroomdk-2.0.3/
+-rw-r--r--   0 jim        (501) staff       (20)     1073 2022-07-25 21:42:15.000000 shroomdk-2.0.3/LICENSE.txt
+-rw-r--r--   0 jim        (501) staff       (20)       69 2022-07-25 21:42:15.000000 shroomdk-2.0.3/MANIFEST.in
+-rw-r--r--   0 jim        (501) staff       (20)     1510 2023-05-02 20:15:21.212468 shroomdk-2.0.3/PKG-INFO
+-rw-r--r--   0 jim        (501) staff       (20)      709 2023-05-02 18:18:58.000000 shroomdk-2.0.3/README.md
+-rw-r--r--   0 jim        (501) staff       (20)        5 2023-05-02 20:14:01.000000 shroomdk-2.0.3/VERSION
+-rw-r--r--   0 jim        (501) staff       (20)       30 2022-07-25 21:42:15.000000 shroomdk-2.0.3/requirements-dev.txt
+-rw-r--r--   0 jim        (501) staff       (20)       33 2023-05-02 18:10:35.000000 shroomdk-2.0.3/requirements.txt
+-rw-r--r--   0 jim        (501) staff       (20)       79 2023-05-02 20:15:21.213132 shroomdk-2.0.3/setup.cfg
+-rw-r--r--   0 jim        (501) staff       (20)     1557 2023-05-02 18:10:35.000000 shroomdk-2.0.3/setup.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.197098 shroomdk-2.0.3/shroomdk/
+-rw-r--r--   0 jim        (501) staff       (20)      147 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.198395 shroomdk-2.0.3/shroomdk/errors/
+-rw-r--r--   0 jim        (501) staff       (20)      336 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/errors/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     1583 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/errors/api_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      121 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/errors/base_error.py
+-rw-r--r--   0 jim        (501) staff       (20)     2077 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/errors/query_run_errors.py
+-rw-r--r--   0 jim        (501) staff       (20)      262 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/errors/sdk_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      361 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/errors/server_error.py
+-rw-r--r--   0 jim        (501) staff       (20)     2968 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/flipside.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.198512 shroomdk-2.0.3/shroomdk/integrations/
+-rw-r--r--   0 jim        (501) staff       (20)       69 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/integrations/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.198967 shroomdk-2.0.3/shroomdk/integrations/query_integration/
+-rw-r--r--   0 jim        (501) staff       (20)       77 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/integrations/query_integration/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     9884 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/integrations/query_integration/compass_query_integration.py
+-rw-r--r--   0 jim        (501) staff       (20)      237 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/integrations/query_integration/defaults.py
+-rw-r--r--   0 jim        (501) staff       (20)     3570 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/integrations/query_integration/query_result_set_builder.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.199768 shroomdk-2.0.3/shroomdk/models/
+-rw-r--r--   0 jim        (501) staff       (20)      365 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/models/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.200570 shroomdk-2.0.3/shroomdk/models/compass/
+-rw-r--r--   0 jim        (501) staff       (20)       50 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/models/compass/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      571 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/models/compass/cancel_query_run.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.201890 shroomdk-2.0.3/shroomdk/models/compass/core/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/models/compass/core/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      187 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/models/compass/core/column_metadata.py
+-rw-r--r--   0 jim        (501) staff       (20)      117 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/models/compass/core/page.py
+-rw-r--r--   0 jim        (501) staff       (20)      183 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/models/compass/core/page_stats.py
+-rw-r--r--   0 jim        (501) staff       (20)      358 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/models/compass/core/query_request.py
+-rw-r--r--   0 jim        (501) staff       (20)      807 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/models/compass/core/query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)       89 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/models/compass/core/result_format.py
+-rw-r--r--   0 jim        (501) staff       (20)      149 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/models/compass/core/rpc_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      198 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/models/compass/core/rpc_request.py
+-rw-r--r--   0 jim        (501) staff       (20)      252 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/models/compass/core/rpc_response.py
+-rw-r--r--   0 jim        (501) staff       (20)      340 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/models/compass/core/sql_statement.py
+-rw-r--r--   0 jim        (501) staff       (20)      221 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/models/compass/core/tags.py
+-rw-r--r--   0 jim        (501) staff       (20)      845 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/models/compass/create_query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)      639 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/models/compass/get_query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)     2026 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/models/compass/get_query_run_results.py
+-rw-r--r--   0 jim        (501) staff       (20)      582 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/models/compass/get_sql_statement.py
+-rw-r--r--   0 jim        (501) staff       (20)      852 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/models/compass/query_results.py
+-rw-r--r--   0 jim        (501) staff       (20)     1422 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/models/query.py
+-rw-r--r--   0 jim        (501) staff       (20)      836 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/models/query_defaults.py
+-rw-r--r--   0 jim        (501) staff       (20)     1031 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/models/query_result_set.py
+-rw-r--r--   0 jim        (501) staff       (20)     1658 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/models/query_run_stats.py
+-rw-r--r--   0 jim        (501) staff       (20)      544 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/models/query_status.py
+-rw-r--r--   0 jim        (501) staff       (20)      194 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/models/sleep_config.py
+-rw-r--r--   0 jim        (501) staff       (20)     5898 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/rpc.py
+-rw-r--r--   0 jim        (501) staff       (20)       68 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/shroomdk.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.202107 shroomdk-2.0.3/shroomdk/tests/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/tests/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.202217 shroomdk-2.0.3/shroomdk/tests/integrations/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/tests/integrations/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.202507 shroomdk-2.0.3/shroomdk/tests/integrations/query_integration/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/tests/integrations/query_integration/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     8712 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/tests/integrations/query_integration/test_query_compass_integration.py
+-rw-r--r--   0 jim        (501) staff       (20)     3438 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/tests/integrations/query_integration/test_query_result_set_builder.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.202720 shroomdk-2.0.3/shroomdk/tests/models/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/tests/models/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      931 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/tests/models/test_query_status.py
+-rw-r--r--   0 jim        (501) staff       (20)     5218 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/tests/test_rpc.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.202913 shroomdk-2.0.3/shroomdk/tests/utils/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/tests/utils/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     2242 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/tests/utils/test_sleep.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.203121 shroomdk-2.0.3/shroomdk/utils/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/utils/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     1966 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/utils/sleep.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.197713 shroomdk-2.0.3/shroomdk.egg-info/
+-rw-r--r--   0 jim        (501) staff       (20)     1510 2023-05-02 20:15:21.000000 shroomdk-2.0.3/shroomdk.egg-info/PKG-INFO
+-rw-r--r--   0 jim        (501) staff       (20)     4101 2023-05-02 20:15:21.000000 shroomdk-2.0.3/shroomdk.egg-info/SOURCES.txt
+-rw-r--r--   0 jim        (501) staff       (20)        1 2023-05-02 20:15:21.000000 shroomdk-2.0.3/shroomdk.egg-info/dependency_links.txt
+-rw-r--r--   0 jim        (501) staff       (20)       34 2023-05-02 20:15:21.000000 shroomdk-2.0.3/shroomdk.egg-info/requires.txt
+-rw-r--r--   0 jim        (501) staff       (20)       13 2023-05-02 20:15:21.000000 shroomdk-2.0.3/shroomdk.egg-info/top_level.txt
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.194853 shroomdk-2.0.3/src/
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.203777 shroomdk-2.0.3/src/errors/
+-rw-r--r--   0 jim        (501) staff       (20)      336 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/errors/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     1583 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/errors/api_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      121 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/errors/base_error.py
+-rw-r--r--   0 jim        (501) staff       (20)     2077 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/errors/query_run_errors.py
+-rw-r--r--   0 jim        (501) staff       (20)      262 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/errors/sdk_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      361 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/errors/server_error.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.203894 shroomdk-2.0.3/src/integrations/
+-rw-r--r--   0 jim        (501) staff       (20)       69 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/integrations/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.204326 shroomdk-2.0.3/src/integrations/query_integration/
+-rw-r--r--   0 jim        (501) staff       (20)       77 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/integrations/query_integration/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     9884 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/integrations/query_integration/compass_query_integration.py
+-rw-r--r--   0 jim        (501) staff       (20)      237 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/integrations/query_integration/defaults.py
+-rw-r--r--   0 jim        (501) staff       (20)     3570 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/integrations/query_integration/query_result_set_builder.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.205111 shroomdk-2.0.3/src/models/
+-rw-r--r--   0 jim        (501) staff       (20)      365 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/models/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.208103 shroomdk-2.0.3/src/models/compass/
+-rw-r--r--   0 jim        (501) staff       (20)       50 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/models/compass/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      571 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/models/compass/cancel_query_run.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.210281 shroomdk-2.0.3/src/models/compass/core/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/models/compass/core/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      187 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/models/compass/core/column_metadata.py
+-rw-r--r--   0 jim        (501) staff       (20)      117 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/models/compass/core/page.py
+-rw-r--r--   0 jim        (501) staff       (20)      183 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/models/compass/core/page_stats.py
+-rw-r--r--   0 jim        (501) staff       (20)      358 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/models/compass/core/query_request.py
+-rw-r--r--   0 jim        (501) staff       (20)      807 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/models/compass/core/query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)       89 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/models/compass/core/result_format.py
+-rw-r--r--   0 jim        (501) staff       (20)      149 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/models/compass/core/rpc_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      198 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/models/compass/core/rpc_request.py
+-rw-r--r--   0 jim        (501) staff       (20)      252 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/models/compass/core/rpc_response.py
+-rw-r--r--   0 jim        (501) staff       (20)      340 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/models/compass/core/sql_statement.py
+-rw-r--r--   0 jim        (501) staff       (20)      221 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/models/compass/core/tags.py
+-rw-r--r--   0 jim        (501) staff       (20)      845 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/models/compass/create_query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)      639 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/models/compass/get_query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)     2026 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/models/compass/get_query_run_results.py
+-rw-r--r--   0 jim        (501) staff       (20)      582 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/models/compass/get_sql_statement.py
+-rw-r--r--   0 jim        (501) staff       (20)      852 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/models/compass/query_results.py
+-rw-r--r--   0 jim        (501) staff       (20)     1422 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/models/query.py
+-rw-r--r--   0 jim        (501) staff       (20)      836 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/models/query_defaults.py
+-rw-r--r--   0 jim        (501) staff       (20)     1031 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/models/query_result_set.py
+-rw-r--r--   0 jim        (501) staff       (20)     1658 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/models/query_run_stats.py
+-rw-r--r--   0 jim        (501) staff       (20)      544 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/models/query_status.py
+-rw-r--r--   0 jim        (501) staff       (20)      194 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/models/sleep_config.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.210653 shroomdk-2.0.3/src/tests/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/tests/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.210840 shroomdk-2.0.3/src/tests/integrations/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/tests/integrations/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.211345 shroomdk-2.0.3/src/tests/integrations/query_integration/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/tests/integrations/query_integration/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     8712 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/tests/integrations/query_integration/test_query_compass_integration.py
+-rw-r--r--   0 jim        (501) staff       (20)     3438 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/tests/integrations/query_integration/test_query_result_set_builder.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.211644 shroomdk-2.0.3/src/tests/models/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/tests/models/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      931 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/tests/models/test_query_status.py
+-rw-r--r--   0 jim        (501) staff       (20)     5218 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/tests/test_rpc.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.211952 shroomdk-2.0.3/src/tests/utils/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/tests/utils/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     2242 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/tests/utils/test_sleep.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.212241 shroomdk-2.0.3/src/utils/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/utils/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     1966 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/utils/sleep.py
```

### Comparing `shroomdk-2.0.2/LICENSE.txt` & `shroomdk-2.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.2/PKG-INFO` & `shroomdk-2.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shroomdk
-Version: 2.0.2
+Version: 2.0.3
 Summary: SDK by Flipside Crypto: Query the most reliable & comprehensive blockchain data in crypto
 Home-page: https://github.com/FlipsideCrypto/sdk/python
 Author: dev@flipsidecrypto.com
 Author-email: dev@flipsidecrypto.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `shroomdk-2.0.2/README.md` & `shroomdk-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.2/setup.py` & `shroomdk-2.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.2/shroomdk/errors/api_error.py` & `shroomdk-2.0.3/shroomdk/errors/api_error.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.2/shroomdk/errors/query_run_errors.py` & `shroomdk-2.0.3/shroomdk/errors/query_run_errors.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.2/shroomdk/flipside.py` & `shroomdk-2.0.3/shroomdk/flipside.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,37 +7,42 @@
 from .models.compass.core.query_run import QueryRun
 from .models.compass.core.sql_statement import SqlStatement
 from .models.query_result_set import QueryResultSet
 from .rpc import RPC
 
 API_BASE_URL = "https://api-v2.flipsidecrypto.xyz"
 
+SDK_VERSION = "2.0.3"
+SDK_PACKAGE = "python"
+
 DEFAULT_DATA_SOURCE = "snowflake-default"
 DEFAULT_DATA_PROVIDER = "flipside"
-
-SDK_VERSION = "2.0.2"
-SDK_PACKAGE = "python"
+DEFAULT_PAGE_SIZE = 1000
+DEFAULT_PAGE_NUMBER = 1
+DEFAULT_TIMEOUT_MINUTES = 15
+DEFAULT_TTL_MINUTES = 60
+DEFAULT_MAX_AGE_MINUTES = 0
 
 
 class Flipside(object):
     def __init__(self, api_key: str, api_base_url: str = API_BASE_URL):
         if "api." in api_base_url.lower():
             api_base_url = API_BASE_URL
         self.rpc = RPC(api_base_url, api_key)
         self.query_integration = CompassQueryIntegration(self.rpc)
 
     def query(
         self,
         sql,
-        ttl_minutes=30,
-        max_age_minutes=0,
+        ttl_minutes=DEFAULT_TTL_MINUTES,
+        max_age_minutes=DEFAULT_MAX_AGE_MINUTES,
         cached=True,
-        timeout_minutes=20,
+        timeout_minutes=DEFAULT_TIMEOUT_MINUTES,
         retry_interval_seconds=1,
-        page_size=100000,
+        page_size=DEFAULT_PAGE_SIZE,
         page_number=1,
         data_source=DEFAULT_DATA_SOURCE,
         data_provider=DEFAULT_DATA_PROVIDER,
     ) -> QueryResultSet:
         query_integration = CompassQueryIntegration(self.rpc)
 
         return query_integration.run(
```

### Comparing `shroomdk-2.0.2/shroomdk/integrations/query_integration/compass_query_integration.py` & `shroomdk-2.0.3/shroomdk/integrations/query_integration/compass_query_integration.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.2/shroomdk/integrations/query_integration/query_result_set_builder.py` & `shroomdk-2.0.3/shroomdk/integrations/query_integration/query_result_set_builder.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.2/shroomdk/models/compass/cancel_query_run.py` & `shroomdk-2.0.3/shroomdk/models/compass/cancel_query_run.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.2/shroomdk/models/compass/core/query_run.py` & `shroomdk-2.0.3/shroomdk/models/compass/core/query_run.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.2/shroomdk/models/compass/create_query_run.py` & `shroomdk-2.0.3/shroomdk/models/compass/create_query_run.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.2/shroomdk/models/compass/get_query_run.py` & `shroomdk-2.0.3/shroomdk/models/compass/get_query_run.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.2/shroomdk/models/compass/get_query_run_results.py` & `shroomdk-2.0.3/shroomdk/models/compass/get_query_run_results.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.2/shroomdk/models/compass/get_sql_statement.py` & `shroomdk-2.0.3/shroomdk/models/compass/get_sql_statement.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.2/shroomdk/models/compass/query_results.py` & `shroomdk-2.0.3/shroomdk/models/compass/query_results.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.2/shroomdk/models/query.py` & `shroomdk-2.0.3/shroomdk/models/query.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.2/shroomdk/models/query_defaults.py` & `shroomdk-2.0.3/shroomdk/models/query_defaults.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.2/shroomdk/models/query_result_set.py` & `shroomdk-2.0.3/shroomdk/models/query_result_set.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.2/shroomdk/models/query_run_stats.py` & `shroomdk-2.0.3/shroomdk/models/query_run_stats.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.2/shroomdk/models/query_status.py` & `shroomdk-2.0.3/shroomdk/models/query_status.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.2/shroomdk/rpc.py` & `shroomdk-2.0.3/shroomdk/rpc.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.2/shroomdk/tests/integrations/query_integration/test_query_compass_integration.py` & `shroomdk-2.0.3/shroomdk/tests/integrations/query_integration/test_query_compass_integration.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.2/shroomdk/tests/integrations/query_integration/test_query_result_set_builder.py` & `shroomdk-2.0.3/shroomdk/tests/integrations/query_integration/test_query_result_set_builder.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.2/shroomdk/tests/models/test_query_status.py` & `shroomdk-2.0.3/shroomdk/tests/models/test_query_status.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.2/shroomdk/tests/test_rpc.py` & `shroomdk-2.0.3/shroomdk/tests/test_rpc.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.2/shroomdk/tests/utils/test_sleep.py` & `shroomdk-2.0.3/shroomdk/tests/utils/test_sleep.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.2/shroomdk/utils/sleep.py` & `shroomdk-2.0.3/shroomdk/utils/sleep.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.2/shroomdk.egg-info/PKG-INFO` & `shroomdk-2.0.3/shroomdk.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shroomdk
-Version: 2.0.2
+Version: 2.0.3
 Summary: SDK by Flipside Crypto: Query the most reliable & comprehensive blockchain data in crypto
 Home-page: https://github.com/FlipsideCrypto/sdk/python
 Author: dev@flipsidecrypto.com
 Author-email: dev@flipsidecrypto.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `shroomdk-2.0.2/shroomdk.egg-info/SOURCES.txt` & `shroomdk-2.0.3/shroomdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.2/src/errors/api_error.py` & `shroomdk-2.0.3/src/errors/api_error.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.2/src/errors/query_run_errors.py` & `shroomdk-2.0.3/src/errors/query_run_errors.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.2/src/integrations/query_integration/compass_query_integration.py` & `shroomdk-2.0.3/src/integrations/query_integration/compass_query_integration.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.2/src/integrations/query_integration/query_result_set_builder.py` & `shroomdk-2.0.3/src/integrations/query_integration/query_result_set_builder.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.2/src/models/compass/cancel_query_run.py` & `shroomdk-2.0.3/src/models/compass/cancel_query_run.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.2/src/models/compass/core/query_run.py` & `shroomdk-2.0.3/src/models/compass/core/query_run.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.2/src/models/compass/create_query_run.py` & `shroomdk-2.0.3/src/models/compass/create_query_run.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.2/src/models/compass/get_query_run.py` & `shroomdk-2.0.3/src/models/compass/get_query_run.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.2/src/models/compass/get_query_run_results.py` & `shroomdk-2.0.3/src/models/compass/get_query_run_results.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.2/src/models/compass/get_sql_statement.py` & `shroomdk-2.0.3/src/models/compass/get_sql_statement.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.2/src/models/compass/query_results.py` & `shroomdk-2.0.3/src/models/compass/query_results.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.2/src/models/query.py` & `shroomdk-2.0.3/src/models/query.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.2/src/models/query_defaults.py` & `shroomdk-2.0.3/src/models/query_defaults.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.2/src/models/query_result_set.py` & `shroomdk-2.0.3/src/models/query_result_set.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.2/src/models/query_run_stats.py` & `shroomdk-2.0.3/src/models/query_run_stats.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.2/src/models/query_status.py` & `shroomdk-2.0.3/src/models/query_status.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.2/src/tests/integrations/query_integration/test_query_compass_integration.py` & `shroomdk-2.0.3/src/tests/integrations/query_integration/test_query_compass_integration.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.2/src/tests/integrations/query_integration/test_query_result_set_builder.py` & `shroomdk-2.0.3/src/tests/integrations/query_integration/test_query_result_set_builder.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.2/src/tests/models/test_query_status.py` & `shroomdk-2.0.3/src/tests/models/test_query_status.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.2/src/tests/test_rpc.py` & `shroomdk-2.0.3/src/tests/test_rpc.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.2/src/tests/utils/test_sleep.py` & `shroomdk-2.0.3/src/tests/utils/test_sleep.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.2/src/utils/sleep.py` & `shroomdk-2.0.3/src/utils/sleep.py`

 * *Files identical despite different names*

