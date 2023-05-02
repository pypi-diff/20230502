# Comparing `tmp/jaaql-middleware-python-4.7.2.tar.gz` & `tmp/jaaql-middleware-python-4.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaaql-middleware-python-4.7.2.tar", last modified: Tue May  2 12:59:49 2023, max compression
+gzip compressed data, was "jaaql-middleware-python-4.7.3.tar", last modified: Tue May  2 17:07:31 2023, max compression
```

## Comparing `jaaql-middleware-python-4.7.2.tar` & `jaaql-middleware-python-4.7.3.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 12:59:49.140244 jaaql-middleware-python-4.7.2/
--rw-rw-rw-   0        0        0    18134 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.7.2/LICENSE.txt
--rw-rw-rw-   0        0        0      946 2023-05-02 12:59:49.140244 jaaql-middleware-python-4.7.2/PKG-INFO
--rw-rw-rw-   0        0        0      453 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 12:59:49.085244 jaaql-middleware-python-4.7.2/jaaql/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.7.2/jaaql/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:59:49.089244 jaaql-middleware-python-4.7.2/jaaql/config/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.7.2/jaaql/config/__init__.py
--rw-rw-rw-   0        0        0      324 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.2/jaaql/config/config-docker.ini
--rw-rw-rw-   0        0        0      253 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.2/jaaql/config/config-test.ini
--rw-rw-rw-   0        0        0      291 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.2/jaaql/config/config.ini
--rw-rw-rw-   0        0        0      470 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.2/jaaql/config_constants.py
--rw-rw-rw-   0        0        0     4862 2023-05-02 12:58:07.000000 jaaql-middleware-python-4.7.2/jaaql/constants.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:59:49.092244 jaaql-middleware-python-4.7.2/jaaql/db/
--rw-rw-rw-   0        0        0        0 2022-05-19 20:40:08.000000 jaaql-middleware-python-4.7.2/jaaql/db/__init__.py
--rw-rw-rw-   0        0        0     7043 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.2/jaaql/db/db_interface.py
--rw-rw-rw-   0        0        0    11198 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.2/jaaql/db/db_pg_interface.py
--rw-rw-rw-   0        0        0     6545 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.2/jaaql/db/db_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:59:49.096243 jaaql-middleware-python-4.7.2/jaaql/documentation/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.7.2/jaaql/documentation/__init__.py
--rw-rw-rw-   0        0        0     6592 2023-05-02 12:22:14.000000 jaaql-middleware-python-4.7.2/jaaql/documentation/documentation_internal.py
--rw-rw-rw-   0        0        0     8192 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.2/jaaql/documentation/documentation_public.py
--rw-rw-rw-   0        0        0     3456 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.2/jaaql/documentation/documentation_shared.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:59:49.099243 jaaql-middleware-python-4.7.2/jaaql/email/
--rw-rw-rw-   0        0        0        0 2022-05-05 10:44:50.000000 jaaql-middleware-python-4.7.2/jaaql/email/__init__.py
--rw-rw-rw-   0        0        0     3687 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.2/jaaql/email/email_manager.py
--rw-rw-rw-   0        0        0    19242 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.2/jaaql/email/email_manager_service.py
--rw-rw-rw-   0        0        0      234 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.2/jaaql/email/patch_ems.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:59:49.103243 jaaql-middleware-python-4.7.2/jaaql/exceptions/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.7.2/jaaql/exceptions/__init__.py
--rw-rw-rw-   0        0        0      401 2022-04-17 07:42:21.000000 jaaql-middleware-python-4.7.2/jaaql/exceptions/custom_http_status.py
--rw-rw-rw-   0        0        0      985 2022-05-20 15:36:28.000000 jaaql-middleware-python-4.7.2/jaaql/exceptions/http_status_exception.py
--rw-rw-rw-   0        0        0      321 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.7.2/jaaql/exceptions/not_yet_implement_exception.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:59:49.105244 jaaql-middleware-python-4.7.2/jaaql/interpreter/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.7.2/jaaql/interpreter/__init__.py
--rw-rw-rw-   0        0        0    23250 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.2/jaaql/interpreter/interpret_jaaql.py
--rw-rw-rw-   0        0        0     5962 2023-05-02 12:06:24.000000 jaaql-middleware-python-4.7.2/jaaql/jaaql.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:59:49.107244 jaaql-middleware-python-4.7.2/jaaql/migrations/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.7.2/jaaql/migrations/__init__.py
--rw-rw-rw-   0        0        0      683 2022-09-19 00:09:13.000000 jaaql-middleware-python-4.7.2/jaaql/migrations/migration_history.sql
--rw-rw-rw-   0        0        0     8913 2023-05-02 12:47:13.000000 jaaql-middleware-python-4.7.2/jaaql/migrations/migrations.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:59:49.117243 jaaql-middleware-python-4.7.2/jaaql/mvc/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.7.2/jaaql/mvc/__init__.py
--rw-rw-rw-   0        0        0    32327 2023-05-02 11:26:06.000000 jaaql-middleware-python-4.7.2/jaaql/mvc/base_controller.py
--rw-rw-rw-   0        0        0    11591 2023-05-02 12:24:40.000000 jaaql-middleware-python-4.7.2/jaaql/mvc/base_model.py
--rw-rw-rw-   0        0        0     3928 2023-05-02 12:51:04.000000 jaaql-middleware-python-4.7.2/jaaql/mvc/controller.py
--rw-rw-rw-   0        0        0      274 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.7.2/jaaql/mvc/controller_interface.py
--rw-rw-rw-   0        0        0     7494 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.2/jaaql/mvc/exception_queries.py
--rw-rw-rw-   0        0        0    43043 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.2/jaaql/mvc/generated_queries.py
--rw-rw-rw-   0        0        0      232 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.2/jaaql/mvc/handmade_queries.py
--rw-rw-rw-   0        0        0    43432 2023-05-02 12:27:47.000000 jaaql-middleware-python-4.7.2/jaaql/mvc/model.py
--rw-rw-rw-   0        0        0      257 2022-05-07 20:33:26.000000 jaaql-middleware-python-4.7.2/jaaql/mvc/model_interface.py
--rw-rw-rw-   0        0        0      209 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.2/jaaql/mvc/response.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:59:49.118243 jaaql-middleware-python-4.7.2/jaaql/openapi/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.7.2/jaaql/openapi/__init__.py
--rw-rw-rw-   0        0        0    28821 2023-05-02 11:33:27.000000 jaaql-middleware-python-4.7.2/jaaql/openapi/swagger_documentation.py
--rw-rw-rw-   0        0        0      149 2022-06-11 20:45:39.000000 jaaql-middleware-python-4.7.2/jaaql/patch.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:59:49.125243 jaaql-middleware-python-4.7.2/jaaql/scripts/
--rw-rw-rw-   0        0        0     1379 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.2/jaaql/scripts/01.install_domains.generated.sql
--rw-rw-rw-   0        0        0      939 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.2/jaaql/scripts/02.install_super_user.exceptions.sql
--rw-rw-rw-   0        0        0     1859 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.2/jaaql/scripts/03.install_super_user.handwritten.sql
--rw-rw-rw-   0        0        0     7492 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.2/jaaql/scripts/04.install_jaaql_data_structures.generated.sql
--rw-rw-rw-   0        0        0      324 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.2/jaaql/scripts/05.install_jaaql.exceptions.sql
--rw-rw-rw-   0        0        0      990 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.2/jaaql/scripts/06.install_jaaql.handwritten.sql
--rw-rw-rw-   0        0        0     4105 2023-02-12 10:12:32.000000 jaaql-middleware-python-4.7.2/jaaql/scripts/swagger_template.html
-drwxrwxrwx   0        0        0        0 2023-05-02 12:59:49.128244 jaaql-middleware-python-4.7.2/jaaql/services/
--rw-rw-rw-   0        0        0        0 2022-07-10 13:56:37.000000 jaaql-middleware-python-4.7.2/jaaql/services/__init__.py
--rw-rw-rw-   0        0        0     2688 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.2/jaaql/services/cached_canned_query_service.py
--rw-rw-rw-   0        0        0     2047 2023-05-02 12:22:14.000000 jaaql-middleware-python-4.7.2/jaaql/services/migrations_manager_service.py
--rw-rw-rw-   0        0        0      296 2023-05-02 12:09:59.000000 jaaql-middleware-python-4.7.2/jaaql/services/patch_mms.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:59:49.133244 jaaql-middleware-python-4.7.2/jaaql/utilities/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.7.2/jaaql/utilities/__init__.py
--rw-rw-rw-   0        0        0     6698 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.2/jaaql/utilities/crypt_utils.py
--rw-rw-rw-   0        0        0     5357 2023-05-02 10:06:52.000000 jaaql-middleware-python-4.7.2/jaaql/utilities/options.py
--rw-rw-rw-   0        0        0     4970 2023-05-02 12:18:13.000000 jaaql-middleware-python-4.7.2/jaaql/utilities/utils.py
--rw-rw-rw-   0        0        0     2428 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.2/jaaql/utilities/utils_no_project_imports.py
--rw-rw-rw-   0        0        0     2160 2022-05-22 11:21:40.000000 jaaql-middleware-python-4.7.2/jaaql/utilities/vault.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:59:49.139244 jaaql-middleware-python-4.7.2/jaaql_middleware_python.egg-info/
--rw-rw-rw-   0        0        0      946 2023-05-02 12:59:49.000000 jaaql-middleware-python-4.7.2/jaaql_middleware_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2192 2023-05-02 12:59:49.000000 jaaql-middleware-python-4.7.2/jaaql_middleware_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 12:59:49.000000 jaaql-middleware-python-4.7.2/jaaql_middleware_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      337 2023-05-02 12:59:49.000000 jaaql-middleware-python-4.7.2/jaaql_middleware_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-02 12:59:49.000000 jaaql-middleware-python-4.7.2/jaaql_middleware_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 12:59:49.140244 jaaql-middleware-python-4.7.2/setup.cfg
--rw-rw-rw-   0        0        0      893 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.7.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 17:07:31.264637 jaaql-middleware-python-4.7.3/
+-rw-rw-rw-   0        0        0    18134 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.7.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      946 2023-05-02 17:07:31.264637 jaaql-middleware-python-4.7.3/PKG-INFO
+-rw-rw-rw-   0        0        0      453 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 17:07:31.210617 jaaql-middleware-python-4.7.3/jaaql/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.7.3/jaaql/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 17:07:31.213148 jaaql-middleware-python-4.7.3/jaaql/config/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.7.3/jaaql/config/__init__.py
+-rw-rw-rw-   0        0        0      324 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.3/jaaql/config/config-docker.ini
+-rw-rw-rw-   0        0        0      253 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.3/jaaql/config/config-test.ini
+-rw-rw-rw-   0        0        0      291 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.3/jaaql/config/config.ini
+-rw-rw-rw-   0        0        0      470 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.3/jaaql/config_constants.py
+-rw-rw-rw-   0        0        0     4462 2023-05-02 17:07:29.000000 jaaql-middleware-python-4.7.3/jaaql/constants.py
+drwxrwxrwx   0        0        0        0 2023-05-02 17:07:31.217128 jaaql-middleware-python-4.7.3/jaaql/db/
+-rw-rw-rw-   0        0        0        0 2022-05-19 20:40:08.000000 jaaql-middleware-python-4.7.3/jaaql/db/__init__.py
+-rw-rw-rw-   0        0        0     7043 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.3/jaaql/db/db_interface.py
+-rw-rw-rw-   0        0        0    11198 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.3/jaaql/db/db_pg_interface.py
+-rw-rw-rw-   0        0        0     6545 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.3/jaaql/db/db_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-02 17:07:31.220127 jaaql-middleware-python-4.7.3/jaaql/documentation/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.7.3/jaaql/documentation/__init__.py
+-rw-rw-rw-   0        0        0     6592 2023-05-02 12:22:14.000000 jaaql-middleware-python-4.7.3/jaaql/documentation/documentation_internal.py
+-rw-rw-rw-   0        0        0     8192 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.3/jaaql/documentation/documentation_public.py
+-rw-rw-rw-   0        0        0     3456 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.3/jaaql/documentation/documentation_shared.py
+drwxrwxrwx   0        0        0        0 2023-05-02 17:07:31.224638 jaaql-middleware-python-4.7.3/jaaql/email/
+-rw-rw-rw-   0        0        0        0 2022-05-05 10:44:50.000000 jaaql-middleware-python-4.7.3/jaaql/email/__init__.py
+-rw-rw-rw-   0        0        0     3662 2023-05-02 15:17:44.000000 jaaql-middleware-python-4.7.3/jaaql/email/email_manager.py
+-rw-rw-rw-   0        0        0    19242 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.3/jaaql/email/email_manager_service.py
+-rw-rw-rw-   0        0        0      234 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.3/jaaql/email/patch_ems.py
+drwxrwxrwx   0        0        0        0 2023-05-02 17:07:31.227637 jaaql-middleware-python-4.7.3/jaaql/exceptions/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.7.3/jaaql/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      401 2022-04-17 07:42:21.000000 jaaql-middleware-python-4.7.3/jaaql/exceptions/custom_http_status.py
+-rw-rw-rw-   0        0        0      985 2022-05-20 15:36:28.000000 jaaql-middleware-python-4.7.3/jaaql/exceptions/http_status_exception.py
+-rw-rw-rw-   0        0        0      321 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.7.3/jaaql/exceptions/not_yet_implement_exception.py
+drwxrwxrwx   0        0        0        0 2023-05-02 17:07:31.229637 jaaql-middleware-python-4.7.3/jaaql/interpreter/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.7.3/jaaql/interpreter/__init__.py
+-rw-rw-rw-   0        0        0    23250 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.3/jaaql/interpreter/interpret_jaaql.py
+-rw-rw-rw-   0        0        0     5962 2023-05-02 12:06:24.000000 jaaql-middleware-python-4.7.3/jaaql/jaaql.py
+drwxrwxrwx   0        0        0        0 2023-05-02 17:07:31.231638 jaaql-middleware-python-4.7.3/jaaql/migrations/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.7.3/jaaql/migrations/__init__.py
+-rw-rw-rw-   0        0        0      683 2022-09-19 00:09:13.000000 jaaql-middleware-python-4.7.3/jaaql/migrations/migration_history.sql
+-rw-rw-rw-   0        0        0     8576 2023-05-02 17:01:26.000000 jaaql-middleware-python-4.7.3/jaaql/migrations/migrations.py
+drwxrwxrwx   0        0        0        0 2023-05-02 17:07:31.241637 jaaql-middleware-python-4.7.3/jaaql/mvc/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.7.3/jaaql/mvc/__init__.py
+-rw-rw-rw-   0        0        0    32613 2023-05-02 17:00:38.000000 jaaql-middleware-python-4.7.3/jaaql/mvc/base_controller.py
+-rw-rw-rw-   0        0        0    11591 2023-05-02 12:24:40.000000 jaaql-middleware-python-4.7.3/jaaql/mvc/base_model.py
+-rw-rw-rw-   0        0        0     3928 2023-05-02 12:51:04.000000 jaaql-middleware-python-4.7.3/jaaql/mvc/controller.py
+-rw-rw-rw-   0        0        0      274 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.7.3/jaaql/mvc/controller_interface.py
+-rw-rw-rw-   0        0        0     7494 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.3/jaaql/mvc/exception_queries.py
+-rw-rw-rw-   0        0        0    43043 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.3/jaaql/mvc/generated_queries.py
+-rw-rw-rw-   0        0        0      232 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.3/jaaql/mvc/handmade_queries.py
+-rw-rw-rw-   0        0        0    43099 2023-05-02 17:00:38.000000 jaaql-middleware-python-4.7.3/jaaql/mvc/model.py
+-rw-rw-rw-   0        0        0      257 2022-05-07 20:33:26.000000 jaaql-middleware-python-4.7.3/jaaql/mvc/model_interface.py
+-rw-rw-rw-   0        0        0      209 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.3/jaaql/mvc/response.py
+drwxrwxrwx   0        0        0        0 2023-05-02 17:07:31.243637 jaaql-middleware-python-4.7.3/jaaql/openapi/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.7.3/jaaql/openapi/__init__.py
+-rw-rw-rw-   0        0        0    28821 2023-05-02 11:33:27.000000 jaaql-middleware-python-4.7.3/jaaql/openapi/swagger_documentation.py
+-rw-rw-rw-   0        0        0      149 2022-06-11 20:45:39.000000 jaaql-middleware-python-4.7.3/jaaql/patch.py
+drwxrwxrwx   0        0        0        0 2023-05-02 17:07:31.250639 jaaql-middleware-python-4.7.3/jaaql/scripts/
+-rw-rw-rw-   0        0        0     1379 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.3/jaaql/scripts/01.install_domains.generated.sql
+-rw-rw-rw-   0        0        0      939 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.3/jaaql/scripts/02.install_super_user.exceptions.sql
+-rw-rw-rw-   0        0        0     1859 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.3/jaaql/scripts/03.install_super_user.handwritten.sql
+-rw-rw-rw-   0        0        0     7492 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.3/jaaql/scripts/04.install_jaaql_data_structures.generated.sql
+-rw-rw-rw-   0        0        0      324 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.3/jaaql/scripts/05.install_jaaql.exceptions.sql
+-rw-rw-rw-   0        0        0      990 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.3/jaaql/scripts/06.install_jaaql.handwritten.sql
+-rw-rw-rw-   0        0        0     4105 2023-02-12 10:12:32.000000 jaaql-middleware-python-4.7.3/jaaql/scripts/swagger_template.html
+drwxrwxrwx   0        0        0        0 2023-05-02 17:07:31.253637 jaaql-middleware-python-4.7.3/jaaql/services/
+-rw-rw-rw-   0        0        0        0 2022-07-10 13:56:37.000000 jaaql-middleware-python-4.7.3/jaaql/services/__init__.py
+-rw-rw-rw-   0        0        0     2688 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.3/jaaql/services/cached_canned_query_service.py
+-rw-rw-rw-   0        0        0     2047 2023-05-02 12:22:14.000000 jaaql-middleware-python-4.7.3/jaaql/services/migrations_manager_service.py
+-rw-rw-rw-   0        0        0      296 2023-05-02 12:09:59.000000 jaaql-middleware-python-4.7.3/jaaql/services/patch_mms.py
+drwxrwxrwx   0        0        0        0 2023-05-02 17:07:31.259639 jaaql-middleware-python-4.7.3/jaaql/utilities/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.7.3/jaaql/utilities/__init__.py
+-rw-rw-rw-   0        0        0     6698 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.3/jaaql/utilities/crypt_utils.py
+-rw-rw-rw-   0        0        0     5357 2023-05-02 10:06:52.000000 jaaql-middleware-python-4.7.3/jaaql/utilities/options.py
+-rw-rw-rw-   0        0        0     5370 2023-05-02 17:00:38.000000 jaaql-middleware-python-4.7.3/jaaql/utilities/utils.py
+-rw-rw-rw-   0        0        0     2428 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.3/jaaql/utilities/utils_no_project_imports.py
+-rw-rw-rw-   0        0        0     2160 2022-05-22 11:21:40.000000 jaaql-middleware-python-4.7.3/jaaql/utilities/vault.py
+drwxrwxrwx   0        0        0        0 2023-05-02 17:07:31.263637 jaaql-middleware-python-4.7.3/jaaql_middleware_python.egg-info/
+-rw-rw-rw-   0        0        0      946 2023-05-02 17:07:31.000000 jaaql-middleware-python-4.7.3/jaaql_middleware_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2192 2023-05-02 17:07:31.000000 jaaql-middleware-python-4.7.3/jaaql_middleware_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 17:07:31.000000 jaaql-middleware-python-4.7.3/jaaql_middleware_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      337 2023-05-02 17:07:31.000000 jaaql-middleware-python-4.7.3/jaaql_middleware_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-02 17:07:31.000000 jaaql-middleware-python-4.7.3/jaaql_middleware_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 17:07:31.264637 jaaql-middleware-python-4.7.3/setup.cfg
+-rw-rw-rw-   0        0        0      893 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.7.3/setup.py
```

### Comparing `jaaql-middleware-python-4.7.2/LICENSE.txt` & `jaaql-middleware-python-4.7.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.7.2/PKG-INFO` & `jaaql-middleware-python-4.7.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-middleware-python
-Version: 4.7.2
+Version: 4.7.3
 Summary: The jaaql package, allowing for rapid development and deployment of RESTful HTTP applications
 Home-page: https://github.com/JAAQL/JAAQL-middleware-python
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-middleware-python-4.7.2/jaaql/constants.py` & `jaaql-middleware-python-4.7.3/jaaql/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-SQL__where = "WHERE"
-SQL__order_by = "ORDER BY"
-SQL__limit = "LIMIT"
-SQL__offset = "OFFSET"
-SQL__asc = "ASC"
-SQL__desc = "DESC"
-SQL__and = "AND"
-SQL__or = "OR"
-SQL__like = "LIKE"
-SQL__eq = "="
-SQL__paren_open = "("
-SQL__paren_close = ")"
-SQL__single_quote = "'"
-SQL__double_quote = '"'
-SQL__lower = "lower"
-SQL__varchar_cast = "::varchar"
-SQL__is_null = "is null"
-
 KEY__username = "username"
 KEY__password = "password"
 KEY__attach_as = "attach_as"
 KEY__ip_address = "ip_address"
 KEY__created = "created"
 KEY__ip_id = "ip_id"
 KEY__application = "application"
