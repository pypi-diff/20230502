# Comparing `tmp/jaaql-middleware-python-4.8.2.tar.gz` & `tmp/jaaql-middleware-python-4.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaaql-middleware-python-4.8.2.tar", last modified: Tue May  2 18:18:45 2023, max compression
+gzip compressed data, was "jaaql-middleware-python-4.8.3.tar", last modified: Tue May  2 18:45:33 2023, max compression
```

## Comparing `jaaql-middleware-python-4.8.2.tar` & `jaaql-middleware-python-4.8.3.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 18:18:45.079110 jaaql-middleware-python-4.8.2/
--rw-rw-rw-   0        0        0    18134 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.2/LICENSE.txt
--rw-rw-rw-   0        0        0      946 2023-05-02 18:18:45.078110 jaaql-middleware-python-4.8.2/PKG-INFO
--rw-rw-rw-   0        0        0      453 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 18:18:45.011109 jaaql-middleware-python-4.8.2/jaaql/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.2/jaaql/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 18:18:45.014111 jaaql-middleware-python-4.8.2/jaaql/config/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.2/jaaql/config/__init__.py
--rw-rw-rw-   0        0        0      324 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.2/jaaql/config/config-docker.ini
--rw-rw-rw-   0        0        0      253 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.2/jaaql/config/config-test.ini
--rw-rw-rw-   0        0        0      291 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.2/jaaql/config/config.ini
--rw-rw-rw-   0        0        0      470 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.2/jaaql/config_constants.py
--rw-rw-rw-   0        0        0     4462 2023-05-02 18:14:10.000000 jaaql-middleware-python-4.8.2/jaaql/constants.py
-drwxrwxrwx   0        0        0        0 2023-05-02 18:18:45.019122 jaaql-middleware-python-4.8.2/jaaql/db/
--rw-rw-rw-   0        0        0        0 2022-05-19 20:40:08.000000 jaaql-middleware-python-4.8.2/jaaql/db/__init__.py
--rw-rw-rw-   0        0        0     6929 2023-05-02 18:15:39.000000 jaaql-middleware-python-4.8.2/jaaql/db/db_interface.py
--rw-rw-rw-   0        0        0    11198 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.2/jaaql/db/db_pg_interface.py
--rw-rw-rw-   0        0        0     7025 2023-05-02 17:43:52.000000 jaaql-middleware-python-4.8.2/jaaql/db/db_utils.py
--rw-rw-rw-   0        0        0     2729 2023-05-02 18:09:01.000000 jaaql-middleware-python-4.8.2/jaaql/db/db_utils_no_circ.py
-drwxrwxrwx   0        0        0        0 2023-05-02 18:18:45.023111 jaaql-middleware-python-4.8.2/jaaql/documentation/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.2/jaaql/documentation/__init__.py
--rw-rw-rw-   0        0        0     6592 2023-05-02 12:22:14.000000 jaaql-middleware-python-4.8.2/jaaql/documentation/documentation_internal.py
--rw-rw-rw-   0        0        0     8192 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.2/jaaql/documentation/documentation_public.py
--rw-rw-rw-   0        0        0     3456 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.2/jaaql/documentation/documentation_shared.py
-drwxrwxrwx   0        0        0        0 2023-05-02 18:18:45.026110 jaaql-middleware-python-4.8.2/jaaql/email/
--rw-rw-rw-   0        0        0        0 2022-05-05 10:44:50.000000 jaaql-middleware-python-4.8.2/jaaql/email/__init__.py
--rw-rw-rw-   0        0        0     7405 2023-05-02 17:44:48.000000 jaaql-middleware-python-4.8.2/jaaql/email/email_manager.py
--rw-rw-rw-   0        0        0    19242 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.2/jaaql/email/email_manager_service.py
--rw-rw-rw-   0        0        0      234 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.2/jaaql/email/patch_ems.py
-drwxrwxrwx   0        0        0        0 2023-05-02 18:18:45.030110 jaaql-middleware-python-4.8.2/jaaql/exceptions/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.2/jaaql/exceptions/__init__.py
--rw-rw-rw-   0        0        0      401 2022-04-17 07:42:21.000000 jaaql-middleware-python-4.8.2/jaaql/exceptions/custom_http_status.py
--rw-rw-rw-   0        0        0      985 2022-05-20 15:36:28.000000 jaaql-middleware-python-4.8.2/jaaql/exceptions/http_status_exception.py
--rw-rw-rw-   0        0        0      321 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.2/jaaql/exceptions/not_yet_implement_exception.py
-drwxrwxrwx   0        0        0        0 2023-05-02 18:18:45.032110 jaaql-middleware-python-4.8.2/jaaql/interpreter/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.2/jaaql/interpreter/__init__.py
--rw-rw-rw-   0        0        0    23250 2023-05-02 18:09:24.000000 jaaql-middleware-python-4.8.2/jaaql/interpreter/interpret_jaaql.py
--rw-rw-rw-   0        0        0     5962 2023-05-02 12:06:24.000000 jaaql-middleware-python-4.8.2/jaaql/jaaql.py
-drwxrwxrwx   0        0        0        0 2023-05-02 18:18:45.035109 jaaql-middleware-python-4.8.2/jaaql/migrations/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.2/jaaql/migrations/__init__.py
--rw-rw-rw-   0        0        0      683 2022-09-19 00:09:13.000000 jaaql-middleware-python-4.8.2/jaaql/migrations/migration_history.sql
--rw-rw-rw-   0        0        0     8576 2023-05-02 17:01:26.000000 jaaql-middleware-python-4.8.2/jaaql/migrations/migrations.py
-drwxrwxrwx   0        0        0        0 2023-05-02 18:18:45.045109 jaaql-middleware-python-4.8.2/jaaql/mvc/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.2/jaaql/mvc/__init__.py
--rw-rw-rw-   0        0        0    32609 2023-05-02 17:45:39.000000 jaaql-middleware-python-4.8.2/jaaql/mvc/base_controller.py
--rw-rw-rw-   0        0        0    11591 2023-05-02 12:24:40.000000 jaaql-middleware-python-4.8.2/jaaql/mvc/base_model.py
--rw-rw-rw-   0        0        0     3928 2023-05-02 12:51:04.000000 jaaql-middleware-python-4.8.2/jaaql/mvc/controller.py
--rw-rw-rw-   0        0        0      274 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.2/jaaql/mvc/controller_interface.py
--rw-rw-rw-   0        0        0     7494 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.2/jaaql/mvc/exception_queries.py
--rw-rw-rw-   0        0        0    43043 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.2/jaaql/mvc/generated_queries.py
--rw-rw-rw-   0        0        0      232 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.2/jaaql/mvc/handmade_queries.py
--rw-rw-rw-   0        0        0    38170 2023-05-02 18:18:38.000000 jaaql-middleware-python-4.8.2/jaaql/mvc/model.py
--rw-rw-rw-   0        0        0      257 2022-05-07 20:33:26.000000 jaaql-middleware-python-4.8.2/jaaql/mvc/model_interface.py
--rw-rw-rw-   0        0        0      209 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.2/jaaql/mvc/response.py
-drwxrwxrwx   0        0        0        0 2023-05-02 18:18:45.047110 jaaql-middleware-python-4.8.2/jaaql/openapi/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.2/jaaql/openapi/__init__.py
--rw-rw-rw-   0        0        0    28821 2023-05-02 11:33:27.000000 jaaql-middleware-python-4.8.2/jaaql/openapi/swagger_documentation.py
--rw-rw-rw-   0        0        0      149 2022-06-11 20:45:39.000000 jaaql-middleware-python-4.8.2/jaaql/patch.py
-drwxrwxrwx   0        0        0        0 2023-05-02 18:18:45.057111 jaaql-middleware-python-4.8.2/jaaql/scripts/
--rw-rw-rw-   0        0        0     1379 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.2/jaaql/scripts/01.install_domains.generated.sql
--rw-rw-rw-   0        0        0      939 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.2/jaaql/scripts/02.install_super_user.exceptions.sql
--rw-rw-rw-   0        0        0     1859 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.2/jaaql/scripts/03.install_super_user.handwritten.sql
--rw-rw-rw-   0        0        0     7492 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.2/jaaql/scripts/04.install_jaaql_data_structures.generated.sql
--rw-rw-rw-   0        0        0      324 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.2/jaaql/scripts/05.install_jaaql.exceptions.sql
--rw-rw-rw-   0        0        0      990 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.2/jaaql/scripts/06.install_jaaql.handwritten.sql
--rw-rw-rw-   0        0        0     4105 2023-02-12 10:12:32.000000 jaaql-middleware-python-4.8.2/jaaql/scripts/swagger_template.html
-drwxrwxrwx   0        0        0        0 2023-05-02 18:18:45.062114 jaaql-middleware-python-4.8.2/jaaql/services/
--rw-rw-rw-   0        0        0        0 2022-07-10 13:56:37.000000 jaaql-middleware-python-4.8.2/jaaql/services/__init__.py
--rw-rw-rw-   0        0        0     2688 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.2/jaaql/services/cached_canned_query_service.py
--rw-rw-rw-   0        0        0     2047 2023-05-02 12:22:14.000000 jaaql-middleware-python-4.8.2/jaaql/services/migrations_manager_service.py
--rw-rw-rw-   0        0        0      296 2023-05-02 12:09:59.000000 jaaql-middleware-python-4.8.2/jaaql/services/patch_mms.py
-drwxrwxrwx   0        0        0        0 2023-05-02 18:18:45.070114 jaaql-middleware-python-4.8.2/jaaql/utilities/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.2/jaaql/utilities/__init__.py
--rw-rw-rw-   0        0        0     6698 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.2/jaaql/utilities/crypt_utils.py
--rw-rw-rw-   0        0        0     5357 2023-05-02 10:06:52.000000 jaaql-middleware-python-4.8.2/jaaql/utilities/options.py
--rw-rw-rw-   0        0        0     5162 2023-05-02 17:32:54.000000 jaaql-middleware-python-4.8.2/jaaql/utilities/utils.py
--rw-rw-rw-   0        0        0     2636 2023-05-02 18:18:38.000000 jaaql-middleware-python-4.8.2/jaaql/utilities/utils_no_project_imports.py
--rw-rw-rw-   0        0        0     2160 2022-05-22 11:21:40.000000 jaaql-middleware-python-4.8.2/jaaql/utilities/vault.py
-drwxrwxrwx   0        0        0        0 2023-05-02 18:18:45.077113 jaaql-middleware-python-4.8.2/jaaql_middleware_python.egg-info/
--rw-rw-rw-   0        0        0      946 2023-05-02 18:18:44.000000 jaaql-middleware-python-4.8.2/jaaql_middleware_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2221 2023-05-02 18:18:44.000000 jaaql-middleware-python-4.8.2/jaaql_middleware_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 18:18:44.000000 jaaql-middleware-python-4.8.2/jaaql_middleware_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      337 2023-05-02 18:18:44.000000 jaaql-middleware-python-4.8.2/jaaql_middleware_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-02 18:18:44.000000 jaaql-middleware-python-4.8.2/jaaql_middleware_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 18:18:45.079110 jaaql-middleware-python-4.8.2/setup.cfg
--rw-rw-rw-   0        0        0      893 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 18:45:33.600150 jaaql-middleware-python-4.8.3/
+-rw-rw-rw-   0        0        0    18134 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      946 2023-05-02 18:45:33.600150 jaaql-middleware-python-4.8.3/PKG-INFO
+-rw-rw-rw-   0        0        0      453 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 18:45:33.548175 jaaql-middleware-python-4.8.3/jaaql/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.3/jaaql/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 18:45:33.552177 jaaql-middleware-python-4.8.3/jaaql/config/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.3/jaaql/config/__init__.py
+-rw-rw-rw-   0        0        0      324 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.3/jaaql/config/config-docker.ini
+-rw-rw-rw-   0        0        0      253 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.3/jaaql/config/config-test.ini
+-rw-rw-rw-   0        0        0      291 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.3/jaaql/config/config.ini
+-rw-rw-rw-   0        0        0      470 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.3/jaaql/config_constants.py
+-rw-rw-rw-   0        0        0     4462 2023-05-02 18:45:26.000000 jaaql-middleware-python-4.8.3/jaaql/constants.py
+drwxrwxrwx   0        0        0        0 2023-05-02 18:45:33.556149 jaaql-middleware-python-4.8.3/jaaql/db/
+-rw-rw-rw-   0        0        0        0 2022-05-19 20:40:08.000000 jaaql-middleware-python-4.8.3/jaaql/db/__init__.py
+-rw-rw-rw-   0        0        0     6929 2023-05-02 18:15:39.000000 jaaql-middleware-python-4.8.3/jaaql/db/db_interface.py
+-rw-rw-rw-   0        0        0    11198 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.3/jaaql/db/db_pg_interface.py
+-rw-rw-rw-   0        0        0     7025 2023-05-02 17:43:52.000000 jaaql-middleware-python-4.8.3/jaaql/db/db_utils.py
+-rw-rw-rw-   0        0        0     2934 2023-05-02 18:45:07.000000 jaaql-middleware-python-4.8.3/jaaql/db/db_utils_no_circ.py
+drwxrwxrwx   0        0        0        0 2023-05-02 18:45:33.559149 jaaql-middleware-python-4.8.3/jaaql/documentation/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.3/jaaql/documentation/__init__.py
+-rw-rw-rw-   0        0        0     6592 2023-05-02 12:22:14.000000 jaaql-middleware-python-4.8.3/jaaql/documentation/documentation_internal.py
+-rw-rw-rw-   0        0        0     8192 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.3/jaaql/documentation/documentation_public.py
+-rw-rw-rw-   0        0        0     3456 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.3/jaaql/documentation/documentation_shared.py
+drwxrwxrwx   0        0        0        0 2023-05-02 18:45:33.563149 jaaql-middleware-python-4.8.3/jaaql/email/
+-rw-rw-rw-   0        0        0        0 2022-05-05 10:44:50.000000 jaaql-middleware-python-4.8.3/jaaql/email/__init__.py
+-rw-rw-rw-   0        0        0     7475 2023-05-02 18:34:17.000000 jaaql-middleware-python-4.8.3/jaaql/email/email_manager.py
+-rw-rw-rw-   0        0        0    19242 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.3/jaaql/email/email_manager_service.py
+-rw-rw-rw-   0        0        0      234 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.3/jaaql/email/patch_ems.py
+drwxrwxrwx   0        0        0        0 2023-05-02 18:45:33.566149 jaaql-middleware-python-4.8.3/jaaql/exceptions/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.3/jaaql/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      401 2022-04-17 07:42:21.000000 jaaql-middleware-python-4.8.3/jaaql/exceptions/custom_http_status.py
+-rw-rw-rw-   0        0        0      985 2022-05-20 15:36:28.000000 jaaql-middleware-python-4.8.3/jaaql/exceptions/http_status_exception.py
+-rw-rw-rw-   0        0        0      321 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.3/jaaql/exceptions/not_yet_implement_exception.py
+drwxrwxrwx   0        0        0        0 2023-05-02 18:45:33.568149 jaaql-middleware-python-4.8.3/jaaql/interpreter/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.3/jaaql/interpreter/__init__.py
+-rw-rw-rw-   0        0        0    23250 2023-05-02 18:09:24.000000 jaaql-middleware-python-4.8.3/jaaql/interpreter/interpret_jaaql.py
+-rw-rw-rw-   0        0        0     5962 2023-05-02 12:06:24.000000 jaaql-middleware-python-4.8.3/jaaql/jaaql.py
+drwxrwxrwx   0        0        0        0 2023-05-02 18:45:33.570149 jaaql-middleware-python-4.8.3/jaaql/migrations/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.3/jaaql/migrations/__init__.py
+-rw-rw-rw-   0        0        0      683 2022-09-19 00:09:13.000000 jaaql-middleware-python-4.8.3/jaaql/migrations/migration_history.sql
+-rw-rw-rw-   0        0        0     8576 2023-05-02 17:01:26.000000 jaaql-middleware-python-4.8.3/jaaql/migrations/migrations.py
+drwxrwxrwx   0        0        0        0 2023-05-02 18:45:33.579187 jaaql-middleware-python-4.8.3/jaaql/mvc/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.3/jaaql/mvc/__init__.py
+-rw-rw-rw-   0        0        0    32609 2023-05-02 17:45:39.000000 jaaql-middleware-python-4.8.3/jaaql/mvc/base_controller.py
+-rw-rw-rw-   0        0        0    11591 2023-05-02 12:24:40.000000 jaaql-middleware-python-4.8.3/jaaql/mvc/base_model.py
+-rw-rw-rw-   0        0        0     3928 2023-05-02 12:51:04.000000 jaaql-middleware-python-4.8.3/jaaql/mvc/controller.py
+-rw-rw-rw-   0        0        0      274 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.3/jaaql/mvc/controller_interface.py
+-rw-rw-rw-   0        0        0     7494 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.3/jaaql/mvc/exception_queries.py
+-rw-rw-rw-   0        0        0    43043 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.3/jaaql/mvc/generated_queries.py
+-rw-rw-rw-   0        0        0      232 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.3/jaaql/mvc/handmade_queries.py
+-rw-rw-rw-   0        0        0    38055 2023-05-02 18:45:01.000000 jaaql-middleware-python-4.8.3/jaaql/mvc/model.py
+-rw-rw-rw-   0        0        0      257 2022-05-07 20:33:26.000000 jaaql-middleware-python-4.8.3/jaaql/mvc/model_interface.py
+-rw-rw-rw-   0        0        0      209 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.3/jaaql/mvc/response.py
+drwxrwxrwx   0        0        0        0 2023-05-02 18:45:33.581150 jaaql-middleware-python-4.8.3/jaaql/openapi/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.3/jaaql/openapi/__init__.py
+-rw-rw-rw-   0        0        0    28821 2023-05-02 11:33:27.000000 jaaql-middleware-python-4.8.3/jaaql/openapi/swagger_documentation.py
+-rw-rw-rw-   0        0        0      149 2022-06-11 20:45:39.000000 jaaql-middleware-python-4.8.3/jaaql/patch.py
+drwxrwxrwx   0        0        0        0 2023-05-02 18:45:33.587149 jaaql-middleware-python-4.8.3/jaaql/scripts/
+-rw-rw-rw-   0        0        0     1379 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.3/jaaql/scripts/01.install_domains.generated.sql
+-rw-rw-rw-   0        0        0      939 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.3/jaaql/scripts/02.install_super_user.exceptions.sql
+-rw-rw-rw-   0        0        0     1859 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.3/jaaql/scripts/03.install_super_user.handwritten.sql
+-rw-rw-rw-   0        0        0     7492 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.3/jaaql/scripts/04.install_jaaql_data_structures.generated.sql
+-rw-rw-rw-   0        0        0      324 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.3/jaaql/scripts/05.install_jaaql.exceptions.sql
+-rw-rw-rw-   0        0        0      990 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.3/jaaql/scripts/06.install_jaaql.handwritten.sql
+-rw-rw-rw-   0        0        0     4105 2023-02-12 10:12:32.000000 jaaql-middleware-python-4.8.3/jaaql/scripts/swagger_template.html
+drwxrwxrwx   0        0        0        0 2023-05-02 18:45:33.590148 jaaql-middleware-python-4.8.3/jaaql/services/
+-rw-rw-rw-   0        0        0        0 2022-07-10 13:56:37.000000 jaaql-middleware-python-4.8.3/jaaql/services/__init__.py
+-rw-rw-rw-   0        0        0     2688 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.3/jaaql/services/cached_canned_query_service.py
+-rw-rw-rw-   0        0        0     2047 2023-05-02 12:22:14.000000 jaaql-middleware-python-4.8.3/jaaql/services/migrations_manager_service.py
+-rw-rw-rw-   0        0        0      296 2023-05-02 12:09:59.000000 jaaql-middleware-python-4.8.3/jaaql/services/patch_mms.py
+drwxrwxrwx   0        0        0        0 2023-05-02 18:45:33.595149 jaaql-middleware-python-4.8.3/jaaql/utilities/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.3/jaaql/utilities/__init__.py
+-rw-rw-rw-   0        0        0     6698 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.3/jaaql/utilities/crypt_utils.py
+-rw-rw-rw-   0        0        0     5357 2023-05-02 10:06:52.000000 jaaql-middleware-python-4.8.3/jaaql/utilities/options.py
+-rw-rw-rw-   0        0        0     5162 2023-05-02 17:32:54.000000 jaaql-middleware-python-4.8.3/jaaql/utilities/utils.py
+-rw-rw-rw-   0        0        0     2636 2023-05-02 18:18:38.000000 jaaql-middleware-python-4.8.3/jaaql/utilities/utils_no_project_imports.py
+-rw-rw-rw-   0        0        0     2160 2022-05-22 11:21:40.000000 jaaql-middleware-python-4.8.3/jaaql/utilities/vault.py
+drwxrwxrwx   0        0        0        0 2023-05-02 18:45:33.599149 jaaql-middleware-python-4.8.3/jaaql_middleware_python.egg-info/
+-rw-rw-rw-   0        0        0      946 2023-05-02 18:45:33.000000 jaaql-middleware-python-4.8.3/jaaql_middleware_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2221 2023-05-02 18:45:33.000000 jaaql-middleware-python-4.8.3/jaaql_middleware_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 18:45:33.000000 jaaql-middleware-python-4.8.3/jaaql_middleware_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      337 2023-05-02 18:45:33.000000 jaaql-middleware-python-4.8.3/jaaql_middleware_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-02 18:45:33.000000 jaaql-middleware-python-4.8.3/jaaql_middleware_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 18:45:33.600150 jaaql-middleware-python-4.8.3/setup.cfg
+-rw-rw-rw-   0        0        0      893 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.3/setup.py
```

### Comparing `jaaql-middleware-python-4.8.2/LICENSE.txt` & `jaaql-middleware-python-4.8.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.2/PKG-INFO` & `jaaql-middleware-python-4.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-middleware-python
-Version: 4.8.2
+Version: 4.8.3
 Summary: The jaaql package, allowing for rapid development and deployment of RESTful HTTP applications
 Home-page: https://github.com/JAAQL/JAAQL-middleware-python
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-middleware-python-4.8.2/jaaql/constants.py` & `jaaql-middleware-python-4.8.3/jaaql/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,9 +124,9 @@
 USERNAME__anonymous = "anonymous"
 PASSWORD__anonymous = "jaaql_public_password"
 ROLE__jaaql = "jaaql"
 ROLE__postgres = "postgres"
 
 PROTOCOL__postgres = "postgresql://"
 
