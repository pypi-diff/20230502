# Comparing `tmp/flipside-2.0.0.tar.gz` & `tmp/flipside-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flipside-2.0.0.tar", last modified: Tue May  2 18:11:13 2023, max compression
+gzip compressed data, was "flipside-2.0.1.tar", last modified: Tue May  2 18:19:51 2023, max compression
```

## Comparing `flipside-2.0.0.tar` & `flipside-2.0.1.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:13.046581 flipside-2.0.0/
--rw-r--r--   0 jim        (501) staff       (20)     1073 2022-07-25 21:42:15.000000 flipside-2.0.0/LICENSE.txt
--rw-r--r--   0 jim        (501) staff       (20)       69 2022-07-25 21:42:15.000000 flipside-2.0.0/MANIFEST.in
--rw-r--r--   0 jim        (501) staff       (20)     1436 2023-05-02 18:11:13.046663 flipside-2.0.0/PKG-INFO
--rw-r--r--   0 jim        (501) staff       (20)      635 2023-05-02 18:10:35.000000 flipside-2.0.0/README.md
--rw-r--r--   0 jim        (501) staff       (20)        5 2023-05-02 18:10:35.000000 flipside-2.0.0/VERSION
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:13.029411 flipside-2.0.0/flipside/
--rw-r--r--   0 jim        (501) staff       (20)      147 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:13.030826 flipside-2.0.0/flipside/errors/
--rw-r--r--   0 jim        (501) staff       (20)      336 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside/errors/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     1583 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside/errors/api_error.py
--rw-r--r--   0 jim        (501) staff       (20)      121 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside/errors/base_error.py
--rw-r--r--   0 jim        (501) staff       (20)     2077 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside/errors/query_run_errors.py
--rw-r--r--   0 jim        (501) staff       (20)      262 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside/errors/sdk_error.py
--rw-r--r--   0 jim        (501) staff       (20)      361 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside/errors/server_error.py
--rw-r--r--   0 jim        (501) staff       (20)     2766 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside/flipside.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:13.030957 flipside-2.0.0/flipside/integrations/
--rw-r--r--   0 jim        (501) staff       (20)       69 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside/integrations/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:13.031767 flipside-2.0.0/flipside/integrations/query_integration/
--rw-r--r--   0 jim        (501) staff       (20)       77 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside/integrations/query_integration/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     9884 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside/integrations/query_integration/compass_query_integration.py
--rw-r--r--   0 jim        (501) staff       (20)      237 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside/integrations/query_integration/defaults.py
--rw-r--r--   0 jim        (501) staff       (20)     3570 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside/integrations/query_integration/query_result_set_builder.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:13.033009 flipside-2.0.0/flipside/models/
--rw-r--r--   0 jim        (501) staff       (20)      365 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside/models/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:13.034664 flipside-2.0.0/flipside/models/compass/
--rw-r--r--   0 jim        (501) staff       (20)       50 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside/models/compass/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      571 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside/models/compass/cancel_query_run.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:13.036579 flipside-2.0.0/flipside/models/compass/core/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside/models/compass/core/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      187 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside/models/compass/core/column_metadata.py
--rw-r--r--   0 jim        (501) staff       (20)      117 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside/models/compass/core/page.py
--rw-r--r--   0 jim        (501) staff       (20)      183 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside/models/compass/core/page_stats.py
--rw-r--r--   0 jim        (501) staff       (20)      358 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside/models/compass/core/query_request.py
--rw-r--r--   0 jim        (501) staff       (20)      807 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside/models/compass/core/query_run.py
--rw-r--r--   0 jim        (501) staff       (20)       89 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside/models/compass/core/result_format.py
--rw-r--r--   0 jim        (501) staff       (20)      149 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside/models/compass/core/rpc_error.py
--rw-r--r--   0 jim        (501) staff       (20)      198 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside/models/compass/core/rpc_request.py
--rw-r--r--   0 jim        (501) staff       (20)      252 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside/models/compass/core/rpc_response.py
--rw-r--r--   0 jim        (501) staff       (20)      340 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside/models/compass/core/sql_statement.py
--rw-r--r--   0 jim        (501) staff       (20)      221 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside/models/compass/core/tags.py
--rw-r--r--   0 jim        (501) staff       (20)      845 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside/models/compass/create_query_run.py
--rw-r--r--   0 jim        (501) staff       (20)      639 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside/models/compass/get_query_run.py
--rw-r--r--   0 jim        (501) staff       (20)     2026 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside/models/compass/get_query_run_results.py
--rw-r--r--   0 jim        (501) staff       (20)      582 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside/models/compass/get_sql_statement.py
--rw-r--r--   0 jim        (501) staff       (20)      852 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside/models/compass/query_results.py
--rw-r--r--   0 jim        (501) staff       (20)     1422 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside/models/query.py
--rw-r--r--   0 jim        (501) staff       (20)      836 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside/models/query_defaults.py
--rw-r--r--   0 jim        (501) staff       (20)     1031 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside/models/query_result_set.py
--rw-r--r--   0 jim        (501) staff       (20)     1658 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside/models/query_run_stats.py
--rw-r--r--   0 jim        (501) staff       (20)      544 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside/models/query_status.py
--rw-r--r--   0 jim        (501) staff       (20)      194 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside/models/sleep_config.py
--rw-r--r--   0 jim        (501) staff       (20)     5708 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside/rpc.py
--rw-r--r--   0 jim        (501) staff       (20)       68 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside/shroomdk.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:13.036883 flipside-2.0.0/flipside/tests/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside/tests/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:13.037177 flipside-2.0.0/flipside/tests/integrations/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside/tests/integrations/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:13.037654 flipside-2.0.0/flipside/tests/integrations/query_integration/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside/tests/integrations/query_integration/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     8712 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside/tests/integrations/query_integration/test_query_compass_integration.py
--rw-r--r--   0 jim        (501) staff       (20)     3438 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside/tests/integrations/query_integration/test_query_result_set_builder.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:13.037887 flipside-2.0.0/flipside/tests/models/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside/tests/models/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      931 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside/tests/models/test_query_status.py
--rw-r--r--   0 jim        (501) staff       (20)     5218 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside/tests/test_rpc.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:13.038097 flipside-2.0.0/flipside/tests/utils/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside/tests/utils/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     2242 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside/tests/utils/test_sleep.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:13.038327 flipside-2.0.0/flipside/utils/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside/utils/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     1966 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside/utils/sleep.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:13.029986 flipside-2.0.0/flipside.egg-info/
--rw-r--r--   0 jim        (501) staff       (20)     1436 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside.egg-info/PKG-INFO
--rw-r--r--   0 jim        (501) staff       (20)     4101 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside.egg-info/SOURCES.txt
--rw-r--r--   0 jim        (501) staff       (20)        1 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside.egg-info/dependency_links.txt
--rw-r--r--   0 jim        (501) staff       (20)       34 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside.egg-info/requires.txt
--rw-r--r--   0 jim        (501) staff       (20)       13 2023-05-02 18:11:12.000000 flipside-2.0.0/flipside.egg-info/top_level.txt
--rw-r--r--   0 jim        (501) staff       (20)       30 2022-07-25 21:42:15.000000 flipside-2.0.0/requirements-dev.txt
--rw-r--r--   0 jim        (501) staff       (20)       33 2023-05-02 18:10:35.000000 flipside-2.0.0/requirements.txt
--rw-r--r--   0 jim        (501) staff       (20)       79 2023-05-02 18:11:13.047066 flipside-2.0.0/setup.cfg
--rw-r--r--   0 jim        (501) staff       (20)     1557 2023-05-02 18:10:35.000000 flipside-2.0.0/setup.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:13.026925 flipside-2.0.0/src/
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:13.039084 flipside-2.0.0/src/errors/
--rw-r--r--   0 jim        (501) staff       (20)      336 2023-05-02 18:10:35.000000 flipside-2.0.0/src/errors/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     1583 2023-05-02 18:10:35.000000 flipside-2.0.0/src/errors/api_error.py
--rw-r--r--   0 jim        (501) staff       (20)      121 2023-05-02 18:10:35.000000 flipside-2.0.0/src/errors/base_error.py
--rw-r--r--   0 jim        (501) staff       (20)     2077 2023-05-02 18:10:35.000000 flipside-2.0.0/src/errors/query_run_errors.py
--rw-r--r--   0 jim        (501) staff       (20)      262 2023-05-02 18:10:35.000000 flipside-2.0.0/src/errors/sdk_error.py
--rw-r--r--   0 jim        (501) staff       (20)      361 2023-05-02 18:10:35.000000 flipside-2.0.0/src/errors/server_error.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:13.039240 flipside-2.0.0/src/integrations/
--rw-r--r--   0 jim        (501) staff       (20)       69 2023-05-02 18:10:35.000000 flipside-2.0.0/src/integrations/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:13.039903 flipside-2.0.0/src/integrations/query_integration/
--rw-r--r--   0 jim        (501) staff       (20)       77 2023-05-02 18:10:35.000000 flipside-2.0.0/src/integrations/query_integration/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     9884 2023-05-02 18:10:35.000000 flipside-2.0.0/src/integrations/query_integration/compass_query_integration.py
--rw-r--r--   0 jim        (501) staff       (20)      237 2023-05-02 18:10:35.000000 flipside-2.0.0/src/integrations/query_integration/defaults.py
--rw-r--r--   0 jim        (501) staff       (20)     3570 2023-05-02 18:10:35.000000 flipside-2.0.0/src/integrations/query_integration/query_result_set_builder.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:13.041932 flipside-2.0.0/src/models/
--rw-r--r--   0 jim        (501) staff       (20)      365 2023-05-02 18:10:35.000000 flipside-2.0.0/src/models/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:13.043297 flipside-2.0.0/src/models/compass/
--rw-r--r--   0 jim        (501) staff       (20)       50 2023-05-02 18:10:35.000000 flipside-2.0.0/src/models/compass/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      571 2023-05-02 18:10:35.000000 flipside-2.0.0/src/models/compass/cancel_query_run.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:13.045022 flipside-2.0.0/src/models/compass/core/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.0/src/models/compass/core/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      187 2023-05-02 18:10:35.000000 flipside-2.0.0/src/models/compass/core/column_metadata.py
--rw-r--r--   0 jim        (501) staff       (20)      117 2023-05-02 18:10:35.000000 flipside-2.0.0/src/models/compass/core/page.py
--rw-r--r--   0 jim        (501) staff       (20)      183 2023-05-02 18:10:35.000000 flipside-2.0.0/src/models/compass/core/page_stats.py
--rw-r--r--   0 jim        (501) staff       (20)      358 2023-05-02 18:10:35.000000 flipside-2.0.0/src/models/compass/core/query_request.py
--rw-r--r--   0 jim        (501) staff       (20)      807 2023-05-02 18:10:35.000000 flipside-2.0.0/src/models/compass/core/query_run.py
--rw-r--r--   0 jim        (501) staff       (20)       89 2023-05-02 18:10:35.000000 flipside-2.0.0/src/models/compass/core/result_format.py
--rw-r--r--   0 jim        (501) staff       (20)      149 2023-05-02 18:10:35.000000 flipside-2.0.0/src/models/compass/core/rpc_error.py
--rw-r--r--   0 jim        (501) staff       (20)      198 2023-05-02 18:10:35.000000 flipside-2.0.0/src/models/compass/core/rpc_request.py
--rw-r--r--   0 jim        (501) staff       (20)      252 2023-05-02 18:10:35.000000 flipside-2.0.0/src/models/compass/core/rpc_response.py
--rw-r--r--   0 jim        (501) staff       (20)      340 2023-05-02 18:10:35.000000 flipside-2.0.0/src/models/compass/core/sql_statement.py
--rw-r--r--   0 jim        (501) staff       (20)      221 2023-05-02 18:10:35.000000 flipside-2.0.0/src/models/compass/core/tags.py
--rw-r--r--   0 jim        (501) staff       (20)      845 2023-05-02 18:10:35.000000 flipside-2.0.0/src/models/compass/create_query_run.py
--rw-r--r--   0 jim        (501) staff       (20)      639 2023-05-02 18:10:35.000000 flipside-2.0.0/src/models/compass/get_query_run.py
--rw-r--r--   0 jim        (501) staff       (20)     2026 2023-05-02 18:10:35.000000 flipside-2.0.0/src/models/compass/get_query_run_results.py
--rw-r--r--   0 jim        (501) staff       (20)      582 2023-05-02 18:10:35.000000 flipside-2.0.0/src/models/compass/get_sql_statement.py
--rw-r--r--   0 jim        (501) staff       (20)      852 2023-05-02 18:10:35.000000 flipside-2.0.0/src/models/compass/query_results.py
--rw-r--r--   0 jim        (501) staff       (20)     1422 2023-05-02 18:10:35.000000 flipside-2.0.0/src/models/query.py
--rw-r--r--   0 jim        (501) staff       (20)      836 2023-05-02 18:10:35.000000 flipside-2.0.0/src/models/query_defaults.py
--rw-r--r--   0 jim        (501) staff       (20)     1031 2023-05-02 18:10:35.000000 flipside-2.0.0/src/models/query_result_set.py
--rw-r--r--   0 jim        (501) staff       (20)     1658 2023-05-02 18:10:35.000000 flipside-2.0.0/src/models/query_run_stats.py
--rw-r--r--   0 jim        (501) staff       (20)      544 2023-05-02 18:10:35.000000 flipside-2.0.0/src/models/query_status.py
--rw-r--r--   0 jim        (501) staff       (20)      194 2023-05-02 18:10:35.000000 flipside-2.0.0/src/models/sleep_config.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:13.045244 flipside-2.0.0/src/tests/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.0/src/tests/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:13.045368 flipside-2.0.0/src/tests/integrations/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.0/src/tests/integrations/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:13.045705 flipside-2.0.0/src/tests/integrations/query_integration/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.0/src/tests/integrations/query_integration/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     8712 2023-05-02 18:10:35.000000 flipside-2.0.0/src/tests/integrations/query_integration/test_query_compass_integration.py
--rw-r--r--   0 jim        (501) staff       (20)     3438 2023-05-02 18:10:35.000000 flipside-2.0.0/src/tests/integrations/query_integration/test_query_result_set_builder.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:13.046047 flipside-2.0.0/src/tests/models/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.0/src/tests/models/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      931 2023-05-02 18:10:35.000000 flipside-2.0.0/src/tests/models/test_query_status.py
--rw-r--r--   0 jim        (501) staff       (20)     5218 2023-05-02 18:10:35.000000 flipside-2.0.0/src/tests/test_rpc.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:13.046253 flipside-2.0.0/src/tests/utils/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.0/src/tests/utils/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     2242 2023-05-02 18:10:35.000000 flipside-2.0.0/src/tests/utils/test_sleep.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:11:13.046470 flipside-2.0.0/src/utils/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.0/src/utils/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     1966 2023-05-02 18:10:35.000000 flipside-2.0.0/src/utils/sleep.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:19:51.301169 flipside-2.0.1/
+-rw-r--r--   0 jim        (501) staff       (20)     1073 2022-07-25 21:42:15.000000 flipside-2.0.1/LICENSE.txt
+-rw-r--r--   0 jim        (501) staff       (20)       69 2022-07-25 21:42:15.000000 flipside-2.0.1/MANIFEST.in
+-rw-r--r--   0 jim        (501) staff       (20)     1510 2023-05-02 18:19:51.301247 flipside-2.0.1/PKG-INFO
+-rw-r--r--   0 jim        (501) staff       (20)      709 2023-05-02 18:18:58.000000 flipside-2.0.1/README.md
+-rw-r--r--   0 jim        (501) staff       (20)        5 2023-05-02 18:19:19.000000 flipside-2.0.1/VERSION
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:19:51.275734 flipside-2.0.1/flipside/
+-rw-r--r--   0 jim        (501) staff       (20)      147 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:19:51.277460 flipside-2.0.1/flipside/errors/
+-rw-r--r--   0 jim        (501) staff       (20)      336 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside/errors/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     1583 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside/errors/api_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      121 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside/errors/base_error.py
+-rw-r--r--   0 jim        (501) staff       (20)     2077 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside/errors/query_run_errors.py
+-rw-r--r--   0 jim        (501) staff       (20)      262 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside/errors/sdk_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      361 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside/errors/server_error.py
+-rw-r--r--   0 jim        (501) staff       (20)     2766 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside/flipside.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:19:51.277572 flipside-2.0.1/flipside/integrations/
+-rw-r--r--   0 jim        (501) staff       (20)       69 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside/integrations/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:19:51.278017 flipside-2.0.1/flipside/integrations/query_integration/
+-rw-r--r--   0 jim        (501) staff       (20)       77 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside/integrations/query_integration/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     9884 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside/integrations/query_integration/compass_query_integration.py
+-rw-r--r--   0 jim        (501) staff       (20)      237 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside/integrations/query_integration/defaults.py
+-rw-r--r--   0 jim        (501) staff       (20)     3570 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside/integrations/query_integration/query_result_set_builder.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:19:51.278799 flipside-2.0.1/flipside/models/
+-rw-r--r--   0 jim        (501) staff       (20)      365 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside/models/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:19:51.279582 flipside-2.0.1/flipside/models/compass/
+-rw-r--r--   0 jim        (501) staff       (20)       50 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside/models/compass/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      571 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside/models/compass/cancel_query_run.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:19:51.280992 flipside-2.0.1/flipside/models/compass/core/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside/models/compass/core/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      187 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside/models/compass/core/column_metadata.py
+-rw-r--r--   0 jim        (501) staff       (20)      117 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside/models/compass/core/page.py
+-rw-r--r--   0 jim        (501) staff       (20)      183 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside/models/compass/core/page_stats.py
+-rw-r--r--   0 jim        (501) staff       (20)      358 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside/models/compass/core/query_request.py
+-rw-r--r--   0 jim        (501) staff       (20)      807 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside/models/compass/core/query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)       89 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside/models/compass/core/result_format.py
+-rw-r--r--   0 jim        (501) staff       (20)      149 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside/models/compass/core/rpc_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      198 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside/models/compass/core/rpc_request.py
+-rw-r--r--   0 jim        (501) staff       (20)      252 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside/models/compass/core/rpc_response.py
+-rw-r--r--   0 jim        (501) staff       (20)      340 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside/models/compass/core/sql_statement.py
+-rw-r--r--   0 jim        (501) staff       (20)      221 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside/models/compass/core/tags.py
+-rw-r--r--   0 jim        (501) staff       (20)      845 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside/models/compass/create_query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)      639 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside/models/compass/get_query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)     2026 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside/models/compass/get_query_run_results.py
+-rw-r--r--   0 jim        (501) staff       (20)      582 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside/models/compass/get_sql_statement.py
+-rw-r--r--   0 jim        (501) staff       (20)      852 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside/models/compass/query_results.py
+-rw-r--r--   0 jim        (501) staff       (20)     1422 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside/models/query.py
+-rw-r--r--   0 jim        (501) staff       (20)      836 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside/models/query_defaults.py
+-rw-r--r--   0 jim        (501) staff       (20)     1031 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside/models/query_result_set.py
+-rw-r--r--   0 jim        (501) staff       (20)     1658 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside/models/query_run_stats.py
+-rw-r--r--   0 jim        (501) staff       (20)      544 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside/models/query_status.py
+-rw-r--r--   0 jim        (501) staff       (20)      194 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside/models/sleep_config.py
+-rw-r--r--   0 jim        (501) staff       (20)     5708 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside/rpc.py
+-rw-r--r--   0 jim        (501) staff       (20)       68 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside/shroomdk.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:19:51.281201 flipside-2.0.1/flipside/tests/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside/tests/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:19:51.281309 flipside-2.0.1/flipside/tests/integrations/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside/tests/integrations/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:19:51.281661 flipside-2.0.1/flipside/tests/integrations/query_integration/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside/tests/integrations/query_integration/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     8712 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside/tests/integrations/query_integration/test_query_compass_integration.py
+-rw-r--r--   0 jim        (501) staff       (20)     3438 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside/tests/integrations/query_integration/test_query_result_set_builder.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:19:51.281863 flipside-2.0.1/flipside/tests/models/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside/tests/models/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      931 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside/tests/models/test_query_status.py
+-rw-r--r--   0 jim        (501) staff       (20)     5218 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside/tests/test_rpc.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:19:51.282048 flipside-2.0.1/flipside/tests/utils/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside/tests/utils/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     2242 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside/tests/utils/test_sleep.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:19:51.282252 flipside-2.0.1/flipside/utils/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside/utils/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     1966 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside/utils/sleep.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:19:51.276769 flipside-2.0.1/flipside.egg-info/
+-rw-r--r--   0 jim        (501) staff       (20)     1510 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside.egg-info/PKG-INFO
+-rw-r--r--   0 jim        (501) staff       (20)     4101 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside.egg-info/SOURCES.txt
+-rw-r--r--   0 jim        (501) staff       (20)        1 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside.egg-info/dependency_links.txt
+-rw-r--r--   0 jim        (501) staff       (20)       34 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside.egg-info/requires.txt
+-rw-r--r--   0 jim        (501) staff       (20)       13 2023-05-02 18:19:51.000000 flipside-2.0.1/flipside.egg-info/top_level.txt
+-rw-r--r--   0 jim        (501) staff       (20)       30 2022-07-25 21:42:15.000000 flipside-2.0.1/requirements-dev.txt
+-rw-r--r--   0 jim        (501) staff       (20)       33 2023-05-02 18:10:35.000000 flipside-2.0.1/requirements.txt
+-rw-r--r--   0 jim        (501) staff       (20)       79 2023-05-02 18:19:51.301605 flipside-2.0.1/setup.cfg
+-rw-r--r--   0 jim        (501) staff       (20)     1557 2023-05-02 18:10:35.000000 flipside-2.0.1/setup.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:19:51.273306 flipside-2.0.1/src/
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:19:51.282960 flipside-2.0.1/src/errors/
+-rw-r--r--   0 jim        (501) staff       (20)      336 2023-05-02 18:10:35.000000 flipside-2.0.1/src/errors/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     1583 2023-05-02 18:10:35.000000 flipside-2.0.1/src/errors/api_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      121 2023-05-02 18:10:35.000000 flipside-2.0.1/src/errors/base_error.py
+-rw-r--r--   0 jim        (501) staff       (20)     2077 2023-05-02 18:10:35.000000 flipside-2.0.1/src/errors/query_run_errors.py
+-rw-r--r--   0 jim        (501) staff       (20)      262 2023-05-02 18:10:35.000000 flipside-2.0.1/src/errors/sdk_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      361 2023-05-02 18:10:35.000000 flipside-2.0.1/src/errors/server_error.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:19:51.283090 flipside-2.0.1/src/integrations/
+-rw-r--r--   0 jim        (501) staff       (20)       69 2023-05-02 18:10:35.000000 flipside-2.0.1/src/integrations/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:19:51.283589 flipside-2.0.1/src/integrations/query_integration/
+-rw-r--r--   0 jim        (501) staff       (20)       77 2023-05-02 18:10:35.000000 flipside-2.0.1/src/integrations/query_integration/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     9884 2023-05-02 18:10:35.000000 flipside-2.0.1/src/integrations/query_integration/compass_query_integration.py
+-rw-r--r--   0 jim        (501) staff       (20)      237 2023-05-02 18:10:35.000000 flipside-2.0.1/src/integrations/query_integration/defaults.py
+-rw-r--r--   0 jim        (501) staff       (20)     3570 2023-05-02 18:10:35.000000 flipside-2.0.1/src/integrations/query_integration/query_result_set_builder.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:19:51.285135 flipside-2.0.1/src/models/
+-rw-r--r--   0 jim        (501) staff       (20)      365 2023-05-02 18:10:35.000000 flipside-2.0.1/src/models/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:19:51.287968 flipside-2.0.1/src/models/compass/
+-rw-r--r--   0 jim        (501) staff       (20)       50 2023-05-02 18:10:35.000000 flipside-2.0.1/src/models/compass/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      571 2023-05-02 18:10:35.000000 flipside-2.0.1/src/models/compass/cancel_query_run.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:19:51.296162 flipside-2.0.1/src/models/compass/core/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.1/src/models/compass/core/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      187 2023-05-02 18:10:35.000000 flipside-2.0.1/src/models/compass/core/column_metadata.py
+-rw-r--r--   0 jim        (501) staff       (20)      117 2023-05-02 18:10:35.000000 flipside-2.0.1/src/models/compass/core/page.py
+-rw-r--r--   0 jim        (501) staff       (20)      183 2023-05-02 18:10:35.000000 flipside-2.0.1/src/models/compass/core/page_stats.py
+-rw-r--r--   0 jim        (501) staff       (20)      358 2023-05-02 18:10:35.000000 flipside-2.0.1/src/models/compass/core/query_request.py
+-rw-r--r--   0 jim        (501) staff       (20)      807 2023-05-02 18:10:35.000000 flipside-2.0.1/src/models/compass/core/query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)       89 2023-05-02 18:10:35.000000 flipside-2.0.1/src/models/compass/core/result_format.py
+-rw-r--r--   0 jim        (501) staff       (20)      149 2023-05-02 18:10:35.000000 flipside-2.0.1/src/models/compass/core/rpc_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      198 2023-05-02 18:10:35.000000 flipside-2.0.1/src/models/compass/core/rpc_request.py
+-rw-r--r--   0 jim        (501) staff       (20)      252 2023-05-02 18:10:35.000000 flipside-2.0.1/src/models/compass/core/rpc_response.py
+-rw-r--r--   0 jim        (501) staff       (20)      340 2023-05-02 18:10:35.000000 flipside-2.0.1/src/models/compass/core/sql_statement.py
+-rw-r--r--   0 jim        (501) staff       (20)      221 2023-05-02 18:10:35.000000 flipside-2.0.1/src/models/compass/core/tags.py
+-rw-r--r--   0 jim        (501) staff       (20)      845 2023-05-02 18:10:35.000000 flipside-2.0.1/src/models/compass/create_query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)      639 2023-05-02 18:10:35.000000 flipside-2.0.1/src/models/compass/get_query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)     2026 2023-05-02 18:10:35.000000 flipside-2.0.1/src/models/compass/get_query_run_results.py
+-rw-r--r--   0 jim        (501) staff       (20)      582 2023-05-02 18:10:35.000000 flipside-2.0.1/src/models/compass/get_sql_statement.py
+-rw-r--r--   0 jim        (501) staff       (20)      852 2023-05-02 18:10:35.000000 flipside-2.0.1/src/models/compass/query_results.py
+-rw-r--r--   0 jim        (501) staff       (20)     1422 2023-05-02 18:10:35.000000 flipside-2.0.1/src/models/query.py
+-rw-r--r--   0 jim        (501) staff       (20)      836 2023-05-02 18:10:35.000000 flipside-2.0.1/src/models/query_defaults.py
+-rw-r--r--   0 jim        (501) staff       (20)     1031 2023-05-02 18:10:35.000000 flipside-2.0.1/src/models/query_result_set.py
+-rw-r--r--   0 jim        (501) staff       (20)     1658 2023-05-02 18:10:35.000000 flipside-2.0.1/src/models/query_run_stats.py
+-rw-r--r--   0 jim        (501) staff       (20)      544 2023-05-02 18:10:35.000000 flipside-2.0.1/src/models/query_status.py
+-rw-r--r--   0 jim        (501) staff       (20)      194 2023-05-02 18:10:35.000000 flipside-2.0.1/src/models/sleep_config.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:19:51.296433 flipside-2.0.1/src/tests/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.1/src/tests/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:19:51.296594 flipside-2.0.1/src/tests/integrations/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.1/src/tests/integrations/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:19:51.296965 flipside-2.0.1/src/tests/integrations/query_integration/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.1/src/tests/integrations/query_integration/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     8712 2023-05-02 18:10:35.000000 flipside-2.0.1/src/tests/integrations/query_integration/test_query_compass_integration.py
+-rw-r--r--   0 jim        (501) staff       (20)     3438 2023-05-02 18:10:35.000000 flipside-2.0.1/src/tests/integrations/query_integration/test_query_result_set_builder.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:19:51.299838 flipside-2.0.1/src/tests/models/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.1/src/tests/models/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      931 2023-05-02 18:10:35.000000 flipside-2.0.1/src/tests/models/test_query_status.py
+-rw-r--r--   0 jim        (501) staff       (20)     5218 2023-05-02 18:10:35.000000 flipside-2.0.1/src/tests/test_rpc.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:19:51.300704 flipside-2.0.1/src/tests/utils/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.1/src/tests/utils/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     2242 2023-05-02 18:10:35.000000 flipside-2.0.1/src/tests/utils/test_sleep.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:19:51.301040 flipside-2.0.1/src/utils/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.1/src/utils/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     1966 2023-05-02 18:10:35.000000 flipside-2.0.1/src/utils/sleep.py
```

### Comparing `flipside-2.0.0/LICENSE.txt` & `flipside-2.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `flipside-2.0.0/PKG-INFO` & `flipside-2.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flipside
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

### Comparing `flipside-2.0.0/README.md` & `flipside-2.0.1/README.md`

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

### Comparing `flipside-2.0.0/flipside/errors/api_error.py` & `flipside-2.0.1/flipside/errors/api_error.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.0/flipside/errors/query_run_errors.py` & `flipside-2.0.1/flipside/errors/query_run_errors.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.0/flipside/flipside.py` & `flipside-2.0.1/flipside/flipside.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.0/flipside/integrations/query_integration/compass_query_integration.py` & `flipside-2.0.1/flipside/integrations/query_integration/compass_query_integration.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.0/flipside/integrations/query_integration/query_result_set_builder.py` & `flipside-2.0.1/flipside/integrations/query_integration/query_result_set_builder.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.0/flipside/models/compass/cancel_query_run.py` & `flipside-2.0.1/flipside/models/compass/cancel_query_run.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.0/flipside/models/compass/core/query_run.py` & `flipside-2.0.1/flipside/models/compass/core/query_run.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.0/flipside/models/compass/create_query_run.py` & `flipside-2.0.1/flipside/models/compass/create_query_run.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.0/flipside/models/compass/get_query_run.py` & `flipside-2.0.1/flipside/models/compass/get_query_run.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.0/flipside/models/compass/get_query_run_results.py` & `flipside-2.0.1/flipside/models/compass/get_query_run_results.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.0/flipside/models/compass/get_sql_statement.py` & `flipside-2.0.1/flipside/models/compass/get_sql_statement.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.0/flipside/models/compass/query_results.py` & `flipside-2.0.1/flipside/models/compass/query_results.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.0/flipside/models/query.py` & `flipside-2.0.1/flipside/models/query.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.0/flipside/models/query_defaults.py` & `flipside-2.0.1/flipside/models/query_defaults.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.0/flipside/models/query_result_set.py` & `flipside-2.0.1/flipside/models/query_result_set.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.0/flipside/models/query_run_stats.py` & `flipside-2.0.1/flipside/models/query_run_stats.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.0/flipside/models/query_status.py` & `flipside-2.0.1/flipside/models/query_status.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.0/flipside/rpc.py` & `flipside-2.0.1/flipside/rpc.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.0/flipside/tests/integrations/query_integration/test_query_compass_integration.py` & `flipside-2.0.1/flipside/tests/integrations/query_integration/test_query_compass_integration.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.0/flipside/tests/integrations/query_integration/test_query_result_set_builder.py` & `flipside-2.0.1/flipside/tests/integrations/query_integration/test_query_result_set_builder.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.0/flipside/tests/models/test_query_status.py` & `flipside-2.0.1/flipside/tests/models/test_query_status.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.0/flipside/tests/test_rpc.py` & `flipside-2.0.1/flipside/tests/test_rpc.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.0/flipside/tests/utils/test_sleep.py` & `flipside-2.0.1/flipside/tests/utils/test_sleep.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.0/flipside/utils/sleep.py` & `flipside-2.0.1/flipside/utils/sleep.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.0/flipside.egg-info/PKG-INFO` & `flipside-2.0.1/flipside.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flipside
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

