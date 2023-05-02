# Comparing `tmp/flipside-2.0.2.tar.gz` & `tmp/flipside-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flipside-2.0.2.tar", last modified: Tue May  2 18:41:54 2023, max compression
+gzip compressed data, was "flipside-2.0.3.tar", last modified: Tue May  2 20:14:59 2023, max compression
```

## Comparing `flipside-2.0.2.tar` & `flipside-2.0.3.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:41:54.888745 flipside-2.0.2/
--rw-r--r--   0 jim        (501) staff       (20)     1073 2022-07-25 21:42:15.000000 flipside-2.0.2/LICENSE.txt
--rw-r--r--   0 jim        (501) staff       (20)       69 2022-07-25 21:42:15.000000 flipside-2.0.2/MANIFEST.in
--rw-r--r--   0 jim        (501) staff       (20)     1510 2023-05-02 18:41:54.888843 flipside-2.0.2/PKG-INFO
--rw-r--r--   0 jim        (501) staff       (20)      709 2023-05-02 18:18:58.000000 flipside-2.0.2/README.md
--rw-r--r--   0 jim        (501) staff       (20)        5 2023-05-02 18:39:27.000000 flipside-2.0.2/VERSION
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:41:54.860418 flipside-2.0.2/flipside/
--rw-r--r--   0 jim        (501) staff       (20)      147 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:41:54.861709 flipside-2.0.2/flipside/errors/
--rw-r--r--   0 jim        (501) staff       (20)      336 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside/errors/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     1583 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside/errors/api_error.py
--rw-r--r--   0 jim        (501) staff       (20)      121 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside/errors/base_error.py
--rw-r--r--   0 jim        (501) staff       (20)     2077 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside/errors/query_run_errors.py
--rw-r--r--   0 jim        (501) staff       (20)      262 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside/errors/sdk_error.py
--rw-r--r--   0 jim        (501) staff       (20)      361 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside/errors/server_error.py
--rw-r--r--   0 jim        (501) staff       (20)     2766 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside/flipside.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:41:54.861836 flipside-2.0.2/flipside/integrations/
--rw-r--r--   0 jim        (501) staff       (20)       69 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside/integrations/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:41:54.862323 flipside-2.0.2/flipside/integrations/query_integration/
--rw-r--r--   0 jim        (501) staff       (20)       77 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside/integrations/query_integration/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     9884 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside/integrations/query_integration/compass_query_integration.py
--rw-r--r--   0 jim        (501) staff       (20)      237 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside/integrations/query_integration/defaults.py
--rw-r--r--   0 jim        (501) staff       (20)     3570 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside/integrations/query_integration/query_result_set_builder.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:41:54.863944 flipside-2.0.2/flipside/models/
--rw-r--r--   0 jim        (501) staff       (20)      365 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside/models/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:41:54.864800 flipside-2.0.2/flipside/models/compass/
--rw-r--r--   0 jim        (501) staff       (20)       50 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside/models/compass/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      571 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside/models/compass/cancel_query_run.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:41:54.868593 flipside-2.0.2/flipside/models/compass/core/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside/models/compass/core/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      187 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside/models/compass/core/column_metadata.py
--rw-r--r--   0 jim        (501) staff       (20)      117 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside/models/compass/core/page.py
--rw-r--r--   0 jim        (501) staff       (20)      183 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside/models/compass/core/page_stats.py
--rw-r--r--   0 jim        (501) staff       (20)      358 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside/models/compass/core/query_request.py
--rw-r--r--   0 jim        (501) staff       (20)      807 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside/models/compass/core/query_run.py
--rw-r--r--   0 jim        (501) staff       (20)       89 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside/models/compass/core/result_format.py
--rw-r--r--   0 jim        (501) staff       (20)      149 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside/models/compass/core/rpc_error.py
--rw-r--r--   0 jim        (501) staff       (20)      198 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside/models/compass/core/rpc_request.py
--rw-r--r--   0 jim        (501) staff       (20)      252 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside/models/compass/core/rpc_response.py
--rw-r--r--   0 jim        (501) staff       (20)      340 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside/models/compass/core/sql_statement.py
--rw-r--r--   0 jim        (501) staff       (20)      221 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside/models/compass/core/tags.py
--rw-r--r--   0 jim        (501) staff       (20)      845 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside/models/compass/create_query_run.py
--rw-r--r--   0 jim        (501) staff       (20)      639 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside/models/compass/get_query_run.py
--rw-r--r--   0 jim        (501) staff       (20)     2026 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside/models/compass/get_query_run_results.py
--rw-r--r--   0 jim        (501) staff       (20)      582 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside/models/compass/get_sql_statement.py
--rw-r--r--   0 jim        (501) staff       (20)      852 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside/models/compass/query_results.py
--rw-r--r--   0 jim        (501) staff       (20)     1422 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside/models/query.py
--rw-r--r--   0 jim        (501) staff       (20)      836 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside/models/query_defaults.py
--rw-r--r--   0 jim        (501) staff       (20)     1031 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside/models/query_result_set.py
--rw-r--r--   0 jim        (501) staff       (20)     1658 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside/models/query_run_stats.py
--rw-r--r--   0 jim        (501) staff       (20)      544 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside/models/query_status.py
--rw-r--r--   0 jim        (501) staff       (20)      194 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside/models/sleep_config.py
--rw-r--r--   0 jim        (501) staff       (20)     5898 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside/rpc.py
--rw-r--r--   0 jim        (501) staff       (20)       68 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside/shroomdk.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:41:54.868788 flipside-2.0.2/flipside/tests/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside/tests/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:41:54.868907 flipside-2.0.2/flipside/tests/integrations/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside/tests/integrations/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:41:54.869238 flipside-2.0.2/flipside/tests/integrations/query_integration/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside/tests/integrations/query_integration/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     8712 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside/tests/integrations/query_integration/test_query_compass_integration.py
--rw-r--r--   0 jim        (501) staff       (20)     3438 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside/tests/integrations/query_integration/test_query_result_set_builder.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:41:54.869465 flipside-2.0.2/flipside/tests/models/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside/tests/models/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      931 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside/tests/models/test_query_status.py
--rw-r--r--   0 jim        (501) staff       (20)     5218 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside/tests/test_rpc.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:41:54.869663 flipside-2.0.2/flipside/tests/utils/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside/tests/utils/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     2242 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside/tests/utils/test_sleep.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:41:54.870820 flipside-2.0.2/flipside/utils/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside/utils/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     1966 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside/utils/sleep.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:41:54.861034 flipside-2.0.2/flipside.egg-info/
--rw-r--r--   0 jim        (501) staff       (20)     1510 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside.egg-info/PKG-INFO
--rw-r--r--   0 jim        (501) staff       (20)     4101 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside.egg-info/SOURCES.txt
--rw-r--r--   0 jim        (501) staff       (20)        1 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside.egg-info/dependency_links.txt
--rw-r--r--   0 jim        (501) staff       (20)       34 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside.egg-info/requires.txt
--rw-r--r--   0 jim        (501) staff       (20)       13 2023-05-02 18:41:54.000000 flipside-2.0.2/flipside.egg-info/top_level.txt
--rw-r--r--   0 jim        (501) staff       (20)       30 2022-07-25 21:42:15.000000 flipside-2.0.2/requirements-dev.txt
--rw-r--r--   0 jim        (501) staff       (20)       33 2023-05-02 18:10:35.000000 flipside-2.0.2/requirements.txt
--rw-r--r--   0 jim        (501) staff       (20)       79 2023-05-02 18:41:54.891113 flipside-2.0.2/setup.cfg
--rw-r--r--   0 jim        (501) staff       (20)     1557 2023-05-02 18:10:35.000000 flipside-2.0.2/setup.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:41:54.855302 flipside-2.0.2/src/
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:41:54.872152 flipside-2.0.2/src/errors/
--rw-r--r--   0 jim        (501) staff       (20)      336 2023-05-02 18:10:35.000000 flipside-2.0.2/src/errors/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     1583 2023-05-02 18:10:35.000000 flipside-2.0.2/src/errors/api_error.py
--rw-r--r--   0 jim        (501) staff       (20)      121 2023-05-02 18:10:35.000000 flipside-2.0.2/src/errors/base_error.py
--rw-r--r--   0 jim        (501) staff       (20)     2077 2023-05-02 18:10:35.000000 flipside-2.0.2/src/errors/query_run_errors.py
--rw-r--r--   0 jim        (501) staff       (20)      262 2023-05-02 18:10:35.000000 flipside-2.0.2/src/errors/sdk_error.py
--rw-r--r--   0 jim        (501) staff       (20)      361 2023-05-02 18:10:35.000000 flipside-2.0.2/src/errors/server_error.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:41:54.872305 flipside-2.0.2/src/integrations/
--rw-r--r--   0 jim        (501) staff       (20)       69 2023-05-02 18:10:35.000000 flipside-2.0.2/src/integrations/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:41:54.872875 flipside-2.0.2/src/integrations/query_integration/
--rw-r--r--   0 jim        (501) staff       (20)       77 2023-05-02 18:10:35.000000 flipside-2.0.2/src/integrations/query_integration/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     9884 2023-05-02 18:10:35.000000 flipside-2.0.2/src/integrations/query_integration/compass_query_integration.py
--rw-r--r--   0 jim        (501) staff       (20)      237 2023-05-02 18:10:35.000000 flipside-2.0.2/src/integrations/query_integration/defaults.py
--rw-r--r--   0 jim        (501) staff       (20)     3570 2023-05-02 18:10:35.000000 flipside-2.0.2/src/integrations/query_integration/query_result_set_builder.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:41:54.878671 flipside-2.0.2/src/models/
--rw-r--r--   0 jim        (501) staff       (20)      365 2023-05-02 18:10:35.000000 flipside-2.0.2/src/models/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:41:54.880093 flipside-2.0.2/src/models/compass/
--rw-r--r--   0 jim        (501) staff       (20)       50 2023-05-02 18:10:35.000000 flipside-2.0.2/src/models/compass/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      571 2023-05-02 18:10:35.000000 flipside-2.0.2/src/models/compass/cancel_query_run.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:41:54.884307 flipside-2.0.2/src/models/compass/core/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.2/src/models/compass/core/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      187 2023-05-02 18:10:35.000000 flipside-2.0.2/src/models/compass/core/column_metadata.py
--rw-r--r--   0 jim        (501) staff       (20)      117 2023-05-02 18:10:35.000000 flipside-2.0.2/src/models/compass/core/page.py
--rw-r--r--   0 jim        (501) staff       (20)      183 2023-05-02 18:10:35.000000 flipside-2.0.2/src/models/compass/core/page_stats.py
--rw-r--r--   0 jim        (501) staff       (20)      358 2023-05-02 18:10:35.000000 flipside-2.0.2/src/models/compass/core/query_request.py
--rw-r--r--   0 jim        (501) staff       (20)      807 2023-05-02 18:10:35.000000 flipside-2.0.2/src/models/compass/core/query_run.py
--rw-r--r--   0 jim        (501) staff       (20)       89 2023-05-02 18:10:35.000000 flipside-2.0.2/src/models/compass/core/result_format.py
--rw-r--r--   0 jim        (501) staff       (20)      149 2023-05-02 18:10:35.000000 flipside-2.0.2/src/models/compass/core/rpc_error.py
--rw-r--r--   0 jim        (501) staff       (20)      198 2023-05-02 18:10:35.000000 flipside-2.0.2/src/models/compass/core/rpc_request.py
--rw-r--r--   0 jim        (501) staff       (20)      252 2023-05-02 18:10:35.000000 flipside-2.0.2/src/models/compass/core/rpc_response.py
--rw-r--r--   0 jim        (501) staff       (20)      340 2023-05-02 18:10:35.000000 flipside-2.0.2/src/models/compass/core/sql_statement.py
--rw-r--r--   0 jim        (501) staff       (20)      221 2023-05-02 18:10:35.000000 flipside-2.0.2/src/models/compass/core/tags.py
--rw-r--r--   0 jim        (501) staff       (20)      845 2023-05-02 18:10:35.000000 flipside-2.0.2/src/models/compass/create_query_run.py
--rw-r--r--   0 jim        (501) staff       (20)      639 2023-05-02 18:10:35.000000 flipside-2.0.2/src/models/compass/get_query_run.py
--rw-r--r--   0 jim        (501) staff       (20)     2026 2023-05-02 18:10:35.000000 flipside-2.0.2/src/models/compass/get_query_run_results.py
--rw-r--r--   0 jim        (501) staff       (20)      582 2023-05-02 18:10:35.000000 flipside-2.0.2/src/models/compass/get_sql_statement.py
--rw-r--r--   0 jim        (501) staff       (20)      852 2023-05-02 18:10:35.000000 flipside-2.0.2/src/models/compass/query_results.py
--rw-r--r--   0 jim        (501) staff       (20)     1422 2023-05-02 18:10:35.000000 flipside-2.0.2/src/models/query.py
--rw-r--r--   0 jim        (501) staff       (20)      836 2023-05-02 18:10:35.000000 flipside-2.0.2/src/models/query_defaults.py
--rw-r--r--   0 jim        (501) staff       (20)     1031 2023-05-02 18:10:35.000000 flipside-2.0.2/src/models/query_result_set.py
--rw-r--r--   0 jim        (501) staff       (20)     1658 2023-05-02 18:10:35.000000 flipside-2.0.2/src/models/query_run_stats.py
--rw-r--r--   0 jim        (501) staff       (20)      544 2023-05-02 18:10:35.000000 flipside-2.0.2/src/models/query_status.py
--rw-r--r--   0 jim        (501) staff       (20)      194 2023-05-02 18:10:35.000000 flipside-2.0.2/src/models/sleep_config.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:41:54.884501 flipside-2.0.2/src/tests/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.2/src/tests/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:41:54.884620 flipside-2.0.2/src/tests/integrations/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.2/src/tests/integrations/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:41:54.884923 flipside-2.0.2/src/tests/integrations/query_integration/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.2/src/tests/integrations/query_integration/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     8712 2023-05-02 18:10:35.000000 flipside-2.0.2/src/tests/integrations/query_integration/test_query_compass_integration.py
--rw-r--r--   0 jim        (501) staff       (20)     3438 2023-05-02 18:10:35.000000 flipside-2.0.2/src/tests/integrations/query_integration/test_query_result_set_builder.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:41:54.885122 flipside-2.0.2/src/tests/models/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.2/src/tests/models/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      931 2023-05-02 18:10:35.000000 flipside-2.0.2/src/tests/models/test_query_status.py
--rw-r--r--   0 jim        (501) staff       (20)     5218 2023-05-02 18:10:35.000000 flipside-2.0.2/src/tests/test_rpc.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:41:54.887924 flipside-2.0.2/src/tests/utils/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.2/src/tests/utils/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     2242 2023-05-02 18:10:35.000000 flipside-2.0.2/src/tests/utils/test_sleep.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 18:41:54.888335 flipside-2.0.2/src/utils/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.2/src/utils/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     1966 2023-05-02 18:10:35.000000 flipside-2.0.2/src/utils/sleep.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:14:59.361373 flipside-2.0.3/
+-rw-r--r--   0 jim        (501) staff       (20)     1073 2022-07-25 21:42:15.000000 flipside-2.0.3/LICENSE.txt
+-rw-r--r--   0 jim        (501) staff       (20)       69 2022-07-25 21:42:15.000000 flipside-2.0.3/MANIFEST.in
+-rw-r--r--   0 jim        (501) staff       (20)     1510 2023-05-02 20:14:59.361450 flipside-2.0.3/PKG-INFO
+-rw-r--r--   0 jim        (501) staff       (20)      709 2023-05-02 18:18:58.000000 flipside-2.0.3/README.md
+-rw-r--r--   0 jim        (501) staff       (20)        5 2023-05-02 20:14:01.000000 flipside-2.0.3/VERSION
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:14:59.344771 flipside-2.0.3/flipside/
+-rw-r--r--   0 jim        (501) staff       (20)      147 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:14:59.346304 flipside-2.0.3/flipside/errors/
+-rw-r--r--   0 jim        (501) staff       (20)      336 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside/errors/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     1583 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside/errors/api_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      121 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside/errors/base_error.py
+-rw-r--r--   0 jim        (501) staff       (20)     2077 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside/errors/query_run_errors.py
+-rw-r--r--   0 jim        (501) staff       (20)      262 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside/errors/sdk_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      361 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside/errors/server_error.py
+-rw-r--r--   0 jim        (501) staff       (20)     2968 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside/flipside.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:14:59.346425 flipside-2.0.3/flipside/integrations/
+-rw-r--r--   0 jim        (501) staff       (20)       69 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside/integrations/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:14:59.346926 flipside-2.0.3/flipside/integrations/query_integration/
+-rw-r--r--   0 jim        (501) staff       (20)       77 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside/integrations/query_integration/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     9884 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside/integrations/query_integration/compass_query_integration.py
+-rw-r--r--   0 jim        (501) staff       (20)      237 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside/integrations/query_integration/defaults.py
+-rw-r--r--   0 jim        (501) staff       (20)     3570 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside/integrations/query_integration/query_result_set_builder.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:14:59.347794 flipside-2.0.3/flipside/models/
+-rw-r--r--   0 jim        (501) staff       (20)      365 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside/models/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:14:59.348773 flipside-2.0.3/flipside/models/compass/
+-rw-r--r--   0 jim        (501) staff       (20)       50 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside/models/compass/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      571 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside/models/compass/cancel_query_run.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:14:59.350828 flipside-2.0.3/flipside/models/compass/core/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside/models/compass/core/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      187 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside/models/compass/core/column_metadata.py
+-rw-r--r--   0 jim        (501) staff       (20)      117 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside/models/compass/core/page.py
+-rw-r--r--   0 jim        (501) staff       (20)      183 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside/models/compass/core/page_stats.py
+-rw-r--r--   0 jim        (501) staff       (20)      358 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside/models/compass/core/query_request.py
+-rw-r--r--   0 jim        (501) staff       (20)      807 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside/models/compass/core/query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)       89 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside/models/compass/core/result_format.py
+-rw-r--r--   0 jim        (501) staff       (20)      149 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside/models/compass/core/rpc_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      198 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside/models/compass/core/rpc_request.py
+-rw-r--r--   0 jim        (501) staff       (20)      252 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside/models/compass/core/rpc_response.py
+-rw-r--r--   0 jim        (501) staff       (20)      340 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside/models/compass/core/sql_statement.py
+-rw-r--r--   0 jim        (501) staff       (20)      221 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside/models/compass/core/tags.py
+-rw-r--r--   0 jim        (501) staff       (20)      845 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside/models/compass/create_query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)      639 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside/models/compass/get_query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)     2026 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside/models/compass/get_query_run_results.py
+-rw-r--r--   0 jim        (501) staff       (20)      582 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside/models/compass/get_sql_statement.py
+-rw-r--r--   0 jim        (501) staff       (20)      852 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside/models/compass/query_results.py
+-rw-r--r--   0 jim        (501) staff       (20)     1422 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside/models/query.py
+-rw-r--r--   0 jim        (501) staff       (20)      836 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside/models/query_defaults.py
+-rw-r--r--   0 jim        (501) staff       (20)     1031 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside/models/query_result_set.py
+-rw-r--r--   0 jim        (501) staff       (20)     1658 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside/models/query_run_stats.py
+-rw-r--r--   0 jim        (501) staff       (20)      544 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside/models/query_status.py
+-rw-r--r--   0 jim        (501) staff       (20)      194 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside/models/sleep_config.py
+-rw-r--r--   0 jim        (501) staff       (20)     5898 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside/rpc.py
+-rw-r--r--   0 jim        (501) staff       (20)       68 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside/shroomdk.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:14:59.351056 flipside-2.0.3/flipside/tests/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside/tests/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:14:59.351191 flipside-2.0.3/flipside/tests/integrations/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside/tests/integrations/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:14:59.351543 flipside-2.0.3/flipside/tests/integrations/query_integration/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside/tests/integrations/query_integration/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     8712 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside/tests/integrations/query_integration/test_query_compass_integration.py
+-rw-r--r--   0 jim        (501) staff       (20)     3438 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside/tests/integrations/query_integration/test_query_result_set_builder.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:14:59.351789 flipside-2.0.3/flipside/tests/models/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside/tests/models/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      931 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside/tests/models/test_query_status.py
+-rw-r--r--   0 jim        (501) staff       (20)     5218 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside/tests/test_rpc.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:14:59.352002 flipside-2.0.3/flipside/tests/utils/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside/tests/utils/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     2242 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside/tests/utils/test_sleep.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:14:59.352211 flipside-2.0.3/flipside/utils/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside/utils/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     1966 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside/utils/sleep.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:14:59.345452 flipside-2.0.3/flipside.egg-info/
+-rw-r--r--   0 jim        (501) staff       (20)     1510 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside.egg-info/PKG-INFO
+-rw-r--r--   0 jim        (501) staff       (20)     4101 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside.egg-info/SOURCES.txt
+-rw-r--r--   0 jim        (501) staff       (20)        1 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside.egg-info/dependency_links.txt
+-rw-r--r--   0 jim        (501) staff       (20)       34 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside.egg-info/requires.txt
+-rw-r--r--   0 jim        (501) staff       (20)       13 2023-05-02 20:14:59.000000 flipside-2.0.3/flipside.egg-info/top_level.txt
+-rw-r--r--   0 jim        (501) staff       (20)       30 2022-07-25 21:42:15.000000 flipside-2.0.3/requirements-dev.txt
+-rw-r--r--   0 jim        (501) staff       (20)       33 2023-05-02 18:10:35.000000 flipside-2.0.3/requirements.txt
+-rw-r--r--   0 jim        (501) staff       (20)       79 2023-05-02 20:14:59.361829 flipside-2.0.3/setup.cfg
+-rw-r--r--   0 jim        (501) staff       (20)     1557 2023-05-02 18:10:35.000000 flipside-2.0.3/setup.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:14:59.342268 flipside-2.0.3/src/
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:14:59.352941 flipside-2.0.3/src/errors/
+-rw-r--r--   0 jim        (501) staff       (20)      336 2023-05-02 18:10:35.000000 flipside-2.0.3/src/errors/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     1583 2023-05-02 18:10:35.000000 flipside-2.0.3/src/errors/api_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      121 2023-05-02 18:10:35.000000 flipside-2.0.3/src/errors/base_error.py
+-rw-r--r--   0 jim        (501) staff       (20)     2077 2023-05-02 18:10:35.000000 flipside-2.0.3/src/errors/query_run_errors.py
+-rw-r--r--   0 jim        (501) staff       (20)      262 2023-05-02 18:10:35.000000 flipside-2.0.3/src/errors/sdk_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      361 2023-05-02 18:10:35.000000 flipside-2.0.3/src/errors/server_error.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:14:59.353067 flipside-2.0.3/src/integrations/
+-rw-r--r--   0 jim        (501) staff       (20)       69 2023-05-02 18:10:35.000000 flipside-2.0.3/src/integrations/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:14:59.353963 flipside-2.0.3/src/integrations/query_integration/
+-rw-r--r--   0 jim        (501) staff       (20)       77 2023-05-02 18:10:35.000000 flipside-2.0.3/src/integrations/query_integration/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     9884 2023-05-02 18:10:35.000000 flipside-2.0.3/src/integrations/query_integration/compass_query_integration.py
+-rw-r--r--   0 jim        (501) staff       (20)      237 2023-05-02 18:10:35.000000 flipside-2.0.3/src/integrations/query_integration/defaults.py
+-rw-r--r--   0 jim        (501) staff       (20)     3570 2023-05-02 18:10:35.000000 flipside-2.0.3/src/integrations/query_integration/query_result_set_builder.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:14:59.355047 flipside-2.0.3/src/models/
+-rw-r--r--   0 jim        (501) staff       (20)      365 2023-05-02 18:10:35.000000 flipside-2.0.3/src/models/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:14:59.356153 flipside-2.0.3/src/models/compass/
+-rw-r--r--   0 jim        (501) staff       (20)       50 2023-05-02 18:10:35.000000 flipside-2.0.3/src/models/compass/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      571 2023-05-02 18:10:35.000000 flipside-2.0.3/src/models/compass/cancel_query_run.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:14:59.357988 flipside-2.0.3/src/models/compass/core/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.3/src/models/compass/core/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      187 2023-05-02 18:10:35.000000 flipside-2.0.3/src/models/compass/core/column_metadata.py
+-rw-r--r--   0 jim        (501) staff       (20)      117 2023-05-02 18:10:35.000000 flipside-2.0.3/src/models/compass/core/page.py
+-rw-r--r--   0 jim        (501) staff       (20)      183 2023-05-02 18:10:35.000000 flipside-2.0.3/src/models/compass/core/page_stats.py
+-rw-r--r--   0 jim        (501) staff       (20)      358 2023-05-02 18:10:35.000000 flipside-2.0.3/src/models/compass/core/query_request.py
+-rw-r--r--   0 jim        (501) staff       (20)      807 2023-05-02 18:10:35.000000 flipside-2.0.3/src/models/compass/core/query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)       89 2023-05-02 18:10:35.000000 flipside-2.0.3/src/models/compass/core/result_format.py
+-rw-r--r--   0 jim        (501) staff       (20)      149 2023-05-02 18:10:35.000000 flipside-2.0.3/src/models/compass/core/rpc_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      198 2023-05-02 18:10:35.000000 flipside-2.0.3/src/models/compass/core/rpc_request.py
+-rw-r--r--   0 jim        (501) staff       (20)      252 2023-05-02 18:10:35.000000 flipside-2.0.3/src/models/compass/core/rpc_response.py
+-rw-r--r--   0 jim        (501) staff       (20)      340 2023-05-02 18:10:35.000000 flipside-2.0.3/src/models/compass/core/sql_statement.py
+-rw-r--r--   0 jim        (501) staff       (20)      221 2023-05-02 18:10:35.000000 flipside-2.0.3/src/models/compass/core/tags.py
+-rw-r--r--   0 jim        (501) staff       (20)      845 2023-05-02 18:10:35.000000 flipside-2.0.3/src/models/compass/create_query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)      639 2023-05-02 18:10:35.000000 flipside-2.0.3/src/models/compass/get_query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)     2026 2023-05-02 18:10:35.000000 flipside-2.0.3/src/models/compass/get_query_run_results.py
+-rw-r--r--   0 jim        (501) staff       (20)      582 2023-05-02 18:10:35.000000 flipside-2.0.3/src/models/compass/get_sql_statement.py
+-rw-r--r--   0 jim        (501) staff       (20)      852 2023-05-02 18:10:35.000000 flipside-2.0.3/src/models/compass/query_results.py
+-rw-r--r--   0 jim        (501) staff       (20)     1422 2023-05-02 18:10:35.000000 flipside-2.0.3/src/models/query.py
+-rw-r--r--   0 jim        (501) staff       (20)      836 2023-05-02 18:10:35.000000 flipside-2.0.3/src/models/query_defaults.py
+-rw-r--r--   0 jim        (501) staff       (20)     1031 2023-05-02 18:10:35.000000 flipside-2.0.3/src/models/query_result_set.py
+-rw-r--r--   0 jim        (501) staff       (20)     1658 2023-05-02 18:10:35.000000 flipside-2.0.3/src/models/query_run_stats.py
+-rw-r--r--   0 jim        (501) staff       (20)      544 2023-05-02 18:10:35.000000 flipside-2.0.3/src/models/query_status.py
+-rw-r--r--   0 jim        (501) staff       (20)      194 2023-05-02 18:10:35.000000 flipside-2.0.3/src/models/sleep_config.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:14:59.358202 flipside-2.0.3/src/tests/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.3/src/tests/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:14:59.358345 flipside-2.0.3/src/tests/integrations/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.3/src/tests/integrations/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:14:59.358804 flipside-2.0.3/src/tests/integrations/query_integration/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.3/src/tests/integrations/query_integration/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     8712 2023-05-02 18:10:35.000000 flipside-2.0.3/src/tests/integrations/query_integration/test_query_compass_integration.py
+-rw-r--r--   0 jim        (501) staff       (20)     3438 2023-05-02 18:10:35.000000 flipside-2.0.3/src/tests/integrations/query_integration/test_query_result_set_builder.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:14:59.359037 flipside-2.0.3/src/tests/models/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.3/src/tests/models/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      931 2023-05-02 18:10:35.000000 flipside-2.0.3/src/tests/models/test_query_status.py
+-rw-r--r--   0 jim        (501) staff       (20)     5218 2023-05-02 18:10:35.000000 flipside-2.0.3/src/tests/test_rpc.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:14:59.359248 flipside-2.0.3/src/tests/utils/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.3/src/tests/utils/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     2242 2023-05-02 18:10:35.000000 flipside-2.0.3/src/tests/utils/test_sleep.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:14:59.361207 flipside-2.0.3/src/utils/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.3/src/utils/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     1966 2023-05-02 18:10:35.000000 flipside-2.0.3/src/utils/sleep.py
```

### Comparing `flipside-2.0.2/LICENSE.txt` & `flipside-2.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `flipside-2.0.2/PKG-INFO` & `flipside-2.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flipside
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

### Comparing `flipside-2.0.2/README.md` & `flipside-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `flipside-2.0.2/flipside/errors/api_error.py` & `flipside-2.0.3/flipside/errors/api_error.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.2/flipside/errors/query_run_errors.py` & `flipside-2.0.3/flipside/errors/query_run_errors.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.2/flipside/flipside.py` & `flipside-2.0.3/flipside/flipside.py`

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