-VERSION = "4.8.2"
+VERSION = "4.8.3"
```

### Comparing `jaaql-middleware-python-4.8.2/jaaql/db/db_interface.py` & `jaaql-middleware-python-4.8.3/jaaql/db/db_interface.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.2/jaaql/db/db_pg_interface.py` & `jaaql-middleware-python-4.8.3/jaaql/db/db_pg_interface.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.2/jaaql/db/db_utils.py` & `jaaql-middleware-python-4.8.3/jaaql/db/db_utils.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.2/jaaql/db/db_utils_no_circ.py` & `jaaql-middleware-python-4.8.3/jaaql/db/db_utils_no_circ.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 from queue import Queue
 from jaaql.db.db_utils import execute_supplied_statement, create_interface_for_db, ERR__schema_invalid
 from jaaql.exceptions.http_status_exception import HttpStatusException
 from jaaql.interpreter.interpret_jaaql import InterpretJAAQL
 from jaaql.constants import KEY__application, KEY__database, KEY__schema, KEY__role, DB__jaaql, \
     KEY__read_only
 from jaaql.db.db_interface import DBInterface
+from jaaql.utilities.utils_no_project_imports import objectify
 
 
 def submit(vault, config, db_crypt_key, jaaql_connection: DBInterface, inputs: dict, account_id: str, verification_hook: Queue = None,
-           cached_canned_query_service = None):
+           cached_canned_query_service = None, as_objects: bool = False, singleton: bool = False):
     if not isinstance(inputs, dict):
         raise HttpStatusException("Expected object or string input")
 
     if KEY__application in inputs:
         schemas = execute_supplied_statement(jaaql_connection, QUERY__fetch_application_schemas, {
             KG__application_schema__application: inputs[KEY__application]
         }, as_objects=True)