### Comparing `flipside-2.0.0/flipside.egg-info/SOURCES.txt` & `flipside-2.0.1/flipside.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flipside-2.0.0/setup.py` & `flipside-2.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.0/src/errors/api_error.py` & `flipside-2.0.1/src/errors/api_error.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.0/src/errors/query_run_errors.py` & `flipside-2.0.1/src/errors/query_run_errors.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.0/src/integrations/query_integration/compass_query_integration.py` & `flipside-2.0.1/src/integrations/query_integration/compass_query_integration.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.0/src/integrations/query_integration/query_result_set_builder.py` & `flipside-2.0.1/src/integrations/query_integration/query_result_set_builder.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.0/src/models/compass/cancel_query_run.py` & `flipside-2.0.1/src/models/compass/cancel_query_run.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.0/src/models/compass/core/query_run.py` & `flipside-2.0.1/src/models/compass/core/query_run.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.0/src/models/compass/create_query_run.py` & `flipside-2.0.1/src/models/compass/create_query_run.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.0/src/models/compass/get_query_run.py` & `flipside-2.0.1/src/models/compass/get_query_run.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.0/src/models/compass/get_query_run_results.py` & `flipside-2.0.1/src/models/compass/get_query_run_results.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.0/src/models/compass/get_sql_statement.py` & `flipside-2.0.1/src/models/compass/get_sql_statement.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.0/src/models/compass/query_results.py` & `flipside-2.0.1/src/models/compass/query_results.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.0/src/models/query.py` & `flipside-2.0.1/src/models/query.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.0/src/models/query_defaults.py` & `flipside-2.0.1/src/models/query_defaults.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.0/src/models/query_result_set.py` & `flipside-2.0.1/src/models/query_result_set.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.0/src/models/query_run_stats.py` & `flipside-2.0.1/src/models/query_run_stats.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.0/src/models/query_status.py` & `flipside-2.0.1/src/models/query_status.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.0/src/tests/integrations/query_integration/test_query_compass_integration.py` & `flipside-2.0.1/src/tests/integrations/query_integration/test_query_compass_integration.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.0/src/tests/integrations/query_integration/test_query_result_set_builder.py` & `flipside-2.0.1/src/tests/integrations/query_integration/test_query_result_set_builder.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.0/src/tests/models/test_query_status.py` & `flipside-2.0.1/src/tests/models/test_query_status.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.0/src/tests/test_rpc.py` & `flipside-2.0.1/src/tests/test_rpc.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.0/src/tests/utils/test_sleep.py` & `flipside-2.0.1/src/tests/utils/test_sleep.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.0/src/utils/sleep.py` & `flipside-2.0.1/src/utils/sleep.py`

 * *Files identical despite different names*