### Comparing `flipside-2.0.2/flipside/integrations/query_integration/compass_query_integration.py` & `flipside-2.0.3/flipside/integrations/query_integration/compass_query_integration.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.2/flipside/integrations/query_integration/query_result_set_builder.py` & `flipside-2.0.3/flipside/integrations/query_integration/query_result_set_builder.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.2/flipside/models/compass/cancel_query_run.py` & `flipside-2.0.3/flipside/models/compass/cancel_query_run.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.2/flipside/models/compass/core/query_run.py` & `flipside-2.0.3/flipside/models/compass/core/query_run.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.2/flipside/models/compass/create_query_run.py` & `flipside-2.0.3/flipside/models/compass/create_query_run.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.2/flipside/models/compass/get_query_run.py` & `flipside-2.0.3/flipside/models/compass/get_query_run.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.2/flipside/models/compass/get_query_run_results.py` & `flipside-2.0.3/flipside/models/compass/get_query_run_results.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.2/flipside/models/compass/get_sql_statement.py` & `flipside-2.0.3/flipside/models/compass/get_sql_statement.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.2/flipside/models/compass/query_results.py` & `flipside-2.0.3/flipside/models/compass/query_results.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.2/flipside/models/query.py` & `flipside-2.0.3/flipside/models/query.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.2/flipside/models/query_defaults.py` & `flipside-2.0.3/flipside/models/query_defaults.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.2/flipside/models/query_result_set.py` & `flipside-2.0.3/flipside/models/query_result_set.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.2/flipside/models/query_run_stats.py` & `flipside-2.0.3/flipside/models/query_run_stats.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.2/flipside/models/query_status.py` & `flipside-2.0.3/flipside/models/query_status.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.2/flipside/rpc.py` & `flipside-2.0.3/flipside/rpc.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.2/flipside/tests/integrations/query_integration/test_query_compass_integration.py` & `flipside-2.0.3/flipside/tests/integrations/query_integration/test_query_compass_integration.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.2/flipside/tests/integrations/query_integration/test_query_result_set_builder.py` & `flipside-2.0.3/flipside/tests/integrations/query_integration/test_query_result_set_builder.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.2/flipside/tests/models/test_query_status.py` & `flipside-2.0.3/flipside/tests/models/test_query_status.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.2/flipside/tests/test_rpc.py` & `flipside-2.0.3/flipside/tests/test_rpc.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.2/flipside/tests/utils/test_sleep.py` & `flipside-2.0.3/flipside/tests/utils/test_sleep.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.2/flipside/utils/sleep.py` & `flipside-2.0.3/flipside/utils/sleep.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.2/flipside.egg-info/PKG-INFO` & `flipside-2.0.3/flipside.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flipside
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