@@ -43,10 +44,15 @@
 
     if KEY__database not in inputs:
         inputs[KEY__database] = DB__jaaql
 
     sub_role = inputs.pop(KEY__role) if KEY__role in inputs else None
     required_db = create_interface_for_db(vault, config, account_id, inputs[KEY__database], sub_role)
 
-    return InterpretJAAQL(required_db).transform(inputs, skip_commit=inputs.get(KEY__read_only), wait_hook=verification_hook,
-                                                 encryption_key=db_crypt_key,
-                                                 canned_query_service=cached_canned_query_service)
+    ret = InterpretJAAQL(required_db).transform(inputs, skip_commit=inputs.get(KEY__read_only), wait_hook=verification_hook,
+                                                encryption_key=db_crypt_key,
+                                                canned_query_service=cached_canned_query_service)
+
+    if as_objects:
+        ret = objectify(ret, singleton=singleton)
+
+    return ret
```

### Comparing `jaaql-middleware-python-4.8.2/jaaql/documentation/documentation_internal.py` & `jaaql-middleware-python-4.8.3/jaaql/documentation/documentation_internal.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.2/jaaql/documentation/documentation_public.py` & `jaaql-middleware-python-4.8.3/jaaql/documentation/documentation_public.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.2/jaaql/documentation/documentation_shared.py` & `jaaql-middleware-python-4.8.3/jaaql/documentation/documentation_shared.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.2/jaaql/email/email_manager.py` & `jaaql-middleware-python-4.8.3/jaaql/email/email_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,16 @@
         requests.post("http://127.0.0.1:" + str(PORT__ems) + ENDPOINT__send_email, json=email.repr_json())
 
     @staticmethod
     def uri_encode_replace(val):
         return quote(str(val))
 
     def send_email(self, vault, config, db_crypt_key, jaaql_connection, application: str, template: str, application_artifacts_source: str,
-                   application_base_url: str, account_id: str, parameters: dict = None, parameter_id: str = None, none_sanitized_parameters: dict = None):
+                   application_base_url: str, account_id: str, parameters: dict = None, parameter_id: str = None,
+                   none_sanitized_parameters: dict = None, recipient: str = None):
         if none_sanitized_parameters is None:
             none_sanitized_parameters = {}
 
         account = account__select(jaaql_connection, db_crypt_key, account_id)
         template = email_template__select(jaaql_connection, application, template)
 
         if parameters is not None and len(parameters) == 0:
