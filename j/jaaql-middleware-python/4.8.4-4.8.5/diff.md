# Comparing `tmp/jaaql-middleware-python-4.8.4.tar.gz` & `tmp/jaaql-middleware-python-4.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaaql-middleware-python-4.8.4.tar", last modified: Tue May  2 19:35:49 2023, max compression
+gzip compressed data, was "jaaql-middleware-python-4.8.5.tar", last modified: Tue May  2 20:19:50 2023, max compression
```

## Comparing `jaaql-middleware-python-4.8.4.tar` & `jaaql-middleware-python-4.8.5.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 19:35:49.785686 jaaql-middleware-python-4.8.4/
--rw-rw-rw-   0        0        0    18134 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.4/LICENSE.txt
--rw-rw-rw-   0        0        0      946 2023-05-02 19:35:49.785686 jaaql-middleware-python-4.8.4/PKG-INFO
--rw-rw-rw-   0        0        0      453 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 19:35:49.732686 jaaql-middleware-python-4.8.4/jaaql/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.4/jaaql/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 19:35:49.735686 jaaql-middleware-python-4.8.4/jaaql/config/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.4/jaaql/config/__init__.py
--rw-rw-rw-   0        0        0      324 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.4/jaaql/config/config-docker.ini
--rw-rw-rw-   0        0        0      253 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.4/jaaql/config/config-test.ini
--rw-rw-rw-   0        0        0      291 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.4/jaaql/config/config.ini
--rw-rw-rw-   0        0        0      470 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.4/jaaql/config_constants.py
--rw-rw-rw-   0        0        0     4462 2023-05-02 19:35:46.000000 jaaql-middleware-python-4.8.4/jaaql/constants.py
-drwxrwxrwx   0        0        0        0 2023-05-02 19:35:49.740686 jaaql-middleware-python-4.8.4/jaaql/db/
--rw-rw-rw-   0        0        0        0 2022-05-19 20:40:08.000000 jaaql-middleware-python-4.8.4/jaaql/db/__init__.py
--rw-rw-rw-   0        0        0     6929 2023-05-02 18:15:39.000000 jaaql-middleware-python-4.8.4/jaaql/db/db_interface.py
--rw-rw-rw-   0        0        0    11198 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.4/jaaql/db/db_pg_interface.py
--rw-rw-rw-   0        0        0     7062 2023-05-02 19:35:29.000000 jaaql-middleware-python-4.8.4/jaaql/db/db_utils.py
--rw-rw-rw-   0        0        0     2934 2023-05-02 18:45:07.000000 jaaql-middleware-python-4.8.4/jaaql/db/db_utils_no_circ.py
-drwxrwxrwx   0        0        0        0 2023-05-02 19:35:49.743686 jaaql-middleware-python-4.8.4/jaaql/documentation/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.4/jaaql/documentation/__init__.py
--rw-rw-rw-   0        0        0     6592 2023-05-02 12:22:14.000000 jaaql-middleware-python-4.8.4/jaaql/documentation/documentation_internal.py
--rw-rw-rw-   0        0        0     8192 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.4/jaaql/documentation/documentation_public.py
--rw-rw-rw-   0        0        0     3456 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.4/jaaql/documentation/documentation_shared.py
-drwxrwxrwx   0        0        0        0 2023-05-02 19:35:49.746686 jaaql-middleware-python-4.8.4/jaaql/email/
--rw-rw-rw-   0        0        0        0 2022-05-05 10:44:50.000000 jaaql-middleware-python-4.8.4/jaaql/email/__init__.py
--rw-rw-rw-   0        0        0     7475 2023-05-02 18:34:17.000000 jaaql-middleware-python-4.8.4/jaaql/email/email_manager.py
--rw-rw-rw-   0        0        0    19242 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.4/jaaql/email/email_manager_service.py
--rw-rw-rw-   0        0        0      234 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.4/jaaql/email/patch_ems.py
-drwxrwxrwx   0        0        0        0 2023-05-02 19:35:49.749686 jaaql-middleware-python-4.8.4/jaaql/exceptions/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.4/jaaql/exceptions/__init__.py
--rw-rw-rw-   0        0        0      401 2022-04-17 07:42:21.000000 jaaql-middleware-python-4.8.4/jaaql/exceptions/custom_http_status.py
--rw-rw-rw-   0        0        0      985 2022-05-20 15:36:28.000000 jaaql-middleware-python-4.8.4/jaaql/exceptions/http_status_exception.py
--rw-rw-rw-   0        0        0      321 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.4/jaaql/exceptions/not_yet_implement_exception.py
-drwxrwxrwx   0        0        0        0 2023-05-02 19:35:49.751686 jaaql-middleware-python-4.8.4/jaaql/interpreter/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.4/jaaql/interpreter/__init__.py
--rw-rw-rw-   0        0        0    23250 2023-05-02 18:09:24.000000 jaaql-middleware-python-4.8.4/jaaql/interpreter/interpret_jaaql.py
--rw-rw-rw-   0        0        0     5962 2023-05-02 12:06:24.000000 jaaql-middleware-python-4.8.4/jaaql/jaaql.py
-drwxrwxrwx   0        0        0        0 2023-05-02 19:35:49.753685 jaaql-middleware-python-4.8.4/jaaql/migrations/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.4/jaaql/migrations/__init__.py
--rw-rw-rw-   0        0        0      683 2022-09-19 00:09:13.000000 jaaql-middleware-python-4.8.4/jaaql/migrations/migration_history.sql
--rw-rw-rw-   0        0        0     8574 2023-05-02 19:35:29.000000 jaaql-middleware-python-4.8.4/jaaql/migrations/migrations.py
-drwxrwxrwx   0        0        0        0 2023-05-02 19:35:49.762686 jaaql-middleware-python-4.8.4/jaaql/mvc/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.4/jaaql/mvc/__init__.py
--rw-rw-rw-   0        0        0    32609 2023-05-02 17:45:39.000000 jaaql-middleware-python-4.8.4/jaaql/mvc/base_controller.py
--rw-rw-rw-   0        0        0    11591 2023-05-02 12:24:40.000000 jaaql-middleware-python-4.8.4/jaaql/mvc/base_model.py
--rw-rw-rw-   0        0        0     3928 2023-05-02 12:51:04.000000 jaaql-middleware-python-4.8.4/jaaql/mvc/controller.py
--rw-rw-rw-   0        0        0      274 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.4/jaaql/mvc/controller_interface.py
--rw-rw-rw-   0        0        0     7494 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.4/jaaql/mvc/exception_queries.py
--rw-rw-rw-   0        0        0    43043 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.4/jaaql/mvc/generated_queries.py
--rw-rw-rw-   0        0        0      232 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.4/jaaql/mvc/handmade_queries.py
--rw-rw-rw-   0        0        0    38055 2023-05-02 18:45:01.000000 jaaql-middleware-python-4.8.4/jaaql/mvc/model.py
--rw-rw-rw-   0        0        0      257 2022-05-07 20:33:26.000000 jaaql-middleware-python-4.8.4/jaaql/mvc/model_interface.py
--rw-rw-rw-   0        0        0      209 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.4/jaaql/mvc/response.py
-drwxrwxrwx   0        0        0        0 2023-05-02 19:35:49.764686 jaaql-middleware-python-4.8.4/jaaql/openapi/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.4/jaaql/openapi/__init__.py
--rw-rw-rw-   0        0        0    28821 2023-05-02 11:33:27.000000 jaaql-middleware-python-4.8.4/jaaql/openapi/swagger_documentation.py
--rw-rw-rw-   0        0        0      149 2022-06-11 20:45:39.000000 jaaql-middleware-python-4.8.4/jaaql/patch.py
-drwxrwxrwx   0        0        0        0 2023-05-02 19:35:49.771696 jaaql-middleware-python-4.8.4/jaaql/scripts/
--rw-rw-rw-   0        0        0     1379 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.4/jaaql/scripts/01.install_domains.generated.sql
--rw-rw-rw-   0        0        0      939 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.4/jaaql/scripts/02.install_super_user.exceptions.sql
--rw-rw-rw-   0        0        0     1859 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.4/jaaql/scripts/03.install_super_user.handwritten.sql
--rw-rw-rw-   0        0        0     7492 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.4/jaaql/scripts/04.install_jaaql_data_structures.generated.sql
--rw-rw-rw-   0        0        0      324 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.4/jaaql/scripts/05.install_jaaql.exceptions.sql
--rw-rw-rw-   0        0        0      990 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.4/jaaql/scripts/06.install_jaaql.handwritten.sql
--rw-rw-rw-   0        0        0     4105 2023-02-12 10:12:32.000000 jaaql-middleware-python-4.8.4/jaaql/scripts/swagger_template.html
-drwxrwxrwx   0        0        0        0 2023-05-02 19:35:49.775686 jaaql-middleware-python-4.8.4/jaaql/services/
--rw-rw-rw-   0        0        0        0 2022-07-10 13:56:37.000000 jaaql-middleware-python-4.8.4/jaaql/services/__init__.py
--rw-rw-rw-   0        0        0     2688 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.4/jaaql/services/cached_canned_query_service.py
--rw-rw-rw-   0        0        0     2047 2023-05-02 12:22:14.000000 jaaql-middleware-python-4.8.4/jaaql/services/migrations_manager_service.py
--rw-rw-rw-   0        0        0      296 2023-05-02 12:09:59.000000 jaaql-middleware-python-4.8.4/jaaql/services/patch_mms.py
-drwxrwxrwx   0        0        0        0 2023-05-02 19:35:49.780686 jaaql-middleware-python-4.8.4/jaaql/utilities/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.4/jaaql/utilities/__init__.py
--rw-rw-rw-   0        0        0     6698 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.4/jaaql/utilities/crypt_utils.py
--rw-rw-rw-   0        0        0     5357 2023-05-02 10:06:52.000000 jaaql-middleware-python-4.8.4/jaaql/utilities/options.py
--rw-rw-rw-   0        0        0     5162 2023-05-02 17:32:54.000000 jaaql-middleware-python-4.8.4/jaaql/utilities/utils.py
--rw-rw-rw-   0        0        0     2636 2023-05-02 18:18:38.000000 jaaql-middleware-python-4.8.4/jaaql/utilities/utils_no_project_imports.py
--rw-rw-rw-   0        0        0     2160 2022-05-22 11:21:40.000000 jaaql-middleware-python-4.8.4/jaaql/utilities/vault.py
-drwxrwxrwx   0        0        0        0 2023-05-02 19:35:49.784686 jaaql-middleware-python-4.8.4/jaaql_middleware_python.egg-info/
--rw-rw-rw-   0        0        0      946 2023-05-02 19:35:49.000000 jaaql-middleware-python-4.8.4/jaaql_middleware_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2221 2023-05-02 19:35:49.000000 jaaql-middleware-python-4.8.4/jaaql_middleware_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 19:35:49.000000 jaaql-middleware-python-4.8.4/jaaql_middleware_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      337 2023-05-02 19:35:49.000000 jaaql-middleware-python-4.8.4/jaaql_middleware_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-02 19:35:49.000000 jaaql-middleware-python-4.8.4/jaaql_middleware_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 19:35:49.785686 jaaql-middleware-python-4.8.4/setup.cfg
--rw-rw-rw-   0        0        0      893 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 20:19:50.014662 jaaql-middleware-python-4.8.5/
+-rw-rw-rw-   0        0        0    18134 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      946 2023-05-02 20:19:50.014662 jaaql-middleware-python-4.8.5/PKG-INFO
+-rw-rw-rw-   0        0        0      453 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 20:19:49.962677 jaaql-middleware-python-4.8.5/jaaql/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.5/jaaql/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 20:19:49.965662 jaaql-middleware-python-4.8.5/jaaql/config/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.5/jaaql/config/__init__.py
+-rw-rw-rw-   0        0        0      324 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.5/jaaql/config/config-docker.ini
+-rw-rw-rw-   0        0        0      253 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.5/jaaql/config/config-test.ini
+-rw-rw-rw-   0        0        0      291 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.5/jaaql/config/config.ini
+-rw-rw-rw-   0        0        0      470 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.5/jaaql/config_constants.py
+-rw-rw-rw-   0        0        0     4462 2023-05-02 20:19:15.000000 jaaql-middleware-python-4.8.5/jaaql/constants.py
+drwxrwxrwx   0        0        0        0 2023-05-02 20:19:49.969676 jaaql-middleware-python-4.8.5/jaaql/db/
+-rw-rw-rw-   0        0        0        0 2022-05-19 20:40:08.000000 jaaql-middleware-python-4.8.5/jaaql/db/__init__.py
+-rw-rw-rw-   0        0        0     6929 2023-05-02 18:15:39.000000 jaaql-middleware-python-4.8.5/jaaql/db/db_interface.py
+-rw-rw-rw-   0        0        0    11198 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.5/jaaql/db/db_pg_interface.py
+-rw-rw-rw-   0        0        0     7062 2023-05-02 19:35:29.000000 jaaql-middleware-python-4.8.5/jaaql/db/db_utils.py
+-rw-rw-rw-   0        0        0     2934 2023-05-02 18:45:07.000000 jaaql-middleware-python-4.8.5/jaaql/db/db_utils_no_circ.py
+drwxrwxrwx   0        0        0        0 2023-05-02 20:19:49.972661 jaaql-middleware-python-4.8.5/jaaql/documentation/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.5/jaaql/documentation/__init__.py
+-rw-rw-rw-   0        0        0     6592 2023-05-02 12:22:14.000000 jaaql-middleware-python-4.8.5/jaaql/documentation/documentation_internal.py
+-rw-rw-rw-   0        0        0     8192 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.5/jaaql/documentation/documentation_public.py
+-rw-rw-rw-   0        0        0     3456 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.5/jaaql/documentation/documentation_shared.py
+drwxrwxrwx   0        0        0        0 2023-05-02 20:19:49.975660 jaaql-middleware-python-4.8.5/jaaql/email/
+-rw-rw-rw-   0        0        0        0 2022-05-05 10:44:50.000000 jaaql-middleware-python-4.8.5/jaaql/email/__init__.py
+-rw-rw-rw-   0        0        0     7475 2023-05-02 18:34:17.000000 jaaql-middleware-python-4.8.5/jaaql/email/email_manager.py
+-rw-rw-rw-   0        0        0    19242 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.5/jaaql/email/email_manager_service.py
+-rw-rw-rw-   0        0        0      234 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.5/jaaql/email/patch_ems.py
+drwxrwxrwx   0        0        0        0 2023-05-02 20:19:49.979661 jaaql-middleware-python-4.8.5/jaaql/exceptions/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.5/jaaql/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      401 2022-04-17 07:42:21.000000 jaaql-middleware-python-4.8.5/jaaql/exceptions/custom_http_status.py
+-rw-rw-rw-   0        0        0      985 2022-05-20 15:36:28.000000 jaaql-middleware-python-4.8.5/jaaql/exceptions/http_status_exception.py
+-rw-rw-rw-   0        0        0      321 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.5/jaaql/exceptions/not_yet_implement_exception.py
+drwxrwxrwx   0        0        0        0 2023-05-02 20:19:49.981661 jaaql-middleware-python-4.8.5/jaaql/interpreter/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.5/jaaql/interpreter/__init__.py
+-rw-rw-rw-   0        0        0    23250 2023-05-02 18:09:24.000000 jaaql-middleware-python-4.8.5/jaaql/interpreter/interpret_jaaql.py
+-rw-rw-rw-   0        0        0     5962 2023-05-02 12:06:24.000000 jaaql-middleware-python-4.8.5/jaaql/jaaql.py
+drwxrwxrwx   0        0        0        0 2023-05-02 20:19:49.983661 jaaql-middleware-python-4.8.5/jaaql/migrations/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.5/jaaql/migrations/__init__.py
+-rw-rw-rw-   0        0        0      683 2022-09-19 00:09:13.000000 jaaql-middleware-python-4.8.5/jaaql/migrations/migration_history.sql
+-rw-rw-rw-   0        0        0     8574 2023-05-02 19:35:29.000000 jaaql-middleware-python-4.8.5/jaaql/migrations/migrations.py
+drwxrwxrwx   0        0        0        0 2023-05-02 20:19:49.992661 jaaql-middleware-python-4.8.5/jaaql/mvc/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.5/jaaql/mvc/__init__.py
+-rw-rw-rw-   0        0        0    32609 2023-05-02 17:45:39.000000 jaaql-middleware-python-4.8.5/jaaql/mvc/base_controller.py
+-rw-rw-rw-   0        0        0    11591 2023-05-02 12:24:40.000000 jaaql-middleware-python-4.8.5/jaaql/mvc/base_model.py
+-rw-rw-rw-   0        0        0     3928 2023-05-02 12:51:04.000000 jaaql-middleware-python-4.8.5/jaaql/mvc/controller.py
+-rw-rw-rw-   0        0        0      274 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.5/jaaql/mvc/controller_interface.py
+-rw-rw-rw-   0        0        0     7494 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.5/jaaql/mvc/exception_queries.py
+-rw-rw-rw-   0        0        0    43043 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.5/jaaql/mvc/generated_queries.py
+-rw-rw-rw-   0        0        0      232 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.5/jaaql/mvc/handmade_queries.py
+-rw-rw-rw-   0        0        0    38055 2023-05-02 18:45:01.000000 jaaql-middleware-python-4.8.5/jaaql/mvc/model.py
+-rw-rw-rw-   0        0        0      257 2022-05-07 20:33:26.000000 jaaql-middleware-python-4.8.5/jaaql/mvc/model_interface.py
+-rw-rw-rw-   0        0        0      209 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.5/jaaql/mvc/response.py
+drwxrwxrwx   0        0        0        0 2023-05-02 20:19:49.994662 jaaql-middleware-python-4.8.5/jaaql/openapi/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.5/jaaql/openapi/__init__.py
+-rw-rw-rw-   0        0        0    28821 2023-05-02 11:33:27.000000 jaaql-middleware-python-4.8.5/jaaql/openapi/swagger_documentation.py
+-rw-rw-rw-   0        0        0      149 2022-06-11 20:45:39.000000 jaaql-middleware-python-4.8.5/jaaql/patch.py
+drwxrwxrwx   0        0        0        0 2023-05-02 20:19:50.000661 jaaql-middleware-python-4.8.5/jaaql/scripts/
+-rw-rw-rw-   0        0        0     1379 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.5/jaaql/scripts/01.install_domains.generated.sql
+-rw-rw-rw-   0        0        0      939 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.5/jaaql/scripts/02.install_super_user.exceptions.sql
+-rw-rw-rw-   0        0        0     1859 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.5/jaaql/scripts/03.install_super_user.handwritten.sql
+-rw-rw-rw-   0        0        0     7492 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.5/jaaql/scripts/04.install_jaaql_data_structures.generated.sql
+-rw-rw-rw-   0        0        0      324 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.5/jaaql/scripts/05.install_jaaql.exceptions.sql
+-rw-rw-rw-   0        0        0      990 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.5/jaaql/scripts/06.install_jaaql.handwritten.sql
+-rw-rw-rw-   0        0        0     4105 2023-02-12 10:12:32.000000 jaaql-middleware-python-4.8.5/jaaql/scripts/swagger_template.html
+drwxrwxrwx   0        0        0        0 2023-05-02 20:19:50.003661 jaaql-middleware-python-4.8.5/jaaql/services/
+-rw-rw-rw-   0        0        0        0 2022-07-10 13:56:37.000000 jaaql-middleware-python-4.8.5/jaaql/services/__init__.py
+-rw-rw-rw-   0        0        0     2688 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.5/jaaql/services/cached_canned_query_service.py
+-rw-rw-rw-   0        0        0     2047 2023-05-02 12:22:14.000000 jaaql-middleware-python-4.8.5/jaaql/services/migrations_manager_service.py
+-rw-rw-rw-   0        0        0      296 2023-05-02 12:09:59.000000 jaaql-middleware-python-4.8.5/jaaql/services/patch_mms.py
+drwxrwxrwx   0        0        0        0 2023-05-02 20:19:50.008661 jaaql-middleware-python-4.8.5/jaaql/utilities/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.5/jaaql/utilities/__init__.py
+-rw-rw-rw-   0        0        0     6698 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.5/jaaql/utilities/crypt_utils.py
+-rw-rw-rw-   0        0        0     5357 2023-05-02 10:06:52.000000 jaaql-middleware-python-4.8.5/jaaql/utilities/options.py
+-rw-rw-rw-   0        0        0     5162 2023-05-02 17:32:54.000000 jaaql-middleware-python-4.8.5/jaaql/utilities/utils.py
+-rw-rw-rw-   0        0        0     2636 2023-05-02 18:18:38.000000 jaaql-middleware-python-4.8.5/jaaql/utilities/utils_no_project_imports.py
+-rw-rw-rw-   0        0        0     2160 2022-05-22 11:21:40.000000 jaaql-middleware-python-4.8.5/jaaql/utilities/vault.py
+drwxrwxrwx   0        0        0        0 2023-05-02 20:19:50.013662 jaaql-middleware-python-4.8.5/jaaql_middleware_python.egg-info/
+-rw-rw-rw-   0        0        0      946 2023-05-02 20:19:49.000000 jaaql-middleware-python-4.8.5/jaaql_middleware_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2221 2023-05-02 20:19:49.000000 jaaql-middleware-python-4.8.5/jaaql_middleware_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 20:19:49.000000 jaaql-middleware-python-4.8.5/jaaql_middleware_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      337 2023-05-02 20:19:49.000000 jaaql-middleware-python-4.8.5/jaaql_middleware_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-02 20:19:49.000000 jaaql-middleware-python-4.8.5/jaaql_middleware_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 20:19:50.014662 jaaql-middleware-python-4.8.5/setup.cfg
+-rw-rw-rw-   0        0        0      893 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.5/setup.py
```

### Comparing `jaaql-middleware-python-4.8.4/LICENSE.txt` & `jaaql-middleware-python-4.8.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.4/PKG-INFO` & `jaaql-middleware-python-4.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-middleware-python
-Version: 4.8.4
+Version: 4.8.5
 Summary: The jaaql package, allowing for rapid development and deployment of RESTful HTTP applications
 Home-page: https://github.com/JAAQL/JAAQL-middleware-python
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-middleware-python-4.8.4/jaaql/constants.py` & `jaaql-middleware-python-4.8.5/jaaql/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,9 +124,9 @@
 USERNAME__anonymous = "anonymous"
 PASSWORD__anonymous = "jaaql_public_password"
 ROLE__jaaql = "jaaql"
 ROLE__postgres = "postgres"
 
 PROTOCOL__postgres = "postgresql://"
 