@@ -123,15 +105,14 @@
 
 ENDPOINT__send_email = "/send-email"
 ENDPOINT__execute_migrations = "/internal/migrations"
 ENDPOINT__internal_applications = "/internal/applications"
 ENDPOINT__internal_templates = "/internal/emails/templates"
 ENDPOINT__internal_accounts = "/internal/emails/accounts"
 ENDPOINT__is_alive = "/internal/is-alive"
-ENDPOINT__jaaql_emails = "/emails"
 ENDPOINT__report_sentinel_error = "/sentinel/reporting/error"
 ENDPOINT__install = "/internal/install"
 
 CONFIG__default = "Default config"
 CONFIG__default_desc = "Default config description"
 DATASET__default = "Default dataset"
 DATASET__default_desc = "Default dataset description"
@@ -143,9 +124,9 @@
 USERNAME__anonymous = "anonymous"
 PASSWORD__anonymous = "jaaql_public_password"
 ROLE__jaaql = "jaaql"
 ROLE__postgres = "postgres"
 
 PROTOCOL__postgres = "postgresql://"
 
-VERSION = "4.7.2"
+VERSION = "4.7.3"
```

### Comparing `jaaql-middleware-python-4.7.2/jaaql/db/db_interface.py` & `jaaql-middleware-python-4.7.3/jaaql/db/db_interface.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.7.2/jaaql/db/db_pg_interface.py` & `jaaql-middleware-python-4.7.3/jaaql/db/db_pg_interface.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.7.2/jaaql/db/db_utils.py` & `jaaql-middleware-python-4.7.3/jaaql/db/db_utils.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.7.2/jaaql/documentation/documentation_internal.py` & `jaaql-middleware-python-4.7.3/jaaql/documentation/documentation_internal.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.7.2/jaaql/documentation/documentation_public.py` & `jaaql-middleware-python-4.7.3/jaaql/documentation/documentation_public.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.7.2/jaaql/documentation/documentation_shared.py` & `jaaql-middleware-python-4.7.3/jaaql/documentation/documentation_shared.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.7.2/jaaql/email/email_manager.py` & `jaaql-middleware-python-4.7.3/jaaql/email/email_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 
 from typing import Callable
