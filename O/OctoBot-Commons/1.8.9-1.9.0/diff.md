# Comparing `tmp/OctoBot-Commons-1.8.9.tar.gz` & `tmp/OctoBot-Commons-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OctoBot-Commons-1.8.9.tar", last modified: Sat Feb 11 20:39:17 2023, max compression
+gzip compressed data, was "OctoBot-Commons-1.9.0.tar", last modified: Tue May  2 16:30:43 2023, max compression
```

## Comparing `OctoBot-Commons-1.8.9.tar` & `OctoBot-Commons-1.9.0.tar`

### file list

```diff
@@ -1,205 +1,184 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:39:17.759558 OctoBot-Commons-1.8.9/
--rw-r--r--   0 runner    (1001) docker     (123)    17299 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:39:17.739558 OctoBot-Commons-1.8.9/OctoBot_Commons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-02-11 20:39:17.000000 OctoBot-Commons-1.8.9/OctoBot_Commons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-02-11 20:39:17.000000 OctoBot-Commons-1.8.9/OctoBot_Commons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-11 20:39:17.000000 OctoBot-Commons-1.8.9/OctoBot_Commons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-11 20:39:17.000000 OctoBot-Commons-1.8.9/OctoBot_Commons.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-02-11 20:39:17.000000 OctoBot-Commons-1.8.9/OctoBot_Commons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-11 20:39:17.000000 OctoBot-Commons-1.8.9/OctoBot_Commons.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-02-11 20:39:17.759558 OctoBot-Commons-1.8.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:39:17.743558 OctoBot-Commons-1.8.9/octobot_commons/
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/aiohttp_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/async_job.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    10371 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/async_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/asyncio_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/channels_name.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:39:17.743558 OctoBot-Commons-1.8.9/octobot_commons/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6638 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/configuration/config_file_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/configuration/config_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)    11919 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/configuration/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/configuration/fields_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10797 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/configuration/user_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/data_util.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/data_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:39:17.743558 OctoBot-Commons-1.8.9/octobot_commons/databases/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/databases/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/databases/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:39:17.743558 OctoBot-Commons-1.8.9/octobot_commons/databases/bases/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/databases/bases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/databases/bases/base_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/databases/bases/document_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     9482 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/databases/cache_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16509 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/databases/cache_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:39:17.743558 OctoBot-Commons-1.8.9/octobot_commons/databases/database_caches/
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/databases/database_caches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/databases/database_caches/chronological_read_database_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/databases/database_caches/generic_database_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:39:17.743558 OctoBot-Commons-1.8.9/octobot_commons/databases/databases_util/
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/databases/databases_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/databases/databases_util/cache_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:39:17.747558 OctoBot-Commons-1.8.9/octobot_commons/databases/document_database_adaptors/
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/databases/document_database_adaptors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7813 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/databases/document_database_adaptors/abstract_document_database_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11977 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/databases/document_database_adaptors/tinydb_adaptor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:39:17.747558 OctoBot-Commons-1.8.9/octobot_commons/databases/global_storage/
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/databases/global_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/databases/global_storage/global_shared_memory_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:39:17.747558 OctoBot-Commons-1.8.9/octobot_commons/databases/implementations/
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/databases/implementations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/databases/implementations/cache_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/databases/implementations/cache_timestamp_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/databases/implementations/db_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7873 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/databases/implementations/db_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/databases/implementations/db_writer_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/databases/implementations/meta_database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:39:17.747558 OctoBot-Commons-1.8.9/octobot_commons/databases/relational_databases/
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/databases/relational_databases/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/databases/relational_databases/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:39:17.747558 OctoBot-Commons-1.8.9/octobot_commons/databases/relational_databases/sqlite/
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/databases/relational_databases/sqlite/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/databases/relational_databases/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/databases/relational_databases/sqlite/cursor_pool.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/databases/relational_databases/sqlite/cursor_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/databases/relational_databases/sqlite/cursor_wrapper.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/databases/relational_databases/sqlite/cursor_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/databases/relational_databases/sqlite/sqlite_database.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    12692 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/databases/relational_databases/sqlite/sqlite_database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:39:17.747558 OctoBot-Commons-1.8.9/octobot_commons/databases/run_databases/
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/databases/run_databases/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/databases/run_databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/databases/run_databases/abstract_run_databases_pruner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/databases/run_databases/file_system_run_databases_pruner.py
--rw-r--r--   0 runner    (1001) docker     (123)    16252 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/databases/run_databases/run_databases_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/databases/run_databases/run_databases_provider.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/databases/run_databases/run_databases_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/databases/run_databases/run_databases_pruning_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/databases/run_databases/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/databases/run_databases/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/dict_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:39:17.747558 OctoBot-Commons-1.8.9/octobot_commons/display/
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/display/display_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    19813 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/display/display_translator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/display/plot_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     9383 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/evaluator_util.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/evaluators_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/external_resources_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/json_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/list_util.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/list_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:39:17.751558 OctoBot-Commons-1.8.9/octobot_commons/logging/
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/logging/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/logging/logging_util.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     9523 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/logging/logging_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/logical_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/multiprocessing_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/number_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/optimization_campaign.py
--rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/os_clock_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/os_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/pretty_printer.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/pretty_printer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:39:17.751558 OctoBot-Commons-1.8.9/octobot_commons/profiles/
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15995 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/profiles/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9620 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/profiles/profile_sharing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:39:17.751558 OctoBot-Commons-1.8.9/octobot_commons/signals/
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/signals/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/signals/signal_builder_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/signals/signal_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/signals/signal_bundle_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/signals/signal_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/signals/signal_publisher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/signals/signals_emitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:39:17.751558 OctoBot-Commons-1.8.9/octobot_commons/singleton/
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/singleton/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/singleton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/singleton/singleton_class.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/singleton/singleton_class.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/support.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:39:17.751558 OctoBot-Commons-1.8.9/octobot_commons/symbols/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/symbols/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/symbols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/symbols/symbol.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     6948 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/symbols/symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/symbols/symbol_util.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/symbols/symbol_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/system_resources_watcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:39:17.751558 OctoBot-Commons-1.8.9/octobot_commons/tentacles_management/
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/tentacles_management/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/tentacles_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/tentacles_management/abstract_tentacle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/tentacles_management/class_inspector.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/tentacles_management/class_inspector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:39:17.751558 OctoBot-Commons-1.8.9/octobot_commons/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/thread_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/time_frame_manager.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     5164 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/time_frame_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/timestamp_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:39:17.751558 OctoBot-Commons-1.8.9/octobot_commons/tree/
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/tree/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/tree/base_tree.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     9354 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/tree/base_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/tree/event_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/tree/event_tree.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/octobot_commons/tree/event_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-11 20:39:17.759558 OctoBot-Commons-1.8.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:39:17.735558 OctoBot-Commons-1.8.9/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:39:17.751558 OctoBot-Commons-1.8.9/tests/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/tests/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12030 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/tests/configuration/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/tests/configuration/test_fields_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:39:17.751558 OctoBot-Commons-1.8.9/tests/databases/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/tests/databases/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:39:17.751558 OctoBot-Commons-1.8.9/tests/databases/global_storage/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/tests/databases/global_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/tests/databases/global_storage/test_global_shared_memory_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:39:17.751558 OctoBot-Commons-1.8.9/tests/databases/relational_databases/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/tests/databases/relational_databases/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:39:17.755558 OctoBot-Commons-1.8.9/tests/databases/relational_databases/sqlite/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/tests/databases/relational_databases/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11861 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/tests/databases/relational_databases/sqlite/test_sqlite_database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:39:17.755558 OctoBot-Commons-1.8.9/tests/databases/run_databases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/tests/databases/run_databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/tests/databases/run_databases/test_run_databases_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:39:17.755558 OctoBot-Commons-1.8.9/tests/logging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/tests/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/tests/logging/test_logging_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:39:17.755558 OctoBot-Commons-1.8.9/tests/profiles/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/tests/profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15694 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/tests/profiles/test_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9558 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/tests/profiles/test_profile_sharing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:39:17.755558 OctoBot-Commons-1.8.9/tests/signals/
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/tests/signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/tests/signals/test_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/tests/signals/test_signal_builder_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/tests/signals/test_signal_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/tests/signals/test_signal_bundle_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/tests/signals/test_signal_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/tests/signals/test_signal_publisher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:39:17.755558 OctoBot-Commons-1.8.9/tests/symbols/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/tests/symbols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/tests/symbols/test_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/tests/symbols/test_symbol_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:39:17.759558 OctoBot-Commons-1.8.9/tests/tree/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/tests/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/tests/tree/test_base_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-02-11 20:38:56.000000 OctoBot-Commons-1.8.9/tests/tree/test_event_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:30:43.413045 OctoBot-Commons-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    19041 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:30:43.385045 OctoBot-Commons-1.9.0/OctoBot_Commons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-02 16:30:43.000000 OctoBot-Commons-1.9.0/OctoBot_Commons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6307 2023-05-02 16:30:43.000000 OctoBot-Commons-1.9.0/OctoBot_Commons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 16:30:43.000000 OctoBot-Commons-1.9.0/OctoBot_Commons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 16:30:43.000000 OctoBot-Commons-1.9.0/OctoBot_Commons.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-02 16:30:43.000000 OctoBot-Commons-1.9.0/OctoBot_Commons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-02 16:30:43.000000 OctoBot-Commons-1.9.0/OctoBot_Commons.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-02 16:30:43.413045 OctoBot-Commons-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:30:43.389045 OctoBot-Commons-1.9.0/octobot_commons/
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/aiohttp_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10371 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/async_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/asyncio_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/channels_name.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:30:43.389045 OctoBot-Commons-1.9.0/octobot_commons/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6914 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/configuration/config_file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/configuration/config_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12191 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/configuration/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/configuration/fields_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/configuration/user_input_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10797 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/configuration/user_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/data_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:30:43.389045 OctoBot-Commons-1.9.0/octobot_commons/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/databases/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:30:43.389045 OctoBot-Commons-1.9.0/octobot_commons/databases/bases/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/databases/bases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/databases/bases/base_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/databases/bases/document_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9482 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/databases/cache_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16509 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/databases/cache_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:30:43.389045 OctoBot-Commons-1.9.0/octobot_commons/databases/database_caches/
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/databases/database_caches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/databases/database_caches/chronological_read_database_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/databases/database_caches/generic_database_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:30:43.389045 OctoBot-Commons-1.9.0/octobot_commons/databases/databases_util/
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/databases/databases_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/databases/databases_util/cache_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:30:43.393045 OctoBot-Commons-1.9.0/octobot_commons/databases/document_database_adaptors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/databases/document_database_adaptors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7813 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/databases/document_database_adaptors/abstract_document_database_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11991 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/databases/document_database_adaptors/tinydb_adaptor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:30:43.393045 OctoBot-Commons-1.9.0/octobot_commons/databases/global_storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/databases/global_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/databases/global_storage/global_shared_memory_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:30:43.393045 OctoBot-Commons-1.9.0/octobot_commons/databases/implementations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/databases/implementations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/databases/implementations/_exchange_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/databases/implementations/cache_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/databases/implementations/cache_timestamp_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/databases/implementations/db_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7873 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/databases/implementations/db_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/databases/implementations/db_writer_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/databases/implementations/meta_database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:30:43.393045 OctoBot-Commons-1.9.0/octobot_commons/databases/relational_databases/
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/databases/relational_databases/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:30:43.397045 OctoBot-Commons-1.9.0/octobot_commons/databases/relational_databases/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/databases/relational_databases/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/databases/relational_databases/sqlite/cursor_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/databases/relational_databases/sqlite/cursor_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13115 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/databases/relational_databases/sqlite/sqlite_database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:30:43.397045 OctoBot-Commons-1.9.0/octobot_commons/databases/run_databases/
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/databases/run_databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/databases/run_databases/abstract_run_databases_pruner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/databases/run_databases/file_system_run_databases_pruner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16445 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/databases/run_databases/run_databases_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/databases/run_databases/run_databases_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/databases/run_databases/run_databases_pruning_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/databases/run_databases/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/databases/run_databases/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/dict_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:30:43.401045 OctoBot-Commons-1.9.0/octobot_commons/display/
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/display/display_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20532 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/display/display_translator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/display/plot_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12742 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/evaluators_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/external_resources_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/json_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/list_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:30:43.401045 OctoBot-Commons-1.9.0/octobot_commons/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9852 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/logging/logging_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/logical_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/multiprocessing_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/number_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/optimization_campaign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/os_clock_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/os_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11327 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/pretty_printer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:30:43.401045 OctoBot-Commons-1.9.0/octobot_commons/profiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16826 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/profiles/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11913 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/profiles/profile_sharing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:30:43.401045 OctoBot-Commons-1.9.0/octobot_commons/signals/
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/signals/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/signals/signal_builder_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/signals/signal_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/signals/signal_bundle_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/signals/signal_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/signals/signal_publisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/signals/signals_emitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:30:43.401045 OctoBot-Commons-1.9.0/octobot_commons/singleton/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/singleton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/singleton/singleton_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:30:43.405045 OctoBot-Commons-1.9.0/octobot_commons/symbols/
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/symbols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6948 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/symbols/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/symbols/symbol_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/system_resources_watcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:30:43.405045 OctoBot-Commons-1.9.0/octobot_commons/tentacles_management/
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/tentacles_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/tentacles_management/abstract_tentacle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/tentacles_management/class_inspector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:30:43.405045 OctoBot-Commons-1.9.0/octobot_commons/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/thread_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/time_frame_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/timestamp_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:30:43.405045 OctoBot-Commons-1.9.0/octobot_commons/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9354 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/tree/base_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/tree/event_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/octobot_commons/tree/event_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 16:30:43.413045 OctoBot-Commons-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:30:43.381045 OctoBot-Commons-1.9.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:30:43.405045 OctoBot-Commons-1.9.0/tests/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/tests/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12030 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/tests/configuration/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/tests/configuration/test_fields_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:30:43.405045 OctoBot-Commons-1.9.0/tests/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/tests/databases/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:30:43.405045 OctoBot-Commons-1.9.0/tests/databases/global_storage/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/tests/databases/global_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/tests/databases/global_storage/test_global_shared_memory_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:30:43.409045 OctoBot-Commons-1.9.0/tests/databases/relational_databases/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/tests/databases/relational_databases/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:30:43.409045 OctoBot-Commons-1.9.0/tests/databases/relational_databases/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/tests/databases/relational_databases/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13446 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/tests/databases/relational_databases/sqlite/test_sqlite_database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:30:43.409045 OctoBot-Commons-1.9.0/tests/databases/run_databases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/tests/databases/run_databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/tests/databases/run_databases/test_run_databases_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:30:43.409045 OctoBot-Commons-1.9.0/tests/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/tests/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/tests/logging/test_logging_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:30:43.409045 OctoBot-Commons-1.9.0/tests/profiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/tests/profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16320 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/tests/profiles/test_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9440 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/tests/profiles/test_profile_sharing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:30:43.409045 OctoBot-Commons-1.9.0/tests/signals/
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/tests/signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/tests/signals/test_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/tests/signals/test_signal_builder_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/tests/signals/test_signal_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/tests/signals/test_signal_bundle_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/tests/signals/test_signal_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/tests/signals/test_signal_publisher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:30:43.409045 OctoBot-Commons-1.9.0/tests/symbols/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/tests/symbols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/tests/symbols/test_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/tests/symbols/test_symbol_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:30:43.413045 OctoBot-Commons-1.9.0/tests/tentacles_management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/tests/tentacles_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/tests/tentacles_management/test_abstract_tentacle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/tests/tentacles_management/test_class_inspector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:30:43.413045 OctoBot-Commons-1.9.0/tests/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/tests/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/tests/tree/test_base_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-05-02 16:30:03.000000 OctoBot-Commons-1.9.0/tests/tree/test_event_tree.py
```

### Comparing `OctoBot-Commons-1.8.9/CHANGELOG.md` & `OctoBot-Commons-1.9.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,99 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [1.9.0] - 2023-05-02
+### Updated
+- Supported python versions
+
+## [1.8.28] - 2023-04-29
+### Updated
+- [PrettyPrinter] decimal adapter
+- [Enums] BacktestingMetadata
+
+## [1.8.27] - 2023-04-17
+### Fixed
+- [Databases] SQL: delete statement
+
+## [1.8.26] - 2023-04-15
+### Updated
+- [PrettyPrinter] Adapt decimals to number
+### Fixed
+- [Databases] Auto-repair error
+
+## [1.8.25] - 2023-04-15
+### Added
+- [DisplayTranslator] config_by_tentacles
+- [Databases] Auto-repair when necessary
+
+## [1.8.24] - 2023-04-05
+### Added
+- [TimeFrames] is_time_frame
+
+## [1.8.23] - 2023-03-30
+### Added
+- [Orders] historical orders update
+
+## [1.8.22] - 2023-03-28
+### Updated
+- [AbstractTentacle] fix CLASS_UI
+
+## [1.8.21] - 2023-03-27
+### Updated
+- [AbstractTentacle] add cython class and support for generalized user inputs
+
+## [1.8.20] - 2023-03-25
+### Updated
+- [Profiles] add risk and complexity
+
+## [1.8.19] - 2023-03-23
+### Updated
+- [Portfolio] improve portfolio pretty print
+
+## [1.8.18] - 2023-03-22
+### Added
+- [User Inputs] UserInputEditorOptionsTypes
+### Updated
+- [Portfolio] add reference market value in pretty print
+
+## [1.8.17] - 2023-03-21
+### Updated
+- [Logging] add handler-scope level update
+
+## [1.8.16] - 2023-03-19
+### Updated
+- [Profiles] handle profiles sync error
+
+## [1.8.15] - 2023-03-18
+### Updated
+- [PrettyPrinter] telegram lib import
+
+## [1.8.14] - 2023-03-13
+### Updated
+- [Enums] Storage related enums
+
+## [1.8.13] - 2023-03-08
+### Added
+- [Profiles] Validate imported profiles
+
+## [1.8.12] - 2023-03-01
+### Added
+- [Databases] Debug logs
+
+## [1.8.11] - 2023-02-16
+### Updated
+- [Config] Improve config files errors management
+
+## [1.8.10] - 2023-02-12
+### Updated
+- [SystemResourcesWatcher] Enable resources dump in csv file
+
 ## [1.8.9] - 2023-02-11
 ### Updated
 - [Databases] Raise FileNotFoundError on missing path
 
 ## [1.8.8] - 2023-02-10
 ### Added
 - [Enums] TriggerSource
