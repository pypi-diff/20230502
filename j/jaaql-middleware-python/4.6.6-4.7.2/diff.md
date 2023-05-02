# Comparing `tmp/jaaql-middleware-python-4.6.6.tar.gz` & `tmp/jaaql-middleware-python-4.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaaql-middleware-python-4.6.6.tar", last modified: Wed Apr 19 14:39:38 2023, max compression
+gzip compressed data, was "jaaql-middleware-python-4.7.2.tar", last modified: Tue May  2 12:59:49 2023, max compression
```

## Comparing `jaaql-middleware-python-4.6.6.tar` & `jaaql-middleware-python-4.7.2.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 14:39:38.137682 jaaql-middleware-python-4.6.6/
--rw-rw-rw-   0        0        0    18134 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.6/LICENSE.txt
--rw-rw-rw-   0        0        0      946 2023-04-19 14:39:38.136682 jaaql-middleware-python-4.6.6/PKG-INFO
--rw-rw-rw-   0        0        0      453 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 14:39:38.073112 jaaql-middleware-python-4.6.6/jaaql/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.6/jaaql/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 14:39:38.077109 jaaql-middleware-python-4.6.6/jaaql/config/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.6/jaaql/config/__init__.py
--rw-rw-rw-   0        0        0      324 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/config/config-docker.ini
--rw-rw-rw-   0        0        0      253 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/config/config-test.ini
--rw-rw-rw-   0        0        0      291 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/config/config.ini
--rw-rw-rw-   0        0        0      470 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/config_constants.py
--rw-rw-rw-   0        0        0     4835 2023-04-19 14:39:36.000000 jaaql-middleware-python-4.6.6/jaaql/constants.py
-drwxrwxrwx   0        0        0        0 2023-04-19 14:39:38.081109 jaaql-middleware-python-4.6.6/jaaql/db/
--rw-rw-rw-   0        0        0        0 2022-05-19 20:40:08.000000 jaaql-middleware-python-4.6.6/jaaql/db/__init__.py
--rw-rw-rw-   0        0        0     7043 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/db/db_interface.py
--rw-rw-rw-   0        0        0    11198 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/db/db_pg_interface.py
--rw-rw-rw-   0        0        0     6545 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/db/db_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-19 14:39:38.085110 jaaql-middleware-python-4.6.6/jaaql/documentation/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.6/jaaql/documentation/__init__.py
--rw-rw-rw-   0        0        0     6320 2023-04-06 12:25:17.000000 jaaql-middleware-python-4.6.6/jaaql/documentation/documentation_internal.py
--rw-rw-rw-   0        0        0     8192 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/documentation/documentation_public.py
--rw-rw-rw-   0        0        0     3456 2023-04-04 18:02:26.000000 jaaql-middleware-python-4.6.6/jaaql/documentation/documentation_shared.py
-drwxrwxrwx   0        0        0        0 2023-04-19 14:39:38.089113 jaaql-middleware-python-4.6.6/jaaql/email/
--rw-rw-rw-   0        0        0        0 2022-05-05 10:44:50.000000 jaaql-middleware-python-4.6.6/jaaql/email/__init__.py
--rw-rw-rw-   0        0        0     3687 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/email/email_manager.py
--rw-rw-rw-   0        0        0    19242 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/email/email_manager_service.py
--rw-rw-rw-   0        0        0      234 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/email/patch_ems.py
-drwxrwxrwx   0        0        0        0 2023-04-19 14:39:38.093109 jaaql-middleware-python-4.6.6/jaaql/exceptions/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.6/jaaql/exceptions/__init__.py
--rw-rw-rw-   0        0        0      401 2022-04-17 07:42:21.000000 jaaql-middleware-python-4.6.6/jaaql/exceptions/custom_http_status.py
--rw-rw-rw-   0        0        0      985 2022-05-20 15:36:28.000000 jaaql-middleware-python-4.6.6/jaaql/exceptions/http_status_exception.py
--rw-rw-rw-   0        0        0      321 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.6/jaaql/exceptions/not_yet_implement_exception.py
-drwxrwxrwx   0        0        0        0 2023-04-19 14:39:38.095145 jaaql-middleware-python-4.6.6/jaaql/interpreter/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.6/jaaql/interpreter/__init__.py
--rw-rw-rw-   0        0        0    23250 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/interpreter/interpret_jaaql.py
--rw-rw-rw-   0        0        0     6003 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/jaaql.py
-drwxrwxrwx   0        0        0        0 2023-04-19 14:39:38.098109 jaaql-middleware-python-4.6.6/jaaql/migrations/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.6/jaaql/migrations/__init__.py
--rw-rw-rw-   0        0        0      683 2022-09-19 00:09:13.000000 jaaql-middleware-python-4.6.6/jaaql/migrations/migration_history.sql
--rw-rw-rw-   0        0        0    10802 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/migrations/migrations.py
-drwxrwxrwx   0        0        0        0 2023-04-19 14:39:38.110109 jaaql-middleware-python-4.6.6/jaaql/mvc/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.6/jaaql/mvc/__init__.py
--rw-rw-rw-   0        0        0    31004 2023-04-17 22:16:44.000000 jaaql-middleware-python-4.6.6/jaaql/mvc/base_controller.py
--rw-rw-rw-   0        0        0    25344 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/mvc/base_model.py
--rw-rw-rw-   0        0        0     3727 2023-04-17 22:18:42.000000 jaaql-middleware-python-4.6.6/jaaql/mvc/controller.py
--rw-rw-rw-   0        0        0      274 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.6/jaaql/mvc/controller_interface.py
--rw-rw-rw-   0        0        0     7494 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/mvc/exception_queries.py
--rw-rw-rw-   0        0        0    43043 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/mvc/generated_queries.py
--rw-rw-rw-   0        0        0      232 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/mvc/handmade_queries.py
--rw-rw-rw-   0        0        0    41782 2023-04-17 22:17:20.000000 jaaql-middleware-python-4.6.6/jaaql/mvc/model.py
--rw-rw-rw-   0        0        0      257 2022-05-07 20:33:26.000000 jaaql-middleware-python-4.6.6/jaaql/mvc/model_interface.py
--rw-rw-rw-   0        0        0      209 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/mvc/response.py
-drwxrwxrwx   0        0        0        0 2023-04-19 14:39:38.112110 jaaql-middleware-python-4.6.6/jaaql/openapi/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.6/jaaql/openapi/__init__.py
--rw-rw-rw-   0        0        0    28797 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/openapi/swagger_documentation.py
--rw-rw-rw-   0        0        0      149 2022-06-11 20:45:39.000000 jaaql-middleware-python-4.6.6/jaaql/patch.py
-drwxrwxrwx   0        0        0        0 2023-04-19 14:39:38.119684 jaaql-middleware-python-4.6.6/jaaql/scripts/
--rw-rw-rw-   0        0        0     1379 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/scripts/01.install_domains.generated.sql
--rw-rw-rw-   0        0        0      939 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/scripts/02.install_super_user.exceptions.sql
--rw-rw-rw-   0        0        0     1859 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/scripts/03.install_super_user.handwritten.sql
--rw-rw-rw-   0        0        0     7492 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/scripts/04.install_jaaql_data_structures.generated.sql
--rw-rw-rw-   0        0        0      324 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/scripts/05.install_jaaql.exceptions.sql
--rw-rw-rw-   0        0        0      990 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/scripts/06.install_jaaql.handwritten.sql
--rw-rw-rw-   0        0        0     4105 2023-02-12 10:12:32.000000 jaaql-middleware-python-4.6.6/jaaql/scripts/swagger_template.html
-drwxrwxrwx   0        0        0        0 2023-04-19 14:39:38.123683 jaaql-middleware-python-4.6.6/jaaql/services/
--rw-rw-rw-   0        0        0        0 2022-07-10 13:56:37.000000 jaaql-middleware-python-4.6.6/jaaql/services/__init__.py
--rw-rw-rw-   0        0        0     2688 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/services/cached_canned_query_service.py
--rw-rw-rw-   0        0        0      293 2022-07-14 16:23:21.000000 jaaql-middleware-python-4.6.6/jaaql/services/patch_script_install.py
--rw-rw-rw-   0        0        0     3247 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/services/script_install.py
-drwxrwxrwx   0        0        0        0 2023-04-19 14:39:38.128682 jaaql-middleware-python-4.6.6/jaaql/utilities/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.6/jaaql/utilities/__init__.py
--rw-rw-rw-   0        0        0     6698 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/utilities/crypt_utils.py
--rw-rw-rw-   0        0        0     5603 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/utilities/options.py
--rw-rw-rw-   0        0        0     4725 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/utilities/utils.py
--rw-rw-rw-   0        0        0     2428 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/utilities/utils_no_project_imports.py
--rw-rw-rw-   0        0        0     2160 2022-05-22 11:21:40.000000 jaaql-middleware-python-4.6.6/jaaql/utilities/vault.py
-drwxrwxrwx   0        0        0        0 2023-04-19 14:39:38.135683 jaaql-middleware-python-4.6.6/jaaql_middleware_python.egg-info/
--rw-rw-rw-   0        0        0      946 2023-04-19 14:39:37.000000 jaaql-middleware-python-4.6.6/jaaql_middleware_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2191 2023-04-19 14:39:38.000000 jaaql-middleware-python-4.6.6/jaaql_middleware_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 14:39:37.000000 jaaql-middleware-python-4.6.6/jaaql_middleware_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      315 2023-04-19 14:39:38.000000 jaaql-middleware-python-4.6.6/jaaql_middleware_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-19 14:39:38.000000 jaaql-middleware-python-4.6.6/jaaql_middleware_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 14:39:38.137682 jaaql-middleware-python-4.6.6/setup.cfg
--rw-rw-rw-   0        0        0      893 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 12:59:49.140244 jaaql-middleware-python-4.7.2/
+-rw-rw-rw-   0        0        0    18134 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.7.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      946 2023-05-02 12:59:49.140244 jaaql-middleware-python-4.7.2/PKG-INFO
+-rw-rw-rw-   0        0        0      453 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 12:59:49.085244 jaaql-middleware-python-4.7.2/jaaql/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.7.2/jaaql/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 12:59:49.089244 jaaql-middleware-python-4.7.2/jaaql/config/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.7.2/jaaql/config/__init__.py
+-rw-rw-rw-   0        0        0      324 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.2/jaaql/config/config-docker.ini
+-rw-rw-rw-   0        0        0      253 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.2/jaaql/config/config-test.ini
+-rw-rw-rw-   0        0        0      291 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.2/jaaql/config/config.ini
+-rw-rw-rw-   0        0        0      470 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.2/jaaql/config_constants.py
+-rw-rw-rw-   0        0        0     4862 2023-05-02 12:58:07.000000 jaaql-middleware-python-4.7.2/jaaql/constants.py
+drwxrwxrwx   0        0        0        0 2023-05-02 12:59:49.092244 jaaql-middleware-python-4.7.2/jaaql/db/
+-rw-rw-rw-   0        0        0        0 2022-05-19 20:40:08.000000 jaaql-middleware-python-4.7.2/jaaql/db/__init__.py
+-rw-rw-rw-   0        0        0     7043 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.2/jaaql/db/db_interface.py
+-rw-rw-rw-   0        0        0    11198 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.2/jaaql/db/db_pg_interface.py
+-rw-rw-rw-   0        0        0     6545 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.2/jaaql/db/db_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-02 12:59:49.096243 jaaql-middleware-python-4.7.2/jaaql/documentation/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.7.2/jaaql/documentation/__init__.py
+-rw-rw-rw-   0        0        0     6592 2023-05-02 12:22:14.000000 jaaql-middleware-python-4.7.2/jaaql/documentation/documentation_internal.py
+-rw-rw-rw-   0        0        0     8192 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.2/jaaql/documentation/documentation_public.py
+-rw-rw-rw-   0        0        0     3456 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.2/jaaql/documentation/documentation_shared.py
+drwxrwxrwx   0        0        0        0 2023-05-02 12:59:49.099243 jaaql-middleware-python-4.7.2/jaaql/email/
+-rw-rw-rw-   0        0        0        0 2022-05-05 10:44:50.000000 jaaql-middleware-python-4.7.2/jaaql/email/__init__.py
+-rw-rw-rw-   0        0        0     3687 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.2/jaaql/email/email_manager.py
+-rw-rw-rw-   0        0        0    19242 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.2/jaaql/email/email_manager_service.py
+-rw-rw-rw-   0        0        0      234 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.2/jaaql/email/patch_ems.py
+drwxrwxrwx   0        0        0        0 2023-05-02 12:59:49.103243 jaaql-middleware-python-4.7.2/jaaql/exceptions/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.7.2/jaaql/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      401 2022-04-17 07:42:21.000000 jaaql-middleware-python-4.7.2/jaaql/exceptions/custom_http_status.py
+-rw-rw-rw-   0        0        0      985 2022-05-20 15:36:28.000000 jaaql-middleware-python-4.7.2/jaaql/exceptions/http_status_exception.py
+-rw-rw-rw-   0        0        0      321 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.7.2/jaaql/exceptions/not_yet_implement_exception.py
+drwxrwxrwx   0        0        0        0 2023-05-02 12:59:49.105244 jaaql-middleware-python-4.7.2/jaaql/interpreter/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.7.2/jaaql/interpreter/__init__.py
+-rw-rw-rw-   0        0        0    23250 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.2/jaaql/interpreter/interpret_jaaql.py
+-rw-rw-rw-   0        0        0     5962 2023-05-02 12:06:24.000000 jaaql-middleware-python-4.7.2/jaaql/jaaql.py
+drwxrwxrwx   0        0        0        0 2023-05-02 12:59:49.107244 jaaql-middleware-python-4.7.2/jaaql/migrations/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.7.2/jaaql/migrations/__init__.py
+-rw-rw-rw-   0        0        0      683 2022-09-19 00:09:13.000000 jaaql-middleware-python-4.7.2/jaaql/migrations/migration_history.sql
+-rw-rw-rw-   0        0        0     8913 2023-05-02 12:47:13.000000 jaaql-middleware-python-4.7.2/jaaql/migrations/migrations.py
+drwxrwxrwx   0        0        0        0 2023-05-02 12:59:49.117243 jaaql-middleware-python-4.7.2/jaaql/mvc/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.7.2/jaaql/mvc/__init__.py
+-rw-rw-rw-   0        0        0    32327 2023-05-02 11:26:06.000000 jaaql-middleware-python-4.7.2/jaaql/mvc/base_controller.py
+-rw-rw-rw-   0        0        0    11591 2023-05-02 12:24:40.000000 jaaql-middleware-python-4.7.2/jaaql/mvc/base_model.py
+-rw-rw-rw-   0        0        0     3928 2023-05-02 12:51:04.000000 jaaql-middleware-python-4.7.2/jaaql/mvc/controller.py
+-rw-rw-rw-   0        0        0      274 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.7.2/jaaql/mvc/controller_interface.py
+-rw-rw-rw-   0        0        0     7494 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.2/jaaql/mvc/exception_queries.py
+-rw-rw-rw-   0        0        0    43043 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.2/jaaql/mvc/generated_queries.py
+-rw-rw-rw-   0        0        0      232 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.2/jaaql/mvc/handmade_queries.py
+-rw-rw-rw-   0        0        0    43432 2023-05-02 12:27:47.000000 jaaql-middleware-python-4.7.2/jaaql/mvc/model.py
+-rw-rw-rw-   0        0        0      257 2022-05-07 20:33:26.000000 jaaql-middleware-python-4.7.2/jaaql/mvc/model_interface.py
+-rw-rw-rw-   0        0        0      209 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.2/jaaql/mvc/response.py
+drwxrwxrwx   0        0        0        0 2023-05-02 12:59:49.118243 jaaql-middleware-python-4.7.2/jaaql/openapi/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.7.2/jaaql/openapi/__init__.py
+-rw-rw-rw-   0        0        0    28821 2023-05-02 11:33:27.000000 jaaql-middleware-python-4.7.2/jaaql/openapi/swagger_documentation.py
+-rw-rw-rw-   0        0        0      149 2022-06-11 20:45:39.000000 jaaql-middleware-python-4.7.2/jaaql/patch.py
+drwxrwxrwx   0        0        0        0 2023-05-02 12:59:49.125243 jaaql-middleware-python-4.7.2/jaaql/scripts/
+-rw-rw-rw-   0        0        0     1379 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.2/jaaql/scripts/01.install_domains.generated.sql
+-rw-rw-rw-   0        0        0      939 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.2/jaaql/scripts/02.install_super_user.exceptions.sql
+-rw-rw-rw-   0        0        0     1859 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.2/jaaql/scripts/03.install_super_user.handwritten.sql
+-rw-rw-rw-   0        0        0     7492 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.2/jaaql/scripts/04.install_jaaql_data_structures.generated.sql
+-rw-rw-rw-   0        0        0      324 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.2/jaaql/scripts/05.install_jaaql.exceptions.sql
+-rw-rw-rw-   0        0        0      990 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.2/jaaql/scripts/06.install_jaaql.handwritten.sql
+-rw-rw-rw-   0        0        0     4105 2023-02-12 10:12:32.000000 jaaql-middleware-python-4.7.2/jaaql/scripts/swagger_template.html
+drwxrwxrwx   0        0        0        0 2023-05-02 12:59:49.128244 jaaql-middleware-python-4.7.2/jaaql/services/
+-rw-rw-rw-   0        0        0        0 2022-07-10 13:56:37.000000 jaaql-middleware-python-4.7.2/jaaql/services/__init__.py
+-rw-rw-rw-   0        0        0     2688 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.2/jaaql/services/cached_canned_query_service.py
+-rw-rw-rw-   0        0        0     2047 2023-05-02 12:22:14.000000 jaaql-middleware-python-4.7.2/jaaql/services/migrations_manager_service.py
+-rw-rw-rw-   0        0        0      296 2023-05-02 12:09:59.000000 jaaql-middleware-python-4.7.2/jaaql/services/patch_mms.py
+drwxrwxrwx   0        0        0        0 2023-05-02 12:59:49.133244 jaaql-middleware-python-4.7.2/jaaql/utilities/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.7.2/jaaql/utilities/__init__.py
+-rw-rw-rw-   0        0        0     6698 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.2/jaaql/utilities/crypt_utils.py
+-rw-rw-rw-   0        0        0     5357 2023-05-02 10:06:52.000000 jaaql-middleware-python-4.7.2/jaaql/utilities/options.py
+-rw-rw-rw-   0        0        0     4970 2023-05-02 12:18:13.000000 jaaql-middleware-python-4.7.2/jaaql/utilities/utils.py
+-rw-rw-rw-   0        0        0     2428 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.7.2/jaaql/utilities/utils_no_project_imports.py
+-rw-rw-rw-   0        0        0     2160 2022-05-22 11:21:40.000000 jaaql-middleware-python-4.7.2/jaaql/utilities/vault.py
+drwxrwxrwx   0        0        0        0 2023-05-02 12:59:49.139244 jaaql-middleware-python-4.7.2/jaaql_middleware_python.egg-info/
+-rw-rw-rw-   0        0        0      946 2023-05-02 12:59:49.000000 jaaql-middleware-python-4.7.2/jaaql_middleware_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2192 2023-05-02 12:59:49.000000 jaaql-middleware-python-4.7.2/jaaql_middleware_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 12:59:49.000000 jaaql-middleware-python-4.7.2/jaaql_middleware_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      337 2023-05-02 12:59:49.000000 jaaql-middleware-python-4.7.2/jaaql_middleware_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-02 12:59:49.000000 jaaql-middleware-python-4.7.2/jaaql_middleware_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 12:59:49.140244 jaaql-middleware-python-4.7.2/setup.cfg
+-rw-rw-rw-   0        0        0      893 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.7.2/setup.py
```

### Comparing `jaaql-middleware-python-4.6.6/LICENSE.txt` & `jaaql-middleware-python-4.7.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.6/PKG-INFO` & `jaaql-middleware-python-4.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-middleware-python
-Version: 4.6.6
+Version: 4.7.2
 Summary: The jaaql package, allowing for rapid development and deployment of RESTful HTTP applications
 Home-page: https://github.com/JAAQL/JAAQL-middleware-python
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-middleware-python-4.6.6/jaaql/constants.py` & `jaaql-middleware-python-4.7.2/jaaql/constants.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-HEADER__security = "Authentication-Token"
-HEADER__security_bypass = "Authentication-Token-Bypass"
-
 SQL__where = "WHERE"
 SQL__order_by = "ORDER BY"
 SQL__limit = "LIMIT"
 SQL__offset = "OFFSET"
 SQL__asc = "ASC"
 SQL__desc = "DESC"
 SQL__and = "AND"