-from jaaql.email.email_manager_service import Email, TYPE__email_attachments
+from jaaql.email.email_manager_service import Email
 import requests
 from jaaql.exceptions.http_status_exception import HttpStatusException
 from jaaql.constants import *
 from urllib.parse import quote
 from jaaql.utilities.utils_no_project_imports import load_artifact
 from typing import Optional
 from jaaql.mvc.handmade_queries import *
```

### Comparing `jaaql-middleware-python-4.7.2/jaaql/email/email_manager_service.py` & `jaaql-middleware-python-4.7.3/jaaql/email/email_manager_service.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.7.2/jaaql/exceptions/http_status_exception.py` & `jaaql-middleware-python-4.7.3/jaaql/exceptions/http_status_exception.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.7.2/jaaql/interpreter/interpret_jaaql.py` & `jaaql-middleware-python-4.7.3/jaaql/interpreter/interpret_jaaql.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.7.2/jaaql/jaaql.py` & `jaaql-middleware-python-4.7.3/jaaql/jaaql.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.7.2/jaaql/migrations/migration_history.sql` & `jaaql-middleware-python-4.7.3/jaaql/migrations/migration_history.sql`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.7.2/jaaql/migrations/migrations.py` & `jaaql-middleware-python-4.7.3/jaaql/migrations/migrations.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from jaaql.utilities.utils import time_delta_ms, get_jaaql_root, loc, get_base_url, get_external_url
 from datetime import datetime
 import hashlib
 from os.path import join, isdir
 from os import listdir, environ
 from jaaql.interpreter.interpret_jaaql import InterpretJAAQL
 from jaaql.exceptions.http_status_exception import HttpStatusException
-from jaaql.db.db_utils import create_interface
 from jaaql.utilities.crypt_utils import encrypt_raw
 import re
 from jaaql.utilities.crypt_utils import AES__iv_length
 from monitor.main import initialise, MARKER__bypass, MARKER__jaaql_bypass
 from jaaql.constants import USERNAME__jaaql, USERNAME__super_db, DB__jaaql, DB__postgres
 
 
@@ -37,20 +36,14 @@
 
 PROJECT_JAAQL = "JAAQL"
 
 REGEX__migration_replacement = r'{{JAAQL__[A-Z_]+}}'
 REGEX__migration_replacement_and_encrypt = r'#{{JAAQL__[A-Z_]+}}'
 
 
-def create_interface_for_db(config, super_credentials: str, database: str, sub_role: str):
-    address, port, _, username, password = DBInterface.fracture_uri(super_credentials)
-
-    return create_interface(config, address, port, database, username, password=password, sub_role=sub_role)
-
-
 def replace_options_environment_variables(query: str, parsed_options: dict, crypt_key: bytes, is_deployed: bool, config, fixed_salt: bool):
     last_index = 0
     prepared = ""
     for match in re.finditer(REGEX__migration_replacement_and_encrypt, query):
         start_pos = match.regs[0][0]
         end_pos = match.regs[0][1]
         match_str = query[start_pos + 3 + len("JAAQL__"):end_pos - 2]
```