### Comparing `flipside-2.0.2/flipside.egg-info/SOURCES.txt` & `flipside-2.0.3/flipside.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flipside-2.0.2/setup.py` & `flipside-2.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.2/src/errors/api_error.py` & `flipside-2.0.3/src/errors/api_error.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.2/src/errors/query_run_errors.py` & `flipside-2.0.3/src/errors/query_run_errors.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.2/src/integrations/query_integration/compass_query_integration.py` & `flipside-2.0.3/src/integrations/query_integration/compass_query_integration.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.2/src/integrations/query_integration/query_result_set_builder.py` & `flipside-2.0.3/src/integrations/query_integration/query_result_set_builder.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.2/src/models/compass/cancel_query_run.py` & `flipside-2.0.3/src/models/compass/cancel_query_run.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.2/src/models/compass/core/query_run.py` & `flipside-2.0.3/src/models/compass/core/query_run.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.2/src/models/compass/create_query_run.py` & `flipside-2.0.3/src/models/compass/create_query_run.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.2/src/models/compass/get_query_run.py` & `flipside-2.0.3/src/models/compass/get_query_run.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.2/src/models/compass/get_query_run_results.py` & `flipside-2.0.3/src/models/compass/get_query_run_results.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.2/src/models/compass/get_sql_statement.py` & `flipside-2.0.3/src/models/compass/get_sql_statement.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.2/src/models/compass/query_results.py` & `flipside-2.0.3/src/models/compass/query_results.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.2/src/models/query.py` & `flipside-2.0.3/src/models/query.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.2/src/models/query_defaults.py` & `flipside-2.0.3/src/models/query_defaults.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.2/src/models/query_result_set.py` & `flipside-2.0.3/src/models/query_result_set.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.2/src/models/query_run_stats.py` & `flipside-2.0.3/src/models/query_run_stats.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.2/src/models/query_status.py` & `flipside-2.0.3/src/models/query_status.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.2/src/tests/integrations/query_integration/test_query_compass_integration.py` & `flipside-2.0.3/src/tests/integrations/query_integration/test_query_compass_integration.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.2/src/tests/integrations/query_integration/test_query_result_set_builder.py` & `flipside-2.0.3/src/tests/integrations/query_integration/test_query_result_set_builder.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.2/src/tests/models/test_query_status.py` & `flipside-2.0.3/src/tests/models/test_query_status.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.2/src/tests/test_rpc.py` & `flipside-2.0.3/src/tests/test_rpc.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.2/src/tests/utils/test_sleep.py` & `flipside-2.0.3/src/tests/utils/test_sleep.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.2/src/utils/sleep.py` & `flipside-2.0.3/src/utils/sleep.py`

 * *Files identical despite different names*