-VERSION = "4.8.4"
+VERSION = "4.8.5"
```

### Comparing `jaaql-middleware-python-4.8.4/jaaql/db/db_interface.py` & `jaaql-middleware-python-4.8.5/jaaql/db/db_interface.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.4/jaaql/db/db_pg_interface.py` & `jaaql-middleware-python-4.8.5/jaaql/db/db_pg_interface.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.4/jaaql/db/db_utils.py` & `jaaql-middleware-python-4.8.5/jaaql/db/db_utils.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.4/jaaql/db/db_utils_no_circ.py` & `jaaql-middleware-python-4.8.5/jaaql/db/db_utils_no_circ.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.4/jaaql/documentation/documentation_internal.py` & `jaaql-middleware-python-4.8.5/jaaql/documentation/documentation_internal.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.4/jaaql/documentation/documentation_public.py` & `jaaql-middleware-python-4.8.5/jaaql/documentation/documentation_public.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.4/jaaql/documentation/documentation_shared.py` & `jaaql-middleware-python-4.8.5/jaaql/documentation/documentation_shared.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.4/jaaql/email/email_manager.py` & `jaaql-middleware-python-4.8.5/jaaql/email/email_manager.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.4/jaaql/email/email_manager_service.py` & `jaaql-middleware-python-4.8.5/jaaql/email/email_manager_service.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.4/jaaql/exceptions/http_status_exception.py` & `jaaql-middleware-python-4.8.5/jaaql/exceptions/http_status_exception.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.4/jaaql/interpreter/interpret_jaaql.py` & `jaaql-middleware-python-4.8.5/jaaql/interpreter/interpret_jaaql.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.4/jaaql/jaaql.py` & `jaaql-middleware-python-4.8.5/jaaql/jaaql.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.4/jaaql/migrations/migration_history.sql` & `jaaql-middleware-python-4.8.5/jaaql/migrations/migration_history.sql`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.4/jaaql/migrations/migrations.py` & `jaaql-middleware-python-4.8.5/jaaql/migrations/migrations.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.4/jaaql/mvc/base_controller.py` & `jaaql-middleware-python-4.8.5/jaaql/mvc/base_controller.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.4/jaaql/mvc/base_model.py` & `jaaql-middleware-python-4.8.5/jaaql/mvc/base_model.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.4/jaaql/mvc/controller.py` & `jaaql-middleware-python-4.8.5/jaaql/mvc/controller.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.4/jaaql/mvc/exception_queries.py` & `jaaql-middleware-python-4.8.5/jaaql/mvc/exception_queries.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.4/jaaql/mvc/generated_queries.py` & `jaaql-middleware-python-4.8.5/jaaql/mvc/generated_queries.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.4/jaaql/mvc/model.py` & `jaaql-middleware-python-4.8.5/jaaql/mvc/model.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.4/jaaql/openapi/swagger_documentation.py` & `jaaql-middleware-python-4.8.5/jaaql/openapi/swagger_documentation.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.4/jaaql/scripts/01.install_domains.generated.sql` & `jaaql-middleware-python-4.8.5/jaaql/scripts/01.install_domains.generated.sql`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.4/jaaql/scripts/02.install_super_user.exceptions.sql` & `jaaql-middleware-python-4.8.5/jaaql/scripts/02.install_super_user.exceptions.sql`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.4/jaaql/scripts/03.install_super_user.handwritten.sql` & `jaaql-middleware-python-4.8.5/jaaql/scripts/03.install_super_user.handwritten.sql`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.4/jaaql/scripts/04.install_jaaql_data_structures.generated.sql` & `jaaql-middleware-python-4.8.5/jaaql/scripts/04.install_jaaql_data_structures.generated.sql`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.4/jaaql/scripts/06.install_jaaql.handwritten.sql` & `jaaql-middleware-python-4.8.5/jaaql/scripts/06.install_jaaql.handwritten.sql`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.4/jaaql/scripts/swagger_template.html` & `jaaql-middleware-python-4.8.5/jaaql/scripts/swagger_template.html`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.4/jaaql/services/cached_canned_query_service.py` & `jaaql-middleware-python-4.8.5/jaaql/services/cached_canned_query_service.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.4/jaaql/services/migrations_manager_service.py` & `jaaql-middleware-python-4.8.5/jaaql/services/migrations_manager_service.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.4/jaaql/utilities/crypt_utils.py` & `jaaql-middleware-python-4.8.5/jaaql/utilities/crypt_utils.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.4/jaaql/utilities/options.py` & `jaaql-middleware-python-4.8.5/jaaql/utilities/options.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.4/jaaql/utilities/utils.py` & `jaaql-middleware-python-4.8.5/jaaql/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.4/jaaql/utilities/utils_no_project_imports.py` & `jaaql-middleware-python-4.8.5/jaaql/utilities/utils_no_project_imports.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.4/jaaql/utilities/vault.py` & `jaaql-middleware-python-4.8.5/jaaql/utilities/vault.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.4/jaaql_middleware_python.egg-info/PKG-INFO` & `jaaql-middleware-python-4.8.5/jaaql_middleware_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-middleware-python
-Version: 4.8.4
+Version: 4.8.5
 Summary: The jaaql package, allowing for rapid development and deployment of RESTful HTTP applications
 Home-page: https://github.com/JAAQL/JAAQL-middleware-python
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-middleware-python-4.8.4/jaaql_middleware_python.egg-info/SOURCES.txt` & `jaaql-middleware-python-4.8.5/jaaql_middleware_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.4/setup.py` & `jaaql-middleware-python-4.8.5/setup.py`

 * *Files identical despite different names*