@@ -65,14 +62,15 @@
 
 ENCODING__utf = "UTF-8"
 ENCODING__ascii = "ascii"
 EXAMPLE__jwt = "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.e30.yXvILkvUUCBqAFlAv6wQ1Q-QRAjfe3eSosO949U73Vo"
 
 VAULT_KEY__db_crypt_key = "db_crypt_key"
 VAULT_KEY__db_repeatable_salt = "repeatable_salt"
+VAULT_KEY__super_local_access_key = "super_access_key"
 VAULT_KEY__jaaql_local_access_key = "jaaql_access_key"
 VAULT_KEY__super_db_credentials = "super_db_credentials"
 VAULT_KEY__jaaql_lookup_connection = "jaaql_lookup_connection"
 VAULT_KEY__allow_jaaql_uninstall = "Allow jaaql uninstall"
 VAULT_KEY__jaaql_db_password = "Jaaql DB Password"
 
 # Used for re-installation
@@ -117,16 +115,18 @@
 FORMAT__png = "png"
 
 NODE__host_node = "host"
 DB__jaaql = "jaaql"
 DB__postgres = "postgres"
 
 PORT__ems = 6061
+PORT__mms = 6062
 
 ENDPOINT__send_email = "/send-email"
+ENDPOINT__execute_migrations = "/internal/migrations"
 ENDPOINT__internal_applications = "/internal/applications"
 ENDPOINT__internal_templates = "/internal/emails/templates"
 ENDPOINT__internal_accounts = "/internal/emails/accounts"
 ENDPOINT__is_alive = "/internal/is-alive"
 ENDPOINT__jaaql_emails = "/emails"
 ENDPOINT__report_sentinel_error = "/sentinel/reporting/error"
 ENDPOINT__install = "/internal/install"