### Comparing `jaaql-middleware-python-4.7.2/jaaql/mvc/base_controller.py` & `jaaql-middleware-python-4.7.3/jaaql/mvc/base_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from queue import Queue
 from jaaql.utilities.utils import time_delta_ms, Profiler
 from flask import Response, Flask, request, jsonify, current_app
 from jaaql.constants import *
 from jaaql.mvc.model import JAAQLModel
 from jaaql.mvc.response import JAAQLResponse
 from typing import Union
+from jaaql.utilities.utils import create_interface_for_db
 from monitor.main import HEADER__security, HEADER__security_bypass_jaaql, HEADER__security_bypass
 
 from jaaql.openapi.swagger_documentation import SwaggerDocumentation, SwaggerMethod, TYPE__response, \
     SwaggerFlatResponse, REST__DELETE, REST__GET, REST__OPTIONS, REST__POST, REST__PUT, SwaggerList, SwaggerResponse, \
     MOCK__description, ARG_RESP__allow_all, RES__allow_all, SwaggerArgumentResponse, SwaggerSimpleList
 from jaaql.exceptions.http_status_exception import *
 
@@ -479,20 +480,22 @@
 
                         # Do not close created interfaces as they are re-used
                         for arg in inspect.getfullargspec(view_func_local).args:
                             if arg.startswith(ARG_START__connection):
                                 if not swagger_documentation.security:
                                     raise Exception(ERR__method_required_user_connection)
                                 connect_db = arg.split(ARG_START__connection)[1]