@@ -100,15 +101,15 @@
             parameters = {}
 
         none_sanitized_parameters[EMAIL_PARAM__app_url] = application_base_url
         none_sanitized_parameters[EMAIL_PARAM__email_address] = account[KG__account__username]
         parameters = {**parameters, **none_sanitized_parameters}
 
         self.construct_and_send_email(application_artifacts_source, template[KG__email_template__dispatcher], template,
-                                      account[KG__account__username], parameters)
+                                      recipient if recipient else account[KG__account__username], parameters)
 
     def construct_and_send_email(self, application_artifacts_source: Optional[str], dispatcher: str, template: dict, to_email: str,
                                  parameters: Optional[dict], attachments=None, attachment_access_token: str = None):
         loaded_template = load_artifact(self.is_container, application_artifacts_source, template[KG__email_template__content_url])
 
         loaded_template = self.perform_replacements(loaded_template, REPLACE__str, str, REGEX__email_parameter, parameters)
         loaded_template = self.perform_replacements(loaded_template, REPLACE__uri_encoded_str, EmailManager.uri_encode_replace,
```

### Comparing `jaaql-middleware-python-4.8.2/jaaql/email/email_manager_service.py` & `jaaql-middleware-python-4.8.3/jaaql/email/email_manager_service.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.2/jaaql/exceptions/http_status_exception.py` & `jaaql-middleware-python-4.8.3/jaaql/exceptions/http_status_exception.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.2/jaaql/interpreter/interpret_jaaql.py` & `jaaql-middleware-python-4.8.3/jaaql/interpreter/interpret_jaaql.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.2/jaaql/jaaql.py` & `jaaql-middleware-python-4.8.3/jaaql/jaaql.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.2/jaaql/migrations/migration_history.sql` & `jaaql-middleware-python-4.8.3/jaaql/migrations/migration_history.sql`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.2/jaaql/migrations/migrations.py` & `jaaql-middleware-python-4.8.3/jaaql/migrations/migrations.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.2/jaaql/mvc/base_controller.py` & `jaaql-middleware-python-4.8.3/jaaql/mvc/base_controller.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.2/jaaql/mvc/base_model.py` & `jaaql-middleware-python-4.8.3/jaaql/mvc/base_model.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.2/jaaql/mvc/controller.py` & `jaaql-middleware-python-4.8.3/jaaql/mvc/controller.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.2/jaaql/mvc/exception_queries.py` & `jaaql-middleware-python-4.8.3/jaaql/mvc/exception_queries.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.2/jaaql/mvc/generated_queries.py` & `jaaql-middleware-python-4.8.3/jaaql/mvc/generated_queries.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.2/jaaql/mvc/model.py` & `jaaql-middleware-python-4.8.3/jaaql/mvc/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from jaaql.documentation.documentation_public import KEY__oauth_token
 from jaaql.mvc.base_model import BaseJAAQLModel, VAULT_KEY__jwt_crypt_key
 from jaaql.exceptions.http_status_exception import HttpStatusException, HTTPStatus, ERR__already_installed
 from os.path import join
 from jaaql.constants import *
 from jaaql.mvc.response import JAAQLResponse
 from jaaql.utilities.utils import get_jaaql_root, get_base_url
-from jaaql.utilities.utils_no_project_imports import objectify
 from jaaql.db.db_utils import create_interface, jaaql__encrypt
 from jaaql.db.db_utils_no_circ import submit
 from jaaql.utilities import crypt_utils
 import threading
 from datetime import datetime, timedelta
 from jaaql.mvc.handmade_queries import *
 from jwt.utils import base64url_decode
@@ -665,14 +664,9 @@
             })
 
         return {
             KG__security_event__event_lock: reg_env_ins[KG__security_event__event_lock]
         }
 
     def submit(self, inputs: dict, account_id: str, verification_hook: Queue = None, as_objects: bool = False, singleton: bool = False):
-        ret = submit(self.vault, self.config, self.get_db_crypt_key(), self.jaaql_lookup_connection, inputs, account_id, verification_hook,
-                     self.cached_canned_query_service)
-
-        if as_objects:
-            ret = objectify(ret, singleton=singleton)
-
-        return ret
+        return submit(self.vault, self.config, self.get_db_crypt_key(), self.jaaql_lookup_connection, inputs, account_id, verification_hook,
+                      self.cached_canned_query_service, as_objects=as_objects, singleton=singleton)
```

### Comparing `jaaql-middleware-python-4.8.2/jaaql/openapi/swagger_documentation.py` & `jaaql-middleware-python-4.8.3/jaaql/openapi/swagger_documentation.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.2/jaaql/scripts/01.install_domains.generated.sql` & `jaaql-middleware-python-4.8.3/jaaql/scripts/01.install_domains.generated.sql`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.2/jaaql/scripts/02.install_super_user.exceptions.sql` & `jaaql-middleware-python-4.8.3/jaaql/scripts/02.install_super_user.exceptions.sql`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.2/jaaql/scripts/03.install_super_user.handwritten.sql` & `jaaql-middleware-python-4.8.3/jaaql/scripts/03.install_super_user.handwritten.sql`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.2/jaaql/scripts/04.install_jaaql_data_structures.generated.sql` & `jaaql-middleware-python-4.8.3/jaaql/scripts/04.install_jaaql_data_structures.generated.sql`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.2/jaaql/scripts/06.install_jaaql.handwritten.sql` & `jaaql-middleware-python-4.8.3/jaaql/scripts/06.install_jaaql.handwritten.sql`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.2/jaaql/scripts/swagger_template.html` & `jaaql-middleware-python-4.8.3/jaaql/scripts/swagger_template.html`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.2/jaaql/services/cached_canned_query_service.py` & `jaaql-middleware-python-4.8.3/jaaql/services/cached_canned_query_service.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.2/jaaql/services/migrations_manager_service.py` & `jaaql-middleware-python-4.8.3/jaaql/services/migrations_manager_service.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.2/jaaql/utilities/crypt_utils.py` & `jaaql-middleware-python-4.8.3/jaaql/utilities/crypt_utils.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.2/jaaql/utilities/options.py` & `jaaql-middleware-python-4.8.3/jaaql/utilities/options.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.2/jaaql/utilities/utils.py` & `jaaql-middleware-python-4.8.3/jaaql/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.2/jaaql/utilities/utils_no_project_imports.py` & `jaaql-middleware-python-4.8.3/jaaql/utilities/utils_no_project_imports.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.2/jaaql/utilities/vault.py` & `jaaql-middleware-python-4.8.3/jaaql/utilities/vault.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.2/jaaql_middleware_python.egg-info/PKG-INFO` & `jaaql-middleware-python-4.8.3/jaaql_middleware_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-middleware-python
-Version: 4.8.2
+Version: 4.8.3
 Summary: The jaaql package, allowing for rapid development and deployment of RESTful HTTP applications
 Home-page: https://github.com/JAAQL/JAAQL-middleware-python
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-middleware-python-4.8.2/jaaql_middleware_python.egg-info/SOURCES.txt` & `jaaql-middleware-python-4.8.3/jaaql_middleware_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.2/setup.py` & `jaaql-middleware-python-4.8.3/setup.py`

 * *Files identical despite different names*