@@ -143,9 +143,9 @@
 USERNAME__anonymous = "anonymous"
 PASSWORD__anonymous = "jaaql_public_password"
 ROLE__jaaql = "jaaql"
 ROLE__postgres = "postgres"
 
 PROTOCOL__postgres = "postgresql://"
 
-VERSION = "4.6.6"
+VERSION = "4.7.2"
```

### Comparing `jaaql-middleware-python-4.6.6/jaaql/db/db_interface.py` & `jaaql-middleware-python-4.7.2/jaaql/db/db_interface.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.6/jaaql/db/db_pg_interface.py` & `jaaql-middleware-python-4.7.2/jaaql/db/db_pg_interface.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.6/jaaql/db/db_utils.py` & `jaaql-middleware-python-4.7.2/jaaql/db/db_utils.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.6/jaaql/documentation/documentation_internal.py` & `jaaql-middleware-python-4.7.2/jaaql/documentation/documentation_internal.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,24 @@
                 code=HTTPStatus.UNPROCESSABLE_ENTITY,
                 body=ERR__already_installed
             )
         ]
     )
 )
 
+DOCUMENTATION__migrations = SwaggerDocumentation(
+    tags="Migrations",
+    security=True,
+    methods=SwaggerMethod(
+        name="Execute migrations",
+        description="Executes the migrations. Can only be done by the super user",
+        method=REST__POST
+    )
+)
+
 DOCUMENTATION__is_installed = SwaggerDocumentation(
     tags="Installation",
     security=False,
     methods=SwaggerMethod(
         name="Is installed",
         description="Returns 200 OK if the service has installed otherwise a 422",
         method=REST__GET,
```

### Comparing `jaaql-middleware-python-4.6.6/jaaql/documentation/documentation_public.py` & `jaaql-middleware-python-4.7.2/jaaql/documentation/documentation_public.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.6/jaaql/documentation/documentation_shared.py` & `jaaql-middleware-python-4.7.2/jaaql/documentation/documentation_shared.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.6/jaaql/email/email_manager.py` & `jaaql-middleware-python-4.7.2/jaaql/email/email_manager.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.6/jaaql/email/email_manager_service.py` & `jaaql-middleware-python-4.7.2/jaaql/email/email_manager_service.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.6/jaaql/exceptions/http_status_exception.py` & `jaaql-middleware-python-4.7.2/jaaql/exceptions/http_status_exception.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.6/jaaql/interpreter/interpret_jaaql.py` & `jaaql-middleware-python-4.7.2/jaaql/interpreter/interpret_jaaql.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.6/jaaql/jaaql.py` & `jaaql-middleware-python-4.7.2/jaaql/jaaql.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from logging import StreamHandler
 from jaaql.constants import ENVIRON__vault_key, ENVIRON__jaaql_profiling
 import re
 import logging
 import pkgutil
 from jaaql.openapi.swagger_documentation import produce_all_documentation
 from jaaql.email.email_manager_service import create_flask_app as create_email_service_app
-from jaaql.services.script_install import bootup
+from jaaql.services.migrations_manager_service import bootup
 from typing import List
-from jaaql.utilities.options import parse_options, OPT_KEY__vault_key, OPT_KEY__email_credentials, OPT_KEY__local_install, Option, OPT_KEY__profiling
+from jaaql.utilities.options import parse_options, OPT_KEY__vault_key, Option, OPT_KEY__profiling, OPT_KEY__local_install
 import sys
 import threading
 import os
 import jaaql.documentation as documentation
 from jaaql.utilities.utils import load_config, get_base_url
 from jaaql.mvc.controller import JAAQLController
 from jaaql.mvc.model import JAAQLModel
@@ -76,16 +76,15 @@
 
     if not is_gunicorn:
         options = parse_options(sys.argv, False, additional_options=additional_options)
     else:
         options = {}
 
     if not is_gunicorn:
-        threading.Thread(target=create_email_service_app, args=[options.get(OPT_KEY__vault_key)],
-                         daemon=True).start()
+        threading.Thread(target=create_email_service_app, args=[options.get(OPT_KEY__vault_key)], daemon=True).start()
         threading.Thread(target=bootup, args=[options.get(OPT_KEY__vault_key), False, OPT_KEY__local_install in options], daemon=True).start()
 
     if OPT_KEY__vault_key in options:
         print(WARNING__vault_key_stdin, file=sys.stderr)
         vault_key = options[OPT_KEY__vault_key]
     elif is_gunicorn:
         vault_key = os.environ.get(ENVIRON__vault_key)
```

### Comparing `jaaql-middleware-python-4.6.6/jaaql/migrations/migration_history.sql` & `jaaql-middleware-python-4.7.2/jaaql/migrations/migration_history.sql`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.6/jaaql/migrations/migrations.py` & `jaaql-middleware-python-4.7.2/jaaql/migrations/migrations.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,24 @@
+import os
+
 from jaaql.db.db_interface import DBInterface
 from jaaql.utilities.utils import time_delta_ms, get_jaaql_root, loc, get_base_url, get_external_url
 from datetime import datetime
 import hashlib
 from os.path import join, isdir
 from os import listdir, environ
 from jaaql.interpreter.interpret_jaaql import InterpretJAAQL
 from jaaql.exceptions.http_status_exception import HttpStatusException
 from jaaql.db.db_utils import create_interface
 from jaaql.utilities.crypt_utils import encrypt_raw
 import re
 from jaaql.utilities.crypt_utils import AES__iv_length
+from monitor.main import initialise, MARKER__bypass, MARKER__jaaql_bypass
+from jaaql.constants import USERNAME__jaaql, USERNAME__super_db, DB__jaaql, DB__postgres
+
 
 MIGRATION_HISTORY = "migration_history"
 
 
 QUERY_LOAD_TABLE = "SELECT * FROM %s WHERE project_name = :project_name" % MIGRATION_HISTORY
 ATTR_PROJECT_NAME = "project_name"
 QUERY_INS_TABLE = "INSERT INTO %s (project_name, installed_rank, version, description, script, checksum, execution_time) VALUES (:project_name, :installed_rank, :version, :description, :script, :checksum, :execution_time)" % MIGRATION_HISTORY
@@ -21,63 +26,25 @@
 ATTR_VERSION = "version"
 ATTR_DESCRIPTION = "description"
 ATTR_SCRIPT = "script"
 ATTR_CHECKSUM = "checksum"
 ATTR_EXECUTION_TIME = "execution_time"
 PATH_MIGRATIONS = "migrations"
 SCRIPT_MIGRATION_HISTORY = "migration_history.sql"
-EXTENSION_SQL = ".sql"
+EXTENSION_JAAQL = ".jaaql"
 
 VERSION_SPLIT = "__"
 WORD_SPLIT = "_"
 
 PROJECT_JAAQL = "JAAQL"
 
 REGEX__migration_replacement = r'{{JAAQL__[A-Z_]+}}'
 REGEX__migration_replacement_and_encrypt = r'#{{JAAQL__[A-Z_]+}}'
 
 
-def load_config_file(location: str) -> (str, str, str):
-    ret_role = None
-    ret_databases = None
-    try:
-        the_content = open(location, "r").read()
-
-        if "ROLE=" in the_content:
-            ret_role = the_content.split("ROLE=")[1].split("\r")[0].split("\n")[0].strip()
-        if "DATABASES=" in the_content:
-            ret_databases = the_content.split("DATABASES=")[1].split("\r")[0].split("\n")[0].strip()
-    except:
-        pass
-
-    return ret_role, ret_databases
-
-
-def get_config(role: str, folder_role: str, file_role: str, databases: str,
-               folder_databases: str, file_databases: str):
-    ret_role = "jaaql"
-    ret_databases = ["jaaql"]
-
-    if role is not None:
-        ret_role = role
-    if folder_role is not None:
-        ret_role = folder_role
-    if file_role is not None:
-        ret_role = file_role
-
-    if databases is not None:
-        ret_databases = databases.split(",")
-    if folder_databases is not None:
-        ret_databases = folder_databases.split(",")
-    if file_databases is not None:
-        ret_databases = file_databases.split(",")
-
-    return ret_role, ret_databases
-
-
 def create_interface_for_db(config, super_credentials: str, database: str, sub_role: str):
     address, port, _, username, password = DBInterface.fracture_uri(super_credentials)
 
     return create_interface(config, address, port, database, username, password=password, sub_role=sub_role)
 
 
 def replace_options_environment_variables(query: str, parsed_options: dict, crypt_key: bytes, is_deployed: bool, config, fixed_salt: bool):
@@ -144,81 +111,73 @@
         if not was_null and is_double_quote:
             prepared += '"'
 
     prepared += query[last_index:]
     return prepared
 
 
-def run_migrations(db_interface: DBInterface, is_deployed: bool, project_name: str = None, migration_folder: str = None, config=None,
-                   super_credentials: str = None, options: dict = None, key: bytes = None):
+def run_migrations(host: str, bypass_super: str, bypass_jaaql: str, db_interface: DBInterface, is_deployed: bool, project_name: str = None,
+                   migration_folder: str = None, config=None, options: dict = None, key: bytes = None):
     if migration_folder is None:
         migration_folder = join(get_jaaql_root(), PATH_MIGRATIONS)
 
-    base_override_role, base_override_databases = load_config_file(join(migration_folder, "config"))
-
     if project_name is None:
         project_name = PROJECT_JAAQL
 
     ij = InterpretJAAQL(db_interface)
 
     migration_history = None
     conn = db_interface.get_conn()
 
     statement_load_table = {"query": QUERY_LOAD_TABLE, "parameters": {ATTR_PROJECT_NAME: project_name}}
 
-    dbs = {}
-
     try:
         migration_history = db_interface.objectify(ij.transform(statement_load_table, conn=conn))
     except HttpStatusException:
         print("Migration history table does not exist. Creating")
         db_interface.execute_script_file(conn, join(get_jaaql_root(), PATH_MIGRATIONS, SCRIPT_MIGRATION_HISTORY))
         migration_history = db_interface.objectify(ij.transform(statement_load_table, conn=conn))
 
     installed_scripts = [cur[ATTR_SCRIPT] for cur in migration_history]
     cur_installed_rank = ([-1] + sorted([cur[ATTR_INSTALLED_RANK] for cur in migration_history]))[-1]
 
     version_folders = sorted([version_folder for version_folder in listdir(migration_folder) if
                               isdir(join(migration_folder, version_folder)) and '.' in version_folder])
     for version_folder in version_folders:
-        folder_override_role, folder_override_databases = load_config_file(join(migration_folder, version_folder, "config"))
-
         script_files = sorted([script_file for script_file in listdir(join(migration_folder, version_folder)) if
-                               script_file.endswith(EXTENSION_SQL)])
+                               script_file.endswith(EXTENSION_JAAQL)])
         for script_file in script_files:
-            config_file_name = join(migration_folder, version_folder, script_file.split(EXTENSION_SQL)[0] + ".config")
-            script_override_role, script_override_databases = load_config_file(config_file_name)
             full_name = version_folder + "/" + script_file
-            content = open(join(migration_folder, version_folder, script_file), "r").read()
-            cur_role, cur_databases = get_config(base_override_role, folder_override_role, script_override_role,
-                                                             base_override_databases, folder_override_databases, script_override_databases)
+            actual_file_name = join(migration_folder, version_folder, script_file)
+            content = open(actual_file_name, "r").read()
             content_for_hash = replace_options_environment_variables(content, options, key, is_deployed, config,
                                                                      fixed_salt=True)
             content = replace_options_environment_variables(content, options, key, is_deployed, config,
                                                             fixed_salt=False)
 
-            hash_content = content_for_hash + cur_role + str(cur_databases)
+            hash_content = content_for_hash
             checksum = hashlib.md5(hash_content.encode("UTF-8")).digest()
             checksum = int.from_bytes(checksum[0:3], byteorder="little")
             if full_name not in installed_scripts:
+                config_loc = os.environ.get("JAAQL_CONFIG_LOC", "monitor_config")
+                configs = []
+                for fname in os.listdir(config_loc):
+                    config_name = ".".join(fname.split(".")[0:-1])
+                    configs.append([config_name, fname])
+
+                encoded_configs = [[USERNAME__jaaql, host, USERNAME__jaaql, MARKER__bypass + bypass_super, DB__jaaql],
+                                   [USERNAME__super_db, host, USERNAME__super_db, MARKER__jaaql_bypass + bypass_jaaql, DB__postgres]]
+
                 start_time = datetime.now()
 
-                for db in cur_databases:
-                    if db not in dbs:
-                        dbs[db] = create_interface_for_db(config, super_credentials, db, cur_role)
-                    update_db_interface = dbs[db]
-                    if not hasattr(update_db_interface, "attached_conns"):
-                        update_db_interface.attached_conns = {}
-                    update_db_interface.sub_role = cur_role
-                    if cur_role not in update_db_interface.attached_conns:
-                        update_db_interface.attached_conns[cur_role] = update_db_interface.get_conn()
-                    update_db_interface.execute_script_file(update_db_interface.attached_conns[cur_role], as_content=content)
+                initialise(actual_file_name, content, configs, encoded_configs)
+
                 execution_time = time_delta_ms(start_time, datetime.now())
                 version = script_file.split("__")[0][1:]
-                description = " ".join(script_file.split(VERSION_SPLIT)[1].split(EXTENSION_SQL)[0].split(WORD_SPLIT))
+                description = " ".join(script_file.split(VERSION_SPLIT)[1].split(EXTENSION_JAAQL)[0].split(WORD_SPLIT))
                 ij.transform({
                     "query": QUERY_INS_TABLE,
                     "parameters": {
                         ATTR_PROJECT_NAME: project_name,
                         ATTR_INSTALLED_RANK: cur_installed_rank + 1,
                         ATTR_VERSION: version,
                         ATTR_DESCRIPTION: description,
@@ -231,13 +190,8 @@
             else:
                 existing_checksum = loc(migration_history, ATTR_SCRIPT, full_name)
                 existing_checksum = loc(existing_checksum, ATTR_PROJECT_NAME, project_name)[0][ATTR_CHECKSUM]
                 if checksum != existing_checksum:
                     raise Exception("Migration mismatch for " + script_file + ". Locally calculated checksum " + str(
                         checksum) + " yet in db table found " + str(existing_checksum))
 
-    for cur_db in dbs.values():
-        for cur_conn in cur_db.attached_conns.values():
-            cur_db.put_conn(cur_conn)
-        cur_db.close()
-
     db_interface.put_conn(conn)
```

### Comparing `jaaql-middleware-python-4.6.6/jaaql/mvc/base_controller.py` & `jaaql-middleware-python-4.7.2/jaaql/mvc/base_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from queue import Queue
 from jaaql.utilities.utils import time_delta_ms, Profiler
 from flask import Response, Flask, request, jsonify, current_app
 from jaaql.constants import *
 from jaaql.mvc.model import JAAQLModel
 from jaaql.mvc.response import JAAQLResponse
 from typing import Union
+from monitor.main import HEADER__security, HEADER__security_bypass_jaaql, HEADER__security_bypass
 
 from jaaql.openapi.swagger_documentation import SwaggerDocumentation, SwaggerMethod, TYPE__response, \
     SwaggerFlatResponse, REST__DELETE, REST__GET, REST__OPTIONS, REST__POST, REST__PUT, SwaggerList, SwaggerResponse, \
     MOCK__description, ARG_RESP__allow_all, RES__allow_all, SwaggerArgumentResponse, SwaggerSimpleList
 from jaaql.exceptions.http_status_exception import *
 
 ARG__http_inputs = "http_inputs"
@@ -77,14 +78,17 @@
 BOOL__allowed = {
     "True": True,
     "False": False,
     "true": True,
     "false": False
 }
 
+IPS__local = [
+    "127.0.0.1", "localhost"
+]
 
 class BaseJAAQLController:
 
     sentinel_errors = None
     internal_sentinel = False
 
     def __init__(self, model: JAAQLModel, is_prod: bool, base_url: str, do_profiling: bool = False):
@@ -426,15 +430,32 @@
                     verification_hook = None
                     if method.parallel_verification:
                         verification_hook = Queue()
 
                     ip_addr = request.headers.get(HEADER__real_ip, request.remote_addr).split(",")[0]
 
                     if swagger_documentation.security:
-                        if verification_hook:
+                        bypass_super = request.headers.get(HEADER__security_bypass)
+                        bypass_jaaql = request.headers.get(HEADER__security_bypass_jaaql)
+                        if bypass_super or bypass_jaaql:
+                            if ip_addr not in IPS__local:
+                                raise HttpStatusException("Bypass used in none local context", HTTPStatus.UNAUTHORIZED)
+                            miss_super_bypass = bypass_super and bypass_super != self.model.local_super_access_key
+                            miss_jaaql_bypass = bypass_jaaql and bypass_jaaql != self.model.local_super_access_key
+                            if miss_super_bypass or miss_jaaql_bypass:
+                                raise HttpStatusException("Invalid bypass key", HTTPStatus.UNAUTHORIZED)
+
+                            is_public = False
+                            username = USERNAME__super_db if bypass_super else USERNAME__jaaql
+                            account_id, ip_id = self.model.get_bypass_user(username, ip_addr)
+
+                            if verification_hook:
+                                verification_hook.put((True, None, None))
+
+                        elif verification_hook:
                             account_id, username, ip_id, is_public = self.model.verify_auth_token_threaded(request.headers.get(HEADER__security),
                                                                                                            ip_addr, verification_hook)
                             self.perform_profile(request_id, "Verify JWT Threaded")
                         else:
                             account_id, username, ip_id, is_public = self.model.verify_auth_token(request.headers.get(HEADER__security), ip_addr)
                             self.perform_profile(request_id, "Verify JWT")
```

### Comparing `jaaql-middleware-python-4.6.6/jaaql/mvc/controller.py` & `jaaql-middleware-python-4.7.2/jaaql/mvc/controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,18 @@
         def refresh_oauth_token(auth_token_for_refresh: str, ip_address: str):
             return self.model.refresh_auth_token(auth_token_for_refresh, ip_address)
 
         @self.cors_route(ENDPOINT__install, DOCUMENTATION__install)
         def install(http_inputs: dict):
             return self.model.install(**http_inputs)
 
+        @self.cors_route(ENDPOINT__execute_migrations, DOCUMENTATION__migrations)
+        def execute_migrations(connection: DBInterface):
+            return self.model.execute_migrations(connection)
+
         @self.cors_route('/internal/is_installed', DOCUMENTATION__is_installed)
         def is_installed(response: JAAQLResponse):
             return self.model.is_installed(response)
 
         @self.cors_route(ENDPOINT__is_alive, DOCUMENTATION__is_alive)
         def is_alive():
             self.model.is_alive()
```

### Comparing `jaaql-middleware-python-4.6.6/jaaql/mvc/exception_queries.py` & `jaaql-middleware-python-4.7.2/jaaql/mvc/exception_queries.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.6/jaaql/mvc/generated_queries.py` & `jaaql-middleware-python-4.7.2/jaaql/mvc/generated_queries.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.6/jaaql/mvc/model.py` & `jaaql-middleware-python-4.7.2/jaaql/mvc/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,28 +5,30 @@
 from jaaql.documentation.documentation_public import KEY__oauth_token
 from jaaql.mvc.base_model import BaseJAAQLModel, VAULT_KEY__jwt_crypt_key
 from jaaql.exceptions.http_status_exception import HttpStatusException, HTTPStatus, ERR__already_installed
 from os.path import join
 from jaaql.constants import *
 from jaaql.mvc.response import JAAQLResponse
 from jaaql.interpreter.interpret_jaaql import InterpretJAAQL, ASSERT_one, KEY_assert, KEY_query, KEY_parameters
-from jaaql.utilities.utils import get_jaaql_root
+from jaaql.utilities.utils import get_jaaql_root, get_base_url
 from jaaql.db.db_utils import create_interface, jaaql__encrypt
 from jaaql.utilities import crypt_utils
 import threading
 from datetime import datetime, timedelta
 from jaaql.mvc.handmade_queries import *
 from jwt.utils import base64url_decode
 import json
 import os
 from queue import Queue
 import subprocess
 import time
 import random
 
+from jaaql.migrations.migrations import run_migrations
+
 REGEX__object_name = r'^[0-9a-zA-Z_]{1,63}$'
 
 ERR__invalid_object_name = "Object name '%s' is invalid. Must match regex: " + REGEX__object_name
 ERR__refresh_expired = "Token too old to be used for refresh. Please authenticate again"
 ERR__incorrect_install_key = "Incorrect install key!"
 ERR__invalid_level = "Invalid level!"
 ERR__incorrect_credentials = "Incorrect credentials!"
@@ -273,14 +275,22 @@
             raise HttpStatusException(ERR__incorrect_credentials)
 
     def add_my_account_password(self, account_id: str, username: str, ip_address: str, old_password: str, password: str):
         self.verify_current_password(account_id, old_password)
         self.add_account_password(account_id, password)
         return self.get_auth_token(password=password, ip_address=ip_address, username=username)
 
+    def execute_migrations(self, connection: DBInterface):
+        self.is_super_admin(connection)
+
+        base_url = get_base_url(self.config, self.is_container)
+        run_migrations(base_url, self.local_super_access_key, self.local_jaaql_access_key, self.jaaql_lookup_connection, self.is_container,
+                       self.migration_project_name, migration_folder=self.migration_folder, config=self.config, options=self.options,
+                       key=self.get_db_crypt_key())
+
     def is_installed(self, response: JAAQLResponse):
         if not self.has_installed:
             response.response_code = HTTPStatus.UNPROCESSABLE_ENTITY
             return ERR__not_yet_installed
 
     def is_alive(self):
         version = execute_supplied_statement_singleton(self.jaaql_lookup_connection, "SELECT version() as version;", as_objects=True)[ATTR__version]
@@ -389,14 +399,27 @@
             raise HttpStatusException(ERR__invalid_token, HTTPStatus.UNAUTHORIZED)
 
         if datetime.fromisoformat(decoded[KEY__created]) + timedelta(milliseconds=self.refresh_expiry_ms) < datetime.now():
             raise HttpStatusException(ERR__refresh_expired, HTTPStatus.UNAUTHORIZED)
 
         return self.get_auth_token(decoded[KEY__username], ip_address)
 
+    def get_bypass_user(self, username: str, ip_address: str):
+        account = fetch_most_recent_password_from_username(self.jaaql_lookup_connection, self.get_db_crypt_key(),
+                                                           self.get_vault_repeatable_salt(), username, singleton_code=HTTPStatus.UNAUTHORIZED)
+        salt_user = self.get_repeatable_salt(account[KG__account__id])
+        encrypted_salted_ip_address = jaaql__encrypt(ip_address, self.get_db_crypt_key(), salt_user)
+        address = execute_supplied_statement_singleton(self.jaaql_lookup_connection,
+                                                       QUERY___add_or_update_validated_ip_address,
+                                                       {KG__validated_ip_address__account: account[KG__account__id],
+                                                        KG__validated_ip_address__encrypted_salted_ip_address: encrypted_salted_ip_address},
+                                                       as_objects=True)[KG__validated_ip_address__uuid]
+
+        return account[KG__account__id], address
+
     def get_auth_token(self, username: str, ip_address: str, password: str = None, response: JAAQLResponse = None):
         incorrect_credentials = False
         account = None
         encrypted_salted_ip_address = None
 
         try:
             account = fetch_most_recent_password_from_username(self.jaaql_lookup_connection, self.get_db_crypt_key(),
```

### Comparing `jaaql-middleware-python-4.6.6/jaaql/openapi/swagger_documentation.py` & `jaaql-middleware-python-4.7.2/jaaql/openapi/swagger_documentation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import List, Optional, Union, Any, TypeVar
 from types import ModuleType
 from jaaql.exceptions.http_status_exception import *
-from jaaql.constants import EXAMPLE__jwt, HEADER__security
+from jaaql.constants import EXAMPLE__jwt
+from monitor.main import HEADER__security
 import os
 import shutil
 import yaml as yaml_utils
 import json
 from jaaql.utilities.utils import get_jaaql_root
 from jaaql.constants import VERSION
```

### Comparing `jaaql-middleware-python-4.6.6/jaaql/scripts/01.install_domains.generated.sql` & `jaaql-middleware-python-4.7.2/jaaql/scripts/01.install_domains.generated.sql`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.6/jaaql/scripts/02.install_super_user.exceptions.sql` & `jaaql-middleware-python-4.7.2/jaaql/scripts/02.install_super_user.exceptions.sql`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.6/jaaql/scripts/03.install_super_user.handwritten.sql` & `jaaql-middleware-python-4.7.2/jaaql/scripts/03.install_super_user.handwritten.sql`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.6/jaaql/scripts/04.install_jaaql_data_structures.generated.sql` & `jaaql-middleware-python-4.7.2/jaaql/scripts/04.install_jaaql_data_structures.generated.sql`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.6/jaaql/scripts/06.install_jaaql.handwritten.sql` & `jaaql-middleware-python-4.7.2/jaaql/scripts/06.install_jaaql.handwritten.sql`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.6/jaaql/scripts/swagger_template.html` & `jaaql-middleware-python-4.7.2/jaaql/scripts/swagger_template.html`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.6/jaaql/services/cached_canned_query_service.py` & `jaaql-middleware-python-4.7.2/jaaql/services/cached_canned_query_service.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.6/jaaql/utilities/crypt_utils.py` & `jaaql-middleware-python-4.7.2/jaaql/utilities/crypt_utils.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.6/jaaql/utilities/options.py` & `jaaql-middleware-python-4.7.2/jaaql/utilities/options.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,14 @@
         self.long = long
         self.required = required
         self.description = description
         self.is_flag = is_flag
 
 
 OPT_KEY__vault_key = "vault-key"
-OPT_KEY__email_credentials = "email-credentials"
 OPT_KEY__help = "help"
 OPT_KEY__profiling = "profiling"
 OPT_KEY__local_install = "local_install"
 OPT_KEY__canned_queries = "canned_queries"
 
 DEFAULT_OPTIONS: List[Option] = [
     Option(
@@ -47,21 +46,14 @@
         short="v",
         long=OPT_KEY__vault_key,
         required=False,
         description="Encrypts the jaaql vault which stores internal sensitive information",
         is_flag=False
     ),
     Option(
-        short="e",
-        long=OPT_KEY__email_credentials,
-        required=False,
-        description="Provides email credentials into the JAAQL server",
-        is_flag=False
-    ),
-    Option(
         short="p",
         long=OPT_KEY__profiling,
         required=False,
         description="Will now output profiling information about the request",
         is_flag=True
     ),
     Option(
```

### Comparing `jaaql-middleware-python-4.6.6/jaaql/utilities/utils.py` & `jaaql-middleware-python-4.7.2/jaaql/utilities/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import requests
 from os.path import join, exists, dirname
 from datetime import datetime
 import os
 import glob
-from jaaql.constants import DIR__config, FILE__config, CONFIG_KEY__server, CONFIG_KEY_SERVER__port, ENVIRON__install_path, PORT__ems
+from jaaql.constants import DIR__config, FILE__config, CONFIG_KEY__server, CONFIG_KEY_SERVER__port, ENVIRON__install_path, PORT__ems, PORT__mms
 from jaaql.config_constants import *
 from jaaql.db.db_interface import DBInterface
 from jaaql.db.db_utils import create_interface
 from jaaql.constants import VAULT_KEY__jaaql_lookup_connection
 import configparser
 import time
 import urllib.parse
@@ -123,16 +123,27 @@
             if requests.get("http://127.0.0.1:" + str(PORT__ems) + "/").status_code == 200:
                 break
         except:
             pass
         time.sleep(5)
 
 
+def await_migrations_finished():
+    while True:
+        try:
+            if requests.get("http://127.0.0.1:" + str(PORT__mms) + "/").status_code == 200:
+                break
+        except:
+            pass
+        time.sleep(5)
+
+
 def get_jaaql_connection(config, vault):
     jaaql_uri = vault.get_obj(VAULT_KEY__jaaql_lookup_connection)
     address, port, db, username, password = DBInterface.fracture_uri(jaaql_uri)
     return create_interface(config, address, port, db, username, password)
 
+
 def get_db_connection_as_jaaql(config, vault, db: str):
     jaaql_uri = vault.get_obj(VAULT_KEY__jaaql_lookup_connection)
     address, port, _, username, password = DBInterface.fracture_uri(jaaql_uri)
     return create_interface(config, address, port, db, username, password)
```

### Comparing `jaaql-middleware-python-4.6.6/jaaql/utilities/utils_no_project_imports.py` & `jaaql-middleware-python-4.7.2/jaaql/utilities/utils_no_project_imports.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.6/jaaql/utilities/vault.py` & `jaaql-middleware-python-4.7.2/jaaql/utilities/vault.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.6/jaaql_middleware_python.egg-info/PKG-INFO` & `jaaql-middleware-python-4.7.2/jaaql_middleware_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-middleware-python
-Version: 4.6.6
+Version: 4.7.2
 Summary: The jaaql package, allowing for rapid development and deployment of RESTful HTTP applications
 Home-page: https://github.com/JAAQL/JAAQL-middleware-python
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-middleware-python-4.6.6/jaaql_middleware_python.egg-info/SOURCES.txt` & `jaaql-middleware-python-4.7.2/jaaql_middleware_python.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -49,16 +49,16 @@
 jaaql/scripts/03.install_super_user.handwritten.sql
 jaaql/scripts/04.install_jaaql_data_structures.generated.sql
 jaaql/scripts/05.install_jaaql.exceptions.sql
 jaaql/scripts/06.install_jaaql.handwritten.sql
 jaaql/scripts/swagger_template.html
 jaaql/services/__init__.py
 jaaql/services/cached_canned_query_service.py
-jaaql/services/patch_script_install.py
-jaaql/services/script_install.py
+jaaql/services/migrations_manager_service.py
+jaaql/services/patch_mms.py
 jaaql/utilities/__init__.py
 jaaql/utilities/crypt_utils.py
 jaaql/utilities/options.py
 jaaql/utilities/utils.py
 jaaql/utilities/utils_no_project_imports.py
 jaaql/utilities/vault.py
 jaaql_middleware_python.egg-info/PKG-INFO
```

### Comparing `jaaql-middleware-python-4.6.6/setup.py` & `jaaql-middleware-python-4.7.2/setup.py`

 * *Files identical despite different names*