-                                supply_dict[arg] = self.model.create_interface_for_db(account_id, connect_db, sub_role=account_id)
+                                supply_dict[arg] = create_interface_for_db(self.model.vault, self.model.config, account_id, connect_db,
+                                                                           sub_role=account_id)
 
                         for arg in inspect.getfullargspec(view_func_local).args:
                             if arg.startswith(ARG_START__jaaql_connection):
                                 connect_db = arg.split(ARG_START__jaaql_connection)[1]
-                                supply_dict[arg] = self.model.create_interface_for_db(account_id, connect_db, sub_role=ROLE__jaaql)
+                                supply_dict[arg] = create_interface_for_db(self.model.vault, self.model.config, account_id, connect_db,
+                                                                           sub_role=ROLE__jaaql)
 
                         if ARG__username in inspect.getfullargspec(view_func_local).args:
                             if not swagger_documentation.security:
                                 raise Exception(ERR__method_required_username)
                             supply_dict[ARG__username] = username
 
                         if ARG__ip_address in inspect.getfullargspec(view_func_local).args:
@@ -508,15 +511,15 @@
 
                         if ARG__auth_token_for_refresh in inspect.getfullargspec(view_func_local).args:
                             supply_dict[ARG__auth_token_for_refresh] = request.headers.get(HEADER__security)
 
                         if ARG__connection in inspect.getfullargspec(view_func_local).args:
                             if not swagger_documentation.security:
                                 raise Exception(ERR__method_required_connection)