```

### Comparing `OctoBot-Commons-1.8.9/LICENSE` & `OctoBot-Commons-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/OctoBot_Commons.egg-info/PKG-INFO` & `OctoBot-Commons-1.9.0/OctoBot_Commons.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: OctoBot-Commons
-Version: 1.8.9
+Version: 1.9.0
 Summary: OctoBot project common modules
 Home-page: https://github.com/Drakkar-Software/OctoBot-Commons
 Author: Drakkar-Software
-Author-email: drakkar-software@protonmail.com
+Author-email: contact@drakkar.software
 License: LGPL-3.0
-Description: # OctoBot-Commons [1.8.9](https://github.com/Drakkar-Software/OctoBot-Commons/blob/master/CHANGELOG.md)
-        [![Codacy Badge](https://api.codacy.com/project/badge/Grade/b31f3ab3511744a5a5ca6b9bb48e77bb)](https://app.codacy.com/gh/Drakkar-Software/OctoBot-Commons?utm_source=github.com&utm_medium=referral&utm_content=Drakkar-Software/OctoBot-Commons&utm_campaign=Badge_Grade_Dashboard)
-        [![PyPI](https://img.shields.io/pypi/v/OctoBot-Commons.svg)](https://pypi.python.org/pypi/OctoBot-Commons/)
-        [![Coverage Status](https://coveralls.io/repos/github/Drakkar-Software/OctoBot-Commons/badge.svg?branch=master)](https://coveralls.io/github/Drakkar-Software/OctoBot-Commons?branch=master)
-        [![Github-Action-CI](https://github.com/Drakkar-Software/OctoBot-Commons/workflows/Github-Action-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot-Commons/actions)
-        [![Build Status](https://cloud.drone.io/api/badges/Drakkar-Software/OctoBot-Commons/status.svg)](https://cloud.drone.io/Drakkar-Software/OctoBot-Commons)
-        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-        
-        [OctoBot](https://github.com/Drakkar-Software/OctoBot) project common modules.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
+License-File: LICENSE
+
+# OctoBot-Commons [1.9.0](https://github.com/Drakkar-Software/OctoBot-Commons/blob/master/CHANGELOG.md)
+[![Codacy Badge](https://api.codacy.com/project/badge/Grade/b31f3ab3511744a5a5ca6b9bb48e77bb)](https://app.codacy.com/gh/Drakkar-Software/OctoBot-Commons?utm_source=github.com&utm_medium=referral&utm_content=Drakkar-Software/OctoBot-Commons&utm_campaign=Badge_Grade_Dashboard)
+[![PyPI](https://img.shields.io/pypi/v/OctoBot-Commons.svg)](https://pypi.python.org/pypi/OctoBot-Commons/)
+[![Coverage Status](https://coveralls.io/repos/github/Drakkar-Software/OctoBot-Commons/badge.svg?branch=master)](https://coveralls.io/github/Drakkar-Software/OctoBot-Commons?branch=master)
+[![Github-Action-CI](https://github.com/Drakkar-Software/OctoBot-Commons/workflows/Github-Action-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot-Commons/actions)
+[![Build Status](https://cloud.drone.io/api/badges/Drakkar-Software/OctoBot-Commons/status.svg)](https://cloud.drone.io/Drakkar-Software/OctoBot-Commons)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+[OctoBot](https://github.com/Drakkar-Software/OctoBot) project common modules.
```

### Comparing `OctoBot-Commons-1.8.9/OctoBot_Commons.egg-info/SOURCES.txt` & `OctoBot-Commons-1.9.0/OctoBot_Commons.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -6,55 +6,48 @@
 setup.py
 OctoBot_Commons.egg-info/PKG-INFO
 OctoBot_Commons.egg-info/SOURCES.txt
 OctoBot_Commons.egg-info/dependency_links.txt
 OctoBot_Commons.egg-info/not-zip-safe
 OctoBot_Commons.egg-info/requires.txt
 OctoBot_Commons.egg-info/top_level.txt
-octobot_commons/__init__.pxd
 octobot_commons/__init__.py
 octobot_commons/aiohttp_util.py
-octobot_commons/async_job.pxd
 octobot_commons/async_job.py
 octobot_commons/asyncio_tools.py
 octobot_commons/authentication.py
 octobot_commons/channels_name.py
 octobot_commons/constants.py
-octobot_commons/data_util.pxd
 octobot_commons/data_util.py
 octobot_commons/dict_util.py
 octobot_commons/enums.py
 octobot_commons/errors.py
-octobot_commons/evaluator_util.pxd
 octobot_commons/evaluators_util.py
 octobot_commons/external_resources_manager.py
 octobot_commons/json_util.py
-octobot_commons/list_util.pxd
 octobot_commons/list_util.py
 octobot_commons/logical_operators.py
 octobot_commons/multiprocessing_util.py
 octobot_commons/number_util.py
 octobot_commons/optimization_campaign.py
 octobot_commons/os_clock_sync.py
 octobot_commons/os_util.py
-octobot_commons/pretty_printer.pxd
 octobot_commons/pretty_printer.py
 octobot_commons/support.py
 octobot_commons/system_resources_watcher.py
 octobot_commons/thread_util.py
-octobot_commons/time_frame_manager.pxd
 octobot_commons/time_frame_manager.py
 octobot_commons/timestamp_util.py
 octobot_commons/configuration/__init__.py
 octobot_commons/configuration/config_file_manager.py
 octobot_commons/configuration/config_operations.py
 octobot_commons/configuration/configuration.py
 octobot_commons/configuration/fields_utils.py
+octobot_commons/configuration/user_input_configuration.py
 octobot_commons/configuration/user_inputs.py
-octobot_commons/databases/__init__.pxd
 octobot_commons/databases/__init__.py
 octobot_commons/databases/cache_client.py
 octobot_commons/databases/cache_manager.py
 octobot_commons/databases/bases/__init__.py
 octobot_commons/databases/bases/base_database.py
 octobot_commons/databases/bases/document_database.py
 octobot_commons/databases/database_caches/__init__.py
@@ -64,82 +57,64 @@
 octobot_commons/databases/databases_util/cache_wrapper.py
 octobot_commons/databases/document_database_adaptors/__init__.py
 octobot_commons/databases/document_database_adaptors/abstract_document_database_adaptor.py
 octobot_commons/databases/document_database_adaptors/tinydb_adaptor.py
 octobot_commons/databases/global_storage/__init__.py
 octobot_commons/databases/global_storage/global_shared_memory_storage.py
 octobot_commons/databases/implementations/__init__.py
+octobot_commons/databases/implementations/_exchange_database.py
 octobot_commons/databases/implementations/cache_database.py
 octobot_commons/databases/implementations/cache_timestamp_database.py
 octobot_commons/databases/implementations/db_reader.py
 octobot_commons/databases/implementations/db_writer.py
 octobot_commons/databases/implementations/db_writer_reader.py
 octobot_commons/databases/implementations/meta_database.py
-octobot_commons/databases/relational_databases/__init__.pxd
 octobot_commons/databases/relational_databases/__init__.py
-octobot_commons/databases/relational_databases/sqlite/__init__.pxd
 octobot_commons/databases/relational_databases/sqlite/__init__.py
-octobot_commons/databases/relational_databases/sqlite/cursor_pool.pxd
 octobot_commons/databases/relational_databases/sqlite/cursor_pool.py
-octobot_commons/databases/relational_databases/sqlite/cursor_wrapper.pxd
 octobot_commons/databases/relational_databases/sqlite/cursor_wrapper.py
-octobot_commons/databases/relational_databases/sqlite/sqlite_database.pxd
 octobot_commons/databases/relational_databases/sqlite/sqlite_database.py
-octobot_commons/databases/run_databases/__init__.pxd
 octobot_commons/databases/run_databases/__init__.py
 octobot_commons/databases/run_databases/abstract_run_databases_pruner.py
 octobot_commons/databases/run_databases/file_system_run_databases_pruner.py
 octobot_commons/databases/run_databases/run_databases_identifier.py
-octobot_commons/databases/run_databases/run_databases_provider.pxd
 octobot_commons/databases/run_databases/run_databases_provider.py
 octobot_commons/databases/run_databases/run_databases_pruning_factory.py
 octobot_commons/databases/run_databases/storage.py
 octobot_commons/databases/run_databases/utils.py
 octobot_commons/display/__init__.py
 octobot_commons/display/display_factory.py
 octobot_commons/display/display_translator.py
 octobot_commons/display/plot_settings.py
-octobot_commons/logging/__init__.pxd
 octobot_commons/logging/__init__.py
-octobot_commons/logging/logging_util.pxd
 octobot_commons/logging/logging_util.py
 octobot_commons/profiles/__init__.py
 octobot_commons/profiles/profile.py
 octobot_commons/profiles/profile_sharing.py
 octobot_commons/signals/__init__.py
 octobot_commons/signals/signal.py
 octobot_commons/signals/signal_builder_wrapper.py
 octobot_commons/signals/signal_bundle.py
 octobot_commons/signals/signal_bundle_builder.py
 octobot_commons/signals/signal_factory.py
 octobot_commons/signals/signal_publisher.py
 octobot_commons/signals/signals_emitter.py
-octobot_commons/singleton/__init__.pxd
 octobot_commons/singleton/__init__.py
-octobot_commons/singleton/singleton_class.pxd
 octobot_commons/singleton/singleton_class.py
-octobot_commons/symbols/__init__.pxd
 octobot_commons/symbols/__init__.py
-octobot_commons/symbols/symbol.pxd
 octobot_commons/symbols/symbol.py
-octobot_commons/symbols/symbol_util.pxd
 octobot_commons/symbols/symbol_util.py
-octobot_commons/tentacles_management/__init__.pxd
 octobot_commons/tentacles_management/__init__.py
 octobot_commons/tentacles_management/abstract_tentacle.py
-octobot_commons/tentacles_management/class_inspector.pxd
 octobot_commons/tentacles_management/class_inspector.py
 octobot_commons/tests/__init__.py
 octobot_commons/tests/test_config.py
-octobot_commons/tree/__init__.pxd
 octobot_commons/tree/__init__.py
-octobot_commons/tree/base_tree.pxd
 octobot_commons/tree/base_tree.py
 octobot_commons/tree/event_provider.py
-octobot_commons/tree/event_tree.pxd
 octobot_commons/tree/event_tree.py
 tests/configuration/__init__.py
 tests/configuration/test_configuration.py
 tests/configuration/test_fields_util.py
 tests/databases/__init__.py
 tests/databases/global_storage/__init__.py
 tests/databases/global_storage/test_global_shared_memory_storage.py
@@ -159,10 +134,13 @@
 tests/signals/test_signal_bundle.py
 tests/signals/test_signal_bundle_builder.py
 tests/signals/test_signal_factory.py
 tests/signals/test_signal_publisher.py
 tests/symbols/__init__.py
 tests/symbols/test_symbol.py
 tests/symbols/test_symbol_util.py
+tests/tentacles_management/__init__.py
+tests/tentacles_management/test_abstract_tentacle.py
+tests/tentacles_management/test_class_inspector.py
 tests/tree/__init__.py
 tests/tree/test_base_tree.py
 tests/tree/test_event_tree.py
```

### Comparing `OctoBot-Commons-1.8.9/PKG-INFO` & `OctoBot-Commons-1.9.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: OctoBot-Commons
-Version: 1.8.9
+Version: 1.9.0
 Summary: OctoBot project common modules
 Home-page: https://github.com/Drakkar-Software/OctoBot-Commons
 Author: Drakkar-Software
-Author-email: drakkar-software@protonmail.com
+Author-email: contact@drakkar.software
 License: LGPL-3.0
-Description: # OctoBot-Commons [1.8.9](https://github.com/Drakkar-Software/OctoBot-Commons/blob/master/CHANGELOG.md)
-        [![Codacy Badge](https://api.codacy.com/project/badge/Grade/b31f3ab3511744a5a5ca6b9bb48e77bb)](https://app.codacy.com/gh/Drakkar-Software/OctoBot-Commons?utm_source=github.com&utm_medium=referral&utm_content=Drakkar-Software/OctoBot-Commons&utm_campaign=Badge_Grade_Dashboard)
-        [![PyPI](https://img.shields.io/pypi/v/OctoBot-Commons.svg)](https://pypi.python.org/pypi/OctoBot-Commons/)
-        [![Coverage Status](https://coveralls.io/repos/github/Drakkar-Software/OctoBot-Commons/badge.svg?branch=master)](https://coveralls.io/github/Drakkar-Software/OctoBot-Commons?branch=master)
-        [![Github-Action-CI](https://github.com/Drakkar-Software/OctoBot-Commons/workflows/Github-Action-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot-Commons/actions)
-        [![Build Status](https://cloud.drone.io/api/badges/Drakkar-Software/OctoBot-Commons/status.svg)](https://cloud.drone.io/Drakkar-Software/OctoBot-Commons)
-        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-        
-        [OctoBot](https://github.com/Drakkar-Software/OctoBot) project common modules.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
+License-File: LICENSE
+
+# OctoBot-Commons [1.9.0](https://github.com/Drakkar-Software/OctoBot-Commons/blob/master/CHANGELOG.md)
+[![Codacy Badge](https://api.codacy.com/project/badge/Grade/b31f3ab3511744a5a5ca6b9bb48e77bb)](https://app.codacy.com/gh/Drakkar-Software/OctoBot-Commons?utm_source=github.com&utm_medium=referral&utm_content=Drakkar-Software/OctoBot-Commons&utm_campaign=Badge_Grade_Dashboard)
+[![PyPI](https://img.shields.io/pypi/v/OctoBot-Commons.svg)](https://pypi.python.org/pypi/OctoBot-Commons/)
+[![Coverage Status](https://coveralls.io/repos/github/Drakkar-Software/OctoBot-Commons/badge.svg?branch=master)](https://coveralls.io/github/Drakkar-Software/OctoBot-Commons?branch=master)
+[![Github-Action-CI](https://github.com/Drakkar-Software/OctoBot-Commons/workflows/Github-Action-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot-Commons/actions)
+[![Build Status](https://cloud.drone.io/api/badges/Drakkar-Software/OctoBot-Commons/status.svg)](https://cloud.drone.io/Drakkar-Software/OctoBot-Commons)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+[OctoBot](https://github.com/Drakkar-Software/OctoBot) project common modules.
```

### Comparing `OctoBot-Commons-1.8.9/README.md` & `OctoBot-Commons-1.9.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# OctoBot-Commons [1.8.9](https://github.com/Drakkar-Software/OctoBot-Commons/blob/master/CHANGELOG.md)
+# OctoBot-Commons [1.9.0](https://github.com/Drakkar-Software/OctoBot-Commons/blob/master/CHANGELOG.md)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/b31f3ab3511744a5a5ca6b9bb48e77bb)](https://app.codacy.com/gh/Drakkar-Software/OctoBot-Commons?utm_source=github.com&utm_medium=referral&utm_content=Drakkar-Software/OctoBot-Commons&utm_campaign=Badge_Grade_Dashboard)
 [![PyPI](https://img.shields.io/pypi/v/OctoBot-Commons.svg)](https://pypi.python.org/pypi/OctoBot-Commons/)
 [![Coverage Status](https://coveralls.io/repos/github/Drakkar-Software/OctoBot-Commons/badge.svg?branch=master)](https://coveralls.io/github/Drakkar-Software/OctoBot-Commons?branch=master)
 [![Github-Action-CI](https://github.com/Drakkar-Software/OctoBot-Commons/workflows/Github-Action-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot-Commons/actions)
 [![Build Status](https://cloud.drone.io/api/badges/Drakkar-Software/OctoBot-Commons/status.svg)](https://cloud.drone.io/Drakkar-Software/OctoBot-Commons)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/__init__.pxd` & `OctoBot-Commons-1.9.0/octobot_commons/databases/global_storage/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# cython: language_level=3
 #  Drakkar-Software OctoBot-Commons
 #  Copyright (c) Drakkar-Software, All rights reserved.
 #
 #  This library is free software; you can redistribute it and/or
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
@@ -10,7 +9,19 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
+
+
+from octobot_commons.databases.global_storage import global_shared_memory_storage
+
+from octobot_commons.databases.global_storage.global_shared_memory_storage import (
+    GlobalSharedMemoryStorage,
+)
+
+
+__all__ = [
+    "GlobalSharedMemoryStorage",
+]
```

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/__init__.py` & `OctoBot-Commons-1.9.0/octobot_commons/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,14 @@
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 
 PROJECT_NAME = "OctoBot-Commons"
-VERSION = "1.8.9"  # major.minor.revision
+VERSION = "1.9.0"  # major.minor.revision
 
 MARKET_SEPARATOR = "/"
 SETTLEMENT_ASSET_SEPARATOR = ":"
 DICT_BULLET_TOKEN_STR = "\n "
 
 OCTOBOT_KEY = b"uVEw_JJe7uiXepaU_DR4T-ThkjZlDn8Pzl8hYPIv7w0="  # TODO temp
```

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/aiohttp_util.py` & `OctoBot-Commons-1.9.0/octobot_commons/aiohttp_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/async_job.py` & `OctoBot-Commons-1.9.0/octobot_commons/async_job.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/asyncio_tools.py` & `OctoBot-Commons-1.9.0/octobot_commons/asyncio_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         """
         self.errors.append(context)
         if self.print_received_exceptions:
             print(context)
             error = context.get("exception")
             if error:
                 traceback.print_exception(
-                    etype=type(error), value=error, tb=error.__traceback__
+                    type(error), value=error, tb=error.__traceback__
                 )
 
     async def check(self) -> None:
         """
         Will raise AssertionError if an exception has been raised in the registered loop(s)
         :return: None
         """
```

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/authentication.py` & `OctoBot-Commons-1.9.0/octobot_commons/authentication.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,28 +119,29 @@
     async def await_initialization(self, timeout):
         """
         Returns when initialized
         :return:
         """
         await asyncio.wait_for(self.initialized_event.wait(), timeout)
 
-    async def update_trades(self, trades: list):
+    async def update_trades(self, trades: list, reset: bool):
         """
         Updates authenticated account trades
         """
         raise NotImplementedError
 
     async def update_portfolio(
         self,
         current_value: dict,
         initial_value: dict,
         unit: str,
         content: dict,
         history: dict,
         price_by_asset: dict,
+        reset: bool,
     ):
         """
         Updates authenticated account portfolio
         """
         raise NotImplementedError
```

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/channels_name.py` & `OctoBot-Commons-1.9.0/octobot_commons/channels_name.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/configuration/__init__.py` & `OctoBot-Commons-1.9.0/octobot_commons/configuration/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 from octobot_commons.configuration import configuration
 from octobot_commons.configuration import config_file_manager
 from octobot_commons.configuration import config_operations
 from octobot_commons.configuration import fields_utils
 from octobot_commons.configuration import user_inputs
+from octobot_commons.configuration import user_input_configuration
 
 
 from octobot_commons.configuration.configuration import (
     Configuration,
 )
 from octobot_commons.configuration.config_file_manager import (
     get_user_config,
@@ -53,14 +54,20 @@
     UserInputFactory,
     sanitize_user_input_name,
     save_user_input,
     get_user_input_tentacle_type,
     get_user_inputs,
     clear_user_inputs,
 )
+from octobot_commons.configuration.user_input_configuration import (
+    load_user_inputs_from_class,
+    get_raw_config_and_user_inputs_from_class,
+    get_raw_config_and_user_inputs,
+    load_and_save_user_inputs,
+)
 
 
 __all__ = [
     "Configuration",
     "get_user_config",
     "load",
     "dump",
@@ -83,8 +90,12 @@
     "UserInput",
     "UserInputFactory",
     "sanitize_user_input_name",
     "save_user_input",
     "get_user_input_tentacle_type",
     "get_user_inputs",
     "clear_user_inputs",
+    "load_user_inputs_from_class",
+    "get_raw_config_and_user_inputs_from_class",
+    "get_raw_config_and_user_inputs",
+    "load_and_save_user_inputs",
 ]
```

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/configuration/config_file_manager.py` & `OctoBot-Commons-1.9.0/octobot_commons/configuration/config_file_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,18 +41,15 @@
     :param should_raise: if error should be raised
     :param fill_missing_fields: if missing fields should be filled
     :return: the loaded config
     """
     logger = logging.get_logger(LOGGER_NAME)
     basic_error = "Error when load config file {0}".format(config_file)
     try:
-        with open(config_file) as json_data_file:
-            config = json.load(json_data_file)
-            # if fill_missing_fields: TODO
-            #     _fill_missing_config_fields(config)
+        config = json_util.read_file(config_file)
         return config
     except ValueError as value_error:
         error_str = f"{basic_error} : json decoding failed ({value_error})"
         if should_raise:
             raise Exception(error_str)
         logger.error(error_str)
     except IOError as io_error:
@@ -81,28 +78,37 @@
     :param temp_restore_config_file: the temporary config file
     :param schema_file: path to the json schema to validate the updated config
     """
     try:
         # prepare a restoration config file
         prepare_restore_file(temp_restore_config_file, config_file)
 
+    # when failing to create the restore config
+    except Exception as err:
+        error_details = (
+            f"Failed to create the backup configuration file. Is your {commons_constants.USER_FOLDER} "
+            f"folder accessible ? : {err} ({err.__class__.__name__})"
+        )
+        logging.get_logger(LOGGER_NAME).error(error_details)
+        raise err.__class__(error_details) from err
+    try:
         new_content = jsonify_config(config)
 
         # edit the config file
         with open(config_file, "w") as cg_file:
             cg_file.write(new_content)
 
         if schema_file is not None:
             # check if the new config file is correct
             check_config(config_file, schema_file)
 
         # remove temp file
         remove_restore_file(temp_restore_config_file)
 
-    # when fail restore the old config
+    # when failing to restore the previous config
     except Exception as global_exception:
         logging.get_logger(LOGGER_NAME).error(
             f"Save config failed : {global_exception}"
         )
         restore(temp_restore_config_file, config_file)
         raise global_exception
```

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/configuration/config_operations.py` & `OctoBot-Commons-1.9.0/octobot_commons/configuration/config_operations.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/configuration/configuration.py` & `OctoBot-Commons-1.9.0/octobot_commons/configuration/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,16 +152,23 @@
         Update profile partially managed elements for all profiles except self.profile
         with self.config
         """
         for profile in self.profile_by_id.values():
             if profile is self.profile:
                 # do not synchronize self.profile
                 continue
-            profile.remove_deleted_elements(self.config)
-            profile.validate_and_save_config()
+            try:
+                profile.remove_deleted_elements(self.config)
+                profile.validate_and_save_config()
+            except Exception as err:
+                self.logger.exception(
+                    f"Error when synchronizing '{profile.name}' profile at '{profile.path}': {err}",
+                    False,
+                    err,
+                )
 
     def is_loaded(self) -> bool:
         """
         Checks if self has been loaded
         :return: True when self has been loaded (read)
         """
         return self.config is not None
```

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/configuration/fields_utils.py` & `OctoBot-Commons-1.9.0/octobot_commons/configuration/fields_utils.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/configuration/user_inputs.py` & `OctoBot-Commons-1.9.0/octobot_commons/configuration/user_inputs.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/constants.py` & `OctoBot-Commons-1.9.0/octobot_commons/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,22 +52,26 @@
 DEFAULT_CURRENT_LIVE_ID = 1
 
 # profiles
 PROFILES_FOLDER = "profiles"
 USER_PROFILES_FOLDER = f"{USER_FOLDER}/{PROFILES_FOLDER}"
 PROFILE_CONFIG_FILE = "profile.json"
 CONFIG_PROFILE = "profile"
+CONFIG_BACKTESTING_PROFILE = "backtesting_profile"
 DEFAULT_PROFILE = "default"
 DEFAULT_PROFILE_FILE = f"{CONFIG_PROFILE}.json"
 CONFIG_NAME = "name"
 CONFIG_DESCRIPTION = "description"
 CONFIG_AVATAR = "avatar"
 CONFIG_ORIGIN_URL = "origin_url"
 CONFIG_READ_ONLY = "read_only"
 CONFIG_IMPORTED = "imported"
+CONFIG_COMPLEXITY = "complexity"
+CONFIG_RISK = "risk"
+CONFIG_TYPE = "type"
 PROFILE_CONFIG = "config"
 CONFIG_ID = "id"
 PROFILE_FILE_SCHEMA = f"{CONFIG_FOLDER}/profile_{SCHEMA}.json"
 PROFILE_EXPORT_FORMAT = "zip"
 IMPORTED_PROFILE_PREFIX = "imported"
 USE_CURRENT_PROFILE = "use_current_profile"
```

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/data_util.pxd` & `OctoBot-Commons-1.9.0/octobot_commons/signals/signals_emitter.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,29 @@
-# cython: language_level=3
-#  Drakkar-Software OctoBot-Commons
+#  Drakkar-Software OctoBot-Trading
 #  Copyright (c) Drakkar-Software, All rights reserved.
 #
 #  This library is free software; you can redistribute it and/or
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
 #
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
+import octobot_commons.enums as commons_enums
+import octobot_commons.authentication as authentication
+import octobot_commons.signals.signal_bundle as signal_bundle
 
-cimport numpy as np
 
-cpdef object normalize_data(object data)
-cpdef double mean(object number_list)
-cpdef np.ndarray shift_value_array(np.ndarray array, int shift_count=*,
-                                   object fill_value=*, object dtype=*)
+async def emit_signal_bundle(to_send_signal_bundle: signal_bundle.SignalBundle):
+    """
+    Emits a signal bundle
+    """
+    await authentication.Authenticator.instance().send(
+        to_send_signal_bundle.to_dict(),
+        commons_enums.CommunityChannelTypes.SIGNAL,
+        identifier=to_send_signal_bundle.identifier,
+    )
```

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/data_util.py` & `OctoBot-Commons-1.9.0/octobot_commons/data_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/databases/__init__.pxd` & `OctoBot-Commons-1.9.0/octobot_commons/databases/database_caches/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-# cython: language_level=3
-#  Drakkar-Software OctoBot-Backtesting
+#  Drakkar-Software OctoBot-Commons
 #  Copyright (c) Drakkar-Software, All rights reserved.
 #
 #  This library is free software; you can redistribute it and/or
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
 #
@@ -11,21 +10,23 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 
-from octobot_commons.databases cimport relational_databases
-from octobot_commons.databases.relational_databases cimport (
-    SQLiteDatabase,
-)
 
-from octobot_commons.databases cimport run_databases
-from octobot_commons.databases.run_databases cimport (
-    RunDatabasesProvider,
+from octobot_commons.databases.database_caches import generic_database_cache
+from octobot_commons.databases.database_caches import chronological_read_database_cache
+
+from octobot_commons.databases.database_caches.generic_database_cache import (
+    GenericDatabaseCache,
 )
+from octobot_commons.databases.database_caches.chronological_read_database_cache import (
+    ChronologicalReadDatabaseCache,
+)
+
 
 __all__ = [
-    "SQLiteDatabase",
-    "RunDatabasesProvider",
+    "GenericDatabaseCache",
+    "ChronologicalReadDatabaseCache",
 ]
```

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/databases/__init__.py` & `OctoBot-Commons-1.9.0/octobot_commons/databases/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/databases/bases/__init__.py` & `OctoBot-Commons-1.9.0/octobot_commons/databases/bases/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/databases/bases/base_database.py` & `OctoBot-Commons-1.9.0/octobot_commons/databases/bases/base_database.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/databases/bases/document_database.py` & `OctoBot-Commons-1.9.0/octobot_commons/databases/bases/document_database.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 import contextlib
+import octobot_commons.logging
 
 
 class DocumentDatabase:
     """
     DocumentDatabase is used to communicate with an underlying database
     """
 
@@ -129,28 +130,37 @@
         """
         return await self.adaptor.query_factory()
 
     async def hard_reset(self):
         """
         Completely reset the database
         """
+        self.get_logger().debug("hard resetting database")
         return await self.adaptor.hard_reset()
 
     async def flush(self):
         """
         Flushes the database cache
         """
+        self.get_logger().debug("flushing database")
         return await self.adaptor.flush()
 
     async def close(self):
         """
         Closes the database
         """
+        self.get_logger().debug("closing database")
         return await self.adaptor.close()
 
+    def get_logger(self):
+        """
+        :return: the database logger
+        """
+        return octobot_commons.logging.get_logger(str(self))
+
     def __str__(self):
         return f"{self.__class__.__name__} with adaptor: {self.adaptor}"
 
     @classmethod
     @contextlib.asynccontextmanager
     async def locked_database(cls, *args, **kwargs):
         """
```

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/databases/cache_client.py` & `OctoBot-Commons-1.9.0/octobot_commons/databases/cache_client.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/databases/cache_manager.py` & `OctoBot-Commons-1.9.0/octobot_commons/databases/cache_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/databases/database_caches/__init__.py` & `OctoBot-Commons-1.9.0/octobot_commons/databases/relational_databases/sqlite/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,22 +11,18 @@
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 
 
-from octobot_commons.databases.database_caches import generic_database_cache
-from octobot_commons.databases.database_caches import chronological_read_database_cache
-
-from octobot_commons.databases.database_caches.generic_database_cache import (
-    GenericDatabaseCache,
-)
-from octobot_commons.databases.database_caches.chronological_read_database_cache import (
-    ChronologicalReadDatabaseCache,
+from octobot_commons.databases.relational_databases.sqlite import sqlite_database
+from octobot_commons.databases.relational_databases.sqlite.sqlite_database import (
+    SQLiteDatabase,
+    new_sqlite_database,
 )
 
 
 __all__ = [
-    "GenericDatabaseCache",
-    "ChronologicalReadDatabaseCache",
+    "SQLiteDatabase",
+    "new_sqlite_database",
 ]
```

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/databases/database_caches/chronological_read_database_cache.py` & `OctoBot-Commons-1.9.0/octobot_commons/databases/database_caches/chronological_read_database_cache.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/databases/database_caches/generic_database_cache.py` & `OctoBot-Commons-1.9.0/octobot_commons/databases/database_caches/generic_database_cache.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/databases/databases_util/__init__.py` & `OctoBot-Commons-1.9.0/octobot_commons/databases/databases_util/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/databases/databases_util/cache_wrapper.py` & `OctoBot-Commons-1.9.0/octobot_commons/databases/databases_util/cache_wrapper.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/databases/document_database_adaptors/__init__.py` & `OctoBot-Commons-1.9.0/octobot_commons/databases/document_database_adaptors/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/databases/document_database_adaptors/abstract_document_database_adaptor.py` & `OctoBot-Commons-1.9.0/octobot_commons/databases/document_database_adaptors/abstract_document_database_adaptor.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/databases/document_database_adaptors/tinydb_adaptor.py` & `OctoBot-Commons-1.9.0/octobot_commons/databases/document_database_adaptors/tinydb_adaptor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=C0301, R0904, R1732, C0116
+# pylint: disable=C0301, R0904, R1732, C0116, W0231, W0231
 #  Drakkar-Software OctoBot-Commons
 #  Copyright (c) Drakkar-Software, All rights reserved.
 #
 #  This library is free software; you can redistribute it and/or
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
```

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/databases/global_storage/__init__.py` & `OctoBot-Commons-1.9.0/octobot_commons/singleton/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,18 +10,14 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 
+from octobot_commons.singleton import singleton_class
 
-from octobot_commons.databases.global_storage import global_shared_memory_storage
-
-from octobot_commons.databases.global_storage.global_shared_memory_storage import (
-    GlobalSharedMemoryStorage,
-)
-
+from octobot_commons.singleton.singleton_class import Singleton
 
 __all__ = [
-    "GlobalSharedMemoryStorage",
+    "Singleton",
 ]
```

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/databases/global_storage/global_shared_memory_storage.py` & `OctoBot-Commons-1.9.0/octobot_commons/databases/global_storage/global_shared_memory_storage.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/databases/implementations/__init__.py` & `OctoBot-Commons-1.9.0/octobot_commons/databases/implementations/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/databases/implementations/cache_database.py` & `OctoBot-Commons-1.9.0/octobot_commons/databases/implementations/cache_database.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/databases/implementations/cache_timestamp_database.py` & `OctoBot-Commons-1.9.0/octobot_commons/databases/implementations/cache_timestamp_database.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/databases/implementations/db_reader.py` & `OctoBot-Commons-1.9.0/octobot_commons/databases/implementations/db_reader.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/databases/implementations/db_writer.py` & `OctoBot-Commons-1.9.0/octobot_commons/databases/implementations/db_writer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/databases/implementations/db_writer_reader.py` & `OctoBot-Commons-1.9.0/octobot_commons/databases/implementations/db_writer_reader.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/databases/implementations/meta_database.py` & `OctoBot-Commons-1.9.0/octobot_commons/databases/implementations/_exchange_database.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,197 +10,130 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-import contextlib
 import os
 
 import octobot_commons.databases.implementations.db_writer_reader as db_writer_reader
-import octobot_commons.enums as enums
 
 
-class MetaDatabase:
-    def __init__(self, run_dbs_identifier, with_lock=False, cache_size=None):
-        self.run_dbs_identifier = run_dbs_identifier
-        self.with_lock = with_lock
-        self.cache_size = cache_size
-        self.database_adaptor = self.run_dbs_identifier.database_adaptor
-        self.run_db: db_writer_reader.DBWriterReader = None
+class ExchangeDatabase:
+    def __init__(self, meta_database, exchange):
+        self.meta_database = meta_database
+        self.run_dbs_identifier = self.meta_database.run_dbs_identifier
+        self.exchange = exchange
         self.orders_db: db_writer_reader.DBWriterReader = None
         self.trades_db: db_writer_reader.DBWriterReader = None
         self.transactions_db: db_writer_reader.DBWriterReader = None
         self.historical_portfolio_value_db: db_writer_reader.DBWriterReader = None
-        self.backtesting_metadata_db: db_writer_reader.DBWriterReader = None
         self.symbol_dbs: dict = {}
 
-    def get_run_db(self):
-        """
-        :return: the run database. Opens it if not open already
-        """
-        if self.run_db is None:
-            self.run_db = self._get_db(
-                self.run_dbs_identifier.get_run_data_db_identifier()
-            )
-        return self.run_db
-
-    def get_orders_db(self, account_type, exchange=None):
+    def get_orders_db(self, account_type):
         """
         :return: the orders database. Opens it if not open already
         """
         if self.orders_db is None:
-            self.orders_db = self._get_db(
+            self.orders_db = self.meta_database.get_db(
                 self.run_dbs_identifier.get_orders_db_identifier(
                     account_type,
-                    exchange or self.run_dbs_identifier.context.exchange_name,
+                    self.exchange,
                 )
             )
         return self.orders_db
 
-    def get_trades_db(self, account_type, exchange=None):
+    def get_trades_db(self, account_type):
         """
         :return: the trades database. Opens it if not open already
         """
         if self.trades_db is None:
-            self.trades_db = self._get_db(
+            self.trades_db = self.meta_database.get_db(
                 self.run_dbs_identifier.get_trades_db_identifier(
                     account_type,
-                    exchange or self.run_dbs_identifier.context.exchange_name,
+                    self.exchange,
                 )
             )
         return self.trades_db
 
-    def get_transactions_db(self, account_type, exchange=None):
+    def get_transactions_db(self, account_type):
         """
         :return: the transactions database. Opens it if not open already
         """
         if self.transactions_db is None:
-            self.transactions_db = self._get_db(
+            self.transactions_db = self.meta_database.get_db(
                 self.run_dbs_identifier.get_transactions_db_identifier(
                     account_type,
-                    exchange or self.run_dbs_identifier.context.exchange_name,
+                    self.exchange,
                 )
             )
         return self.transactions_db
 
-    def get_historical_portfolio_value_db(self, account_type, exchange):
+    def get_historical_portfolio_value_db(self, account_type):
         """
         :return: the historical portfolio database. Opens it if not open already
         """
         if self.historical_portfolio_value_db is None:
-            self.historical_portfolio_value_db = self._get_db(
+            self.historical_portfolio_value_db = self.meta_database.get_db(
                 self.run_dbs_identifier.get_historical_portfolio_value_db_identifier(
-                    account_type, exchange
+                    account_type, self.exchange
                 )
             )
         return self.historical_portfolio_value_db
 
-    def get_backtesting_metadata_db(self):
-        """
-        :return: the backtesting metadata database. Opens it if not open already
-        """
-        if self.backtesting_metadata_db is None:
-            self.backtesting_metadata_db = self._get_db(
-                self.run_dbs_identifier.get_backtesting_metadata_identifier()
-            )
-        return self.backtesting_metadata_db
-
-    async def get_backtesting_metadata_from_run(self):
-        """
-        :return: the backtesting metadata for the associated run_dbs_identifier's backtesting_id
-        """
-        db = self.get_backtesting_metadata_db()
-        return (
-            await db.select(
-                enums.CacheDatabaseTables.METADATA.value,
-                (await db.search()).id == self.run_dbs_identifier.backtesting_id,
-            )
-        )[0]
-
-    def get_symbol_db(self, exchange, symbol):
+    def get_symbol_db(self, symbol):
         """
         :return: the symbol database. Opens it if not open already
         """
-        key = self._get_symbol_db_key(exchange, symbol)
+        key = self._get_symbol_db_key(self.exchange, symbol)
         if key not in self.symbol_dbs:
-            self.symbol_dbs[key] = self._get_db(
-                self.run_dbs_identifier.get_symbol_db_identifier(exchange, symbol)
+            self.symbol_dbs[key] = self.meta_database.get_db(
+                self.run_dbs_identifier.get_symbol_db_identifier(self.exchange, symbol)
             )
         return self.symbol_dbs[key]
 
-    async def get_all_symbol_dbs(self, exchange):
+    async def get_all_symbol_dbs(self):
         """
         :return: an iterable over each symbol database for the given exchange
         """
         if self.run_dbs_identifier.database_adaptor.is_file_system_based():
             return [
-                self.get_symbol_db(
-                    exchange, self.run_dbs_identifier.get_symbol_db_name(db.name)
-                )
+                self.get_symbol_db(self.run_dbs_identifier.get_symbol_db_name(db.name))
                 for db in os.scandir(
-                    self.run_dbs_identifier.get_exchange_based_identifier(exchange)
+                    self.run_dbs_identifier.get_exchange_based_identifier(self.exchange)
                 )
                 if self.run_dbs_identifier.is_symbol_database(db.name)
             ]
         raise NotImplementedError(
             "get_all_symbol_dbs is not implemented for non is_file_system_based databases"
         )
 
-    def all_basic_run_db(self, account_type, exchange=None):
+    def all_basic_run_db(self, account_type):
         """
         yields the run, orders, trades and transactions databases
         """
-        yield self.get_run_db()
-        yield self.get_orders_db(account_type, exchange)
-        yield self.get_trades_db(account_type, exchange)
-        yield self.get_transactions_db(account_type, exchange)
+        yield self.get_orders_db(account_type)
+        yield self.get_trades_db(account_type)
+        yield self.get_transactions_db(account_type)
 
     @staticmethod
     def _get_symbol_db_key(exchange, symbol):
         return f"{exchange}{symbol}"
 
-    def _get_db(self, db_identifier):
-        return db_writer_reader.DBWriterReader(
-            db_identifier,
-            with_lock=self.with_lock,
-            cache_size=self.cache_size,
-            database_adaptor=self.database_adaptor,
-            enable_storage=self.run_dbs_identifier.enable_storage,
-        )
-
     async def close(self):
         """
         Closes all the open databases
         """
         # avoid asyncio.gather here as it is producing unexplained side effects (frozen thread preventing stop)
         for coro in (
             db.close()
             for db in (
-                self.run_db,
                 self.orders_db,
                 self.trades_db,
                 self.transactions_db,
                 self.historical_portfolio_value_db,
-                self.backtesting_metadata_db,
                 *self.symbol_dbs.values(),
             )
             if db is not None
         ):
             await coro
-
-    @classmethod
-    @contextlib.asynccontextmanager
-    async def database(cls, database_manager, with_lock=False, cache_size=None):
-        """
-        Created a local meta database and closes it upon leaving the context manager
-        """
-        meta_db = None
-        try:
-            meta_db = MetaDatabase(
-                database_manager, with_lock=with_lock, cache_size=cache_size
-            )
-            yield meta_db
-        finally:
-            if meta_db is not None:
-                await meta_db.close()
```

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/databases/relational_databases/__init__.pxd` & `OctoBot-Commons-1.9.0/octobot_commons/databases/relational_databases/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# cython: language_level=3
-#  Drakkar-Software OctoBot-Backtesting
+# pylint: disable=R0801
+#  Drakkar-Software OctoBot-Commons
 #  Copyright (c) Drakkar-Software, All rights reserved.
 #
 #  This library is free software; you can redistribute it and/or
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
 #
@@ -11,15 +11,19 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 
-from octobot_commons.databases.relational_databases cimport sqlite
-from octobot_commons.databases.relational_databases.sqlite cimport (
+
+from octobot_commons.databases.relational_databases import sqlite
+from octobot_commons.databases.relational_databases.sqlite import (
     SQLiteDatabase,
+    new_sqlite_database,
 )
 
+
 __all__ = [
     "SQLiteDatabase",
+    "new_sqlite_database",
 ]
```

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/databases/relational_databases/__init__.py` & `OctoBot-Commons-1.9.0/octobot_commons/display/plot_settings.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=R0801
+# pylint: disable=R0913
 #  Drakkar-Software OctoBot-Commons
 #  Copyright (c) Drakkar-Software, All rights reserved.
 #
 #  This library is free software; you can redistribute it and/or
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
@@ -10,20 +10,24 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
+import octobot_commons.enums as enums
 
 
-from octobot_commons.databases.relational_databases import sqlite
-from octobot_commons.databases.relational_databases.sqlite import (
-    SQLiteDatabase,
-    new_sqlite_database,
-)
-
-
-__all__ = [
-    "SQLiteDatabase",
-    "new_sqlite_database",
-]
+class PlotSettings:
+    def __init__(
+        self,
+        chart=enums.PlotCharts.MAIN_CHART.value,
+        x_multiplier=1000,
+        kind="scattergl",
+        mode="markers",
+        y_data=None,
+    ):
+        self.chart = chart
+        self.x_multiplier = x_multiplier
+        self.kind = kind
+        self.mode = mode
+        self.y_data = y_data
```

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/databases/relational_databases/sqlite/__init__.pxd` & `OctoBot-Commons-1.9.0/octobot_commons/support.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,29 @@
-# cython: language_level=3
-#  Drakkar-Software OctoBot-Backtesting
+#  Drakkar-Software OctoBot
 #  Copyright (c) Drakkar-Software, All rights reserved.
 #
 #  This library is free software; you can redistribute it and/or
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
 #
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
+import abc
 
-from octobot_commons.databases.relational_databases.sqlite cimport sqlite_database
-from octobot_commons.databases.relational_databases.sqlite.sqlite_database cimport (
-    SQLiteDatabase,
-)
 
-__all__ = [
-    "SQLiteDatabase",
-]
+class Support:
+    """
+    Abstract class to be implemented when using supports
+    """
+
+    @abc.abstractmethod
+    def is_supporting(self) -> bool:
+        """
+        Return True when supporting
+        """
+        raise NotImplementedError
```

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/databases/relational_databases/sqlite/__init__.py` & `OctoBot-Commons-1.9.0/octobot_commons/databases/run_databases/run_databases_pruning_factory.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# pylint: disable=W0703
 #  Drakkar-Software OctoBot-Commons
 #  Copyright (c) Drakkar-Software, All rights reserved.
 #
 #  This library is free software; you can redistribute it and/or
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
@@ -9,20 +10,20 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
+import octobot_commons.databases.run_databases.file_system_run_databases_pruner as file_system_run_databases_pruner
 
 
-from octobot_commons.databases.relational_databases.sqlite import sqlite_database
-from octobot_commons.databases.relational_databases.sqlite.sqlite_database import (
-    SQLiteDatabase,
-    new_sqlite_database,
-)
-
-
-__all__ = [
-    "SQLiteDatabase",
-    "new_sqlite_database",
-]
+def run_databases_pruner_factory(run_databases_identifier, max_db_size):
+    """
+    :return: A RunDatabasesPruner instance
+    """
+    if run_databases_identifier.database_adaptor.is_file_system_based():
+        return file_system_run_databases_pruner.FileSystemRunDatabasesPruner(
+            run_databases_identifier,
+            max_db_size,
+        )
+    raise NotImplementedError("Only file system based database pruner is implemented")
```

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/databases/relational_databases/sqlite/cursor_pool.pxd` & `OctoBot-Commons-1.9.0/tests/signals/test_signal.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,29 @@
-# cython: language_level=3
-#  Drakkar-Software OctoBot-Backtesting
+#  Drakkar-Software OctoBot-Commons
 #  Copyright (c) Drakkar-Software, All rights reserved.
 #
 #  This library is free software; you can redistribute it and/or
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
 #
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-#  Lesser General License for more details.
+#  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
+import octobot_commons.enums
 
-cdef class CursorPool:
-    cdef object _db_connection
-    cdef list _cursors
+from tests.signals import signal
+
+
+def test_to_dict(signal):
+    assert signal.to_dict() == {
+        octobot_commons.enums.SignalsAttrs.TOPIC.value: "hello topic",
+        octobot_commons.enums.SignalsAttrs.CONTENT.value: {"hi": "plop"},
+    }
+
+
+def test__str__(signal):
+    assert all(sub_str in str(signal) for sub_str in ("hello topic", "hi", "plop"))
```

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/databases/relational_databases/sqlite/cursor_pool.py` & `OctoBot-Commons-1.9.0/octobot_commons/databases/relational_databases/sqlite/cursor_pool.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/databases/relational_databases/sqlite/cursor_wrapper.pxd` & `OctoBot-Commons-1.9.0/octobot_commons/databases/relational_databases/sqlite/cursor_wrapper.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,27 @@
-# cython: language_level=3
 #  Drakkar-Software OctoBot-Backtesting
 #  Copyright (c) Drakkar-Software, All rights reserved.
 #
 #  This library is free software; you can redistribute it and/or
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
 #
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-#  Lesser General License for more details.
+#  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 
 
-cdef class CursorWrapper:
-    cdef public object cursor
-    cdef public bint idle
+class CursorWrapper:
+    def __init__(self, cursor):
+        self.cursor = cursor
+        self.idle = True
+
+    async def close(self):
+        """
+        Close the underlying cursor
+        """
+        await self.cursor.close()
```

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/databases/relational_databases/sqlite/cursor_wrapper.py` & `OctoBot-Commons-1.9.0/octobot_commons/list_util.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-#  Drakkar-Software OctoBot-Backtesting
+#  Drakkar-Software OctoBot-Commons
 #  Copyright (c) Drakkar-Software, All rights reserved.
 #
 #  This library is free software; you can redistribute it and/or
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
 #
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
+import functools
 
 
-class CursorWrapper:
-    def __init__(self, cursor):
-        self.cursor = cursor
-        self.idle = True
-
-    async def close(self):
-        """
-        Close the underlying cursor
-        """
-        await self.cursor.close()
+def flatten_list(list_to_flatten):
+    """
+    Flatten the list :list_to_flatten:
+    :param list_to_flatten: the list to flatten
+    :return: the flattened list
+    """
+    return functools.reduce(
+        lambda first_level, second_level: first_level + second_level, list_to_flatten
+    )
```

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/databases/relational_databases/sqlite/sqlite_database.py` & `OctoBot-Commons-1.9.0/octobot_commons/databases/relational_databases/sqlite/sqlite_database.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,14 +204,20 @@
         return await self.__execute_select(
             table=table,
             where_clauses=final_where_close,
             additional_clauses=self.__select_order_by(order_by, sort),
             size=size,
         )
 
+    async def delete(self, table, **kwargs):
+        return await self.__execute_delete(
+            table,
+            self.__where_clauses_from_kwargs(**kwargs),
+        )
+
     def __where_clauses_from_kwargs(self, should_quote_value=True, **kwargs) -> str:
         return self.__where_clauses_from_operations(
             list(kwargs.keys()),
             list(kwargs.values()),
             [],
             should_quote_value=should_quote_value,
         )
@@ -285,14 +291,19 @@
                 return await cursor.fetchall()
         except sqlite3.OperationalError as err:
             if not await self.check_table_exists(table):
                 raise errors.DatabaseNotFoundError(err)
             self.logger.error(f"An error occurred when executing select : {err}")
         return []
 
+    async def __execute_delete(self, table, where_clauses):
+        async with self.aio_cursor() as cursor:
+            await cursor.execute(f"DELETE FROM {table.value} WHERE {where_clauses} ")
+            # nothing to return, will raise on error
+
     async def check_table_exists(self, table) -> bool:
         async with self.aio_cursor() as cursor:
             await cursor.execute(
                 f"SELECT name FROM sqlite_master WHERE type='table' AND name='{table.value}'"
             )
             return await cursor.fetchall() != []
```

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/databases/run_databases/__init__.pxd` & `OctoBot-Commons-1.9.0/octobot_commons/tests/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-# cython: language_level=3
-#  Drakkar-Software OctoBot-Backtesting
+#  Drakkar-Software OctoBot-Commons
 #  Copyright (c) Drakkar-Software, All rights reserved.
 #
 #  This library is free software; you can redistribute it and/or
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
 #
@@ -11,15 +10,22 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 
-from octobot_commons.databases.run_databases cimport run_databases_provider
-from octobot_commons.databases.run_databases.run_databases_provider cimport (
-    RunDatabasesProvider,
+from octobot_commons.tests import test_config
+
+from octobot_commons.tests.test_config import (
+    get_test_config,
+    init_config_time_frame_for_tests,
+    load_test_config,
+    TEST_CONFIG_FOLDER,
 )
 
 __all__ = [
-    "RunDatabasesProvider",
+    "get_test_config",
+    "init_config_time_frame_for_tests",
+    "load_test_config",
+    "TEST_CONFIG_FOLDER",
 ]
```

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/databases/run_databases/__init__.py` & `OctoBot-Commons-1.9.0/octobot_commons/databases/run_databases/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/databases/run_databases/abstract_run_databases_pruner.py` & `OctoBot-Commons-1.9.0/octobot_commons/databases/run_databases/abstract_run_databases_pruner.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/databases/run_databases/file_system_run_databases_pruner.py` & `OctoBot-Commons-1.9.0/octobot_commons/databases/run_databases/file_system_run_databases_pruner.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/databases/run_databases/run_databases_identifier.py` & `OctoBot-Commons-1.9.0/octobot_commons/databases/run_databases/run_databases_identifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,20 @@
             if exchange is None
             else self._merge_parts(
                 self._base_folder(from_global_history=from_global_history), exchange
             )
         )
         await self.database_adaptor.create_identifier(deepest_identifier)
 
+    def is_backtesting(self) -> bool:
+        """
+        :return: True when the database identifier associated to a backtesting run
+        """
+        return self.backtesting_id is not None
+
     def get_run_data_db_identifier(self) -> str:
         """
         :return: the database identifier associated to the run database
         """
         return self._get_db_identifier(enums.RunDatabases.RUN_DATA_DB.value, None)
 
     def get_orders_db_identifier(self, account_type, exchange) -> str:
```

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/databases/run_databases/run_databases_provider.py` & `OctoBot-Commons-1.9.0/octobot_commons/databases/run_databases/run_databases_provider.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/databases/run_databases/run_databases_pruning_factory.py` & `OctoBot-Commons-1.9.0/octobot_commons/thread_util.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# pylint: disable=W0703
 #  Drakkar-Software OctoBot-Commons
 #  Copyright (c) Drakkar-Software, All rights reserved.
 #
 #  This library is free software; you can redistribute it and/or
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
@@ -10,20 +9,21 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-import octobot_commons.databases.run_databases.file_system_run_databases_pruner as file_system_run_databases_pruner
 
+import concurrent.futures as futures
 
-def run_databases_pruner_factory(run_databases_identifier, max_db_size):
+
+# pylint: disable=W0212
+def stop_thread_pool_executor_non_gracefully(executor: futures.ThreadPoolExecutor):
     """
-    :return: A RunDatabasesPruner instance
+    From https://gist.github.com/clchiou/f2608cbe54403edb0b13
+    Non graceful and non clean but only way to shutdown a ThreadPoolExecutor
+    :param executor: the ThreadPoolExecutor to stop
     """
-    if run_databases_identifier.database_adaptor.is_file_system_based():
-        return file_system_run_databases_pruner.FileSystemRunDatabasesPruner(
-            run_databases_identifier,
-            max_db_size,
-        )
-    raise NotImplementedError("Only file system based database pruner is implemented")
+    executor.shutdown(False)
+    executor._threads.clear()
+    futures.thread._threads_queues.clear()
```

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/databases/run_databases/storage.py` & `OctoBot-Commons-1.9.0/octobot_commons/databases/run_databases/storage.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,34 +9,52 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
+import json
+
 import octobot_commons.databases.run_databases.run_databases_provider as run_databases_provider
 import octobot_commons.configuration as configuration
+import octobot_commons.enums as enums
+import octobot_commons.logging as logging
 
 
 async def init_bot_storage(bot_id, run_database_identifier, clear_user_inputs):
     """
     Initializes the associated bot_id databases. Deletes any existing user input if clear_user_inputs is True
     """
     if not run_databases_provider.RunDatabasesProvider.instance().has_bot_id(bot_id):
         # only one run database per bot id
         await run_databases_provider.RunDatabasesProvider.instance().add_bot_id(
             bot_id, run_database_identifier
         )
-        if clear_user_inputs:
-            await configuration.clear_user_inputs(
-                run_databases_provider.RunDatabasesProvider.instance().get_run_db(
-                    bot_id
-                )
-            )
+        # always ensure database is valid
+        run_db = run_databases_provider.RunDatabasesProvider.instance().get_run_db(
+            bot_id
+        )
+        if run_database_identifier.enable_storage:
+            await _repair_database_if_necessary(run_db)
+            if clear_user_inputs:
+                await configuration.clear_user_inputs(run_db)
 
 
 async def close_bot_storage(bot_id):
     """
     :return: Close the bot_id associated run databases
     """
     if run_databases_provider.RunDatabasesProvider.instance().has_bot_id(bot_id):
         await run_databases_provider.RunDatabasesProvider.instance().close(bot_id)
+
+
+async def _repair_database_if_necessary(database):
+    try:
+        # will raise if the db has an issue
+        await database.all(enums.DBTables.METADATA.value)
+    except json.JSONDecodeError:
+        logging.get_logger(__name__).warning(
+            f"Invalid database at {database}, resetting content."
+        )
+        # error in database, reset it
+        await database.hard_reset()
```

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/databases/run_databases/utils.py` & `OctoBot-Commons-1.9.0/octobot_commons/databases/run_databases/utils.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/dict_util.py` & `OctoBot-Commons-1.9.0/octobot_commons/dict_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/display/__init__.py` & `OctoBot-Commons-1.9.0/octobot_commons/display/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/display/display_factory.py` & `OctoBot-Commons-1.9.0/octobot_commons/display/display_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/display/display_translator.py` & `OctoBot-Commons-1.9.0/octobot_commons/display/display_translator.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,19 +89,20 @@
         :param name: name of the part
         :param element_type: type of the part to add
         """
         element = self.__class__(element_type=element_type)
         self.nested_elements[name] = element
         yield element
 
-    def add_user_inputs(self, inputs, part=None):
+    def add_user_inputs(self, inputs, part=None, config_by_tentacles=None):
         """
         add user inputs to the given part or self
         """
-        config_by_tentacles = {}
+        has_forced_config = config_by_tentacles is not None
+        config_by_tentacles = config_by_tentacles or {}
         config_schema_by_tentacles = {}
         tentacle_type_by_tentacles = {}
         shown_tentacles = {}
         nested_user_inputs_by_tentacle = self._extract_nested_user_inputs(inputs)
         tentacle = None
         for user_input_element in inputs:
             try:
@@ -116,18 +117,20 @@
                 else:
                     shown_tentacles[tentacle] = True
                 tentacle_type_by_tentacles[tentacle] = user_input_element[
                     "tentacle_type"
                 ]
                 if tentacle not in config_schema_by_tentacles:
                     config_schema_by_tentacles[tentacle] = self._base_schema(tentacle)
-                    config_by_tentacles[tentacle] = {}
-                config_by_tentacles[tentacle][
-                    user_input_element["name"].replace(" ", "_")
-                ] = user_input_element["value"]
+                    if not has_forced_config:
+                        config_by_tentacles[tentacle] = {}
+                if tentacle not in config_by_tentacles:
+                    config_by_tentacles[tentacle][
+                        user_input_element["name"].replace(" ", "_")
+                    ] = user_input_element["value"]
                 if user_input_element["parent_input_name"] is None:
                     # user input with parent_input_name are added alongside their parents, only add top
                     # level user inputs in schema
                     self._generate_schema(
                         config_schema_by_tentacles[tentacle],
                         user_input_element,
                         nested_user_inputs_by_tentacle,
@@ -196,14 +199,19 @@
         if min_val is not None:
             properties["minimum"] = min_val
         max_val = user_input_element.get("max_val")
         if max_val is not None:
             properties["maximum"] = max_val
         if editor_options := user_input_element.get("editor_options"):
             properties["options"].update(editor_options)
+            if "dependencies" in editor_options:
+                other_values = user_input_element.get("other_schema_values", {}) or {}
+                # when using dependencies, set field as not required as it might not be set
+                other_values["required"] = other_values.get("required", False)
+                user_input_element["other_schema_values"] = other_values
         if other_schema_values := user_input_element.get("other_schema_values"):
             properties.update(other_schema_values)
         return properties
 
     def _adapt_to_input_type(
         self,
         user_input_element,
@@ -363,14 +371,16 @@
                 return self.INPUT_TYPE_TO_SCHEMA_TYPE[
                     enums.UserInputTypes.BOOLEAN.value
                 ]
             if isinstance(options[0], str):
                 return default_type
         except IndexError:
             pass
+        except TypeError as error:
+            raise TypeError("a user input element is malformed.") from error
         return default_type
 
     def add_user_inputs_element(
         self,
         name,
         config_values,
         schema,
```

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/display/plot_settings.py` & `OctoBot-Commons-1.9.0/octobot_commons/signals/signal_bundle.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=R0913
+# pylint: disable=C0116
 #  Drakkar-Software OctoBot-Commons
 #  Copyright (c) Drakkar-Software, All rights reserved.
 #
 #  This library is free software; you can redistribute it and/or
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
@@ -10,24 +10,36 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-import octobot_commons.enums as enums
+import octobot_commons.enums
 
 
-class PlotSettings:
-    def __init__(
-        self,
-        chart=enums.PlotCharts.MAIN_CHART.value,
-        x_multiplier=1000,
-        kind="scattergl",
-        mode="markers",
-        y_data=None,
-    ):
-        self.chart = chart
-        self.x_multiplier = x_multiplier
-        self.kind = kind
-        self.mode = mode
-        self.y_data = y_data
+class SignalBundle:
+    def __init__(self, identifier: str, signals=None, version=None):
+        self.identifier: str = identifier
+        self.signals: list = signals or []
+        self.version: str = version or self._get_version()
+
+    def to_dict(self) -> dict:
+        return {
+            octobot_commons.enums.SignalBundlesAttrs.IDENTIFIER.value: self.identifier,
+            octobot_commons.enums.SignalBundlesAttrs.SIGNALS.value: [
+                signal.to_dict() for signal in self.signals
+            ],
+            octobot_commons.enums.SignalBundlesAttrs.VERSION.value: self.version,
+        }
+
+    def __str__(self):
+        return f"{self.to_dict()}"
+
+    # pylint: disable=C0415
+    def _get_version(self) -> str:
+        try:
+            import octobot.constants
+
+            return octobot.constants.COMMUNITY_FEED_CURRENT_MINIMUM_VERSION
+        except ImportError:
+            return "1.0.0"
```

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/errors.py` & `OctoBot-Commons-1.9.0/octobot_commons/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,20 @@
 
 class ProfileRemovalError(Exception):
     """
     Profile related Exception: raised when the current profile can't be can't be removed
     """
 
 
+class ProfileImportError(Exception):
+    """
+    Profile related Exception: raised when the imported profile is invalid
+    """
+
+
 class ConfigEvaluatorError(Exception):
     """
     Evaluator config related Exception
     """
 
 
 class ConfigTradingError(Exception):
```

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/evaluator_util.pxd` & `OctoBot-Commons-1.9.0/tests/configuration/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# cython: language_level=3
 #  Drakkar-Software OctoBot-Commons
 #  Copyright (c) Drakkar-Software, All rights reserved.
 #
 #  This library is free software; you can redistribute it and/or
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
@@ -10,10 +9,7 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-
-cpdef bint check_valid_eval_note(object eval_note, object eval_type=*, object expected_eval_type=*,
-                                 object eval_time=*, object expiry_delay=*, object current_time=*)
```

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/evaluators_util.py` & `OctoBot-Commons-1.9.0/octobot_commons/evaluators_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/external_resources_manager.py` & `OctoBot-Commons-1.9.0/octobot_commons/external_resources_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/json_util.py` & `OctoBot-Commons-1.9.0/tests/profiles/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,21 +9,31 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-import json
-import jsonschema
+import os
 
+import pytest
+import pathlib
+import octobot_commons.profiles as profiles
+import octobot_commons.tests.test_config as test_config
 
-def validate(config, schema_file) -> None:
-    """
-    Validate a config file, raise upon validation error
-    :param config: the config
-    :param schema_file: the config schema
-    :return: None
-    """
-    with open(schema_file) as json_schema:
-        loaded_schema = json.load(json_schema)
-    jsonschema.validate(instance=config, schema=loaded_schema)
+
+def get_profile_path():
+    return test_config.TEST_CONFIG_FOLDER
+
+
+def get_profiles_path():
+    return pathlib.Path(get_profile_path()).parent
+
+
+@pytest.fixture
+def profile():
+    return profiles.Profile(get_profile_path())
+
+
+@pytest.fixture
+def invalid_profile():
+    return profiles.Profile(os.path.join(get_profile_path(), "invalid_profile"))
```

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/logging/__init__.pxd` & `OctoBot-Commons-1.9.0/octobot_commons/logging/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# cython: language_level=3
 #  Drakkar-Software OctoBot-Commons
 #  Copyright (c) Drakkar-Software, All rights reserved.
 #
 #  This library is free software; you can redistribute it and/or
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
@@ -11,30 +10,51 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 
-from octobot_commons.logging cimport logging_util
-
-from octobot_commons.logging.logging_util cimport (
+from octobot_commons.logging import logging_util
+from octobot_commons.logging.logging_util import (
     BotLogger,
     set_global_logger_level,
     get_global_logger_level,
+    get_logger_level_per_handler,
     get_logger,
     set_logging_level,
     get_backtesting_errors_count,
     reset_backtesting_errors,
     set_error_publication_enabled,
+    BACKTESTING_NEW_ERRORS_COUNT,
+    LOG_DATABASE,
+    LOG_NEW_ERRORS_COUNT,
+    logs_database,
+    error_notifier_callbacks,
+    LOGS_MAX_COUNT,
+    add_log,
+    get_errors_count,
+    reset_errors_count,
+    register_error_notifier,
 )
 
 __all__ = [
     "BotLogger",
     "set_global_logger_level",
     "get_global_logger_level",
+    "get_logger_level_per_handler",
     "get_logger",
     "set_logging_level",
     "get_backtesting_errors_count",
     "reset_backtesting_errors",
     "set_error_publication_enabled",
+    "BACKTESTING_NEW_ERRORS_COUNT",
+    "LOG_DATABASE",
+    "LOG_NEW_ERRORS_COUNT",
+    "logs_database",
+    "error_notifier_callbacks",
+    "LOGS_MAX_COUNT",
+    "add_log",
+    "get_errors_count",
+    "reset_errors_count",
+    "register_error_notifier",
 ]
```

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/logging/logging_util.py` & `OctoBot-Commons-1.9.0/octobot_commons/logging/logging_util.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,33 +42,42 @@
 def _default_callback(*_, **__):
     pass
 
 
 _ERROR_CALLBACK = _default_callback
 
 
-def set_global_logger_level(level) -> None:
+def set_global_logger_level(level, handler_levels=None) -> None:
     """
     Set the global logger level
     :param level: the level to set
     """
     logger = logging.getLogger()
     logger.setLevel(level)
-    for handler in logger.handlers:
-        handler.setLevel(level)
+    levels = handler_levels or [level] * len(logger.handlers)
+    for handler, updated_level in zip(logger.handlers, levels):
+        handler.setLevel(updated_level)
 
 
 def get_global_logger_level() -> object:
     """
     Return the global logger level
     :return: the global logger level
     """
     return logging.getLogger().getEffectiveLevel()
 
 
+def get_logger_level_per_handler() -> list:
+    """
+    Return the global logger level
+    :return: order handles logging levels
+    """
+    return [handler.level for handler in logging.getLogger().handlers]
+
+
 def get_logger(logger_name="Anonymous"):
     """
     Return the logger from the logger_name
     :param logger_name: the logger name
     :return: the logger from the logger name
     """
     return BotLogger(logger_name)
```

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/logical_operators.py` & `OctoBot-Commons-1.9.0/octobot_commons/logical_operators.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/multiprocessing_util.py` & `OctoBot-Commons-1.9.0/octobot_commons/multiprocessing_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/number_util.py` & `OctoBot-Commons-1.9.0/octobot_commons/number_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/optimization_campaign.py` & `OctoBot-Commons-1.9.0/octobot_commons/optimization_campaign.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/os_clock_sync.py` & `OctoBot-Commons-1.9.0/octobot_commons/os_clock_sync.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/os_util.py` & `OctoBot-Commons-1.9.0/octobot_commons/os_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/pretty_printer.py` & `OctoBot-Commons-1.9.0/octobot_commons/pretty_printer.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-
 import octobot_commons
 import octobot_commons.enums as enums
 import octobot_commons.constants as constants
 import octobot_commons.logging as logging_util
 import octobot_commons.symbols.symbol_util as symbol_util
 import octobot_commons.timestamp_util as timestamp_util
 import octobot_commons.number_util as number_util
@@ -56,16 +55,18 @@
                 dict_order.get(ExchangeConstantsOrderColumns.SIDE.value)
             )
         quantity = dict_order.get(ExchangeConstantsOrderColumns.AMOUNT.value, 0.0)
         price = dict_order.get(ExchangeConstantsOrderColumns.PRICE.value, 0.0)
 
         return (
             f"{code}{order_type.name.replace('_', ' ')}{code}: {code}"
-            f"{get_min_string_from_number(quantity)} {quantity_currency}{code} at {code}"
-            f"{get_min_string_from_number(price)} {market}{code} on {exchange_name.capitalize()}"
+            f"{get_min_string_from_number(quantity)} "
+            f"{quantity_currency}{code} at {code}"
+            f"{get_min_string_from_number(price)} {market}{code} "
+            f"on {exchange_name.capitalize()}"
         )
     except ImportError:
         LOGGER.error(
             "open_order_pretty_printer requires OctoBot-Trading package installed"
         )
     return ""
 
@@ -91,15 +92,16 @@
                 trade.executed_time, time_format=ORDER_TIME_FORMAT
             )
             if trade.executed_time
             else ""
         )
         return (
             f"{code}{trade_type.name.replace('_', ' ')}{code}: {code}"
-            f"{get_min_string_from_number(trade.executed_quantity)} {trade.quantity_currency}{code} at {code}"
+            f"{get_min_string_from_number(trade.executed_quantity)} "
+            f"{trade.quantity_currency}{code} at {code}"
             f"{get_min_string_from_number(trade.executed_price)} {trade.market}{code} "
             f"{exchange_name.capitalize()} "
             f"{trade_executed_time_str} "
         )
     except ImportError:
         LOGGER.error(
             "open_order_pretty_printer requires OctoBot-Trading package installed"
@@ -111,54 +113,137 @@
     """
     Cryptocurrency alert
     :param result: the result
     :param final_eval: the final eval
     :return: alert and the markdown alert
     """
     try:
-        from telegram.utils.helpers import escape_markdown
+        import telegram.helpers
 
         _, _, code = get_markers(True)
         display_result = str(result).split(".")[1].replace("_", " ")
         alert = f"Result : {display_result}\n" f"Evaluation : {final_eval}"
         alert_markdown = (
             f"Result : {code}{display_result}{code}\n"
-            f"Evaluation : {code}{escape_markdown(str(final_eval))}{code}"
+            f"Evaluation : {code}{telegram.helpers.escape_markdown(str(final_eval))}{code}"
         )
         return alert, alert_markdown
     except ImportError:
         LOGGER.error("cryptocurrency_alert requires Telegram package installed")
     return "", ""
 
 
+def _get_row_pretty_portfolio_row(holdings, currency, ref_market, ref_market_value):
+    """
+    :return: the portfolio row adapted for a raw format
+    """
+    str_holdings = get_min_string_from_number(holdings)
+    if ref_market:
+        return f"{str_holdings} {currency}{get_min_string_from_number(ref_market_value)} {ref_market}"
+    return f"{str_holdings} {currency}"
+
+
+def _get_max_digits(number):
+    abs_number = abs(number)
+    if abs_number < 0.0001:
+        return 8
+    if abs_number < 0.01:
+        return 6
+    if abs_number < 1:
+        return 4
+    if abs_number < 1000:
+        return 2
+    return 0
+
+
+def _get_markdown_pretty_portfolio_row(
+    holdings, currency, ref_market, ref_market_value
+):
+    """
+    :return: the portfolio row adapted for a markdown format
+    """
+    str_currency = "{:<4}".format(currency)
+    str_holdings = "{:<12}".format(get_min_string_from_number(holdings))
+    str_ref_market_value = "{:<12}".format("")
+    if ref_market:
+        str_ref_market_value = "{:<12}".format(
+            get_min_string_from_number(ref_market_value)
+        )
+    return f"{str_currency} {str_holdings} {str_ref_market_value}"
+
+
 def global_portfolio_pretty_print(
-    global_portfolio, separator="\n", markdown=False
+    global_portfolio,
+    currency_values=None,
+    ref_market_name=None,
+    separator="\n",
+    markdown=False,
 ) -> str:
     """
     Global portfolio pretty printer
     :param global_portfolio: the global portfolio
+    :param currency_values: dict of current currency values {"BTC": 20000, "ETH": 1000 }
+    :param ref_market_name: current ref market "USD"
     :param separator: the printer separator
     :param markdown: if printer use markdown
     :return: the global portfolio pretty printed
     """
-    result = []
-    for currency, asset_dict in global_portfolio.items():
+    results = []
+    currency = "currency"
+    holdings = "holdings"
+    value = "value"
+    for asset, asset_dict in global_portfolio.items():
         if asset_dict[constants.PORTFOLIO_TOTAL] > 0:
             # fill lines with empty spaces if necessary
-            total = get_min_string_from_number(asset_dict[constants.PORTFOLIO_TOTAL])
-            if markdown:
-                total = "{:<10}".format(total)
-            available = f"({get_min_string_from_number(asset_dict[constants.PORTFOLIO_AVAILABLE])})"
-            if markdown:
-                available = "{:<12}".format(available)
-
-            holding_str = f"{total} {available} {currency}"
-            result.append(holding_str)
-
-    return separator.join(result)
+            holdings_value = 0
+            if currency_values and ref_market_name:
+                if ref_market_name == asset:
+                    holdings_value = asset_dict[constants.PORTFOLIO_TOTAL]
+                else:
+                    try:
+                        holdings_value = (
+                            currency_values[asset]
+                            * asset_dict[constants.PORTFOLIO_TOTAL]
+                        )
+                    except KeyError:
+                        # no currency value
+                        pass
+            results.append(
+                {
+                    currency: asset,
+                    holdings: asset_dict[constants.PORTFOLIO_TOTAL],
+                    value: holdings_value,
+                }
+            )
+    # force "value" str for cythonization
+    results.sort(key=lambda r: r["value"], reverse=True)
+    if markdown:
+        header = (
+            f"{'{:<4}'.format('')} "
+            f"{'  {:<9}'.format('Holdings')}  "
+            f"{'    {:<7}'.format(ref_market_name or '')}"
+        )
+        header_separator = f"{'-' * 4}|{'-' * 12}|{'-' * 12}"
+        content = separator.join(
+            [
+                _get_markdown_pretty_portfolio_row(
+                    result[holdings], result[currency], ref_market_name, result[value]
+                )
+                for result in results
+            ]
+        )
+        return f"{header}\n{header_separator}\n{content}"
+    return separator.join(
+        [
+            _get_row_pretty_portfolio_row(
+                result[holdings], result[currency], ref_market_name, result[value]
+            )
+            for result in results
+        ]
+    )
 
 
 def portfolio_profitability_pretty_print(
     profitability, profitability_percent, reference
 ) -> str:
     """
     Profitability pretty printer
@@ -202,21 +287,22 @@
     :return: the rounded number
     """
     if number is None:
         return 0
     return float(get_min_string_from_number(number, max_digits))
 
 
-def get_min_string_from_number(number, max_digits=8) -> str:
+def get_min_string_from_number(number, max_digits=None) -> str:
     """
     Get a min string from number
     :param number: the number
     :param max_digits: the mex digits
     :return: the string from number
     """
+    max_digits = _get_max_digits(number) if max_digits is None else max_digits
     if number is None or round(number, max_digits) == 0.0:
         return "0"
     if number % 1 != 0:
         number_str = number_util.round_into_str_with_max_digits(number, max_digits)
         # remove post comma trailing 0
         if "." in number_str:
             # remove "0" first and only the "." to avoid removing 2x"0" in 10.0 and returning 1 for example.
```

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/profiles/__init__.py` & `OctoBot-Commons-1.9.0/octobot_commons/profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/profiles/profile.py` & `OctoBot-Commons-1.9.0/octobot_commons/profiles/profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 #  License along with this library.
 import json
 import copy
 import os
 import shutil
 import uuid
 import octobot_commons.constants as constants
+import octobot_commons.enums as enums
 import octobot_commons.logging as commons_logging
 import octobot_commons.json_util as json_util
 import octobot_commons.errors as errors
 
 
 class Profile:
     """
@@ -65,34 +66,46 @@
         self.name: str = None
         self.description: str = None
         self.avatar: str = None
         self.avatar_path: str = None
         self.origin_url: str = None
         self.read_only: bool = False
         self.imported: bool = False
+        self.complexity: enums.ProfileComplexity = enums.ProfileComplexity.MEDIUM
+        self.risk: enums.ProfileRisk = enums.ProfileRisk.MODERATE
+        self.profile_type: enums.ProfileType = enums.ProfileType.LIVE
 
         self.config: dict = {}
 
     def read_config(self):
         """
         Reads a profile from self.path
         :return: self
         """
-        with open(self.config_file()) as profile_file:
-            parsed_profile = json.load(profile_file)
-            profile_config = parsed_profile.get(constants.CONFIG_PROFILE, {})
-            self.profile_id = profile_config.get(constants.CONFIG_ID, str(uuid.uuid4()))
-            self.name = profile_config.get(constants.CONFIG_NAME, "")
-            self.description = profile_config.get(constants.CONFIG_DESCRIPTION, "")
-            self.avatar = profile_config.get(constants.CONFIG_AVATAR, "")
-            self.origin_url = profile_config.get(constants.CONFIG_ORIGIN_URL, None)
-            self.read_only = profile_config.get(constants.CONFIG_READ_ONLY, False)
-            self.imported = profile_config.get(constants.CONFIG_IMPORTED, False)
-            self.config = parsed_profile[constants.PROFILE_CONFIG]
-
+        parsed_profile = json_util.read_file(self.config_file())
+        profile_config = parsed_profile.get(constants.CONFIG_PROFILE, {})
+        self.profile_id = profile_config.get(constants.CONFIG_ID, str(uuid.uuid4()))
+        self.name = profile_config.get(constants.CONFIG_NAME, "")
+        self.description = profile_config.get(constants.CONFIG_DESCRIPTION, "")
+        self.avatar = profile_config.get(constants.CONFIG_AVATAR, "")
+        self.origin_url = profile_config.get(constants.CONFIG_ORIGIN_URL, None)
+        self.read_only = profile_config.get(constants.CONFIG_READ_ONLY, False)
+        self.imported = profile_config.get(constants.CONFIG_IMPORTED, False)
+        self.complexity = enums.ProfileComplexity(
+            profile_config.get(
+                constants.CONFIG_COMPLEXITY, enums.ProfileComplexity.MEDIUM.value
+            )
+        )
+        self.risk = enums.ProfileRisk(
+            profile_config.get(constants.CONFIG_RISK, enums.ProfileRisk.MODERATE.value)
+        )
+        self.profile_type = enums.ProfileType(
+            profile_config.get(constants.CONFIG_TYPE, enums.ProfileType.LIVE.value)
+        )
+        self.config = parsed_profile[constants.PROFILE_CONFIG]
         if self.avatar:
             avatar_path = os.path.join(self.path, self.avatar)
             if os.path.isfile(avatar_path):
                 self.avatar_path = avatar_path
         return self
 
     def save_config(self, global_config: dict):
@@ -222,14 +235,17 @@
                 constants.CONFIG_ID: self.profile_id,
                 constants.CONFIG_NAME: self.name,
                 constants.CONFIG_DESCRIPTION: self.description,
                 constants.CONFIG_AVATAR: self.avatar,
                 constants.CONFIG_ORIGIN_URL: self.origin_url,
                 constants.CONFIG_READ_ONLY: self.read_only,
                 constants.CONFIG_IMPORTED: self.imported,
+                constants.CONFIG_COMPLEXITY: self.complexity.value,
+                constants.CONFIG_RISK: self.risk.value,
+                constants.CONFIG_TYPE: self.profile_type.value,
             },
             constants.PROFILE_CONFIG: self.config,
         }
 
     def config_file(self):
         """
         :return: the path to this profile config file
```

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/profiles/profile_sharing.py` & `OctoBot-Commons-1.9.0/octobot_commons/profiles/profile_sharing.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,22 +18,36 @@
 import os
 import zipfile
 import shutil
 import pathlib
 import uuid
 import time
 import requests
+import jsonschema
 import octobot_commons.constants as constants
 import octobot_commons.logging as bot_logging
 import octobot_commons.errors as errors
+import octobot_commons.json_util as json_util
 
 # avoid cyclic import
 from octobot_commons.profiles.profile import Profile
 
 
+NON_OVERWRITTEN_PROFILE_FOLDERS = []
+NON_OVERWRITTEN_PROFILE_FILES = [constants.PROFILE_CONFIG_FILE]
+try:
+    import octobot_tentacles_manager.constants as tentacles_manager_constants
+
+    NON_OVERWRITTEN_PROFILE_FOLDERS.append(
+        tentacles_manager_constants.TENTACLES_SPECIFIC_CONFIG_FOLDER
+    )
+except ImportError:
+    pass
+
+
 def export_profile(profile, export_path: str) -> str:
     """
     Exports the given profile into export_path, appends ".zip" as a file extension
     :param profile: profile to export
     :param export_path: export path ending with filename
     :return: the exported profile path including file extension
     """
@@ -59,67 +73,81 @@
     import_path: str,
     profile_name: str,
     bot_install_path: str,
     replace_if_exists: bool,
     is_imported: bool,
     origin_url: str = None,
     quite: bool = False,
+    profile_schema: str = None,
 ) -> Profile:
     """
     Installs the given profile export archive into the user's profile directory
     :param import_path: path to the profile zipped archive
     :param profile_name: name of the profile folder
     :param bot_install_path: path to the octobot installation
     :param replace_if_exists: when True erase the profile with the same name if it exists
-    :param is_imported: when True erase the profile is set as imported
+    :param is_imported: when True the profile is set as imported
     :param origin_url: url the profile is coming from (if relevant)
     :param quite: when True, only log errors
+    :param profile_schema: the schema to validate profile against
     :return: The created profile
     """
     logger = bot_logging.get_logger("ProfileSharing")
-    target_import_path, replaced = _get_target_import_path(
+    target_import_path = _get_target_import_path(
         bot_install_path, profile_name, replace_if_exists
     )
     action = "Creat"
-    if replaced:
+    if replace_if_exists:
         action = "Updat"
     if not quite:
         logger.info(f"{action}ing {profile_name} profile.")
     _import_profile_files(import_path, target_import_path)
-    profile = Profile(target_import_path).read_config()
+    profile = Profile(target_import_path, schema_path=profile_schema).read_config()
     profile.imported = is_imported
     profile.origin_url = origin_url
     _ensure_unique_profile_id(profile)
+    if is_imported:
+        try:
+            profile.validate()
+        except jsonschema.exceptions.ValidationError as err:
+            shutil.rmtree(target_import_path)
+            raise errors.ProfileImportError(
+                f"Invalid imported profile: {err.message} in '{'/'.join(err.absolute_path)}'"
+            ) from err
+    profile.save()
     if not quite:
         logger.info(f"{action}ed {profile.name} ({profile_name}) profile.")
     return profile
 
 
 def import_profile(
     import_path: str,
+    profile_schema: str,
     name: str = None,
     bot_install_path: str = ".",
     origin_url: str = None,
 ) -> Profile:
     """
     Imports the given profile export archive into the user's profile directory with the "imported_" prefix
     :param import_path: path to the profile zipped archive
+    :param profile_schema: the schema to validate profile against
     :param name: name of the profile folder
     :param bot_install_path: path to the octobot installation
     :param origin_url: url the profile is coming from
     :return: The created profile
     """
     temp_profile_name = _get_profile_name(name, import_path)
     profile = install_profile(
         import_path,
         temp_profile_name,
         bot_install_path,
         False,
         True,
         origin_url=origin_url,
+        profile_schema=profile_schema,
     )
     if profile.name != temp_profile_name:
         profile.rename_folder(_get_unique_profile_folder_from_name(profile), False)
     return profile
 
 
 def download_profile(url, target_file, timeout=60):
@@ -135,25 +163,28 @@
         req.raise_for_status()
         with open(target_file, "wb") as write_file:
             for chunk in req.iter_content(chunk_size=8192):
                 write_file.write(chunk)
     return target_file
 
 
-def download_and_install_profile(download_url):
+def download_and_install_profile(download_url, profile_schema):
     """
     :param download_url: profile url
+    :param profile_schema: the schema to validate profile against
     :return: the installed profile, None if an error occurred
     """
     logger = bot_logging.get_logger("ProfileSharing")
     name = download_url.split("/")[-1]
     file_path = None
     try:
         file_path = download_profile(download_url, name)
-        profile = import_profile(file_path, name=name, origin_url=download_url)
+        profile = import_profile(
+            file_path, profile_schema, name=name, origin_url=download_url
+        )
         logger.info(
             f"Downloaded and installed {profile.name} from {profile.origin_url}"
         )
         return profile
     except errors.UnsupportedError as err:
         logger.error(f"Error when installing profile: {err}")
         return None
@@ -171,16 +202,15 @@
     )
     return profile_name.split(f".{constants.PROFILE_EXPORT_FORMAT}")[0]
 
 
 def _filter_profile_export(profile_path: str):
     profile_file = os.path.join(profile_path, constants.PROFILE_CONFIG_FILE)
     if os.path.isfile(profile_file):
-        with open(profile_file) as open_file:
-            parsed_profile = json.load(open_file)
+        parsed_profile = json_util.read_file(profile_file)
         _filter_disabled(parsed_profile, constants.CONFIG_EXCHANGES)
         with open(profile_file, "w") as open_file:
             json.dump(parsed_profile, open_file, indent=4, sort_keys=True)
 
 
 def _filter_disabled(profile_config: dict, element):
     filtered_exchanges = {
@@ -191,51 +221,82 @@
         if details.get(constants.CONFIG_ENABLED_OPTION, True)
     }
     profile_config[constants.PROFILE_CONFIG][element] = filtered_exchanges
 
 
 def _get_target_import_path(
     bot_install_path: str, profile_name: str, replace_if_exists: bool
-) -> (str, bool):
+) -> str:
     """
     Get the target profile folder path
     :param bot_install_path: path to the octobot installation
     :param profile_name: name of the profile folder
     :param replace_if_exists: when True erase the profile with the same name if it exists
     :return: (the final target import path, True if the profile is replaced)
     """
     target_import_path = os.path.join(
         bot_install_path, constants.USER_PROFILES_FOLDER, profile_name
     )
     if replace_if_exists:
-        try:
-            replaced = True
-            shutil.rmtree(target_import_path)
-        except FileNotFoundError:
-            replaced = False
-        return target_import_path, replaced
-    return _get_unique_profile_folder(target_import_path), False
+        return target_import_path
+    return _get_unique_profile_folder(target_import_path)
 
 
 def _import_profile_files(profile_path: str, target_profile_path: str) -> None:
     """
-    Copy or extract profile files to destination
+    Copy or extract profile files to destination. Does not override local tentacles configuration
     :param profile_path: the current profile path
     :param target_profile_path: the target profile path
     :return: None
     """
     if zipfile.is_zipfile(profile_path):
-        with zipfile.ZipFile(profile_path) as zipped:
-            zipped.extractall(target_profile_path)
+        with zipfile.ZipFile(profile_path) as zipped_profile:
+            for archive_member in zipped_profile.namelist():
+                if _should_profile_file_be_imported(
+                    target_profile_path, archive_member
+                ):
+                    zipped_profile.extract(archive_member, target_profile_path)
     else:
         if not os.path.isdir(profile_path):
             raise errors.UnsupportedError(
                 f"Profile format not supported ({profile_path})"
             )
-        shutil.copytree(profile_path, target_profile_path)
+
+        def _get_ignored_elements(current_dir, sub_elements):
+            return [
+                element
+                for element in sub_elements
+                if not _should_profile_file_be_imported(
+                    target_profile_path,
+                    os.path.join(current_dir, element).replace(
+                        f"{profile_path}{os.path.sep}", ""
+                    ),  # force local path
+                )
+            ]
+
+        shutil.copytree(
+            profile_path,
+            target_profile_path,
+            ignore=_get_ignored_elements,
+            dirs_exist_ok=True,
+        )
+
+
+def _should_profile_file_be_imported(
+    target_profile_path: str, profile_file_path: str
+) -> bool:
+    for non_overwritten_element in NON_OVERWRITTEN_PROFILE_FOLDERS:
+        # ignore files in NON_OVERWRITTEN_PROFILE_FOLDERS that already exist
+        element_path = pathlib.Path(profile_file_path)
+        if (
+            element_path.name in NON_OVERWRITTEN_PROFILE_FILES
+            or non_overwritten_element in element_path.parts[:-1]
+        ) and os.path.isfile(os.path.join(target_profile_path, profile_file_path)):
+            return False
+    return True
 
 
 def _get_unique_profile_folder_from_name(profile) -> str:
     folder = _get_unique_profile_folder(
         os.path.join(os.path.split(profile.path)[0], profile.name)
     )
     return os.path.split(folder)[1]
@@ -264,8 +325,7 @@
     ids = Profile.get_all_profiles_ids(
         pathlib.Path(profile.path).parent, ignore=profile.path
     )
     iteration = 1
     while profile.profile_id in ids and iteration < 100:
         profile.profile_id = str(uuid.uuid4())
         iteration += 1
-    profile.save()
```

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/signals/__init__.py` & `OctoBot-Commons-1.9.0/octobot_commons/signals/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/signals/signal.py` & `OctoBot-Commons-1.9.0/octobot_commons/signals/signal.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/signals/signal_builder_wrapper.py` & `OctoBot-Commons-1.9.0/octobot_commons/signals/signal_builder_wrapper.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/signals/signal_bundle.py` & `OctoBot-Commons-1.9.0/octobot_commons/signals/signal_bundle_builder.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,62 @@
-# pylint: disable=C0116
-#  Drakkar-Software OctoBot-Commons
+#  Drakkar-Software OctoBot-Trading
 #  Copyright (c) Drakkar-Software, All rights reserved.
 #
 #  This library is free software; you can redistribute it and/or
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
 #
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-import octobot_commons.enums
+import octobot_commons.signals.signal_bundle as signal_bundle
+import octobot_commons.signals.signal as signal
 
 
-class SignalBundle:
-    def __init__(self, identifier: str, signals=None, version=None):
-        self.identifier: str = identifier
-        self.signals: list = signals or []
-        self.version: str = version or self._get_version()
+class SignalBundleBuilder:
+    DEFAULT_SIGNAL_CLASS = signal.Signal
 
-    def to_dict(self) -> dict:
-        return {
-            octobot_commons.enums.SignalBundlesAttrs.IDENTIFIER.value: self.identifier,
-            octobot_commons.enums.SignalBundlesAttrs.SIGNALS.value: [
-                signal.to_dict() for signal in self.signals
-            ],
-            octobot_commons.enums.SignalBundlesAttrs.VERSION.value: self.version,
-        }
-
-    def __str__(self):
-        return f"{self.to_dict()}"
-
-    # pylint: disable=C0415
-    def _get_version(self) -> str:
-        try:
-            import octobot.constants
-
-            return octobot.constants.COMMUNITY_FEED_CURRENT_MINIMUM_VERSION
-        except ImportError:
-            return "1.0.0"
+    def __init__(self, identifier: str):
+        self.signals: list = []
+        self.identifier: str = identifier
+        self.version: str = None
+        self.signal_class = self.__class__.DEFAULT_SIGNAL_CLASS
+        self.reset()
+
+    def register_signal(self, topic: str, content: dict, **kwargs):
+        """
+        Store a signal to be packed on build call
+        """
+        self.signals.append(self.create_signal(topic, content, **kwargs))
+
+    def create_signal(self, topic: str, content: dict, **kwargs):
+        """
+        Create a signal from self.signal_class
+        """
+        return self.signal_class(topic, content, **kwargs)
+
+    def is_empty(self) -> bool:
+        """
+        Return True when no signal are to be built
+        """
+        return not self.signals
+
+    def build(self) -> signal_bundle.SignalBundle:
+        """
+        Create a signal_bundle.SignalBundle from registered signals
+        """
+        return signal_bundle.SignalBundle(
+            self.identifier,
+            signals=self.signals,
+            version=self.version,
+        )
+
+    def reset(self):
+        """
+        Remove all registered signals
+        """
+        self.signals = []
```

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/signals/signal_factory.py` & `OctoBot-Commons-1.9.0/octobot_commons/signals/signal_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/signals/signal_publisher.py` & `OctoBot-Commons-1.9.0/octobot_commons/signals/signal_publisher.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/singleton/singleton_class.py` & `OctoBot-Commons-1.9.0/octobot_commons/singleton/singleton_class.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/symbols/__init__.py` & `OctoBot-Commons-1.9.0/octobot_commons/symbols/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/symbols/symbol.py` & `OctoBot-Commons-1.9.0/octobot_commons/symbols/symbol.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/symbols/symbol_util.py` & `OctoBot-Commons-1.9.0/octobot_commons/symbols/symbol_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/system_resources_watcher.py` & `OctoBot-Commons-1.9.0/octobot_commons/system_resources_watcher.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,56 +11,94 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 import threading
+import csv
+import gc
 
 import octobot_commons.constants as commons_constants
 import octobot_commons.singleton as singleton
+import octobot_commons.timestamp_util as timestamp_util
 import octobot_commons.logging as logging
 import octobot_commons.async_job as async_job
 import octobot_commons.os_util as os_util
 
 
 class SystemResourcesWatcher(singleton.Singleton):
     DEFAULT_WATCHER_INTERVAL = (
         commons_constants.RESOURCES_WATCHER_MINUTES_INTERVAL
         * commons_constants.MINUTE_TO_SECONDS
     )
     CPU_WATCHING_SECONDS = 2
 
-    def __init__(self):
+    def __init__(self, dump_resources, output_file):
         super().__init__()
         self.watcher_job = None
         self.watcher_interval = self.DEFAULT_WATCHER_INTERVAL
         self.logger = logging.get_logger(self.__class__.__name__)
+        self.dump_resources = dump_resources
+        self.output_file = output_file
+        self.initialized_output = False
 
     def _exec_log_used_resources(self):
         try:
+            # trigger garbage collector to get a fresh memory picture
+            gc.collect()
             # warning: blocking to monitor CPU usage, to be used in a thread
             cpu, percent_ram, ram, process_ram = os_util.get_cpu_and_ram_usage(
                 self.CPU_WATCHING_SECONDS
             )
             self.logger.debug(
                 f"Used system resources: {cpu}% CPU, {round(ram, 3)} GB in RAM ({percent_ram}% of total "
-                f"including {round(process_ram, 3)} GB from this process). "
+                f"including {process_ram} GB from this process). "
             )
+            if self.dump_resources:
+                self._dump_resources(cpu, percent_ram, ram, process_ram)
         except Exception as err:
             self.logger.exception(err, False)
             self.logger.debug(f"Error when checking system resources: {err}")
 
     async def _log_used_resources(self):
         threading.Thread(
             target=self._exec_log_used_resources,
             daemon=True,
             name=f"{self.__class__.__name__}-_exec_log_used_resources",
         ).start()
 
+    def _dump_resources(self, cpu, percent_ram, ram, process_ram):
+        reset_file = not self.initialized_output
+        self.initialized_output = True
+        mode = "w" if reset_file else "a"
+        row = (
+            str(element).replace(".", ",")
+            for element in (
+                timestamp_util.get_now_time(),
+                process_ram,
+                cpu,
+                percent_ram,
+                ram,
+            )
+        )
+        with open(self.output_file, mode, newline="") as csv_file:
+            writer = csv.writer(csv_file, delimiter=";")
+            if reset_file:
+                writer.writerow(
+                    [
+                        "TIME",
+                        "PROCESS USED RAM",
+                        "% USED CPU",
+                        "% USED RAM",
+                        "TOTAL USED RAM",
+                    ]
+                )
+            writer.writerow(row)
+
     async def start(self):
         """
         Synch the clock and start the clock synchronization loop if possible on this system
         """
         self.logger.debug("Starting system resources watcher")
         self.watcher_job = async_job.AsyncJob(
             self._log_used_resources,
@@ -73,19 +111,19 @@
         Stop the synchronization loop
         """
         if self.watcher_job is not None and not self.watcher_job.is_stopped():
             self.logger.debug("Stopping system resources watcher")
             self.watcher_job.stop()
 
 
-async def start_system_resources_watcher():
+async def start_system_resources_watcher(dump_resources, output_file):
     """
     Start the resources watcher loop
     """
-    await SystemResourcesWatcher.instance().start()
+    await SystemResourcesWatcher.instance(dump_resources, output_file).start()
 
 
 async def stop_system_resources_watcher():
     """
     Stop the watcher loop
     """
     return SystemResourcesWatcher.instance().stop()
```

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/tentacles_management/__init__.pxd` & `OctoBot-Commons-1.9.0/octobot_commons/tentacles_management/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# cython: language_level=3
 #  Drakkar-Software OctoBot-Commons
 #  Copyright (c) Drakkar-Software, All rights reserved.
 #
 #  This library is free software; you can redistribute it and/or
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
@@ -11,32 +10,37 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 
-from octobot_commons.tentacles_management cimport class_inspector
+from octobot_commons.tentacles_management import abstract_tentacle
+from octobot_commons.tentacles_management import class_inspector
 
-from octobot_commons.tentacles_management.class_inspector cimport (
+from octobot_commons.tentacles_management.abstract_tentacle import AbstractTentacle
+from octobot_commons.tentacles_management.class_inspector import (
     default_parent_inspection,
     default_parents_inspection,
     evaluator_parent_inspection,
     trading_mode_parent_inspection,
     get_class_from_parent_subclasses,
     get_deep_class_from_parent_subclasses,
+    get_class_from_string,
     is_abstract_using_inspection_and_class_naming,
     get_all_classes_from_parent,
     get_single_deepest_child_class,
 )
 
 __all__ = [
+    "AbstractTentacle",
     "default_parent_inspection",
     "default_parents_inspection",
     "evaluator_parent_inspection",
     "trading_mode_parent_inspection",
     "get_class_from_parent_subclasses",
     "get_deep_class_from_parent_subclasses",
+    "get_class_from_string",
     "is_abstract_using_inspection_and_class_naming",
     "get_all_classes_from_parent",
     "get_single_deepest_child_class",
 ]
```

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/tentacles_management/abstract_tentacle.py` & `OctoBot-Commons-1.9.0/octobot_commons/tentacles_management/abstract_tentacle.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,30 +15,41 @@
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 import abc
 import copy
 
 
 import octobot_commons.enums as commons_enums
+import octobot_commons.configuration.user_inputs as user_inputs
 import octobot_commons.configuration as configuration
-import octobot_commons.databases as databases
 
 
 class AbstractTentacle:
     """
     The parent class of any OctoBot tentacle
     """
 
     __metaclass__ = abc.ABCMeta
-    ALLOW_SUPER_CLASS_CONFIG = False
-    USER_INPUT_TENTACLE_TYPE = commons_enums.UserInputTentacleTypes.UNDEFINED
+
+    ALLOW_SUPER_CLASS_CONFIG = (
+        False  # when True, the given tentacle can read its parent class configuration
+    )
+    USER_INPUT_TENTACLE_TYPE = (
+        commons_enums.UserInputTentacleTypes.UNDEFINED
+    )  # tentacle type, saved in user inputs
+    HISTORIZE_USER_INPUT_CONFIG = (
+        False  # when True, user input values can be saved and read from the run data db
+    )
+    CLASS_UI = user_inputs.UserInputFactory(
+        commons_enums.UserInputTentacleTypes.UNDEFINED
+    )  # class-level user input factory. Used when initializing user inputs with classmethods
 
     def __init__(self):
         self.logger = None
-        self.UI: configuration.UserInputFactory = configuration.UserInputFactory(
+        self.UI: user_inputs.UserInputFactory = user_inputs.UserInputFactory(
             self.USER_INPUT_TENTACLE_TYPE
         )
         self.UI.set_tentacle_class(self.__class__).set_tentacle_config_proxy(
             self.get_local_config
         )
 
     @classmethod
@@ -58,83 +69,90 @@
         subclasses_list = cls.__subclasses__()
         if cls.__subclasses__():
             for subclass in copy.deepcopy(subclasses_list):
                 subclasses_list += subclass.get_all_subclasses()
         return subclasses_list
 
     @classmethod
+    def is_configurable(cls):
+        """
+        Override if the tentacle is allowed to be configured
+        """
+        return True
+
+    @classmethod
     def get_user_commands(cls) -> dict:
         """
         Return the dict of user commands for this tentacle
         :return: the commands dict
         """
         return {}
 
     def get_local_config(self):
         """
+        Implementation required if cls.HISTORIZE_USER_INPUT_CONFIG is True
         :return: the config of the tentacle
         """
         raise NotImplementedError
 
     @classmethod
     def create_local_instance(cls, config, tentacles_setup_config, tentacle_config):
         """
+        Implementation required if cls.HISTORIZE_USER_INPUT_CONFIG is True
         :param config: the global configuration to give to the tentacle
         :param tentacles_setup_config: the global tentacles setup configuration to give to the tentacle
         :param tentacle_config: the tentacle configuration to give to the tentacle
         :return: a local, aimed to be short-lived, tentacle instance
         """
         raise NotImplementedError
 
     def init_user_inputs(self, inputs: dict) -> None:
         """
+        instance method API for user inputs. Used by load_and_save_user_inputs
+        Override if this tentacle has user inputs that should be initialized on a specific instance
         Called right before starting the tentacle, should define all the tentacle's user inputs unless
         those are defined somewhere else.
         """
 
-    async def load_and_save_user_inputs(self, bot_id: str):
+    @classmethod
+    def init_user_inputs_from_class(cls, inputs: dict) -> None:
         """
-        Initialize and save the user inputs of the tentacle
+        classmethod API for user inputs. Used by init_user_inputs_from_class
+        Override if this tentacle has user inputs that can be initialized on a class level
+        Called by load_user_inputs_from_class, should define all the tentacle user inputs.
         """
-        try:
-            inputs = {}
-            self.init_user_inputs(inputs)
-            if databases.RunDatabasesProvider.instance().is_storage_enabled(bot_id):
-                run_db = databases.RunDatabasesProvider.instance().get_run_db(bot_id)
-                await configuration.clear_user_inputs(run_db, self.get_name())
-                for user_input in inputs.values():
-                    await configuration.save_user_input(user_input, run_db)
-                await run_db.flush()
-        except Exception as err:
-            self.logger.exception(
-                err, True, f"Error when initializing user inputs: {err}"
-            )
+
+    async def load_and_save_user_inputs(self, bot_id: str) -> dict:
+        """
+        instance method API for user inputs
+        Initialize and save the tentacle user inputs in run data
+        :return: the filled user input configuration
+        """
+        return await configuration.load_and_save_user_inputs(self, bot_id)
+
+    @classmethod
+    def load_user_inputs_from_class(
+        cls, tentacles_setup_config, tentacle_config
+    ) -> dict:
+        """
+        classmethod API for user inputs
+        Initialize the tentacle user inputs
+        Called by get_raw_config_and_user_inputs
+        """
+        return configuration.load_user_inputs_from_class(
+            cls, tentacles_setup_config, tentacle_config
+        )
 
     @classmethod
     async def get_raw_config_and_user_inputs(
         cls, config, tentacles_setup_config, bot_id
     ):
         """
         :return: the tentacle configuration and its list of user inputs
         """
-        try:
-            import octobot_tentacles_manager.api as api
-
-            specific_config = api.get_tentacle_config(tentacles_setup_config, cls)
-        except ImportError as err:
-            raise ImportError("octobot_tentacles_manager is required") from err
-        if saved_user_inputs := await configuration.get_user_inputs(
-            databases.RunDatabasesProvider.instance().get_run_db(bot_id),
-            cls.get_name(),
-        ):
-            # user inputs have been saved in run database, use those as they might contain additional
-            # (nested) user inputs
-            return specific_config, saved_user_inputs
-        # use user inputs from init_user_inputs
-        tentacle_instance = cls.create_local_instance(
-            config, tentacles_setup_config, specific_config
-        )
-        user_inputs = {}
-        tentacle_instance.init_user_inputs(user_inputs)
-        return specific_config, list(
-            user_input.to_dict() for user_input in user_inputs.values()
+        if not cls.HISTORIZE_USER_INPUT_CONFIG:
+            return configuration.get_raw_config_and_user_inputs_from_class(
+                cls, tentacles_setup_config
+            )
+        return await configuration.get_raw_config_and_user_inputs(
+            cls, config, tentacles_setup_config, bot_id
         )
```

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/tentacles_management/class_inspector.py` & `OctoBot-Commons-1.9.0/octobot_commons/tentacles_management/class_inspector.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/tests/test_config.py` & `OctoBot-Commons-1.9.0/octobot_commons/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/time_frame_manager.py` & `OctoBot-Commons-1.9.0/octobot_commons/time_frame_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,7 +144,18 @@
                 "No time frame available for: '{0}'. Available time "
                 "frames are: {1}. '{0}' time frame requirement "
                 "ignored.".format(
                     time_frame_string, [t.value for t in enums.TimeFrames]
                 )
             )
     return result_list
+
+
+def is_time_frame(value):
+    """
+    :return: True if the value represents a TimeFrame
+    """
+    try:
+        enums.TimeFrames(value)
+        return True
+    except ValueError:
+        return False
```

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/timestamp_util.py` & `OctoBot-Commons-1.9.0/octobot_commons/timestamp_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/tree/__init__.pxd` & `OctoBot-Commons-1.9.0/octobot_commons/tree/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# cython: language_level=3
 #  Drakkar-Software OctoBot-Commons
 #  Copyright (c) Drakkar-Software, All rights reserved.
 #
 #  This library is free software; you can redistribute it and/or
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
@@ -10,30 +9,40 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-from octobot_commons.tree cimport base_tree
 
-from octobot_commons.tree.base_tree cimport (
+from octobot_commons.tree import base_tree
+
+from octobot_commons.tree.base_tree import (
     BaseTree,
     BaseTreeNode,
     NodeExistsError,
 )
 
-from octobot_commons.tree cimport event_tree
+from octobot_commons.tree import event_tree
 
-from octobot_commons.tree.event_tree cimport (
+from octobot_commons.tree.event_tree import (
     EventTreeNode,
     EventTree,
 )
 
+from octobot_commons.tree import event_provider
+
+from octobot_commons.tree.event_provider import (
+    EventProvider,
+    get_exchange_path,
+)
+
 
 __all__ = [
     "BaseTree",
     "BaseTreeNode",
     "NodeExistsError",
     "EventTreeNode",
     "EventTree",
-]
+    "EventProvider",
+    "get_exchange_path",
+]
```

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/tree/base_tree.py` & `OctoBot-Commons-1.9.0/octobot_commons/tree/base_tree.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/tree/event_provider.py` & `OctoBot-Commons-1.9.0/octobot_commons/tree/event_provider.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/octobot_commons/tree/event_tree.py` & `OctoBot-Commons-1.9.0/octobot_commons/tree/event_tree.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/tests/configuration/test_configuration.py` & `OctoBot-Commons-1.9.0/tests/configuration/test_configuration.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/tests/configuration/test_fields_util.py` & `OctoBot-Commons-1.9.0/tests/configuration/test_fields_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/tests/databases/global_storage/test_global_shared_memory_storage.py` & `OctoBot-Commons-1.9.0/tests/databases/global_storage/test_global_shared_memory_storage.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/tests/databases/relational_databases/sqlite/test_sqlite_database.py` & `OctoBot-Commons-1.9.0/tests/databases/relational_databases/sqlite/test_sqlite_database.py`

 * *Files 14% similar despite different names*

```diff
@@ -237,14 +237,41 @@
                                              timestamp=[1, 2],
                                              price=[1, 10],
                                              date=["01", "05"])
         assert await temp_empty_database.select(OHLCV) == [(2, 'abc', '10', '05'), (1, 'xyz', '1', '01')]
         assert await temp_empty_database.select(OHLCV, date="05") == [(2, 'abc', '10', '05')]
 
 
+async def test_delete():
+    async with get_temp_empty_database() as temp_empty_database:
+        await temp_empty_database.insert_all(OHLCV,
+                                             symbol=["xyz", "abc"],
+                                             timestamp=[1, 2],
+                                             price=[1, 10],
+                                             date=["01", "05"])
+        assert await temp_empty_database.select(OHLCV) == [(2, 'abc', '10', '05'), (1, 'xyz', '1', '01')]
+        # no matching row to delete
+        await temp_empty_database.delete(OHLCV, symbol="plop")
+        assert await temp_empty_database.select(OHLCV) == [(2, 'abc', '10', '05'), (1, 'xyz', '1', '01')]
+        await temp_empty_database.delete(OHLCV, symbol="xyz")
+        assert await temp_empty_database.select(OHLCV) == [(2, 'abc', '10', '05')]
+        await temp_empty_database.insert_all(OHLCV,
+                                             symbol=["hoho", "dd"],
+                                             timestamp=[11, 11],
+                                             price=[1, 10],
+                                             date=["01", "05"])
+        assert await temp_empty_database.select(OHLCV) == [
+            (11, 'dd', '10', '05'), (11, 'hoho', '1', '01'), (2, 'abc', '10', '05')
+        ]
+        await temp_empty_database.delete(OHLCV, timestamp="11")
+        assert await temp_empty_database.select(OHLCV) == [(2, 'abc', '10', '05')]
+        await temp_empty_database.delete(OHLCV, date="05")
+        assert await temp_empty_database.select(OHLCV) == []
+
+
 async def test_create_index():
     async with get_temp_empty_database() as temp_empty_database:
         await temp_empty_database.insert(OHLCV, 1, symbol="xyz", price="1", date="01")
         # ensure no exception
         await temp_empty_database.create_index(OHLCV, ["symbol", "timestamp"])
         assert await temp_empty_database.select(OHLCV) == [(1, 'xyz', '1', '01')]
```

### Comparing `OctoBot-Commons-1.8.9/tests/databases/run_databases/test_run_databases_provider.py` & `OctoBot-Commons-1.9.0/tests/databases/run_databases/test_run_databases_provider.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/tests/logging/test_logging_util.py` & `OctoBot-Commons-1.9.0/tests/logging/test_logging_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/tests/profiles/test_profile.py` & `OctoBot-Commons-1.9.0/tests/profiles/test_profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 import json
 import shutil
 import pytest
 import mock
 import octobot_commons.json_util
 import octobot_commons.profiles as profiles
 import octobot_commons.constants as constants
+import octobot_commons.enums as enums
 import octobot_commons.tests.test_config as test_config
 
 from tests.profiles import profile, get_profile_path, get_profiles_path
 
 
 def test_read_config(profile):
     save_ref = profile
@@ -162,30 +163,39 @@
             constants.CONFIG_ID: None,
             constants.CONFIG_NAME: None,
             constants.CONFIG_DESCRIPTION: None,
             constants.CONFIG_AVATAR: None,
             constants.CONFIG_ORIGIN_URL: None,
             constants.CONFIG_READ_ONLY: False,
             constants.CONFIG_IMPORTED: False,
+            constants.CONFIG_COMPLEXITY: enums.ProfileComplexity.MEDIUM.value,
+            constants.CONFIG_RISK: enums.ProfileRisk.MODERATE.value,
+            constants.CONFIG_TYPE: enums.ProfileType.LIVE.value,
         },
         constants.PROFILE_CONFIG: {},
     }
     profile.read_config()
     # do not test read config
     profile.config = {"a": 1}
     profile.imported = True
+    profile.complexity = enums.ProfileComplexity.DIFFICULT
+    profile.risk = enums.ProfileRisk.LOW
+    profile.profile_type = enums.ProfileType.BACKTESTING
     assert profile.as_dict() == {
         constants.CONFIG_PROFILE: {
             constants.CONFIG_ID: "default",
             constants.CONFIG_NAME: "default",
             constants.CONFIG_DESCRIPTION: "OctoBot default profile.",
             constants.CONFIG_AVATAR: "default_profile.png",
             constants.CONFIG_ORIGIN_URL: "https://default.url",
             constants.CONFIG_READ_ONLY: False,
             constants.CONFIG_IMPORTED: True,
+            constants.CONFIG_COMPLEXITY: enums.ProfileComplexity.DIFFICULT.value,
+            constants.CONFIG_RISK: enums.ProfileRisk.LOW.value,
+            constants.CONFIG_TYPE: enums.ProfileType.BACKTESTING.value,
         },
         constants.PROFILE_CONFIG: {
             "a": 1
         },
     }
```

### Comparing `OctoBot-Commons-1.8.9/tests/profiles/test_profile_sharing.py` & `OctoBot-Commons-1.9.0/tests/profiles/test_profile_sharing.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,22 +15,26 @@
 #  License along with this library.
 import os
 import shutil
 import zipfile
 import contextlib
 import mock
 import pathlib
+
+import pytest
+
 import octobot_commons.constants as constants
+import octobot_commons.errors as commons_errors
 import octobot_commons.profiles as profiles
 import octobot_commons.profiles.profile_sharing as profile_sharing
 from octobot_commons.profiles.profile_sharing import _get_unique_profile_folder, _ensure_unique_profile_id, \
     _get_profile_name
 import octobot_commons.tests.test_config as test_config
 
-from tests.profiles import profile, get_profile_path
+from tests.profiles import profile, get_profile_path, invalid_profile
 
 
 def test_export_profile(profile):
     export_path = "exported"
     exported_file = f"{export_path}.zip"
     tentacles_config = os.path.join(get_profile_path(), "tentacles_config.json")
     spec_tentacles_config = os.path.join(get_profile_path(), "specific_config")
@@ -89,20 +93,21 @@
             dir_path = os.path.join(other_profile, "specific_config") if "specific_config" in root else other_profile
             assert all(
                 os.path.isfile(os.path.join(dir_path, f))
                 for f in files
             )
 
 
-def test_import_install_profile(profile):
+def test_import_install_profile(profile, invalid_profile):
     export_path = os.path.join(test_config.TEST_FOLDER, "super_profile")
     exported_file = f"{export_path}.zip"
     spec_tentacles_config = os.path.join(get_profile_path(), "specific_config")
     tentacles_config = os.path.join(get_profile_path(), "tentacles_config.json")
     other_profile = os.path.join(constants.USER_PROFILES_FOLDER, "default")
+    profile_schema = os.path.join(test_config.TEST_CONFIG_FOLDER, "profile_schema.json")
     with _cleaned_tentacles(export_path,
                             exported_file,
                             tentacles_config,
                             dir1=other_profile,
                             dir2=constants.USER_FOLDER,
                             dir3=spec_tentacles_config):
         # create fake tentacles config
@@ -110,15 +115,15 @@
         os.mkdir(spec_tentacles_config)
         shutil.copy(profile.config_file(), os.path.join(spec_tentacles_config, "t1.json"))
         shutil.copy(profile.config_file(), os.path.join(spec_tentacles_config, "t2.json"))
         profiles.export_profile(profile, export_path)
         imported_profile_path = os.path.join(constants.USER_PROFILES_FOLDER, "default")
         with mock.patch.object(profile_sharing, "_ensure_unique_profile_id", mock.Mock()) \
                 as _ensure_unique_profile_id_mock:
-            imported_profile = profiles.import_profile(exported_file, origin_url="plop.wow")
+            imported_profile = profiles.import_profile(exported_file, profile_schema, origin_url="plop.wow")
             assert isinstance(imported_profile, profiles.Profile)
             profile.read_config()
             assert profile.name == imported_profile.name
             assert profile.path != imported_profile.path
             assert profile.imported is False
             assert imported_profile.imported is True
             assert imported_profile.origin_url == "plop.wow"
@@ -127,28 +132,24 @@
         # ensure all files got imported
         for root, dirs, files in os.walk(profile.path):
             dir_path = os.path.join(other_profile, "specific_config") if "specific_config" in root else other_profile
             assert all(
                 os.path.isfile(os.path.join(dir_path, f))
                 for f in files
             )
-        assert isinstance(profiles.import_profile(exported_file), profiles.Profile)
-        # todo
+        assert isinstance(profiles.import_profile(exported_file, profile_schema), profiles.Profile)
         assert os.path.isdir(f"{imported_profile_path}_2")
-        with mock.patch.object(shutil, "rmtree", mock.Mock()) as shutil_rmtree_mock:
-            assert isinstance(profiles.install_profile(exported_file,
-                                                       _get_profile_name(None, exported_file),
-                                                       ".",
-                                                       True,
-                                                       False,
-                                                       origin_url="hello"), profiles.Profile)
-            shutil_rmtree_mock.assert_called_once()
         assert os.path.isdir(imported_profile_path)
         assert not os.path.isdir(f"{imported_profile_path}_3")
 
+        # now with invalid profile
+        profiles.export_profile(invalid_profile, export_path)
+        with pytest.raises(commons_errors.ProfileImportError):
+            profiles.import_profile(exported_file, profile_schema)
+
 
 def test_get_unique_profile_folder(profile):
     assert _get_unique_profile_folder(profile.config_file()) == f"{profile.config_file()}_2"
     other_file = f"{profile.config_file()}_2"
     other_file_2 = f"{profile.config_file()}_3"
     other_file_3 = f"{profile.config_file()}_5"
     with _cleaned_tentacles(other_file, other_file_2, other_file_3):
@@ -164,14 +165,15 @@
     other_profile = "second_profile"
     profiles_path = pathlib.Path(profile.path).parent
     other_profile_path = profiles_path.joinpath(other_profile)
     with _cleaned_tentacles(dir1=other_profile_path):
         shutil.copytree(profile.path, other_profile_path)
         other_profile = profiles.Profile(other_profile_path).read_config()
         _ensure_unique_profile_id(other_profile)
+        other_profile.save()
         ids = profiles.Profile.get_all_profiles_ids(profiles_path)
         assert len(ids) == 2
         # changed new profile id
         assert ids[0] != ids[1]
 
 
 @contextlib.contextmanager
```

### Comparing `OctoBot-Commons-1.8.9/tests/signals/__init__.py` & `OctoBot-Commons-1.9.0/tests/signals/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/tests/signals/test_signal_builder_wrapper.py` & `OctoBot-Commons-1.9.0/tests/signals/test_signal_builder_wrapper.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/tests/signals/test_signal_bundle.py` & `OctoBot-Commons-1.9.0/tests/signals/test_signal_bundle.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/tests/signals/test_signal_bundle_builder.py` & `OctoBot-Commons-1.9.0/tests/signals/test_signal_bundle_builder.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/tests/signals/test_signal_factory.py` & `OctoBot-Commons-1.9.0/tests/signals/test_signal_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/tests/signals/test_signal_publisher.py` & `OctoBot-Commons-1.9.0/tests/signals/test_signal_publisher.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/tests/symbols/test_symbol.py` & `OctoBot-Commons-1.9.0/tests/symbols/test_symbol.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/tests/symbols/test_symbol_util.py` & `OctoBot-Commons-1.9.0/tests/symbols/test_symbol_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/tests/tree/test_base_tree.py` & `OctoBot-Commons-1.9.0/tests/tree/test_base_tree.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.8.9/tests/tree/test_event_tree.py` & `OctoBot-Commons-1.9.0/tests/tree/test_event_tree.py`

 * *Files identical despite different names*