-                            supply_dict[ARG__connection] = self.model.create_interface_for_db(account_id, DB__jaaql)
+                            supply_dict[ARG__connection] = create_interface_for_db(self.model.vault, self.model.config, account_id, DB__jaaql)
 
                         if ARG__is_the_anonymous_user in inspect.getfullargspec(view_func_local).args:
                             if not swagger_documentation.security:
                                 raise Exception(ERR__method_required_is_the_anonymous_user)
                             supply_dict[ARG__is_the_anonymous_user] = is_public
 
                         self.perform_profile(request_id, "Fetch args")
```

### Comparing `jaaql-middleware-python-4.7.2/jaaql/mvc/base_model.py` & `jaaql-middleware-python-4.7.3/jaaql/mvc/base_model.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.7.2/jaaql/mvc/controller.py` & `jaaql-middleware-python-4.7.3/jaaql/mvc/controller.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.7.2/jaaql/mvc/exception_queries.py` & `jaaql-middleware-python-4.7.3/jaaql/mvc/exception_queries.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.7.2/jaaql/mvc/generated_queries.py` & `jaaql-middleware-python-4.7.3/jaaql/mvc/generated_queries.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.7.2/jaaql/mvc/model.py` & `jaaql-middleware-python-4.7.3/jaaql/mvc/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from jaaql.documentation.documentation_public import KEY__oauth_token
 from jaaql.mvc.base_model import BaseJAAQLModel, VAULT_KEY__jwt_crypt_key
 from jaaql.exceptions.http_status_exception import HttpStatusException, HTTPStatus, ERR__already_installed
 from os.path import join
 from jaaql.constants import *
 from jaaql.mvc.response import JAAQLResponse
 from jaaql.interpreter.interpret_jaaql import InterpretJAAQL, ASSERT_one, KEY_assert, KEY_query, KEY_parameters
-from jaaql.utilities.utils import get_jaaql_root, get_base_url
+from jaaql.utilities.utils import get_jaaql_root, get_base_url, create_interface_for_db
 from jaaql.db.db_utils import create_interface, jaaql__encrypt
 from jaaql.utilities import crypt_utils
 import threading
 from datetime import datetime, timedelta
 from jaaql.mvc.handmade_queries import *
 from jwt.utils import base64url_decode
 import json
@@ -462,19 +462,14 @@
 
         if response is not None:
             response.account_id = str(account[KG__account__id]),
             response.ip_id = str(address)
 
         return crypt_utils.jwt_encode(self.vault.get_obj(VAULT_KEY__jwt_crypt_key), jwt_data, JWT_PURPOSE__oauth, expiry_ms=self.token_expiry_ms)
 
-    def create_interface_for_db(self, user_id: str, database: str, sub_role: str = None):
-        jaaql_uri = self.vault.get_obj(VAULT_KEY__super_db_credentials)
-        address, port, _, username, password = DBInterface.fracture_uri(jaaql_uri)
-        return create_interface(self.config, address, port, database, username, password=password, role=user_id, sub_role=sub_role)
-
     def attach_dispatcher_credentials(self, connection: DBInterface, inputs: dict):
         email_dispatcher__update(connection, self.get_db_crypt_key(), **inputs)
 
     def send_email(self, application: str, template: str, application_artifacts_source: str, application_base_url: str, account_id: str,
                    parameters: dict = None, parameter_id: str = None, none_sanitized_parameters: dict = None):
         if none_sanitized_parameters is None:
             none_sanitized_parameters = {}
@@ -769,12 +764,12 @@
 
             inputs[KEY__database] = found_db
 
         if KEY__database not in inputs:
             inputs[KEY__database] = DB__jaaql
 
         sub_role = inputs.pop(KEY__role) if KEY__role in inputs else None
-        required_db = self.create_interface_for_db(account_id, inputs[KEY__database], sub_role)
+        required_db = create_interface_for_db(self.vault, self.config, account_id, inputs[KEY__database], sub_role)
 
         return InterpretJAAQL(required_db).transform(inputs, skip_commit=inputs.get(KEY__read_only), wait_hook=verification_hook,
                                                      encryption_key=self.get_db_crypt_key(),
                                                      canned_query_service=self.cached_canned_query_service)
```

### Comparing `jaaql-middleware-python-4.7.2/jaaql/openapi/swagger_documentation.py` & `jaaql-middleware-python-4.7.3/jaaql/openapi/swagger_documentation.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.7.2/jaaql/scripts/01.install_domains.generated.sql` & `jaaql-middleware-python-4.7.3/jaaql/scripts/01.install_domains.generated.sql`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.7.2/jaaql/scripts/02.install_super_user.exceptions.sql` & `jaaql-middleware-python-4.7.3/jaaql/scripts/02.install_super_user.exceptions.sql`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.7.2/jaaql/scripts/03.install_super_user.handwritten.sql` & `jaaql-middleware-python-4.7.3/jaaql/scripts/03.install_super_user.handwritten.sql`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.7.2/jaaql/scripts/04.install_jaaql_data_structures.generated.sql` & `jaaql-middleware-python-4.7.3/jaaql/scripts/04.install_jaaql_data_structures.generated.sql`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.7.2/jaaql/scripts/06.install_jaaql.handwritten.sql` & `jaaql-middleware-python-4.7.3/jaaql/scripts/06.install_jaaql.handwritten.sql`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.7.2/jaaql/scripts/swagger_template.html` & `jaaql-middleware-python-4.7.3/jaaql/scripts/swagger_template.html`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.7.2/jaaql/services/cached_canned_query_service.py` & `jaaql-middleware-python-4.7.3/jaaql/services/cached_canned_query_service.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.7.2/jaaql/services/migrations_manager_service.py` & `jaaql-middleware-python-4.7.3/jaaql/services/migrations_manager_service.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.7.2/jaaql/utilities/crypt_utils.py` & `jaaql-middleware-python-4.7.3/jaaql/utilities/crypt_utils.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.7.2/jaaql/utilities/options.py` & `jaaql-middleware-python-4.7.3/jaaql/utilities/options.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.7.2/jaaql/utilities/utils.py` & `jaaql-middleware-python-4.7.3/jaaql/utilities/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import requests
 from os.path import join, exists, dirname
 from datetime import datetime
 import os
 import glob
-from jaaql.constants import DIR__config, FILE__config, CONFIG_KEY__server, CONFIG_KEY_SERVER__port, ENVIRON__install_path, PORT__ems, PORT__mms
+from jaaql.constants import DIR__config, FILE__config, CONFIG_KEY__server, CONFIG_KEY_SERVER__port, ENVIRON__install_path, PORT__ems, PORT__mms,\
+    VAULT_KEY__super_db_credentials
 from jaaql.config_constants import *
 from jaaql.db.db_interface import DBInterface
 from jaaql.db.db_utils import create_interface
 from jaaql.constants import VAULT_KEY__jaaql_lookup_connection
 import configparser
 import time
 import urllib.parse
@@ -143,7 +144,13 @@
     return create_interface(config, address, port, db, username, password)
 
 
 def get_db_connection_as_jaaql(config, vault, db: str):
     jaaql_uri = vault.get_obj(VAULT_KEY__jaaql_lookup_connection)
     address, port, _, username, password = DBInterface.fracture_uri(jaaql_uri)
     return create_interface(config, address, port, db, username, password)
+
+
+def create_interface_for_db(vault, config, user_id: str, database: str, sub_role: str = None):
+    jaaql_uri = vault.get_obj(VAULT_KEY__super_db_credentials)
+    address, port, _, username, password = DBInterface.fracture_uri(jaaql_uri)
+    return create_interface(config, address, port, database, username, password=password, role=user_id, sub_role=sub_role)
```

### Comparing `jaaql-middleware-python-4.7.2/jaaql/utilities/utils_no_project_imports.py` & `jaaql-middleware-python-4.7.3/jaaql/utilities/utils_no_project_imports.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.7.2/jaaql/utilities/vault.py` & `jaaql-middleware-python-4.7.3/jaaql/utilities/vault.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.7.2/jaaql_middleware_python.egg-info/PKG-INFO` & `jaaql-middleware-python-4.7.3/jaaql_middleware_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-middleware-python
-Version: 4.7.2
+Version: 4.7.3
 Summary: The jaaql package, allowing for rapid development and deployment of RESTful HTTP applications
 Home-page: https://github.com/JAAQL/JAAQL-middleware-python
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-middleware-python-4.7.2/jaaql_middleware_python.egg-info/SOURCES.txt` & `jaaql-middleware-python-4.7.3/jaaql_middleware_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.7.2/setup.py` & `jaaql-middleware-python-4.7.3/setup.py`

 * *Files identical despite different names*

