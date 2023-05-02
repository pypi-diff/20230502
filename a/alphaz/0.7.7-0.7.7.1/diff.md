# Comparing `tmp/alphaz-0.7.7.tar.gz` & `tmp/alphaz-0.7.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alphaz-0.7.7.tar", last modified: Thu Apr 27 20:33:30 2023, max compression
+gzip compressed data, was "dist/alphaz-0.7.7.1.tar", last modified: Tue May  2 17:08:56 2023, max compression
```

## Comparing `alphaz-0.7.7.tar` & `alphaz-0.7.7.1.tar`

### file list

```diff
@@ -1,397 +1,398 @@
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.722307 alphaz-0.7.7/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11211 2023-04-27 20:33:30.000000 alphaz-0.7.7/MANIFEST.in
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      585 2023-04-27 20:33:30.722307 alphaz-0.7.7/PKG-INFO
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1348 2021-07-12 18:07:51.000000 alphaz-0.7.7/README.md
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.658307 alphaz-0.7.7/alphaz/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        9 2023-04-18 09:00:04.000000 alphaz-0.7.7/alphaz/README.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      455 2023-04-27 10:12:16.000000 alphaz-0.7.7/alphaz/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      104 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/alphaz.bat
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       70 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/alphaz.code-workspace
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      208 2022-04-19 08:43:27.000000 alphaz-0.7.7/alphaz/alphaz.sh
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       48 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/api.bat
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      713 2023-04-18 09:00:04.000000 alphaz-0.7.7/alphaz/api.json
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      770 2022-04-13 09:59:51.000000 alphaz-0.7.7/alphaz/api.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.658307 alphaz-0.7.7/alphaz/apis/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.7/alphaz/apis/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-07-21 11:35:27.000000 alphaz-0.7.7/alphaz/apis/log.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2721 2023-03-17 07:06:42.000000 alphaz-0.7.7/alphaz/apis/mails.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.658307 alphaz-0.7.7/alphaz/apis/routes/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/apis/routes/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1577 2023-02-23 09:08:35.000000 alphaz-0.7.7/alphaz/apis/routes/admin.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1137 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/apis/routes/api.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3039 2023-04-27 10:12:16.000000 alphaz-0.7.7/alphaz/apis/routes/basic_tests.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3070 2023-04-27 10:12:16.000000 alphaz-0.7.7/alphaz/apis/routes/database.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      413 2022-04-12 11:53:03.000000 alphaz-0.7.7/alphaz/apis/routes/git.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     7272 2023-04-27 10:12:16.000000 alphaz-0.7.7/alphaz/apis/routes/logs.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1810 2022-04-12 11:53:03.000000 alphaz-0.7.7/alphaz/apis/routes/mails.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6384 2023-04-27 10:12:16.000000 alphaz-0.7.7/alphaz/apis/routes/main.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1548 2023-04-27 20:33:27.000000 alphaz-0.7.7/alphaz/apis/routes/tests.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.662307 alphaz-0.7.7/alphaz/apis/routes/user_management/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      114 2022-04-27 13:24:50.000000 alphaz-0.7.7/alphaz/apis/routes/user_management/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2479 2023-04-27 10:12:16.000000 alphaz-0.7.7/alphaz/apis/routes/user_management/application_management.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2243 2023-04-27 10:12:16.000000 alphaz-0.7.7/alphaz/apis/routes/user_management/permission_management.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4104 2023-04-27 10:12:16.000000 alphaz-0.7.7/alphaz/apis/routes/user_management/role_management.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1291 2022-08-31 08:56:44.000000 alphaz-0.7.7/alphaz/apis/routes/user_management/user_management.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3324 2023-04-21 07:47:57.000000 alphaz-0.7.7/alphaz/apis/routes/users.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      584 2023-02-23 09:08:35.000000 alphaz-0.7.7/alphaz/apis/tests.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.662307 alphaz-0.7.7/alphaz/apis/users/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-07-21 11:35:27.000000 alphaz-0.7.7/alphaz/apis/users/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2718 2023-01-25 21:39:07.000000 alphaz-0.7.7/alphaz/apis/users/ldap.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11572 2023-04-27 10:12:16.000000 alphaz-0.7.7/alphaz/apis/users/users.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.662307 alphaz-0.7.7/alphaz/config/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/config/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      795 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/config/config.css
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    12602 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/config/config.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      707 2022-08-11 06:44:17.000000 alphaz-0.7.7/alphaz/config/main_configuration.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      823 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/config/page.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1700 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/config/source.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1564 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/config.json
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      238 2023-01-06 09:14:28.000000 alphaz-0.7.7/alphaz/core.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.662307 alphaz-0.7.7/alphaz/documentations/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.662307 alphaz-0.7.7/alphaz/documentations/docs/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-07-21 11:35:27.000000 alphaz-0.7.7/alphaz/documentations/docs/alpha_admin.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1408 2023-04-12 11:28:51.000000 alphaz-0.7.7/alphaz/documentations/docs/alpha_core.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2595 2022-07-21 11:35:27.000000 alphaz-0.7.7/alphaz/documentations/docs/alpha_screens.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2222 2023-04-12 11:28:51.000000 alphaz-0.7.7/alphaz/documentations/docs/alpha_setup.md
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.666307 alphaz-0.7.7/alphaz/documentations/docs/api/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1527 2023-04-18 09:00:04.000000 alphaz-0.7.7/alphaz/documentations/docs/api/authorizations.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       72 2023-04-18 09:00:04.000000 alphaz-0.7.7/alphaz/documentations/docs/api/cache.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2931 2023-04-27 10:12:16.000000 alphaz-0.7.7/alphaz/documentations/docs/api/configuration.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       24 2023-04-18 09:00:04.000000 alphaz-0.7.7/alphaz/documentations/docs/api/issues.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      705 2023-04-18 09:00:04.000000 alphaz-0.7.7/alphaz/documentations/docs/api/main.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      559 2023-04-18 09:00:04.000000 alphaz-0.7.7/alphaz/documentations/docs/api/methods.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1728 2023-04-18 09:00:04.000000 alphaz-0.7.7/alphaz/documentations/docs/api/parameters.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1197 2023-04-18 09:00:04.000000 alphaz-0.7.7/alphaz/documentations/docs/api/routes.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      486 2023-04-18 09:00:04.000000 alphaz-0.7.7/alphaz/documentations/docs/api/sqlalchemy.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1129 2023-04-18 09:00:04.000000 alphaz-0.7.7/alphaz/documentations/docs/api_database.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2520 2023-01-06 09:14:28.000000 alphaz-0.7.7/alphaz/documentations/docs/configuration.md
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.666307 alphaz-0.7.7/alphaz/documentations/docs/database/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2187 2023-04-27 10:12:16.000000 alphaz-0.7.7/alphaz/documentations/docs/database/init.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      442 2023-04-18 09:00:04.000000 alphaz-0.7.7/alphaz/documentations/docs/database/instantiate.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      113 2023-04-18 09:00:04.000000 alphaz-0.7.7/alphaz/documentations/docs/database/main.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1806 2023-04-18 09:00:04.000000 alphaz-0.7.7/alphaz/documentations/docs/database/model.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      373 2023-04-18 09:00:04.000000 alphaz-0.7.7/alphaz/documentations/docs/database/relations.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1087 2023-04-18 09:00:04.000000 alphaz-0.7.7/alphaz/documentations/docs/database/schema.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      615 2023-04-18 09:00:04.000000 alphaz-0.7.7/alphaz/documentations/docs/database/update.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      357 2021-04-14 08:59:25.000000 alphaz-0.7.7/alphaz/documentations/docs/documentation.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3526 2023-04-12 11:28:51.000000 alphaz-0.7.7/alphaz/documentations/docs/index.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1090 2023-04-18 09:00:04.000000 alphaz-0.7.7/alphaz/documentations/mkdocs.yml
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.666307 alphaz-0.7.7/alphaz/documentations/site/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    13156 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/404.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.666307 alphaz-0.7.7/alphaz/documentations/site/alpha_admin/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    14222 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/alpha_admin/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.666307 alphaz-0.7.7/alphaz/documentations/site/alpha_core/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    22752 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/alpha_core/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.666307 alphaz-0.7.7/alphaz/documentations/site/alpha_screens/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    21873 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/alpha_screens/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.666307 alphaz-0.7.7/alphaz/documentations/site/alpha_setup/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    24071 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/alpha_setup/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.650307 alphaz-0.7.7/alphaz/documentations/site/api/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.666307 alphaz-0.7.7/alphaz/documentations/site/api/authorizations/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    17905 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/api/authorizations/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.666307 alphaz-0.7.7/alphaz/documentations/site/api/cache/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    14918 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/api/cache/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.666307 alphaz-0.7.7/alphaz/documentations/site/api/configuration/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    27645 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/api/configuration/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.666307 alphaz-0.7.7/alphaz/documentations/site/api/issues/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    16365 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/api/issues/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.666307 alphaz-0.7.7/alphaz/documentations/site/api/main/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    17987 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/api/main/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.666307 alphaz-0.7.7/alphaz/documentations/site/api/methods/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    17722 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/api/methods/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.666307 alphaz-0.7.7/alphaz/documentations/site/api/parameters/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    20075 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/api/parameters/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.670307 alphaz-0.7.7/alphaz/documentations/site/api/routes/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    19333 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/api/routes/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.670307 alphaz-0.7.7/alphaz/documentations/site/api/sqlalchemy/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    17109 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/api/sqlalchemy/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.670307 alphaz-0.7.7/alphaz/documentations/site/api_database/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    22959 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/api_database/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.650307 alphaz-0.7.7/alphaz/documentations/site/assets/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.670307 alphaz-0.7.7/alphaz/documentations/site/assets/images/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1870 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/assets/images/favicon.png
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.670307 alphaz-0.7.7/alphaz/documentations/site/assets/javascripts/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    79520 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)   384391 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js.map
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.670307 alphaz-0.7.7/alphaz/documentations/site/assets/javascripts/lunr/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.674307 alphaz-0.7.7/alphaz/documentations/site/assets/javascripts/lunr/min/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    17058 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ar.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4654 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.da.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6119 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.de.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6208 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.du.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11499 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.es.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     9342 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fi.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    10669 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fr.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     9437 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.hu.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11232 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.it.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2313 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ja.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       36 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.jp.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      817 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.multi.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6026 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.nl.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4754 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.no.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    10171 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.pt.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    10958 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ro.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    10331 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ru.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3647 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4523 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.sv.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    15009 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.tr.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      784 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.vi.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    22878 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/assets/javascripts/lunr/tinyseg.js
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.674307 alphaz-0.7.7/alphaz/documentations/site/assets/javascripts/workers/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    34936 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)   167496 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js.map
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.674307 alphaz-0.7.7/alphaz/documentations/site/assets/stylesheets/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    87332 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css
--rw-rw-r--   0 aurele    (1000) aurele    (1000)   319950 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css.map
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    10915 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    37512 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css.map
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.674307 alphaz-0.7.7/alphaz/documentations/site/configuration/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    28465 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/configuration/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.650307 alphaz-0.7.7/alphaz/documentations/site/database/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.674307 alphaz-0.7.7/alphaz/documentations/site/database/init/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    23029 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/database/init/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.674307 alphaz-0.7.7/alphaz/documentations/site/database/instantiate/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    17445 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/database/instantiate/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.674307 alphaz-0.7.7/alphaz/documentations/site/database/main/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    14939 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/database/main/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.674307 alphaz-0.7.7/alphaz/documentations/site/database/model/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    24758 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/database/model/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.674307 alphaz-0.7.7/alphaz/documentations/site/database/relations/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    16511 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/database/relations/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.674307 alphaz-0.7.7/alphaz/documentations/site/database/schema/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    18704 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/database/schema/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.674307 alphaz-0.7.7/alphaz/documentations/site/database/update/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    20308 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/database/update/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.674307 alphaz-0.7.7/alphaz/documentations/site/documentation/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    17065 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/documentation/index.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    29467 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.678307 alphaz-0.7.7/alphaz/documentations/site/search/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    54135 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/search/search_index.json
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2809 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/sitemap.xml
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      209 2023-04-27 20:33:29.000000 alphaz-0.7.7/alphaz/documentations/site/sitemap.xml.gz
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       50 2022-04-19 08:43:27.000000 alphaz-0.7.7/alphaz/git.sh
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       45 2022-05-14 15:57:01.000000 alphaz-0.7.7/alphaz/help.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      905 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.682307 alphaz-0.7.7/alphaz/libs/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/libs/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5807 2023-04-27 20:33:27.000000 alphaz-0.7.7/alphaz/libs/api_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1901 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/libs/barcode_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    13989 2023-04-27 10:12:16.000000 alphaz-0.7.7/alphaz/libs/config_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2420 2023-03-29 19:04:59.000000 alphaz-0.7.7/alphaz/libs/converter_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5961 2023-04-27 10:12:16.000000 alphaz-0.7.7/alphaz/libs/database_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4223 2023-02-06 12:52:51.000000 alphaz-0.7.7/alphaz/libs/date_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6381 2023-04-27 20:33:27.000000 alphaz-0.7.7/alphaz/libs/dict_lib.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.682307 alphaz-0.7.7/alphaz/libs/emulation/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1758 2023-02-02 21:07:35.000000 alphaz-0.7.7/alphaz/libs/emulation/vt102_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1642 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/libs/events.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3351 2022-01-17 10:25:20.000000 alphaz-0.7.7/alphaz/libs/files_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1184 2023-04-27 10:12:16.000000 alphaz-0.7.7/alphaz/libs/flask_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       49 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/libs/ftp_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1093 2022-07-21 11:35:27.000000 alphaz-0.7.7/alphaz/libs/img_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6207 2023-04-27 10:12:16.000000 alphaz-0.7.7/alphaz/libs/io_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3233 2023-04-27 10:12:16.000000 alphaz-0.7.7/alphaz/libs/json_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1151 2023-04-27 10:12:16.000000 alphaz-0.7.7/alphaz/libs/logs_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    13008 2023-04-27 10:12:16.000000 alphaz-0.7.7/alphaz/libs/mail_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      508 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/libs/nav_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      614 2022-09-07 06:57:10.000000 alphaz-0.7.7/alphaz/libs/notifications_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1348 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/libs/number_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      177 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/libs/os_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2782 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/libs/process_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    12411 2023-04-27 20:33:27.000000 alphaz-0.7.7/alphaz/libs/py_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      886 2023-04-21 07:47:57.000000 alphaz-0.7.7/alphaz/libs/scp_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     8082 2022-01-17 10:25:20.000000 alphaz-0.7.7/alphaz/libs/search_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6362 2023-04-27 10:12:16.000000 alphaz-0.7.7/alphaz/libs/secure_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2929 2023-04-27 10:12:16.000000 alphaz-0.7.7/alphaz/libs/soap_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      139 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/libs/sql_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    18623 2023-04-27 10:12:16.000000 alphaz-0.7.7/alphaz/libs/ssh_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     9896 2023-04-27 10:12:16.000000 alphaz-0.7.7/alphaz/libs/string_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5556 2023-04-27 20:33:27.000000 alphaz-0.7.7/alphaz/libs/test_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      703 2023-03-16 15:41:50.000000 alphaz-0.7.7/alphaz/libs/time_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4492 2023-04-27 10:12:16.000000 alphaz-0.7.7/alphaz/libs/transactions_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     7664 2023-04-27 10:12:16.000000 alphaz-0.7.7/alphaz/libs/user_lib.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.682307 alphaz-0.7.7/alphaz/libs/user_management/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-04-27 13:24:50.000000 alphaz-0.7.7/alphaz/libs/user_management/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1336 2023-04-27 10:12:16.000000 alphaz-0.7.7/alphaz/libs/user_management/application_management_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1597 2023-04-27 10:12:16.000000 alphaz-0.7.7/alphaz/libs/user_management/permission_management_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3376 2023-04-27 10:12:16.000000 alphaz-0.7.7/alphaz/libs/user_management/role_management_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2313 2023-04-27 10:12:16.000000 alphaz-0.7.7/alphaz/libs/user_management/user_management_lib.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.686307 alphaz-0.7.7/alphaz/mails/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.686307 alphaz-0.7.7/alphaz/mails/Images/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)   948952 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/mails/Images/Background.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1835 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/mails/Images/Facebook_logo.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2484 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/mails/Images/Twitter_logo.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3522 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/mails/Images/Web_logo.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.7/alphaz/mails/Images/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)   966605 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/mails/Mail.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5097 2022-04-13 09:59:51.000000 alphaz-0.7.7/alphaz/mails/Webmail.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.7/alphaz/mails/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    22029 2023-03-17 05:42:16.000000 alphaz-0.7.7/alphaz/mails/debug.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    23078 2023-03-16 20:48:51.000000 alphaz-0.7.7/alphaz/mails/mail.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2331 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/mails/password_reset.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    24598 2022-04-13 09:59:51.000000 alphaz-0.7.7/alphaz/mails/stay_in_touch.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       40 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/mails/template.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.686307 alphaz-0.7.7/alphaz/models/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      107 2023-04-27 10:12:16.000000 alphaz-0.7.7/alphaz/models/__init__.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.690307 alphaz-0.7.7/alphaz/models/api/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      185 2022-04-12 11:53:03.000000 alphaz-0.7.7/alphaz/models/api/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      926 2023-04-27 10:12:16.000000 alphaz-0.7.7/alphaz/models/api/_answer.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2179 2021-09-13 12:55:49.000000 alphaz-0.7.7/alphaz/models/api/_colorations.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      133 2021-09-06 13:56:36.000000 alphaz-0.7.7/alphaz/models/api/_methods.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    14173 2023-04-27 10:12:16.000000 alphaz-0.7.7/alphaz/models/api/_parameter.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    14445 2023-04-27 10:12:16.000000 alphaz-0.7.7/alphaz/models/api/_reloader.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3717 2023-04-27 10:12:16.000000 alphaz-0.7.7/alphaz/models/api/_reloaders.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2332 2023-04-27 11:30:37.000000 alphaz-0.7.7/alphaz/models/api/_requests.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    18839 2023-04-27 20:33:27.000000 alphaz-0.7.7/alphaz/models/api/_route.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    20272 2023-04-27 11:30:37.000000 alphaz-0.7.7/alphaz/models/api/_structures.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      651 2022-02-01 21:43:05.000000 alphaz-0.7.7/alphaz/models/api/_utils.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      388 2022-07-22 14:00:51.000000 alphaz-0.7.7/alphaz/models/base.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.690307 alphaz-0.7.7/alphaz/models/config/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       32 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/models/config/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    26517 2023-04-27 10:12:16.000000 alphaz-0.7.7/alphaz/models/config/_config.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    12350 2023-04-25 15:54:12.000000 alphaz-0.7.7/alphaz/models/config/_utils.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.690307 alphaz-0.7.7/alphaz/models/database/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       53 2022-01-13 15:32:15.000000 alphaz-0.7.7/alphaz/models/database/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5495 2023-03-17 15:16:42.000000 alphaz-0.7.7/alphaz/models/database/main_definitions.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     9992 2023-04-27 10:12:16.000000 alphaz-0.7.7/alphaz/models/database/models.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      609 2022-04-28 08:55:29.000000 alphaz-0.7.7/alphaz/models/database/operators.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1164 2023-01-25 21:39:07.000000 alphaz-0.7.7/alphaz/models/database/requests.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1087 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/models/database/row.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    56477 2023-04-27 10:12:16.000000 alphaz-0.7.7/alphaz/models/database/structure.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1826 2023-02-23 09:08:35.000000 alphaz-0.7.7/alphaz/models/database/tests.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4529 2023-04-21 13:36:09.000000 alphaz-0.7.7/alphaz/models/database/users_definitions.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     9301 2023-04-27 10:12:16.000000 alphaz-0.7.7/alphaz/models/database/utils.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1061 2022-04-12 11:53:03.000000 alphaz-0.7.7/alphaz/models/database/views.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1241 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/models/excel.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6683 2023-04-27 10:12:16.000000 alphaz-0.7.7/alphaz/models/ftp.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      150 2022-07-19 09:10:48.000000 alphaz-0.7.7/alphaz/models/img.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.690307 alphaz-0.7.7/alphaz/models/json/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       41 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/models/json/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2609 2023-01-06 09:14:28.000000 alphaz-0.7.7/alphaz/models/json/_converters.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.690307 alphaz-0.7.7/alphaz/models/logger/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       68 2022-01-19 15:41:22.000000 alphaz-0.7.7/alphaz/models/logger/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1319 2023-01-06 09:14:28.000000 alphaz-0.7.7/alphaz/models/logger/_colorations.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    14322 2023-04-27 20:33:27.000000 alphaz-0.7.7/alphaz/models/logger/_logger.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      757 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/models/logger/_utils.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.694307 alphaz-0.7.7/alphaz/models/logs/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1280 2021-11-12 08:53:17.000000 alphaz-0.7.7/alphaz/models/logs/main.log
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      160 2021-11-07 15:22:58.000000 alphaz-0.7.7/alphaz/models/logs/main.log.2021-11-07
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.694307 alphaz-0.7.7/alphaz/models/main/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      354 2023-04-27 20:33:27.000000 alphaz-0.7.7/alphaz/models/main/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    27268 2023-04-27 20:33:27.000000 alphaz-0.7.7/alphaz/models/main/_base.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.694307 alphaz-0.7.7/alphaz/models/main/_core/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/models/main/_core/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    15986 2023-04-27 10:12:16.000000 alphaz-0.7.7/alphaz/models/main/_core/_core.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       13 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/models/main/_core/_utils.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      339 2023-02-06 09:05:20.000000 alphaz-0.7.7/alphaz/models/main/_enum.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2001 2023-04-27 20:33:27.000000 alphaz-0.7.7/alphaz/models/main/_exception.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      501 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/models/main/_file.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      477 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/models/main/_process.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1305 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/models/main/_request.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      925 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/models/main/_singleton.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2218 2023-04-27 10:12:16.000000 alphaz-0.7.7/alphaz/models/request.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.694307 alphaz-0.7.7/alphaz/models/tests/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      167 2023-04-25 15:54:12.000000 alphaz-0.7.7/alphaz/models/tests/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     8070 2023-04-27 10:12:16.000000 alphaz-0.7.7/alphaz/models/tests/_category.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3446 2023-04-27 10:12:16.000000 alphaz-0.7.7/alphaz/models/tests/_group.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      163 2023-04-25 15:54:12.000000 alphaz-0.7.7/alphaz/models/tests/_levels.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4125 2023-04-27 10:12:16.000000 alphaz-0.7.7/alphaz/models/tests/_method.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4578 2023-04-27 10:12:16.000000 alphaz-0.7.7/alphaz/models/tests/_save.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    14832 2023-04-27 20:33:27.000000 alphaz-0.7.7/alphaz/models/tests/_test.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     7505 2023-04-27 10:12:16.000000 alphaz-0.7.7/alphaz/models/tests/_wrappers.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2896 2023-04-27 10:12:16.000000 alphaz-0.7.7/alphaz/models/user.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2367 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/models/watcher.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.694307 alphaz-0.7.7/alphaz/pocs/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      685 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/pocs/main.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       72 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/reload_gitignore.bat
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       67 2022-04-12 12:30:24.000000 alphaz-0.7.7/alphaz/req.sh
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      460 2023-04-11 14:13:25.000000 alphaz-0.7.7/alphaz/requirements.txt
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1345 2022-04-19 08:43:27.000000 alphaz-0.7.7/alphaz/run.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.694307 alphaz-0.7.7/alphaz/src/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.7/alphaz/src/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    23747 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/src/alpha.png
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.698307 alphaz-0.7.7/alphaz/src/configs/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      135 2022-04-19 08:43:27.000000 alphaz-0.7.7/alphaz/src/configs/config.json
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      674 2023-01-25 21:39:07.000000 alphaz-0.7.7/alphaz/src/configs/loggers.json
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      490 2022-01-13 15:32:15.000000 alphaz-0.7.7/alphaz/src/configs/loggers_colors.json
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.698307 alphaz-0.7.7/alphaz/src/database/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.7/alphaz/src/database/__init__.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.698307 alphaz-0.7.7/alphaz/stitch/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1769 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/stitch/Core.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       26 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/stitch/__init__.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.698307 alphaz-0.7.7/alphaz/stitch/imports/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       78 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/stitch/imports/__init__.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.698307 alphaz-0.7.7/alphaz/stitch/models/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.7/alphaz/stitch/models/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      391 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/stitch/models/element.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       46 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/stitch/run.bat
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1857 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/stitch/stitch.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.706307 alphaz-0.7.7/alphaz/stitch/web-drivers/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)  8738816 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/stitch/web-drivers/chromedriver.exe
--rw-rw-r--   0 aurele    (1000) aurele    (1000)  7008696 2022-04-19 08:43:27.000000 alphaz-0.7.7/alphaz/stitch/web-drivers/geckodriver
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.654307 alphaz-0.7.7/alphaz/stitch/websites/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.714307 alphaz-0.7.7/alphaz/stitch/websites/Test/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      204 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/stitch/websites/Test/init.json
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.718307 alphaz-0.7.7/alphaz/stitch/websites/stiki/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      363 2022-04-13 09:59:51.000000 alphaz-0.7.7/alphaz/stitch/websites/stiki/init.json
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.718307 alphaz-0.7.7/alphaz/templates/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.7/alphaz/templates/__init__.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.718307 alphaz-0.7.7/alphaz/templates/assets/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.7/alphaz/templates/assets/__init__.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.718307 alphaz-0.7.7/alphaz/templates/assets/css/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    95923 2021-09-10 07:16:32.000000 alphaz-0.7.7/alphaz/templates/assets/css/home.css
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2356 2021-08-06 18:55:11.000000 alphaz-0.7.7/alphaz/templates/assets/css/logs.css
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.718307 alphaz-0.7.7/alphaz/templates/assets/images/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.718307 alphaz-0.7.7/alphaz/templates/assets/images/icons/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      276 2021-08-06 18:55:11.000000 alphaz-0.7.7/alphaz/templates/assets/images/icons/admin.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1444 2021-08-06 18:55:11.000000 alphaz-0.7.7/alphaz/templates/assets/images/icons/alpha.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      142 2021-08-06 18:55:11.000000 alphaz-0.7.7/alphaz/templates/assets/images/icons/save.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     8889 2021-08-06 18:55:11.000000 alphaz-0.7.7/alphaz/templates/assets/images/icons/start-icon.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      136 2021-08-06 18:55:11.000000 alphaz-0.7.7/alphaz/templates/assets/images/icons/user.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    23747 2021-08-06 18:55:11.000000 alphaz-0.7.7/alphaz/templates/assets/images/icons/wsalpha.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1165 2021-08-06 18:55:11.000000 alphaz-0.7.7/alphaz/templates/assets/images/loading.gif
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.718307 alphaz-0.7.7/alphaz/templates/assets/js/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.718307 alphaz-0.7.7/alphaz/templates/assets/js/libs/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    21922 2021-08-06 18:55:11.000000 alphaz-0.7.7/alphaz/templates/assets/js/libs/ansi_up.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    89475 2021-08-06 18:55:11.000000 alphaz-0.7.7/alphaz/templates/assets/js/libs/jquery.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     7339 2022-10-26 14:51:00.000000 alphaz-0.7.7/alphaz/templates/assets/js/logs.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       37 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/templates/hello.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    19017 2022-01-17 10:25:20.000000 alphaz-0.7.7/alphaz/templates/home.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3779 2021-08-06 18:55:11.000000 alphaz-0.7.7/alphaz/templates/logs.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1153 2023-01-25 21:39:07.000000 alphaz-0.7.7/alphaz/test.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.718307 alphaz-0.7.7/alphaz/tests/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      119 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/tests/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    14409 2023-04-27 20:33:27.000000 alphaz-0.7.7/alphaz/tests/api.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2498 2023-04-27 20:33:27.000000 alphaz-0.7.7/alphaz/tests/basic_test.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1526 2021-11-30 22:30:57.000000 alphaz-0.7.7/alphaz/tests/configurations.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    25295 2023-04-25 15:54:12.000000 alphaz-0.7.7/alphaz/tests/database.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      397 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/tests/processes.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      555 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/tests/utils.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.722307 alphaz-0.7.7/alphaz/utils/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       57 2023-04-27 10:12:16.000000 alphaz-0.7.7/alphaz/utils/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11583 2023-04-27 20:33:27.000000 alphaz-0.7.7/alphaz/utils/api.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.722307 alphaz-0.7.7/alphaz/utils/apm/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-04-21 13:36:09.000000 alphaz-0.7.7/alphaz/utils/apm/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1671 2023-04-22 14:04:43.000000 alphaz-0.7.7/alphaz/utils/apm/ora.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      338 2022-04-19 08:43:27.000000 alphaz-0.7.7/alphaz/utils/clean.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      813 2022-05-02 08:25:25.000000 alphaz-0.7.7/alphaz/utils/configuration.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.722307 alphaz-0.7.7/alphaz/utils/database/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    13818 2023-04-27 10:12:16.000000 alphaz-0.7.7/alphaz/utils/database/init.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5438 2023-04-27 10:12:16.000000 alphaz-0.7.7/alphaz/utils/database_to_dataclass.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2207 2023-03-16 15:41:50.000000 alphaz-0.7.7/alphaz/utils/decorators.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3112 2021-03-29 08:42:45.000000 alphaz-0.7.7/alphaz/utils/ensure.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1653 2023-04-25 15:54:12.000000 alphaz-0.7.7/alphaz/utils/init_database.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4405 2022-01-13 15:32:15.000000 alphaz-0.7.7/alphaz/utils/mep.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     7639 2021-04-21 22:36:11.000000 alphaz-0.7.7/alphaz/utils/screens.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    23624 2023-04-27 10:12:16.000000 alphaz-0.7.7/alphaz/utils/selectionMenu.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      764 2022-01-17 10:25:20.000000 alphaz-0.7.7/alphaz/utils/tasks.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1901 2023-04-26 18:21:23.000000 alphaz-0.7.7/alphaz/utils/tests.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      628 2023-03-16 15:41:50.000000 alphaz-0.7.7/alphaz/utils/time.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3849 2023-04-27 10:12:16.000000 alphaz-0.7.7/alphaz/utils/transactions.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 20:33:30.658307 alphaz-0.7.7/alphaz.egg-info/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      585 2023-04-27 20:33:30.000000 alphaz-0.7.7/alphaz.egg-info/PKG-INFO
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11365 2023-04-27 20:33:30.000000 alphaz-0.7.7/alphaz.egg-info/SOURCES.txt
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        1 2023-04-27 20:33:30.000000 alphaz-0.7.7/alphaz.egg-info/dependency_links.txt
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      458 2023-04-27 20:33:30.000000 alphaz-0.7.7/alphaz.egg-info/requires.txt
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        7 2023-04-27 20:33:30.000000 alphaz-0.7.7/alphaz.egg-info/top_level.txt
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       79 2023-04-27 20:33:30.722307 alphaz-0.7.7/setup.cfg
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3092 2023-04-27 20:33:20.000000 alphaz-0.7.7/setup.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.248816 alphaz-0.7.7.1/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1085 2019-07-02 13:36:12.000000 alphaz-0.7.7.1/LICENSE
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11211 2023-05-02 17:08:54.000000 alphaz-0.7.7.1/MANIFEST.in
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      600 2023-05-02 17:08:56.248816 alphaz-0.7.7.1/PKG-INFO
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1348 2021-07-12 18:07:51.000000 alphaz-0.7.7.1/README.md
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.188816 alphaz-0.7.7.1/alphaz/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        9 2023-04-18 09:00:04.000000 alphaz-0.7.7.1/alphaz/README.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      498 2023-05-02 17:06:49.000000 alphaz-0.7.7.1/alphaz/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      104 2021-03-29 08:42:45.000000 alphaz-0.7.7.1/alphaz/alphaz.bat
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       70 2021-03-29 08:42:45.000000 alphaz-0.7.7.1/alphaz/alphaz.code-workspace
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      208 2022-04-19 08:43:27.000000 alphaz-0.7.7.1/alphaz/alphaz.sh
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       48 2021-03-29 08:42:45.000000 alphaz-0.7.7.1/alphaz/api.bat
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      713 2023-04-18 09:00:04.000000 alphaz-0.7.7.1/alphaz/api.json
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      770 2022-04-13 09:59:51.000000 alphaz-0.7.7.1/alphaz/api.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.192816 alphaz-0.7.7.1/alphaz/apis/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.7.1/alphaz/apis/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-07-21 11:35:27.000000 alphaz-0.7.7.1/alphaz/apis/log.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2721 2023-03-17 07:06:42.000000 alphaz-0.7.7.1/alphaz/apis/mails.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.192816 alphaz-0.7.7.1/alphaz/apis/routes/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.7.1/alphaz/apis/routes/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1601 2023-05-02 08:30:13.000000 alphaz-0.7.7.1/alphaz/apis/routes/admin.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1143 2023-05-02 08:31:09.000000 alphaz-0.7.7.1/alphaz/apis/routes/api.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3039 2023-04-27 10:12:16.000000 alphaz-0.7.7.1/alphaz/apis/routes/basic_tests.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3193 2023-05-01 13:05:14.000000 alphaz-0.7.7.1/alphaz/apis/routes/database.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      413 2022-04-12 11:53:03.000000 alphaz-0.7.7.1/alphaz/apis/routes/git.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     7272 2023-04-27 10:12:16.000000 alphaz-0.7.7.1/alphaz/apis/routes/logs.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1810 2022-04-12 11:53:03.000000 alphaz-0.7.7.1/alphaz/apis/routes/mails.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6384 2023-04-27 10:12:16.000000 alphaz-0.7.7.1/alphaz/apis/routes/main.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1548 2023-04-27 20:33:27.000000 alphaz-0.7.7.1/alphaz/apis/routes/tests.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.192816 alphaz-0.7.7.1/alphaz/apis/routes/user_management/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      114 2022-04-27 13:24:50.000000 alphaz-0.7.7.1/alphaz/apis/routes/user_management/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2479 2023-04-27 10:12:16.000000 alphaz-0.7.7.1/alphaz/apis/routes/user_management/application_management.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2243 2023-04-27 10:12:16.000000 alphaz-0.7.7.1/alphaz/apis/routes/user_management/permission_management.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4104 2023-04-27 10:12:16.000000 alphaz-0.7.7.1/alphaz/apis/routes/user_management/role_management.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1291 2022-08-31 08:56:44.000000 alphaz-0.7.7.1/alphaz/apis/routes/user_management/user_management.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3476 2023-04-30 11:42:27.000000 alphaz-0.7.7.1/alphaz/apis/routes/users.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      584 2023-02-23 09:08:35.000000 alphaz-0.7.7.1/alphaz/apis/tests.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.192816 alphaz-0.7.7.1/alphaz/apis/users/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-07-21 11:35:27.000000 alphaz-0.7.7.1/alphaz/apis/users/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2718 2023-01-25 21:39:07.000000 alphaz-0.7.7.1/alphaz/apis/users/ldap.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11859 2023-05-02 12:00:06.000000 alphaz-0.7.7.1/alphaz/apis/users/users.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.196816 alphaz-0.7.7.1/alphaz/config/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.7.1/alphaz/config/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      795 2021-03-29 08:42:45.000000 alphaz-0.7.7.1/alphaz/config/config.css
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    12602 2021-03-29 08:42:45.000000 alphaz-0.7.7.1/alphaz/config/config.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      707 2022-08-11 06:44:17.000000 alphaz-0.7.7.1/alphaz/config/main_configuration.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      823 2021-03-29 08:42:45.000000 alphaz-0.7.7.1/alphaz/config/page.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1700 2021-03-29 08:42:45.000000 alphaz-0.7.7.1/alphaz/config/source.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1564 2021-03-29 08:42:45.000000 alphaz-0.7.7.1/alphaz/config.json
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      238 2023-01-06 09:14:28.000000 alphaz-0.7.7.1/alphaz/core.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.196816 alphaz-0.7.7.1/alphaz/documentations/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.196816 alphaz-0.7.7.1/alphaz/documentations/docs/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-07-21 11:35:27.000000 alphaz-0.7.7.1/alphaz/documentations/docs/alpha_admin.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1408 2023-04-12 11:28:51.000000 alphaz-0.7.7.1/alphaz/documentations/docs/alpha_core.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2595 2022-07-21 11:35:27.000000 alphaz-0.7.7.1/alphaz/documentations/docs/alpha_screens.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2222 2023-04-12 11:28:51.000000 alphaz-0.7.7.1/alphaz/documentations/docs/alpha_setup.md
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.196816 alphaz-0.7.7.1/alphaz/documentations/docs/api/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1527 2023-04-18 09:00:04.000000 alphaz-0.7.7.1/alphaz/documentations/docs/api/authorizations.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       72 2023-04-18 09:00:04.000000 alphaz-0.7.7.1/alphaz/documentations/docs/api/cache.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2931 2023-04-27 10:12:16.000000 alphaz-0.7.7.1/alphaz/documentations/docs/api/configuration.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       24 2023-04-18 09:00:04.000000 alphaz-0.7.7.1/alphaz/documentations/docs/api/issues.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      705 2023-04-18 09:00:04.000000 alphaz-0.7.7.1/alphaz/documentations/docs/api/main.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      559 2023-04-18 09:00:04.000000 alphaz-0.7.7.1/alphaz/documentations/docs/api/methods.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1728 2023-04-18 09:00:04.000000 alphaz-0.7.7.1/alphaz/documentations/docs/api/parameters.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1197 2023-04-18 09:00:04.000000 alphaz-0.7.7.1/alphaz/documentations/docs/api/routes.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      486 2023-04-18 09:00:04.000000 alphaz-0.7.7.1/alphaz/documentations/docs/api/sqlalchemy.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1129 2023-04-18 09:00:04.000000 alphaz-0.7.7.1/alphaz/documentations/docs/api_database.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2520 2023-01-06 09:14:28.000000 alphaz-0.7.7.1/alphaz/documentations/docs/configuration.md
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.196816 alphaz-0.7.7.1/alphaz/documentations/docs/database/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2187 2023-04-27 10:12:16.000000 alphaz-0.7.7.1/alphaz/documentations/docs/database/init.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      442 2023-04-18 09:00:04.000000 alphaz-0.7.7.1/alphaz/documentations/docs/database/instantiate.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      113 2023-04-18 09:00:04.000000 alphaz-0.7.7.1/alphaz/documentations/docs/database/main.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1806 2023-04-18 09:00:04.000000 alphaz-0.7.7.1/alphaz/documentations/docs/database/model.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      373 2023-04-18 09:00:04.000000 alphaz-0.7.7.1/alphaz/documentations/docs/database/relations.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1087 2023-04-18 09:00:04.000000 alphaz-0.7.7.1/alphaz/documentations/docs/database/schema.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      615 2023-04-18 09:00:04.000000 alphaz-0.7.7.1/alphaz/documentations/docs/database/update.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      357 2021-04-14 08:59:25.000000 alphaz-0.7.7.1/alphaz/documentations/docs/documentation.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3526 2023-04-12 11:28:51.000000 alphaz-0.7.7.1/alphaz/documentations/docs/index.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1090 2023-04-18 09:00:04.000000 alphaz-0.7.7.1/alphaz/documentations/mkdocs.yml
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.200816 alphaz-0.7.7.1/alphaz/documentations/site/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    13156 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/404.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.200816 alphaz-0.7.7.1/alphaz/documentations/site/alpha_admin/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14222 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/alpha_admin/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.200816 alphaz-0.7.7.1/alphaz/documentations/site/alpha_core/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    22752 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/alpha_core/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.200816 alphaz-0.7.7.1/alphaz/documentations/site/alpha_screens/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    21873 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/alpha_screens/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.200816 alphaz-0.7.7.1/alphaz/documentations/site/alpha_setup/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    24071 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/alpha_setup/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.184816 alphaz-0.7.7.1/alphaz/documentations/site/api/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.200816 alphaz-0.7.7.1/alphaz/documentations/site/api/authorizations/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    17905 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/api/authorizations/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.200816 alphaz-0.7.7.1/alphaz/documentations/site/api/cache/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14918 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/api/cache/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.200816 alphaz-0.7.7.1/alphaz/documentations/site/api/configuration/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    27645 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/api/configuration/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.200816 alphaz-0.7.7.1/alphaz/documentations/site/api/issues/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    16365 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/api/issues/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.200816 alphaz-0.7.7.1/alphaz/documentations/site/api/main/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    17987 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/api/main/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.200816 alphaz-0.7.7.1/alphaz/documentations/site/api/methods/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    17722 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/api/methods/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.200816 alphaz-0.7.7.1/alphaz/documentations/site/api/parameters/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    20075 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/api/parameters/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.200816 alphaz-0.7.7.1/alphaz/documentations/site/api/routes/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    19333 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/api/routes/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.200816 alphaz-0.7.7.1/alphaz/documentations/site/api/sqlalchemy/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    17109 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/api/sqlalchemy/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.200816 alphaz-0.7.7.1/alphaz/documentations/site/api_database/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    22959 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/api_database/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.184816 alphaz-0.7.7.1/alphaz/documentations/site/assets/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.200816 alphaz-0.7.7.1/alphaz/documentations/site/assets/images/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1870 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/assets/images/favicon.png
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.200816 alphaz-0.7.7.1/alphaz/documentations/site/assets/javascripts/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    79520 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)   384391 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js.map
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.200816 alphaz-0.7.7.1/alphaz/documentations/site/assets/javascripts/lunr/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.204816 alphaz-0.7.7.1/alphaz/documentations/site/assets/javascripts/lunr/min/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    17058 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ar.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4654 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.da.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6119 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.de.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6208 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.du.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11499 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.es.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     9342 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fi.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    10669 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fr.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     9437 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.hu.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11232 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.it.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2313 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ja.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       36 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.jp.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      817 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.multi.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6026 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.nl.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4754 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.no.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    10171 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.pt.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    10958 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ro.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    10331 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ru.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3647 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4523 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.sv.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    15009 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.tr.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      784 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.vi.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    22878 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/assets/javascripts/lunr/tinyseg.js
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.204816 alphaz-0.7.7.1/alphaz/documentations/site/assets/javascripts/workers/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    34936 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)   167496 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js.map
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.204816 alphaz-0.7.7.1/alphaz/documentations/site/assets/stylesheets/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    87332 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)   319950 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css.map
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    10915 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    37512 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css.map
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.204816 alphaz-0.7.7.1/alphaz/documentations/site/configuration/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    28465 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/configuration/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.184816 alphaz-0.7.7.1/alphaz/documentations/site/database/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.204816 alphaz-0.7.7.1/alphaz/documentations/site/database/init/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    23029 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/database/init/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.208816 alphaz-0.7.7.1/alphaz/documentations/site/database/instantiate/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    17445 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/database/instantiate/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.208816 alphaz-0.7.7.1/alphaz/documentations/site/database/main/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14939 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/database/main/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.208816 alphaz-0.7.7.1/alphaz/documentations/site/database/model/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    24758 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/database/model/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.208816 alphaz-0.7.7.1/alphaz/documentations/site/database/relations/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    16511 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/database/relations/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.208816 alphaz-0.7.7.1/alphaz/documentations/site/database/schema/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    18704 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/database/schema/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.208816 alphaz-0.7.7.1/alphaz/documentations/site/database/update/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    20308 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/database/update/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.208816 alphaz-0.7.7.1/alphaz/documentations/site/documentation/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    17065 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/documentation/index.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    29467 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.208816 alphaz-0.7.7.1/alphaz/documentations/site/search/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    54135 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/search/search_index.json
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2809 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/sitemap.xml
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      209 2023-04-27 20:33:29.000000 alphaz-0.7.7.1/alphaz/documentations/site/sitemap.xml.gz
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       50 2022-04-19 08:43:27.000000 alphaz-0.7.7.1/alphaz/git.sh
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       45 2022-05-14 15:57:01.000000 alphaz-0.7.7.1/alphaz/help.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      905 2021-03-29 08:42:45.000000 alphaz-0.7.7.1/alphaz/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.212816 alphaz-0.7.7.1/alphaz/libs/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.7.1/alphaz/libs/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     5807 2023-04-27 20:33:27.000000 alphaz-0.7.7.1/alphaz/libs/api_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1901 2021-03-29 08:42:45.000000 alphaz-0.7.7.1/alphaz/libs/barcode_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    13989 2023-04-27 10:12:16.000000 alphaz-0.7.7.1/alphaz/libs/config_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2420 2023-03-29 19:04:59.000000 alphaz-0.7.7.1/alphaz/libs/converter_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     9264 2023-05-01 16:19:41.000000 alphaz-0.7.7.1/alphaz/libs/database_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4223 2023-02-06 12:52:51.000000 alphaz-0.7.7.1/alphaz/libs/date_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6381 2023-04-27 20:33:27.000000 alphaz-0.7.7.1/alphaz/libs/dict_lib.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.212816 alphaz-0.7.7.1/alphaz/libs/emulation/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1758 2023-02-02 21:07:35.000000 alphaz-0.7.7.1/alphaz/libs/emulation/vt102_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1642 2021-03-29 08:42:45.000000 alphaz-0.7.7.1/alphaz/libs/events.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3351 2022-01-17 10:25:20.000000 alphaz-0.7.7.1/alphaz/libs/files_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1184 2023-04-27 10:12:16.000000 alphaz-0.7.7.1/alphaz/libs/flask_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       49 2021-03-29 08:42:45.000000 alphaz-0.7.7.1/alphaz/libs/ftp_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1093 2022-07-21 11:35:27.000000 alphaz-0.7.7.1/alphaz/libs/img_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6207 2023-04-27 10:12:16.000000 alphaz-0.7.7.1/alphaz/libs/io_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3233 2023-04-27 10:12:16.000000 alphaz-0.7.7.1/alphaz/libs/json_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1151 2023-04-27 10:12:16.000000 alphaz-0.7.7.1/alphaz/libs/logs_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    13008 2023-04-27 10:12:16.000000 alphaz-0.7.7.1/alphaz/libs/mail_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      508 2021-03-29 08:42:45.000000 alphaz-0.7.7.1/alphaz/libs/nav_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      614 2022-09-07 06:57:10.000000 alphaz-0.7.7.1/alphaz/libs/notifications_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1348 2021-03-29 08:42:45.000000 alphaz-0.7.7.1/alphaz/libs/number_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      177 2021-03-29 08:42:45.000000 alphaz-0.7.7.1/alphaz/libs/os_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2782 2021-03-29 08:42:45.000000 alphaz-0.7.7.1/alphaz/libs/process_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14220 2023-05-02 17:06:49.000000 alphaz-0.7.7.1/alphaz/libs/py_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      886 2023-04-21 07:47:57.000000 alphaz-0.7.7.1/alphaz/libs/scp_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     8082 2022-01-17 10:25:20.000000 alphaz-0.7.7.1/alphaz/libs/search_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6362 2023-04-27 10:12:16.000000 alphaz-0.7.7.1/alphaz/libs/secure_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2929 2023-04-27 10:12:16.000000 alphaz-0.7.7.1/alphaz/libs/soap_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      139 2021-03-29 08:42:45.000000 alphaz-0.7.7.1/alphaz/libs/sql_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    18623 2023-04-27 10:12:16.000000 alphaz-0.7.7.1/alphaz/libs/ssh_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     9896 2023-04-27 10:12:16.000000 alphaz-0.7.7.1/alphaz/libs/string_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     5556 2023-04-27 20:33:27.000000 alphaz-0.7.7.1/alphaz/libs/test_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      703 2023-03-16 15:41:50.000000 alphaz-0.7.7.1/alphaz/libs/time_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4492 2023-04-27 10:12:16.000000 alphaz-0.7.7.1/alphaz/libs/transactions_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6565 2023-05-02 12:02:14.000000 alphaz-0.7.7.1/alphaz/libs/user_lib.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.212816 alphaz-0.7.7.1/alphaz/libs/user_management/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-04-27 13:24:50.000000 alphaz-0.7.7.1/alphaz/libs/user_management/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1336 2023-04-27 10:12:16.000000 alphaz-0.7.7.1/alphaz/libs/user_management/application_management_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1597 2023-04-27 10:12:16.000000 alphaz-0.7.7.1/alphaz/libs/user_management/permission_management_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3376 2023-04-27 10:12:16.000000 alphaz-0.7.7.1/alphaz/libs/user_management/role_management_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2313 2023-04-27 10:12:16.000000 alphaz-0.7.7.1/alphaz/libs/user_management/user_management_lib.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.216816 alphaz-0.7.7.1/alphaz/mails/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.216816 alphaz-0.7.7.1/alphaz/mails/Images/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)   948952 2021-03-29 08:42:45.000000 alphaz-0.7.7.1/alphaz/mails/Images/Background.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1835 2021-03-29 08:42:45.000000 alphaz-0.7.7.1/alphaz/mails/Images/Facebook_logo.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2484 2021-03-29 08:42:45.000000 alphaz-0.7.7.1/alphaz/mails/Images/Twitter_logo.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3522 2021-03-29 08:42:45.000000 alphaz-0.7.7.1/alphaz/mails/Images/Web_logo.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.7.1/alphaz/mails/Images/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)   966605 2021-03-29 08:42:45.000000 alphaz-0.7.7.1/alphaz/mails/Mail.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     5097 2022-04-13 09:59:51.000000 alphaz-0.7.7.1/alphaz/mails/Webmail.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.7.1/alphaz/mails/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    22029 2023-03-17 05:42:16.000000 alphaz-0.7.7.1/alphaz/mails/debug.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    23078 2023-03-16 20:48:51.000000 alphaz-0.7.7.1/alphaz/mails/mail.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2331 2021-03-29 08:42:45.000000 alphaz-0.7.7.1/alphaz/mails/password_reset.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    24598 2022-04-13 09:59:51.000000 alphaz-0.7.7.1/alphaz/mails/stay_in_touch.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       40 2021-03-29 08:42:45.000000 alphaz-0.7.7.1/alphaz/mails/template.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.216816 alphaz-0.7.7.1/alphaz/models/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      107 2023-04-27 10:12:16.000000 alphaz-0.7.7.1/alphaz/models/__init__.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.220816 alphaz-0.7.7.1/alphaz/models/api/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      185 2022-04-12 11:53:03.000000 alphaz-0.7.7.1/alphaz/models/api/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      926 2023-04-27 10:12:16.000000 alphaz-0.7.7.1/alphaz/models/api/_answer.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2179 2021-09-13 12:55:49.000000 alphaz-0.7.7.1/alphaz/models/api/_colorations.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      133 2021-09-06 13:56:36.000000 alphaz-0.7.7.1/alphaz/models/api/_methods.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14340 2023-05-02 17:06:49.000000 alphaz-0.7.7.1/alphaz/models/api/_parameter.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14445 2023-04-27 10:12:16.000000 alphaz-0.7.7.1/alphaz/models/api/_reloader.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3717 2023-04-27 10:12:16.000000 alphaz-0.7.7.1/alphaz/models/api/_reloaders.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2402 2023-05-02 12:00:06.000000 alphaz-0.7.7.1/alphaz/models/api/_requests.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    18839 2023-04-27 20:33:27.000000 alphaz-0.7.7.1/alphaz/models/api/_route.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    20527 2023-05-02 12:00:06.000000 alphaz-0.7.7.1/alphaz/models/api/_structures.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      651 2022-02-01 21:43:05.000000 alphaz-0.7.7.1/alphaz/models/api/_utils.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      388 2022-07-22 14:00:51.000000 alphaz-0.7.7.1/alphaz/models/base.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.220816 alphaz-0.7.7.1/alphaz/models/config/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       32 2021-03-29 08:42:45.000000 alphaz-0.7.7.1/alphaz/models/config/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    26517 2023-04-27 10:12:16.000000 alphaz-0.7.7.1/alphaz/models/config/_config.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    12350 2023-04-25 15:54:12.000000 alphaz-0.7.7.1/alphaz/models/config/_utils.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.220816 alphaz-0.7.7.1/alphaz/models/database/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       53 2022-01-13 15:32:15.000000 alphaz-0.7.7.1/alphaz/models/database/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     5495 2023-03-17 15:16:42.000000 alphaz-0.7.7.1/alphaz/models/database/main_definitions.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     9992 2023-04-27 10:12:16.000000 alphaz-0.7.7.1/alphaz/models/database/models.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      609 2022-04-28 08:55:29.000000 alphaz-0.7.7.1/alphaz/models/database/operators.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1164 2023-01-25 21:39:07.000000 alphaz-0.7.7.1/alphaz/models/database/requests.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1087 2021-03-29 08:42:45.000000 alphaz-0.7.7.1/alphaz/models/database/row.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    57072 2023-05-02 17:06:49.000000 alphaz-0.7.7.1/alphaz/models/database/structure.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1826 2023-02-23 09:08:35.000000 alphaz-0.7.7.1/alphaz/models/database/tests.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4797 2023-05-01 13:14:01.000000 alphaz-0.7.7.1/alphaz/models/database/users_definitions.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     9301 2023-04-27 10:12:16.000000 alphaz-0.7.7.1/alphaz/models/database/utils.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1061 2022-04-12 11:53:03.000000 alphaz-0.7.7.1/alphaz/models/database/views.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1241 2021-03-29 08:42:45.000000 alphaz-0.7.7.1/alphaz/models/excel.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6683 2023-04-27 10:12:16.000000 alphaz-0.7.7.1/alphaz/models/ftp.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      150 2022-07-19 09:10:48.000000 alphaz-0.7.7.1/alphaz/models/img.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.220816 alphaz-0.7.7.1/alphaz/models/json/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       41 2021-03-29 08:42:45.000000 alphaz-0.7.7.1/alphaz/models/json/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2609 2023-01-06 09:14:28.000000 alphaz-0.7.7.1/alphaz/models/json/_converters.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.220816 alphaz-0.7.7.1/alphaz/models/logger/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       68 2022-01-19 15:41:22.000000 alphaz-0.7.7.1/alphaz/models/logger/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1319 2023-01-06 09:14:28.000000 alphaz-0.7.7.1/alphaz/models/logger/_colorations.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14322 2023-04-27 20:33:27.000000 alphaz-0.7.7.1/alphaz/models/logger/_logger.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      757 2021-03-29 08:42:45.000000 alphaz-0.7.7.1/alphaz/models/logger/_utils.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.220816 alphaz-0.7.7.1/alphaz/models/logs/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1280 2021-11-12 08:53:17.000000 alphaz-0.7.7.1/alphaz/models/logs/main.log
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      160 2021-11-07 15:22:58.000000 alphaz-0.7.7.1/alphaz/models/logs/main.log.2021-11-07
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.220816 alphaz-0.7.7.1/alphaz/models/main/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      354 2023-04-27 20:33:27.000000 alphaz-0.7.7.1/alphaz/models/main/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    30099 2023-05-02 17:06:49.000000 alphaz-0.7.7.1/alphaz/models/main/_base.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.224816 alphaz-0.7.7.1/alphaz/models/main/_core/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.7.1/alphaz/models/main/_core/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    16001 2023-05-01 12:34:28.000000 alphaz-0.7.7.1/alphaz/models/main/_core/_core.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       13 2021-03-29 08:42:45.000000 alphaz-0.7.7.1/alphaz/models/main/_core/_utils.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      335 2023-05-02 17:06:49.000000 alphaz-0.7.7.1/alphaz/models/main/_enum.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2001 2023-04-27 20:33:27.000000 alphaz-0.7.7.1/alphaz/models/main/_exception.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      501 2021-03-29 08:42:45.000000 alphaz-0.7.7.1/alphaz/models/main/_file.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      477 2021-03-29 08:42:45.000000 alphaz-0.7.7.1/alphaz/models/main/_process.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1305 2021-03-29 08:42:45.000000 alphaz-0.7.7.1/alphaz/models/main/_request.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      925 2021-03-29 08:42:45.000000 alphaz-0.7.7.1/alphaz/models/main/_singleton.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2218 2023-04-27 10:12:16.000000 alphaz-0.7.7.1/alphaz/models/request.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.224816 alphaz-0.7.7.1/alphaz/models/tests/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      167 2023-04-25 15:54:12.000000 alphaz-0.7.7.1/alphaz/models/tests/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     8070 2023-04-27 10:12:16.000000 alphaz-0.7.7.1/alphaz/models/tests/_category.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3446 2023-04-27 10:12:16.000000 alphaz-0.7.7.1/alphaz/models/tests/_group.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      163 2023-04-25 15:54:12.000000 alphaz-0.7.7.1/alphaz/models/tests/_levels.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4125 2023-04-27 10:12:16.000000 alphaz-0.7.7.1/alphaz/models/tests/_method.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4578 2023-04-27 10:12:16.000000 alphaz-0.7.7.1/alphaz/models/tests/_save.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14883 2023-05-02 17:06:49.000000 alphaz-0.7.7.1/alphaz/models/tests/_test.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     7505 2023-04-27 10:12:16.000000 alphaz-0.7.7.1/alphaz/models/tests/_wrappers.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2910 2023-05-02 12:00:06.000000 alphaz-0.7.7.1/alphaz/models/user.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2367 2021-03-29 08:42:45.000000 alphaz-0.7.7.1/alphaz/models/watcher.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.224816 alphaz-0.7.7.1/alphaz/pocs/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      685 2021-03-29 08:42:45.000000 alphaz-0.7.7.1/alphaz/pocs/main.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       72 2021-03-29 08:42:45.000000 alphaz-0.7.7.1/alphaz/reload_gitignore.bat
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       67 2022-04-12 12:30:24.000000 alphaz-0.7.7.1/alphaz/req.sh
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      460 2023-04-11 14:13:25.000000 alphaz-0.7.7.1/alphaz/requirements.txt
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1345 2022-04-19 08:43:27.000000 alphaz-0.7.7.1/alphaz/run.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.224816 alphaz-0.7.7.1/alphaz/src/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.7.1/alphaz/src/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    23747 2021-03-29 08:42:45.000000 alphaz-0.7.7.1/alphaz/src/alpha.png
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.224816 alphaz-0.7.7.1/alphaz/src/configs/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      135 2022-04-19 08:43:27.000000 alphaz-0.7.7.1/alphaz/src/configs/config.json
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      674 2023-01-25 21:39:07.000000 alphaz-0.7.7.1/alphaz/src/configs/loggers.json
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      490 2022-01-13 15:32:15.000000 alphaz-0.7.7.1/alphaz/src/configs/loggers_colors.json
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.224816 alphaz-0.7.7.1/alphaz/src/database/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.7.1/alphaz/src/database/__init__.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.224816 alphaz-0.7.7.1/alphaz/stitch/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1769 2021-03-29 08:42:45.000000 alphaz-0.7.7.1/alphaz/stitch/Core.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       26 2021-03-29 08:42:45.000000 alphaz-0.7.7.1/alphaz/stitch/__init__.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.224816 alphaz-0.7.7.1/alphaz/stitch/imports/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       78 2021-03-29 08:42:45.000000 alphaz-0.7.7.1/alphaz/stitch/imports/__init__.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.224816 alphaz-0.7.7.1/alphaz/stitch/models/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.7.1/alphaz/stitch/models/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      391 2021-03-29 08:42:45.000000 alphaz-0.7.7.1/alphaz/stitch/models/element.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       46 2021-03-29 08:42:45.000000 alphaz-0.7.7.1/alphaz/stitch/run.bat
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1857 2021-03-29 08:42:45.000000 alphaz-0.7.7.1/alphaz/stitch/stitch.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.236816 alphaz-0.7.7.1/alphaz/stitch/web-drivers/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)  8738816 2021-03-29 08:42:45.000000 alphaz-0.7.7.1/alphaz/stitch/web-drivers/chromedriver.exe
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)  7008696 2022-04-19 08:43:27.000000 alphaz-0.7.7.1/alphaz/stitch/web-drivers/geckodriver
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.184816 alphaz-0.7.7.1/alphaz/stitch/websites/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.244816 alphaz-0.7.7.1/alphaz/stitch/websites/Test/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      204 2021-03-29 08:42:45.000000 alphaz-0.7.7.1/alphaz/stitch/websites/Test/init.json
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.244816 alphaz-0.7.7.1/alphaz/stitch/websites/stiki/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      363 2022-04-13 09:59:51.000000 alphaz-0.7.7.1/alphaz/stitch/websites/stiki/init.json
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.244816 alphaz-0.7.7.1/alphaz/templates/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.7.1/alphaz/templates/__init__.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.244816 alphaz-0.7.7.1/alphaz/templates/assets/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.7.1/alphaz/templates/assets/__init__.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.244816 alphaz-0.7.7.1/alphaz/templates/assets/css/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    95923 2021-09-10 07:16:32.000000 alphaz-0.7.7.1/alphaz/templates/assets/css/home.css
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2356 2021-08-06 18:55:11.000000 alphaz-0.7.7.1/alphaz/templates/assets/css/logs.css
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.244816 alphaz-0.7.7.1/alphaz/templates/assets/images/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.244816 alphaz-0.7.7.1/alphaz/templates/assets/images/icons/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      276 2021-08-06 18:55:11.000000 alphaz-0.7.7.1/alphaz/templates/assets/images/icons/admin.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1444 2021-08-06 18:55:11.000000 alphaz-0.7.7.1/alphaz/templates/assets/images/icons/alpha.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      142 2021-08-06 18:55:11.000000 alphaz-0.7.7.1/alphaz/templates/assets/images/icons/save.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     8889 2021-08-06 18:55:11.000000 alphaz-0.7.7.1/alphaz/templates/assets/images/icons/start-icon.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      136 2021-08-06 18:55:11.000000 alphaz-0.7.7.1/alphaz/templates/assets/images/icons/user.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    23747 2021-08-06 18:55:11.000000 alphaz-0.7.7.1/alphaz/templates/assets/images/icons/wsalpha.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1165 2021-08-06 18:55:11.000000 alphaz-0.7.7.1/alphaz/templates/assets/images/loading.gif
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.244816 alphaz-0.7.7.1/alphaz/templates/assets/js/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.244816 alphaz-0.7.7.1/alphaz/templates/assets/js/libs/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    21922 2021-08-06 18:55:11.000000 alphaz-0.7.7.1/alphaz/templates/assets/js/libs/ansi_up.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    89475 2021-08-06 18:55:11.000000 alphaz-0.7.7.1/alphaz/templates/assets/js/libs/jquery.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     7339 2022-10-26 14:51:00.000000 alphaz-0.7.7.1/alphaz/templates/assets/js/logs.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       37 2021-03-29 08:42:45.000000 alphaz-0.7.7.1/alphaz/templates/hello.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    19017 2022-01-17 10:25:20.000000 alphaz-0.7.7.1/alphaz/templates/home.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3779 2021-08-06 18:55:11.000000 alphaz-0.7.7.1/alphaz/templates/logs.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1153 2023-01-25 21:39:07.000000 alphaz-0.7.7.1/alphaz/test.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.248816 alphaz-0.7.7.1/alphaz/tests/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      119 2021-03-29 08:42:45.000000 alphaz-0.7.7.1/alphaz/tests/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14409 2023-04-27 20:33:27.000000 alphaz-0.7.7.1/alphaz/tests/api.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4444 2023-05-02 17:06:49.000000 alphaz-0.7.7.1/alphaz/tests/basic_test.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1526 2021-11-30 22:30:57.000000 alphaz-0.7.7.1/alphaz/tests/configurations.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    25295 2023-04-25 15:54:12.000000 alphaz-0.7.7.1/alphaz/tests/database.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      397 2021-03-29 08:42:45.000000 alphaz-0.7.7.1/alphaz/tests/processes.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      555 2021-03-29 08:42:45.000000 alphaz-0.7.7.1/alphaz/tests/utils.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.248816 alphaz-0.7.7.1/alphaz/utils/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       57 2023-04-27 10:12:16.000000 alphaz-0.7.7.1/alphaz/utils/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11705 2023-05-02 09:06:19.000000 alphaz-0.7.7.1/alphaz/utils/api.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.248816 alphaz-0.7.7.1/alphaz/utils/apm/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-04-21 13:36:09.000000 alphaz-0.7.7.1/alphaz/utils/apm/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1671 2023-04-22 14:04:43.000000 alphaz-0.7.7.1/alphaz/utils/apm/ora.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      338 2022-04-19 08:43:27.000000 alphaz-0.7.7.1/alphaz/utils/clean.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      813 2022-05-02 08:25:25.000000 alphaz-0.7.7.1/alphaz/utils/configuration.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.248816 alphaz-0.7.7.1/alphaz/utils/database/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    12809 2023-05-01 16:05:30.000000 alphaz-0.7.7.1/alphaz/utils/database/init.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     5438 2023-04-27 10:12:16.000000 alphaz-0.7.7.1/alphaz/utils/database_to_dataclass.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2207 2023-03-16 15:41:50.000000 alphaz-0.7.7.1/alphaz/utils/decorators.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3112 2021-03-29 08:42:45.000000 alphaz-0.7.7.1/alphaz/utils/ensure.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1653 2023-04-25 15:54:12.000000 alphaz-0.7.7.1/alphaz/utils/init_database.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4405 2022-01-13 15:32:15.000000 alphaz-0.7.7.1/alphaz/utils/mep.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     7639 2021-04-21 22:36:11.000000 alphaz-0.7.7.1/alphaz/utils/screens.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    23624 2023-04-27 10:12:16.000000 alphaz-0.7.7.1/alphaz/utils/selectionMenu.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      764 2022-01-17 10:25:20.000000 alphaz-0.7.7.1/alphaz/utils/tasks.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1901 2023-04-26 18:21:23.000000 alphaz-0.7.7.1/alphaz/utils/tests.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      628 2023-03-16 15:41:50.000000 alphaz-0.7.7.1/alphaz/utils/time.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3849 2023-04-27 10:12:16.000000 alphaz-0.7.7.1/alphaz/utils/transactions.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-02 17:08:56.192816 alphaz-0.7.7.1/alphaz.egg-info/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      600 2023-05-02 17:08:55.000000 alphaz-0.7.7.1/alphaz.egg-info/PKG-INFO
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11373 2023-05-02 17:08:56.000000 alphaz-0.7.7.1/alphaz.egg-info/SOURCES.txt
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        1 2023-05-02 17:08:55.000000 alphaz-0.7.7.1/alphaz.egg-info/dependency_links.txt
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      458 2023-05-02 17:08:55.000000 alphaz-0.7.7.1/alphaz.egg-info/requires.txt
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        7 2023-05-02 17:08:55.000000 alphaz-0.7.7.1/alphaz.egg-info/top_level.txt
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       79 2023-05-02 17:08:56.248816 alphaz-0.7.7.1/setup.cfg
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3094 2023-05-02 17:08:50.000000 alphaz-0.7.7.1/setup.py
```

### Comparing `alphaz-0.7.7/MANIFEST.in` & `alphaz-0.7.7.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/PKG-INFO` & `alphaz-0.7.7.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,20 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: alphaz
-Version: 0.7.7
+Version: 0.7.7.1
 Summary: A package full of very nice tools
 Home-page: https://github.com/ZAurele/alphaz
+Download-URL: https://github.com/ZAurele/alphaz/archive/refs/tags/0.7.7.1.tar.gz
 Author: Aurèle
 Author-email: contact@aurele.eu
 License: MIT
-Download-URL: https://github.com/ZAurele/alphaz/archive/refs/tags/0.7.7.tar.gz
-Description: UNKNOWN
 Keywords: Flask,Json
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
+License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `alphaz-0.7.7/README.md` & `alphaz-0.7.7.1/README.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/api.json` & `alphaz-0.7.7.1/alphaz/api.json`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/api.py` & `alphaz-0.7.7.1/alphaz/api.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/apis/mails.py` & `alphaz-0.7.7.1/alphaz/apis/mails.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/apis/routes/admin.py` & `alphaz-0.7.7.1/alphaz/apis/routes/admin.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from core import core
 
 api = core.api
 db = core.db
 log = core.get_logger("api")
 
 
-@route("/admin/key", parameters=[Parameter("key")], methods=["POST"])
+@route("/admin/key", parameters=[Parameter("key")], methods=["POST"], admin=True)
 def get_key():
     return secure_lib.get_cry_operation_code(api["key"])
 
 
 @route("/admin/logs/clear", methods=["GET"], admin=True, parameters=[])
 def clear_logs():
     done = logs_lib.clear_logs(api)
@@ -37,15 +37,15 @@
     ],
     logged=True,
 )
 def admin_logs():
     return logs_lib.get_logs(**api.get_parameters())
 
 
-@route("/admin/process")
+@route("/admin/process", admin=True)
 def get_admin_process():
     import psutil
 
     output = {}
     # Iterate over all running process
     i = 0
     for proc in psutil.process_iter():
```

### Comparing `alphaz-0.7.7/alphaz/apis/routes/basic_tests.py` & `alphaz-0.7.7.1/alphaz/apis/routes/basic_tests.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/apis/routes/database.py` & `alphaz-0.7.7.1/alphaz/apis/routes/database.py`

 * *Files 3% similar despite different names*

```diff
@@ -124,7 +124,12 @@
         Parameter("value", required=True),
         Parameter("bind", required=True),
         Parameter("column_name"),
     ],
 )
 def get_database_whereused():
     return database_lib.whereused(**API.gets())
+
+
+@route("/database/structure")
+def get_database_structure():
+    return database_lib.get_database_structure(**API.gets())
```

### Comparing `alphaz-0.7.7/alphaz/apis/routes/logs.py` & `alphaz-0.7.7.1/alphaz/apis/routes/logs.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/apis/routes/mails.py` & `alphaz-0.7.7.1/alphaz/apis/routes/mails.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/apis/routes/main.py` & `alphaz-0.7.7.1/alphaz/apis/routes/main.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/apis/routes/tests.py` & `alphaz-0.7.7.1/alphaz/apis/routes/tests.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/apis/routes/user_management/application_management.py` & `alphaz-0.7.7.1/alphaz/apis/routes/user_management/application_management.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/apis/routes/user_management/permission_management.py` & `alphaz-0.7.7.1/alphaz/apis/routes/user_management/permission_management.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/apis/routes/user_management/role_management.py` & `alphaz-0.7.7.1/alphaz/apis/routes/user_management/role_management.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/apis/routes/user_management/user_management.py` & `alphaz-0.7.7.1/alphaz/apis/routes/user_management/user_management.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/apis/routes/users.py` & `alphaz-0.7.7.1/alphaz/apis/routes/users.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 # UTILS
 from ...utils.api import ADMIN_USER_ID_PUBLIC, ADMIN_USER_NAME_PUBLIC, route, Parameter
 
 # MODELS
 from ...models.main import AlphaException
 
 # LIBS
-from ...libs import user_lib
+from ...libs import user_lib, secure_lib
 
 from ..users import users
 
 
 @route("user/infos", logged=True)
 def user_infos():
     return API.get_logged_user()
 
 
 @route(
-    "user/data",
+    "/user/data",
     parameters=[
         Parameter("value", required=True),
-        Parameter("column", required=True),
+        Parameter("columns", required=True),
         Parameter("activity", ptype=bool),
     ],
 )
 def user_data():
     return user_lib.get_user_data_from_database(**API.gets(), force_local=True)
 
 
@@ -44,14 +44,19 @@
 )
 def register():
     if API.get_logged_user() is not None:
         raise AlphaException("logged")
     users.try_register_user(**API.gets())
 
 
+@route("/password", parameters=[Parameter("password")], admin=True)
+def password():
+    return secure_lib.secure_password(**API.gets())
+
+
 @route(
     "/register/validation",
     methods=["POST"],
     parameters=[Parameter("tmp_token", required=True)],
 )
 def register_validation():
     if API.get_logged_user() is not None:
```

### Comparing `alphaz-0.7.7/alphaz/apis/tests.py` & `alphaz-0.7.7.1/alphaz/apis/tests.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/apis/users/ldap.py` & `alphaz-0.7.7.1/alphaz/apis/users/ldap.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/apis/users/users.py` & `alphaz-0.7.7.1/alphaz/apis/users/users.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # MODULES
-import datetime, jwt, itertools
+import datetime, jwt, itertools, socket
 import enum
 from flask import request
 
 # CORE
 from core import core, API, DB
 
 # MODELS
@@ -262,20 +262,28 @@
 
     if user is None:
         raise AlphaException("incorrect_username_or_password")
 
     expire = get_expire_datetime()
     token = get_encoded_jwt_from_user_data(user)
 
+    try:
+        ip_address = request.remote_addr
+    except:
+        ## getting the hostname by socket.gethostname() method
+        hostname = socket.gethostname()
+        ## getting the IP address using socket.gethostbyname() method
+        ip_address = socket.gethostbyname(hostname)
+
     # Add new token session related to user
     if not DB.add_or_update(
         UserSession(
             user_id=user.id,
             token=token,
-            ip=request.remote_addr,
+            ip=ip_address,
             expire=expire,
         )
     ):
         raise AlphaException("Cannot update user session")
 
     return {
         **{
```

### Comparing `alphaz-0.7.7/alphaz/config/config.css` & `alphaz-0.7.7.1/alphaz/config/config.css`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/config/config.html` & `alphaz-0.7.7.1/alphaz/config/config.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/config/main_configuration.py` & `alphaz-0.7.7.1/alphaz/config/main_configuration.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/config/page.py` & `alphaz-0.7.7.1/alphaz/config/page.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/config/source.html` & `alphaz-0.7.7.1/alphaz/config/source.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/config.json` & `alphaz-0.7.7.1/alphaz/config.json`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/docs/alpha_core.md` & `alphaz-0.7.7.1/alphaz/documentations/docs/alpha_core.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/docs/alpha_screens.md` & `alphaz-0.7.7.1/alphaz/documentations/docs/alpha_screens.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/docs/alpha_setup.md` & `alphaz-0.7.7.1/alphaz/documentations/docs/alpha_setup.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/docs/api/authorizations.md` & `alphaz-0.7.7.1/alphaz/documentations/docs/api/authorizations.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/docs/api/configuration.md` & `alphaz-0.7.7.1/alphaz/documentations/docs/api/configuration.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/docs/api/main.md` & `alphaz-0.7.7.1/alphaz/documentations/docs/api/main.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/docs/api/methods.md` & `alphaz-0.7.7.1/alphaz/documentations/docs/api/methods.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/docs/api/parameters.md` & `alphaz-0.7.7.1/alphaz/documentations/docs/api/parameters.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/docs/api/routes.md` & `alphaz-0.7.7.1/alphaz/documentations/docs/api/routes.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/docs/api_database.md` & `alphaz-0.7.7.1/alphaz/documentations/docs/api_database.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/docs/configuration.md` & `alphaz-0.7.7.1/alphaz/documentations/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/docs/database/init.md` & `alphaz-0.7.7.1/alphaz/documentations/docs/database/init.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/docs/database/model.md` & `alphaz-0.7.7.1/alphaz/documentations/docs/database/model.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/docs/database/schema.md` & `alphaz-0.7.7.1/alphaz/documentations/docs/database/schema.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/docs/database/update.md` & `alphaz-0.7.7.1/alphaz/documentations/docs/database/update.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/docs/index.md` & `alphaz-0.7.7.1/alphaz/documentations/docs/index.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/mkdocs.yml` & `alphaz-0.7.7.1/alphaz/documentations/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/404.html` & `alphaz-0.7.7.1/alphaz/documentations/site/404.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/alpha_admin/index.html` & `alphaz-0.7.7.1/alphaz/documentations/site/alpha_admin/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/alpha_core/index.html` & `alphaz-0.7.7.1/alphaz/documentations/site/alpha_core/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/alpha_screens/index.html` & `alphaz-0.7.7.1/alphaz/documentations/site/alpha_screens/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/alpha_setup/index.html` & `alphaz-0.7.7.1/alphaz/documentations/site/alpha_setup/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/api/authorizations/index.html` & `alphaz-0.7.7.1/alphaz/documentations/site/api/authorizations/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/api/cache/index.html` & `alphaz-0.7.7.1/alphaz/documentations/site/api/cache/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/api/configuration/index.html` & `alphaz-0.7.7.1/alphaz/documentations/site/api/configuration/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/api/issues/index.html` & `alphaz-0.7.7.1/alphaz/documentations/site/api/issues/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/api/main/index.html` & `alphaz-0.7.7.1/alphaz/documentations/site/api/main/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/api/methods/index.html` & `alphaz-0.7.7.1/alphaz/documentations/site/api/methods/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/api/parameters/index.html` & `alphaz-0.7.7.1/alphaz/documentations/site/api/parameters/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/api/routes/index.html` & `alphaz-0.7.7.1/alphaz/documentations/site/api/routes/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/api/sqlalchemy/index.html` & `alphaz-0.7.7.1/alphaz/documentations/site/api/sqlalchemy/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/api_database/index.html` & `alphaz-0.7.7.1/alphaz/documentations/site/api_database/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/assets/images/favicon.png` & `alphaz-0.7.7.1/alphaz/documentations/site/assets/images/favicon.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js` & `alphaz-0.7.7.1/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js.map` & `alphaz-0.7.7.1/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js.map`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ar.min.js` & `alphaz-0.7.7.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ar.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.da.min.js` & `alphaz-0.7.7.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.da.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.de.min.js` & `alphaz-0.7.7.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.de.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.du.min.js` & `alphaz-0.7.7.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.du.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.es.min.js` & `alphaz-0.7.7.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.es.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fi.min.js` & `alphaz-0.7.7.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fi.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fr.min.js` & `alphaz-0.7.7.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fr.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.hu.min.js` & `alphaz-0.7.7.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.hu.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.it.min.js` & `alphaz-0.7.7.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.it.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ja.min.js` & `alphaz-0.7.7.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ja.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.multi.min.js` & `alphaz-0.7.7.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.multi.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.nl.min.js` & `alphaz-0.7.7.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.nl.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.no.min.js` & `alphaz-0.7.7.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.no.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.pt.min.js` & `alphaz-0.7.7.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.pt.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ro.min.js` & `alphaz-0.7.7.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ro.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ru.min.js` & `alphaz-0.7.7.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ru.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js` & `alphaz-0.7.7.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.sv.min.js` & `alphaz-0.7.7.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.sv.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.tr.min.js` & `alphaz-0.7.7.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.tr.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.vi.min.js` & `alphaz-0.7.7.1/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.vi.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/assets/javascripts/lunr/tinyseg.js` & `alphaz-0.7.7.1/alphaz/documentations/site/assets/javascripts/lunr/tinyseg.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js` & `alphaz-0.7.7.1/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js.map` & `alphaz-0.7.7.1/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js.map`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css` & `alphaz-0.7.7.1/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css.map` & `alphaz-0.7.7.1/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css.map`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css` & `alphaz-0.7.7.1/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css.map` & `alphaz-0.7.7.1/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css.map`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/configuration/index.html` & `alphaz-0.7.7.1/alphaz/documentations/site/configuration/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/database/init/index.html` & `alphaz-0.7.7.1/alphaz/documentations/site/database/init/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/database/instantiate/index.html` & `alphaz-0.7.7.1/alphaz/documentations/site/database/instantiate/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/database/main/index.html` & `alphaz-0.7.7.1/alphaz/documentations/site/database/main/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/database/model/index.html` & `alphaz-0.7.7.1/alphaz/documentations/site/database/model/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/database/relations/index.html` & `alphaz-0.7.7.1/alphaz/documentations/site/database/relations/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/database/schema/index.html` & `alphaz-0.7.7.1/alphaz/documentations/site/database/schema/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/database/update/index.html` & `alphaz-0.7.7.1/alphaz/documentations/site/database/update/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/documentation/index.html` & `alphaz-0.7.7.1/alphaz/documentations/site/documentation/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/index.html` & `alphaz-0.7.7.1/alphaz/documentations/site/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/search/search_index.json` & `alphaz-0.7.7.1/alphaz/documentations/site/search/search_index.json`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/documentations/site/sitemap.xml` & `alphaz-0.7.7.1/alphaz/documentations/site/sitemap.xml`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/index.html` & `alphaz-0.7.7.1/alphaz/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/libs/api_lib.py` & `alphaz-0.7.7.1/alphaz/libs/api_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/libs/barcode_lib.py` & `alphaz-0.7.7.1/alphaz/libs/barcode_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/libs/config_lib.py` & `alphaz-0.7.7.1/alphaz/libs/config_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/libs/converter_lib.py` & `alphaz-0.7.7.1/alphaz/libs/converter_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/libs/date_lib.py` & `alphaz-0.7.7.1/alphaz/libs/date_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/libs/dict_lib.py` & `alphaz-0.7.7.1/alphaz/libs/dict_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/libs/emulation/vt102_lib.py` & `alphaz-0.7.7.1/alphaz/libs/emulation/vt102_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/libs/events.py` & `alphaz-0.7.7.1/alphaz/libs/events.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/libs/files_lib.py` & `alphaz-0.7.7.1/alphaz/libs/files_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/libs/flask_lib.py` & `alphaz-0.7.7.1/alphaz/libs/flask_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/libs/img_lib.py` & `alphaz-0.7.7.1/alphaz/libs/img_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/libs/io_lib.py` & `alphaz-0.7.7.1/alphaz/libs/io_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/libs/json_lib.py` & `alphaz-0.7.7.1/alphaz/libs/json_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/libs/logs_lib.py` & `alphaz-0.7.7.1/alphaz/libs/logs_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/libs/mail_lib.py` & `alphaz-0.7.7.1/alphaz/libs/mail_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/libs/notifications_lib.py` & `alphaz-0.7.7.1/alphaz/libs/notifications_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/libs/number_lib.py` & `alphaz-0.7.7.1/alphaz/libs/number_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/libs/process_lib.py` & `alphaz-0.7.7.1/alphaz/libs/process_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/libs/py_lib.py` & `alphaz-0.7.7.1/alphaz/libs/py_lib.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-import sys, imp, inspect, os, glob, re
+import sys, imp, inspect, os, glob, re, dataclasses
+from types import UnionType
+from typing import OrderedDict, Type, List, Dict, Any, get_origin, get_args, Union
 
-from typing import OrderedDict, Type, List, Dict, Any, get_origin, get_args
+# MODELS
 from ..models.watcher import ModuleWatcher
 
 myself = lambda: inspect.stack()[1][3]
 
 
 def get_modules_infos(
     name: str | None = None, url: str | None = None, mode: str = None
@@ -208,42 +210,109 @@
     if not isinstance(obj, type):
         return is_subtype(type(obj), parent_type)
     if hasattr(obj, "__origin__"):
         return obj.__origin__ == parent_type
     return issubclass(obj, parent_type)
 
 
-def is_subtype(sub_type, parent_type):
+def is_union_type(o):
+    sub_origin = get_origin(o)
+    sub_args = get_args(o)
+    return sub_args and sub_origin and (sub_origin is Union or sub_origin is UnionType)
+
+
+def get_first_non_none_type(o):
+    if not is_union_type(o):
+        return o
+    sub_args = get_args(o)
+    sub_args = [t for t in sub_args if t != type(None)]
+    return sub_args[0]
+
+
+def is_subtype(sub_type, parent_type, debug: bool = False) -> bool:
     sub_origin = get_origin(sub_type)
     parent_origin = get_origin(parent_type)
 
     sub_args = get_args(sub_type)
+    if sub_args:
+        sub_args = [t for t in sub_args if t != type(None)]
     parent_args = get_args(parent_type)
+    if parent_args:
+        parent_args = [t for t in parent_args if t != type(None)]
 
     if not isinstance(sub_type, type) and sub_origin is None:
         return is_subtype(type(sub_type), parent_type)
 
+    if is_union_type(sub_type):
+        return all([is_subtype(s, parent_type) for s in sub_args])
+    if is_union_type(sub_origin):
+        return all([is_subtype(s, parent_type) for s in sub_args])
+
+    infos = " / ".join(
+        [
+            str(x)
+            for x in [
+                sub_type,
+                parent_type,
+                sub_origin,
+                parent_origin,
+                sub_args,
+                parent_args,
+            ]
+        ]
+    )
+
     if sub_origin is not None and sub_origin == parent_type:
         return True
 
     if sub_type == parent_type:
         return True
 
+    if sub_args and parent_args and all(a == b for a, b in zip(sub_args, parent_args)):
+        return True
+
+    try:
+        if sub_args and any([issubclass(s, parent_type) for s in sub_args]):
+            return True
+    except:
+        pass
+
+    try:
+        if issubclass(sub_type, parent_type):
+            return True
+    except:
+        pass
+
+    try:
+        if isinstance(sub_type, parent_type):
+            return True
+    except:
+        pass
+
     if sub_origin is None or parent_origin is None:
+        if debug:
+            print("   no origin: ", infos)
         return False
 
     if sub_origin != parent_origin:
+        if debug:
+            print("   diff origin: ", infos)
         return False
 
     if not parent_args and sub_origin == parent_origin:
         return True
+
     if not sub_args or not parent_args:
+        if debug:
+            print("   no args: ", infos)
         return False
 
     if not all(a == b for a, b in zip(sub_args, parent_args)):
+        if debug:
+            print("   diff args: ", infos)
         return False
     return True
 
 
 def is_subtype_old(sub_type: type | Any, parent_type: type):
     if not isinstance(sub_type, type):
         return is_subtype(type(sub_type), parent_type)
@@ -282,15 +351,18 @@
 
 
 def sort_by_key(input_dict):
     return OrderedDict(sorted(input_dict.items(), key=lambda x: x[0]))
 
 
 def compare_dicts(
-    dict_obj_1, dict_obj_2, sub_elements: dict = None, ignore: list[str] = None
+    dict_obj_1,
+    dict_obj_2,
+    sub_elements: dict | None = None,
+    ignore: list[str] | None = None,
 ):
     if not sub_elements:
         sub_elements = {}
 
     level_dict = {}
 
     if dict_obj_1 is None and dict_obj_2 is None:
```

### Comparing `alphaz-0.7.7/alphaz/libs/scp_lib.py` & `alphaz-0.7.7.1/alphaz/libs/scp_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/libs/search_lib.py` & `alphaz-0.7.7.1/alphaz/libs/search_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/libs/secure_lib.py` & `alphaz-0.7.7.1/alphaz/libs/secure_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/libs/soap_lib.py` & `alphaz-0.7.7.1/alphaz/libs/soap_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/libs/ssh_lib.py` & `alphaz-0.7.7.1/alphaz/libs/ssh_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/libs/string_lib.py` & `alphaz-0.7.7.1/alphaz/libs/string_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/libs/test_lib.py` & `alphaz-0.7.7.1/alphaz/libs/test_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/libs/time_lib.py` & `alphaz-0.7.7.1/alphaz/libs/time_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/libs/transactions_lib.py` & `alphaz-0.7.7.1/alphaz/libs/transactions_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/libs/user_lib.py` & `alphaz-0.7.7.1/alphaz/libs/user_lib.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # CORE
+from sqlalchemy import or_
 from core import core
 
 DB = core.db
 
 # MODULES
 import datetime
 from sqlalchemy.orm import sessionmaker
@@ -15,102 +16,63 @@
 # LIBS
 from . import secure_lib, string_lib, api_lib
 
 
 def __get_user_data_by_identifier_and_password(
     identifier,
     password_attempt,
-    identifier_type="username",
     no_password_check: bool = False,
 ) -> AlphaUser | None:
-    user = __get_user_data(identifier, identifier_type.lower())
+    user = __get_user_data(identifier, ["username", "mail"])
 
     if user is not None and password_attempt is not None:
         if no_password_check:
             return user
         valid_password = secure_lib.compare_passwords(password_attempt, user.password)
         if valid_password:
             return user
     return None
 
 
-def get_user_data_by_username_and_password(
-    username, password_attempt
-) -> AlphaUser | None:
-    """Get user data from database by username.
-
-    Args:
-        mail ([type]): [description]
-        password_attempt ([type]): [description]
-
-    Returns:
-        [type]: [description]
-    """
-    return __get_user_data_by_identifier_and_password(
-        identifier=username,
-        password_attempt=password_attempt,
-        identifier_type="username",
-    )
-
-
-def get_user_data_by_mail_and_password(mail, password_attempt) -> AlphaUser | None:
-    """Get user data from database by mail.
-
-    Args:
-        mail ([type]): [description]
-        password_attempt ([type]): [description]
-
-    Returns:
-        [type]: [description]
-    """
-    return __get_user_data_by_identifier_and_password(
-        identifier=mail, password_attempt=password_attempt, identifier_type="mail"
-    )
-
-
 def get_user_data_from_login(
     login, password=None, no_password_check: bool = False
 ) -> AlphaUser | None:
     """Get user data from database either by mail or username.
 
     Args:
         login ([type]): [description]
         password ([type]): [description]
 
     Returns:
         [type]: [description]
     """
-    user_mail = __get_user_data_by_identifier_and_password(
-        login, password, identifier_type="mail", no_password_check=no_password_check
-    )
-    user_username = __get_user_data_by_identifier_and_password(
-        login, password, identifier_type="username", no_password_check=no_password_check
+    user = __get_user_data_by_identifier_and_password(
+        login, password, no_password_check=no_password_check
     )
-    if user_mail is not None:
-        return user_mail
-    if user_username is not None:
-        return user_username
-    return None
+    return user
 
 
 def get_user_data_from_database(
     value,
-    column,
+    columns: str | list[str],
     activity: bool = False,
     force_local: bool = False,
     scoped_session: bool = False,
 ) -> dict | None:
     """Get the user associated with given column."""
     user = None
+    if type(columns) == str:
+        columns = [columns]
+    filters = [or_(*[User.__dict__[column] == value for column in columns])]
 
     if DB.user_api is None or force_local:
         if not scoped_session:
             user = DB.select(
                 User,
-                filters=[User.__dict__[column] == value],
+                filters=filters,
                 first=True,
                 relationship=True,
                 # disabled_relationships=["notifications"],
             )
             if user is not None and activity:
                 with user.query.session.begin(subtransactions=True):
                     user.last_activity = datetime.datetime.now()
@@ -124,24 +86,24 @@
 
             try:
                 # Commencer une transaction avec la session spécifique
                 with scoped_session.begin():
                     # Mettre à jour la personne avec la session spécifique
                     user = (
                         scoped_session.query(User)
-                        .filter(User.__dict__[column] == value)
+                        .filter(*filters)
                         .first()
                     )
 
                     if user is not None and activity:
                         # Stocker la valeur de user.mail dans une variable
                         user_mail = "-" if user.mail is None else user.mail
 
                         scoped_session.query(User).filter(
-                            User.__dict__[column] == value
+                            *filters
                         ).update(
                             {
                                 User.last_activity: datetime.datetime.now(),
                                 User.mail: user_mail,
                             }
                         )
                         scoped_session.commit()
@@ -157,22 +119,24 @@
             finally:
                 # Fermer la session spécifique
                 scoped_session.close()
     else:
         user_api = DB.user_api + "/user/data"
         user = api_lib.get_api_data(
             user_api,
-            params={"value": value, "column": column, "activity": activity},
+            params={"value": value, "columns": columns, "activity": activity},
         )
     return user if user is not None else None
 
 
-def __get_user_data(value, column, activity: bool = False) -> AlphaUser | None:
-    user = get_user_data_from_database(value, column, activity=activity)
-    alpha_user = AlphaUser.auto_map_from_dict(user) if user is not None else None
+def __get_user_data(
+    value, columns: str | list[str], activity: bool = False
+) -> AlphaUser | None:
+    user = get_user_data_from_database(value, columns, activity=activity)
+    alpha_user = AlphaUser.map_from_dict(user) if user is not None else None
     return alpha_user
 
 
 def get_user_data_by_id(user_id, activity: bool = False) -> AlphaUser | None:
     if not string_lib.is_number(user_id):
         return None
     return __get_user_data(user_id, "id", activity=activity)
@@ -233,8 +197,8 @@
         != None
     )
 
 
 def get_all_address_mails():
     return DB.select(
         defs.MailingList, distinct=defs.MailingList.email, unique=defs.MailingList.email
-    )
+    )
```

### Comparing `alphaz-0.7.7/alphaz/libs/user_management/application_management_lib.py` & `alphaz-0.7.7.1/alphaz/libs/user_management/application_management_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/libs/user_management/permission_management_lib.py` & `alphaz-0.7.7.1/alphaz/libs/user_management/permission_management_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/libs/user_management/role_management_lib.py` & `alphaz-0.7.7.1/alphaz/libs/user_management/role_management_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/libs/user_management/user_management_lib.py` & `alphaz-0.7.7.1/alphaz/libs/user_management/user_management_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/mails/Images/Background.png` & `alphaz-0.7.7.1/alphaz/mails/Images/Background.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/mails/Images/Facebook_logo.png` & `alphaz-0.7.7.1/alphaz/mails/Images/Facebook_logo.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/mails/Images/Twitter_logo.png` & `alphaz-0.7.7.1/alphaz/mails/Images/Twitter_logo.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/mails/Images/Web_logo.png` & `alphaz-0.7.7.1/alphaz/mails/Images/Web_logo.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/mails/Mail.png` & `alphaz-0.7.7.1/alphaz/mails/Mail.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/mails/Webmail.html` & `alphaz-0.7.7.1/alphaz/mails/Webmail.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/mails/debug.html` & `alphaz-0.7.7.1/alphaz/mails/debug.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/mails/mail.html` & `alphaz-0.7.7.1/alphaz/mails/mail.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/mails/password_reset.html` & `alphaz-0.7.7.1/alphaz/mails/password_reset.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/mails/stay_in_touch.html` & `alphaz-0.7.7.1/alphaz/mails/stay_in_touch.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/models/api/_answer.py` & `alphaz-0.7.7.1/alphaz/models/api/_answer.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/models/api/_colorations.py` & `alphaz-0.7.7.1/alphaz/models/api/_colorations.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/models/api/_parameter.py` & `alphaz-0.7.7.1/alphaz/models/api/_parameter.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from sqlalchemy.ext.declarative import DeclarativeMeta
 from sqlalchemy import inspect as inspect_sqlalchemy
 
 from flask import request
 from collections.abc import Callable
 
 from ..main import AlphaException
+from ..main._base import is_dataclass
+from ..main._enum import MappingMode
 
 from ...libs import date_lib, json_lib, py_lib
 
 from enum import Enum
 
 
 def dict_to_model(model, parameters):
@@ -97,15 +99,15 @@
         cacheable: bool = True,
         required: bool = False,
         ptype: type = str,
         private: bool = False,
         mode: ParameterMode = ParameterMode.NONE,
         override: bool = False,
         function: Callable = None,
-        automap: bool = False,
+        mapping_mode: MappingMode | str | None = None,
         map_none: bool = False,
         max_size: int | None = None,
         min_size: int | None = None,
         separators: list = [",", ";"],
     ):
         """[summary]
 
@@ -129,15 +131,15 @@
         self.ptype: type = ptype
         self.function: Callable = function
         self.type = str(ptype).replace("<class '", "").replace("'>", "")
         self.private = private
         self.mode = mode
         self.override = override
         self.is_value = False
-        self.automap = automap
+        self.mapping_mode = mapping_mode
         self.max_size = max_size
         self.min_size = min_size
         self.map_none = map_none
 
     @property
     def value(self):
         return self._value if self._value is not None else self.default
@@ -236,21 +238,23 @@
                 self._value = self.default
             elif is_empty_value:
                 self._value = (
                     dataDict[self.name] if self.name in dataDict else self.default
                 )
 
             sub_type = py_lib.get_subtype(self.ptype)
-            if dataclasses.is_dataclass(sub_type):
+            if is_dataclass(sub_type):
                 if self._value is not None:
                     values = re.findall(r"{[^{]*}", str(self._value))
                     self._value = self.default if len(values) == 0 else []
                     for val in values:
                         if hasattr(sub_type, "map_from_json"):
-                            val = sub_type.map_from_json(val, automap=self.automap)
+                            val = sub_type.map_from_json(
+                                val, mapping_mode=self.mapping_mode
+                            )
                         else:
                             P = json.loads(val)
                             val = sub_type(**P)
                         self._value.append(val)
                 else:
                     self._value = self.default
 
@@ -270,18 +274,18 @@
                 )
                 parameters = {
                     x: y
                     for x, y in parameters.items()
                     if hasattr(self.ptype, x) and (self.map_none or y is not None)
                 }  # TODO: enhance
             self._value = dict_to_model(self.ptype, parameters)
-        elif dataclasses.is_dataclass(self.ptype):
+        elif is_dataclass(self.ptype):
             if hasattr(self.ptype, "map_from_json"):
                 self._value = self.ptype.map_from_json(
-                    self._value, automap=self.automap
+                    self._value, mapping_mode=self.mapping_mode
                 )
             else:
                 P = json.loads(self._value)
                 self._value = self.ptype(**P)
 
         if self.ptype == dict:
             self._value = json_lib.load_json(self._value)
```

### Comparing `alphaz-0.7.7/alphaz/models/api/_reloader.py` & `alphaz-0.7.7.1/alphaz/models/api/_reloader.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/models/api/_reloaders.py` & `alphaz-0.7.7.1/alphaz/models/api/_reloaders.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/models/api/_requests.py` & `alphaz-0.7.7.1/alphaz/models/api/_requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,19 @@
             data = AlphaRequest.get_json()
             request_uuid = (
                 request.full_path
                 + "&"
                 + "&".join("%s=%s" % (x, y) for x, y in data.items())
             )
         except:
-            raw_data = request.data
+            try:
+                raw_data = request.data
+            except:
+                return None
+
             if isinstance(raw_data, bytes):
                 if b"\x01\x8d" in raw_data:
                     raw_data = raw_data.replace(b"\x01\x8d", b"\n")
                 raw_data = raw_data.decode()
             request_uuid = request.full_path + str(raw_data)  # TODO: update
         return request_uuid
```

### Comparing `alphaz-0.7.7/alphaz/models/api/_route.py` & `alphaz-0.7.7.1/alphaz/models/api/_route.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/models/api/_structures.py` & `alphaz-0.7.7.1/alphaz/models/api/_structures.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # MODULES
-import os, jwt, itertools, sys, importlib, warnings, traceback, time
+import os, jwt, itertools, sys, importlib, warnings, traceback, time, socket
 
 # WSGI
 from gevent.pywsgi import WSGIServer
 
 # WERKZEUG
 from werkzeug.debug import DebuggedApplication
 
@@ -512,15 +512,19 @@
         if admin_parameter and admin_password is not None:
             if secure_lib.check_cry_operation_code(admin_parameter, admin_password):
                 return True
 
         try:
             ip = request.remote_addr
         except:
-            ip = None
+            ## getting the hostname by socket.gethostname() method
+            hostname = socket.gethostname()
+            ## getting the IP address using socket.gethostbyname() method
+            ip_address = socket.gethostbyname(hostname)
+            ip = ip_address
         admins_ips = self.conf.get("admins/ips")
         if admins_ips and (ip in admins_ips or f"::ffff:{ip}" in admins_ips):
             return True
 
         if check_logged_user:
             user = self.get_logged_user()
             if user is not None:
```

### Comparing `alphaz-0.7.7/alphaz/models/api/_utils.py` & `alphaz-0.7.7.1/alphaz/models/api/_utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/models/config/_config.py` & `alphaz-0.7.7.1/alphaz/models/config/_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/models/config/_utils.py` & `alphaz-0.7.7.1/alphaz/models/config/_utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/models/database/main_definitions.py` & `alphaz-0.7.7.1/alphaz/models/database/main_definitions.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/models/database/models.py` & `alphaz-0.7.7.1/alphaz/models/database/models.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/models/database/operators.py` & `alphaz-0.7.7.1/alphaz/models/database/operators.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/models/database/requests.py` & `alphaz-0.7.7.1/alphaz/models/database/requests.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/models/database/row.py` & `alphaz-0.7.7.1/alphaz/models/database/row.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/models/database/structure.py` & `alphaz-0.7.7.1/alphaz/models/database/structure.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # MODULES
+import copy
 import enum, re, itertools, datetime
 import numpy as np
 from collections.abc import Iterable
 from dataclasses import fields
 from time import sleep
 import logging
 
@@ -415,15 +416,15 @@
         self.log: AlphaLogger | None = log
 
         self.error = None
 
         self.query_str = None
         self.full_count = None
         self.pagination_mode = config.get("pagination_mode", "raw")
-        self.mapping_mode = config.get("mapping_mode", MappingMode.AUTO1.value)
+        self.mapping_mode = config.get("mapping_mode", None)
 
         self.models = []
 
     def get_session(self, bind: str | None = None):
         return self.db.session if bind is None else self.get_engine(bind=bind)
 
     def get_meta(self, bind: str | None = None):
@@ -838,19 +839,22 @@
     def commit(self, close=False, session=None) -> bool:
         if self.autocommit:
             return True
         if session is None:
             session = self.session
         valid = True
         try:
-            session.commit()
+            if not session.is_active:
+                session.commit()
         except Exception as ex:
             self.log.error(ex=ex)
             session.rollback()
             valid = False
+            # session.close()
+            # session.begin()
             raise ex
 
         finally:
             if close:
                 session.close()
         return valid
 
@@ -868,31 +872,34 @@
             raise ex
         finally:
             if close:
                 session.close()
 
         return valid
 
-    def delete_obj(self, obj, commit: bool = True, close: bool = False) -> bool:
-        session = self.object_session(obj)
+    def delete_obj(
+        self, obj, commit: bool = True, close: bool = False, session=None
+    ) -> bool:
+        session = self.object_session(obj) if session is None else session
         session.delete(obj)
         if commit:
             return self.commit(close=close, session=session)
         return True
 
     def delete(self, model, filters, commit: bool = True, close: bool = False) -> bool:
         if filters is None or len(filters) == 0:
             raise AlphaException("Cannot delete without specifying filters")
-        objs = self.select(model, filters=filters, json=False)
+        objs = model.query.filter(*filters).all()
         if len(objs) == 0:
             return False
-        for obj in objs:
-            self.delete_obj(obj, commit=False)
-        if commit:
-            return self.commit(close=close)
+        with self.session.begin():
+            for obj in objs:
+                self.session.delete(obj)
+            if commit:
+                self.session.commit()
         return True
 
     def get_tables_names(self, bind: str | None = None):
         return list(
             set(
                 [
                     x.__tablename__
@@ -1029,15 +1036,20 @@
         relationship=True,
         disabled_relationships: list[str] = None,
         page: int | None = None,
         per_page: int | None = None,
         offset: int | None = None,
         dataclass=None,
         default=None,
+        # new_session: bool = True,
     ):
+        # Vérifiez si une transaction est déjà en cours
+        # if not self.session.is_active and new_session:
+        # Aucune transaction n'est en cours, vous pouvez ouvrir une nouvelle transaction
+        #    self.session.begin()
         query = apply_jonctions(model, order_by)
 
         # model_name = inspect.getmro(model)[0].__name__
         # if self.db_type == "mysql": self.test(close=False)
         renames_columns = None
         if type(columns) == dict:
             columns = list(columns.keys())
@@ -1117,26 +1129,26 @@
 
     def select_query(
         self,
         query,
         model=None,
         first: bool = False,
         json: bool = False,
-        unique: InstrumentedAttribute = None,
+        unique: InstrumentedAttribute | None = None,
         count: bool = False,
         limit: int | None = None,
-        filters: list = None,
-        optional_filters: list = None,
+        filters: list | None = None,
+        optional_filters: list | None = None,
         order_by=None,
         order_by_direction=None,
         close=False,
         flush=False,
         schema=None,
         relationship=True,
-        disabled_relationships: list[str] = None,
+        disabled_relationships: list[str] | None = None,
         page: int | None = None,
         per_page: int | None = None,
         offset: int | None = None,
         dataclass=None,
         default=None,
         columns: dict | None = None,
         distinct=None,
@@ -1328,38 +1340,34 @@
                     per_page=per_page,
                     full_count=self.full_count,
                     first=first,
                     pagination_mode=self.pagination_mode,
                 )
 
             is_alpha_dataclass = hasattr(dataclass, "auto_map_from_dict")
-            mapping_mode = (
-                getattr(dataclass, "__map__").lower()
-                if hasattr(dataclass, "__map__")
-                else self.mapping_mode.lower()
-            )
-            field_names = [field.name for field in fields(dataclass)]
 
-            if not first:
-                if is_alpha_dataclass:
+            field_names = [field.name for field in fields(dataclass)]
+            if is_alpha_dataclass:
+                mapping_mode = dataclass._map if dataclass.map is not None else self.mapping_mode
+                if first:
+                    results_json = dataclass.map(results_json, mapping_mode)
+                else:
                     results_json = [
                         dataclass.map(r, mapping_mode) for r in results_json
                     ]
+            else:
+                if first:
+                    results_json = dataclass(
+                        **{x: y for x, y in results_json.items() if x in field_names}
+                    )
                 else:
                     results_json = [
                         dataclass(**{x: y for x, y in k.items() if x in field_names})
                         for k in results_json
                     ]
-            else:
-                if is_alpha_dataclass:
-                    results_json = dataclass.map(results_json, mapping_mode)
-                else:
-                    results_json = dataclass(
-                        **{x: y for x, y in results_json.items() if x in field_names}
-                    )
         return default_return(
             results_json,
             default=default,
             columns=columns,
             page=page,
             per_page=per_page,
             full_count=self.full_count,
@@ -1507,15 +1515,15 @@
                 if hasattr(x, "lower")
                 else str(x).split(".")[1]
                 for x in headers
             ]
 
             columns_names, model_names = {}, []
 
-            for key, el in table.__dict__.items():
+            for key, el in table.__dict__.copy().items():
                 if (
                     hasattr(el, "key")
                     and hasattr(el, "expression")
                     and hasattr(el.expression, "key")
                 ):
                     columns_names[el.expression.key] = key
 
@@ -1550,14 +1558,15 @@
 
     def init_all(
         self,
         binds: list[str] = None,
         tables: list[AlphaTable] = None,
         drop: bool = False,
         create: bool = False,
+        truncate: bool = False,
         sqlite: bool = True,
         log=None,
     ):
         """if sqlite:
         binds = [
             x.upper()
             for x, y in self.db_cnx.items()
@@ -1597,23 +1606,30 @@
                     meta = self.get_meta(bind=bind)
                 except:
                     log.error(f"Cannot find {bind=}")
                     continue
 
             table_names = [x.__tablename__ for x in tables_models]
             tables_names_str = ";".join(table_names)
+
             if drop:
                 if log is not None:
                     log.info(f"Drop tables from {bind=}: {tables_names_str}")
                 meta.drop_all(tables=tables)
+
             if create:
                 if log is not None:
                     log.info(f"Create tables from {bind=}: {tables_names_str}")
                 meta.create_all(tables=tables)
 
+            # Vide les tables si le paramètre 'truncate' est True
+            if truncate:
+                for table_model in tables_models:
+                    self.truncate(table_model)
+
     def create_table(self, table: str, bind: str | None = None, drop: bool = False):
         table_object = self.get_table_model(table, bind)
         if drop:
             try:
                 table_object.__table__.drop(self.engine)
             except:
                 pass
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `alphaz-0.7.7/alphaz/models/database/tests.py` & `alphaz-0.7.7.1/alphaz/models/database/tests.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/models/database/users_definitions.py` & `alphaz-0.7.7.1/alphaz/models/database/users_definitions.py`

 * *Files 16% similar despite different names*

```diff
@@ -51,18 +51,24 @@
 
 
 class UserRole(db.Model, AlphaTableUpdateDate):
     __bind_key__ = BIND
     __tablename__ = "user_role"
 
     user_id = AlphaColumn(
-        Integer, ForeignKey("user.id"), nullable=False, primary_key=True
+        Integer,
+        ForeignKey("user.id", ondelete="CASCADE"),
+        nullable=False,
+        primary_key=True,
     )
     role_name = AlphaColumn(
-        String(200), ForeignKey("role.name"), nullable=False, primary_key=True
+        String(200),
+        ForeignKey("role.name", ondelete="CASCADE"),
+        nullable=False,
+        primary_key=True,
     )
     activated = AlphaColumn(Boolean, default=True)
 
 
 class User(db.Model, AlphaTable):
     __bind_key__ = BIND
     __tablename__ = "user"
@@ -85,29 +91,29 @@
     last_activity = AlphaColumn(
         DateTime, default=datetime.datetime.now, onupdate=datetime.datetime.now
     )
 
     roles = relationship(
         "Role",
         secondary="user_role",
-        cascade="all,delete",
+        cascade="all, delete",
     )
 
 
 class Role(db.Model, AlphaTableUpdateDate):
     __bind_key__ = BIND
     __tablename__ = "role"
 
     name = AlphaColumn(String(200), primary_key=True)
     description = AlphaColumn(String(1000))
     activated = AlphaColumn(Boolean, default=True)
 
     id_app = AlphaColumn(
         Integer,
-        ForeignKey("application.id"),
+        ForeignKey("application.id", ondelete="CASCADE"),
     )
 
     application = relationship(
         "Application",
         backref=backref(__tablename__ + "s", lazy=True, cascade="all, delete-orphan"),
     )
 
@@ -119,41 +125,50 @@
 
 
 class RolePermission(db.Model, AlphaTableUpdateDate):
     __bind_key__ = BIND
     __tablename__ = "role_permission"
 
     role_name = AlphaColumn(
-        String(200), ForeignKey("role.name"), nullable=False, primary_key=True
+        String(200),
+        ForeignKey("role.name", ondelete="CASCADE"),
+        nullable=False,
+        primary_key=True,
     )
     permission_key = AlphaColumn(
-        String(200), ForeignKey("permission.key"), nullable=False, primary_key=True
+        String(200),
+        ForeignKey("permission.key", ondelete="CASCADE"),
+        nullable=False,
+        primary_key=True,
     )
     activated = AlphaColumn(Boolean, default=True)
 
 
 class Permission(db.Model, AlphaTableUpdateDate):
     __bind_key__ = BIND
     __tablename__ = "permission"
 
     key = AlphaColumn(String(200), primary_key=True)
     description = AlphaColumn(String(1000))
     activated = AlphaColumn(Boolean, default=True)
 
     roles = relationship(
-        "Role", secondary="role_permission"
+        "Role", secondary="role_permission", cascade="all,delete"
     )  # TODO: remove overlaps="permissions" and fix the warning
 
 
 class Notification(db.Model, AlphaTableUpdateDate):
     __bind_key__ = BIND
     __tablename__ = "notification"
 
     user_id = AlphaColumn(
-        Integer, ForeignKey("user.id"), nullable=False, primary_key=True
+        Integer,
+        ForeignKey("user.id", ondelete="CASCADE"),
+        nullable=False,
+        primary_key=True,
     )
     user = relationship(
         "User",
         backref=backref(__tablename__ + "s", lazy=True, cascade="all, delete-orphan"),
     )
 
     user_from = AlphaColumn(Integer, nullable=False, primary_key=True)
```

### Comparing `alphaz-0.7.7/alphaz/models/database/utils.py` & `alphaz-0.7.7.1/alphaz/models/database/utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/models/database/views.py` & `alphaz-0.7.7.1/alphaz/models/database/views.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/models/excel.py` & `alphaz-0.7.7.1/alphaz/models/excel.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/models/ftp.py` & `alphaz-0.7.7.1/alphaz/models/ftp.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/models/json/_converters.py` & `alphaz-0.7.7.1/alphaz/models/json/_converters.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/models/logger/_colorations.py` & `alphaz-0.7.7.1/alphaz/models/logger/_colorations.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/models/logger/_logger.py` & `alphaz-0.7.7.1/alphaz/models/logger/_logger.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/models/logger/_utils.py` & `alphaz-0.7.7.1/alphaz/models/logger/_utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/models/logs/main.log` & `alphaz-0.7.7.1/alphaz/models/logs/main.log`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/models/main/_base.py` & `alphaz-0.7.7.1/alphaz/models/main/_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,25 @@
+# MODULS
 import dataclasses, traceback
 import enum, inspect, operator, re, copy
-from dataclasses import dataclass, field, is_dataclass, _MISSING_TYPE, asdict
+
+from dataclasses import dataclass, field, _MISSING_TYPE, asdict
 from collections import OrderedDict
 
-from typing import Iterable
+from typing import Iterable, Union
+from types import UnionType
 from typing_extensions import Annotated
 
+# LOGGER
 from ..logger import AlphaLogger
+
+# LIBS
 from ...libs import py_lib, json_lib, string_lib
 
+# LOCALS
 from ._enum import MappingMode
 from ._exception import AlphaException
 
 FORCE_AUTO_MAP = True
 
 
 class AlphaMappingAttribute:
@@ -40,43 +47,75 @@
     min_size = min(max_keys, key=len)
     best_matchs = [x for x in max_keys if len(x) == len(min_size)]
     if len(best_matchs) > 1:
         print(f"ERROR: multiple match {best_matchs}")
     return best_matchs[0]
 
 
-class AlphaClass:
-    def __init__(self, *args, log: AlphaLogger | None = None, **kwargs):
-        self.init_args: dict = {"args": args, "kwargs": kwargs}
-        self.children: list = []
+def is_auto_map(dataclass_type, mapping_mode: MappingMode | str | None = None) -> bool:
+    if not hasattr(dataclass_type, "auto_map_from_dict"):
+        return False
+    if dataclass_type.get_mapping_mode() is not None and mapping_mode is None:
+        mapping_mode = dataclass_type.get_mapping_mode()
+    elif mapping_mode is None:
+        mapping_mode = MappingMode.STRICT
+
+    mapping_mode_str = str(mapping_mode)
+    if type(mapping_mode) != str:
+        mapping_mode_str: str = str(mapping_mode.value)
+    mapping_mode_str = mapping_mode_str.lower()
+
+    match mapping_mode_str:
+        case MappingMode.AUTO.value:
+            return True
+    return False
+
 
-        self.log = log
+class AlphaClass:
+    _map: MappingMode | None = None
 
-        self.__piles: dict[str, list[str]] = {}
+    def __init__(self, *args, log: AlphaLogger | None = None, **kwargs):
+        self._init_args: dict = {"args": args, "kwargs": kwargs}
+        self._children: list = []
+        self._logger = log
+        self._piles: dict[str, list[str]] = {}
 
     def make_child(self, child_cls, *args, **kwargs):
         if args is None:
-            args = self.init_args["args"]
+            args = self._init_args["args"]
         if kwargs is None:
-            kwargs = self.init_args["kwargs"]
+            kwargs = self._init_args["kwargs"]
         child = child_cls(self, *args, **kwargs)
-        self.children.append(child)
+        self._children.append(child)
         return child
 
+    def get_children(self):
+        return self._children
+
+    @classmethod
+    def get_mapping_mode(class_):
+        return class_._map
+
     def get_attributes(self):
         return py_lib.get_attributes(self)
 
     def to_json(
         self,
         columns: list | None = None,
         rejected: list | None = None,
         not_none: bool = False,
         not_empty: bool = False,
     ):
-        d_rejected = ["_AlphaClass__piles", "init_args", "children", "log"]
+        d_rejected = [
+            "_map",
+            "_piles",
+            "_init_args",
+            "_children",
+            "_log",
+        ]
         if rejected is not None:
             d_rejected.extend(rejected)
         dict_output = {}
         for x, y in self.get_attributes().items():
             if columns is not None and x not in columns:
                 continue
             if x in d_rejected:
@@ -88,29 +127,29 @@
                 continue
             dict_output[x] = json_lib.jsonify_data(
                 y
             )  # if not hasattr(y, "to_json") or inspect.isclass(y) else y.to_json()
         return dict_output
 
     def __log(self, stack, message, ex=None, out: bool = False):
-        if not stack in self.__piles:
-            self.__piles[stack] = []
-        pile = self.__piles[stack]
+        if not stack in self._piles:
+            self._piles[stack] = []
+        pile = self._piles[stack]
 
-        if self.log is not None:
-            method = getattr(self.log, stack)
+        if self._logger is not None:
+            method = getattr(self._logger, stack)
             if len(pile) != 0:
                 for deb in pile:
                     method(deb, ex=ex)
                 stack = []
             method(message, ex=ex)
         else:
             pile.append(message)
             if out:
-                for stack, msg in self.__piles.items():
+                for stack, msg in self._piles.items():
                     print(f"{stack}: {msg}")
                 if ex:
                     print(ex)
 
     def debug(self, message, ex=None):
         self.__log(inspect.stack()[0][3], message=message, ex=ex)
 
@@ -298,14 +337,15 @@
         for x, y in self.dataclass_type.__dataclass_fields__.items():
             if py_lib.is_subtype(y.type, list) or py_lib.is_subtype(y.type, list):
                 self.list_fields[x] = y
             elif is_dataclass(y.type):
                 self.dict_fields[x] = y
             else:
                 self.object_fields[x] = y
+        pass
 
     def identify(self, dict_values: dict[str, object]):
         dict_elements = {
             x: y for x, y in dict_values.items() if type(y) == dict or y is None
         }
         list_elements = {
             x: y for x, y in dict_values.items() if type(y) == list or y is None
@@ -397,68 +437,85 @@
         for field_key, score_dict in self.matchs_object_fields.items():
             best_match = get_score_dict_best_match(score_dict)
             if field_key in self.object_fields:
                 self.identified_object_fields[best_match] = self.object_fields[
                     field_key
                 ]
 
-    def __map_flat(self, dict_values: dict[str, object]):
+    def __map_flat(
+        self,
+        dict_values: dict[str, object],
+        mapping_mode: MappingMode | str | None = None,
+    ):
         if not self.is_identified:
             self.__identify_flat(dict_values)
 
         field_values = {}
         for (
             key,
             fd,
         ) in self.identified_object_fields.items():
-            field_values[fd.name] = convert_value(dict_values[key], fd.type)
+            field_type = py_lib.get_first_non_none_type(fd.type)
+            field_values[fd.name] = convert_value(dict_values[key], field_type)
 
         for fd in self.dict_fields.values():
-            field_values[fd.name] = fd.type.auto_map_from_dict(
+            field_type = py_lib.get_first_non_none_type(fd.type)
+            field_values[fd.name] = field_type.map_from_dict(
                 dict_values={
                     x: y for x, y in dict_values.items() if not x in field_values
-                }
+                },
+                mapping_mode=mapping_mode,
             )
 
         return field_values
 
-    def map(self, dict_values: dict[str, object]):
+    def map(
+        self,
+        dict_values: dict[str, object],
+        mapping_mode: MappingMode | str | None = None,
+    ):
         if self.flat:
             return self.__map_flat(dict_values)
 
         if not self.is_identified:
             self.identify(dict_values)
 
         field_values = {}
         for (
             key,
             fd,
         ) in self.identified_object_fields.items():
-            field_values[fd.name] = convert_value(dict_values[key], fd.type)
+            field_type = py_lib.get_first_non_none_type(fd.type)
+            field_values[fd.name] = convert_value(dict_values[key], field_type)
 
         for (
             key,
             fd,
         ) in self.identified_dict_fields.items():
+            field_type = py_lib.get_first_non_none_type(fd.type)
             field_values[fd.name] = (
-                fd.type.auto_map_from_dict(dict_values=dict_values[key])
+                field_type.map_from_dict(
+                    dict_values=dict_values[key], mapping_mode=mapping_mode
+                )
                 if dict_values[key] is not None
                 else None
             )
 
         for (
             key,
             fd,
         ) in self.identified_list_fields.items():
             sub_type = fd.type.__args__[0]
             if hasattr(sub_type, "auto_map_from_dict"):
                 field_values[fd.name] = (
                     [
                         (
-                            sub_type.auto_map_from_dict(dict_values=f)
+                            sub_type.auto_map_from_dict(
+                                dict_values=f, mapping_mode=mapping_mode
+                            )
                             if f is not None
                             else None
                         )
                         for f in dict_values[key]
                     ]
                     if dict_values[key] is not None
                     else []
@@ -474,45 +531,48 @@
                         ]
                         if dict_values[key] is not None
                         else []
                     )
         return field_values
 
 
-def convert_value_from_field(field_type, value, automap: bool = False):
+def convert_value_from_field(
+    field_type, value, mapping_mode: MappingMode | str | None = None
+):
+    field_type = py_lib.get_first_non_none_type(field_type)
     if value is None:
         return None
     if is_dataclass(field_type):
         return field_type.map_from_dict(
-            asdict(value) if is_dataclass(value) else value, automap=automap
+            asdict(value) if is_dataclass(value) else value, mapping_mode=mapping_mode
         )
     elif isinstance(value, list) and all(isinstance(item, dict) for item in value):
         return [convert_value_from_field(field_type, item) for item in value]
     else:
         try:
             return field_type(value)
         except:
             return value
 
 
 class AlphaDataclass(AlphaClass):
-    def get_fields_dict(self, keys: list[str] = None) -> dict:
+    def get_fields_dict(self, keys: list[str] | None = None) -> dict:
         dct = {}
         # dct['_tname'] = self.__class__.__name__
 
-        for f in dataclasses.fields(self):
-            f_type = f.type
-            value = getattr(self, f.name)
+        for fd in dataclasses.fields(self):
+            # field_type = py_lib.get_first_non_none_type(fd.type)
+            value = getattr(self, fd.name)
             if hasattr(value, "get_fields_dict"):
                 value = value.get_fields_dict()
             else:
                 value = value
-            if keys is not None and f.name not in keys:
+            if keys is not None and fd.name not in keys:
                 continue
-            dct[f.name] = value
+            dct[fd.name] = value
 
         return dct
 
     def compare(
         self, other, attrs_list: list[str], attrs_eq: dict[str, str] = None
     ) -> bool:
         if not isinstance(other, self.__class__) and not issubclass(
@@ -686,15 +746,15 @@
         dataclass_type,
         dict_values: dict[str, object],
         associations: dict[str, str] = {},
         no_match: list[str] = [],
         flat: bool = False,
     ):
         global DATACLASS_AUTO_MAP_MATCHS, FORCE_AUTO_MAP
-        if dict_values is None:
+        if dict_values is None or len(dict_values) == 0:
             return dataclass_type()
 
         dataclass_name = str(dataclass_type).split(".")[-1].replace("'>", "")
         uuid = f"{dataclass_name}({','.join(list(dict_values.keys()))})"
 
         # FIELDS
         if not uuid in DATACLASS_AUTO_MAP_MATCHS or FORCE_AUTO_MAP:
@@ -714,86 +774,121 @@
         is_required_fields = set(required_fields).intersection(
             fields_values.keys()
         ) == set(required_fields)
         if not is_required_fields:
             return None
         try:
             if hasattr(dataclass_type, "map_from_dict"):
-                instance = dataclass_type.map_from_dict(fields_values)
+                instance = dataclass_type.map_from_dict(
+                    fields_values, mapping_mode=MappingMode.STRICT
+                )
             else:
                 fields_values = {
                     x: y
                     for x, y in fields_values.items()
                     if x in dataclass_type.get_fields_names(True)
                 }
                 instance = dataclass_type(**fields_values)
         except Exception as ex:
             print(f"Error mapping {dataclass_type}")
             tb = traceback.format_exc()
             raise ex
         return instance
 
     @classmethod
-    def map_from_json(dataclass_type, json_values: str, automap: bool = False):
-        dict_value = (
+    def map_from_json(
+        dataclass_type, json_values: str, mapping_mode: MappingMode | str | None = None
+    ):
+        dict_values = (
             json_lib.load_json(json_values)
             if type(json_values) != dict
             else json_values
         )
         try:
-            obj = dataclass_type.map_from_dict(dict_value, automap=automap)
+            obj = dataclass_type.map_from_dict(dict_values, mapping_mode=mapping_mode)
         except Exception as ex:
             print(f"Failed to map {dataclass_type} with: {json_values}")
             print(ex)
             obj = None
         return obj
 
     @classmethod
     def map_from_dict(
-        dataclass_type, dict_value: dict[str, object] | dict[str, str], automap: bool = False
+        dataclass_type,
+        dict_values: dict[str, object] | dict[str, str],
+        mapping_mode: MappingMode | str | None = None,
     ):
-        if automap and hasattr(dataclass_type, "auto_map_from_dict"):
-            return dataclass_type.auto_map_from_dict(dict_values=dict_value)
+        if is_auto_map(dataclass_type, mapping_mode=mapping_mode):
+            return dataclass_type.auto_map_from_dict(dict_values=dict_values)
 
         if (
-            not py_lib.is_subtype(type(dict_value), dict)
-            and not py_lib.is_subtype(type(dict_value), dict)
-            and not type(dict_value) == dict
+            not py_lib.is_subtype(type(dict_values), dict)
+            and not py_lib.is_subtype(type(dict_values), dict)
+            and not type(dict_values) == dict
         ):
             return None
-        if dict_value is None:
+        if dict_values is None:
             return None
 
         field_values = {}
-        for key, value in dict_value.items():
+        for key, value in dict_values.items():
             if key not in dataclass_type.__dataclass_fields__:
                 continue
 
             field = dataclass_type.__dataclass_fields__[key]
-            field_type = field.type
+            field_type = py_lib.get_first_non_none_type(field.type)
 
             if not field.init:
                 continue
 
             if py_lib.is_subtype(field_type, list) or py_lib.is_subtype(
                 field_type, list
             ):
                 field_values[key] = []
                 if value is not None:
                     field_values[key] = [
                         convert_value_from_field(
-                            py_lib.get_subtype(field_type), v, automap=automap
+                            py_lib.get_subtype(field_type), v, mapping_mode=mapping_mode
                         )
                         for v in value
                     ]
             else:
                 field_values[key] = convert_value_from_field(
-                    field_type, value, automap=automap
+                    field_type, value, mapping_mode=mapping_mode
                 )
-        return dataclass_type(**field_values)
+
+        try:
+            dc = dataclass_type(**field_values)
+        except Exception as ex:
+            dc = None
+            raise ex
+        return dc
 
     @classmethod
-    def map(dataclass_type, json_values: str, mapping_mode: MappingMode):
-        if mapping_mode == MappingMode.AUTO1.value:
-            return dataclass_type.auto_map_from_dict(json_values)
-        else:
-            return dataclass_type.map_from_dict(json_values)
+    def map(
+        dataclass_type, json_values: dict, mapping_mode: MappingMode | str | None = None
+    ):
+        if dataclass_type.get_mapping_mode() is not None and mapping_mode is None:
+            mapping_mode = dataclass_type.get_mapping_mode()
+        elif mapping_mode is None:
+            mapping_mode = MappingMode.STRICT
+
+        mapping_mode_str = str(mapping_mode)
+        if type(mapping_mode) != str:
+            mapping_mode_str: str = str(mapping_mode.value)
+        mapping_mode_str = mapping_mode_str.lower()
+
+        match mapping_mode_str:
+            case MappingMode.AUTO.value:
+                return dataclass_type.auto_map_from_dict(json_values)
+
+        return dataclass_type.map_from_dict(json_values)
+
+
+def is_dataclass(o):
+    if dataclasses.is_dataclass(o):
+        return True
+    if isinstance(o, AlphaDataclass) or (
+        isinstance(o, type) and issubclass(o, AlphaDataclass)
+    ):
+        return True
+    return py_lib.is_subtype(o, AlphaDataclass)
```

### Comparing `alphaz-0.7.7/alphaz/models/main/_core/_core.py` & `alphaz-0.7.7.1/alphaz/models/main/_core/_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -263,15 +263,15 @@
                     name = cf_db["sid"]
                     c = f"{host}:{port}/{name}"
                 elif "service_name" in cf_db:
                     name = cf_db["service_name"]
                     c = f"(DESCRIPTION = (LOAD_BALANCE=on) (FAILOVER=ON) (ADDRESS = (PROTOCOL = TCP)(HOST = {host})(PORT = {port})) (CONNECT_DATA = (SERVER = DEDICATED) (SERVICE_NAME = {name})))"
                 cnx_str = f"oracle://{user}:{password}@{c}"
             elif db_type == "sqlite":
-                cnx_str = "sqlite:///" + cf_db["path"]
+                cnx_str = "sqlite:///" + cf_db["path"] + "?timeout=5"
 
             if "ssl" in cf_db and cf_db["ssl"] is not None:
                 if not all(
                     elem in cf_db["ssl"].keys()
                     for elem in ["ssl_ca", "ssl_cert", "ssl_key"]
                 ):
                     raise AlphaException(
```

### Comparing `alphaz-0.7.7/alphaz/models/main/_exception.py` & `alphaz-0.7.7.1/alphaz/models/main/_exception.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/models/main/_request.py` & `alphaz-0.7.7.1/alphaz/models/main/_request.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/models/main/_singleton.py` & `alphaz-0.7.7.1/alphaz/models/main/_singleton.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/models/request.py` & `alphaz-0.7.7.1/alphaz/models/request.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/models/tests/_category.py` & `alphaz-0.7.7.1/alphaz/models/tests/_category.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/models/tests/_group.py` & `alphaz-0.7.7.1/alphaz/models/tests/_group.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/models/tests/_method.py` & `alphaz-0.7.7.1/alphaz/models/tests/_method.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/models/tests/_save.py` & `alphaz-0.7.7.1/alphaz/models/tests/_save.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/models/tests/_test.py` & `alphaz-0.7.7.1/alphaz/models/tests/_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,17 +181,19 @@
         status = all(key_in.values())
         if not status:
             LOG.info(
                 f"{self.current_test_name} {msg} - Assert: missing model keys: {','.join([x for x, y in key_in.items() if not y])}"
             )
         return self._assert(status, conditions)
 
-    def assert_is_true(self, a, conditions: list[bool] = [], msg: str = "") -> bool:
+    def assert_is_true(
+        self, a, conditions: list[bool] = [], msg: str = "", no_log: bool = False
+    ) -> bool:
         status = a
-        if not status:
+        if not status and not no_log:
             LOG.info(f"{self.current_test_name} {msg} - Assert: value {a} is not True")
         return self._assert(status, conditions)
 
     def assert_is_false(self, a, conditions: list[bool] = [], msg: str = "") -> bool:
         status = a
         if status:
             LOG.info(f"{self.current_test_name} {msg} - Assert: value {a} is not False")
```

### Comparing `alphaz-0.7.7/alphaz/models/tests/_wrappers.py` & `alphaz-0.7.7.1/alphaz/models/tests/_wrappers.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/models/user.py` & `alphaz-0.7.7.1/alphaz/models/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 
 @dataclass
 class AlphaRole(AlphaDataclass):
     name: str
     activated: bool
     id_app: int
-    app: AlphaApplication
+    app: AlphaApplication | None = None
     description: str | None = None
 
     permissions: list[AlphaPermission] = field(default_factory=lambda: [])
 
 
 @dataclass
 class AlphaUserRole(AlphaDataclass):
```

### Comparing `alphaz-0.7.7/alphaz/models/watcher.py` & `alphaz-0.7.7.1/alphaz/models/watcher.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/pocs/main.py` & `alphaz-0.7.7.1/alphaz/pocs/main.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/run.py` & `alphaz-0.7.7.1/alphaz/run.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/src/alpha.png` & `alphaz-0.7.7.1/alphaz/src/alpha.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/src/configs/loggers.json` & `alphaz-0.7.7.1/alphaz/src/configs/loggers.json`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/stitch/Core.py` & `alphaz-0.7.7.1/alphaz/stitch/Core.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/stitch/stitch.py` & `alphaz-0.7.7.1/alphaz/stitch/stitch.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/stitch/web-drivers/chromedriver.exe` & `alphaz-0.7.7.1/alphaz/stitch/web-drivers/chromedriver.exe`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/stitch/web-drivers/geckodriver` & `alphaz-0.7.7.1/alphaz/stitch/web-drivers/geckodriver`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/templates/assets/css/home.css` & `alphaz-0.7.7.1/alphaz/templates/assets/css/home.css`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/templates/assets/css/logs.css` & `alphaz-0.7.7.1/alphaz/templates/assets/css/logs.css`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/templates/assets/images/icons/alpha.png` & `alphaz-0.7.7.1/alphaz/templates/assets/images/icons/alpha.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/templates/assets/images/icons/start-icon.png` & `alphaz-0.7.7.1/alphaz/templates/assets/images/icons/start-icon.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/templates/assets/images/icons/wsalpha.png` & `alphaz-0.7.7.1/alphaz/templates/assets/images/icons/wsalpha.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/templates/assets/images/loading.gif` & `alphaz-0.7.7.1/alphaz/templates/assets/images/loading.gif`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/templates/assets/js/libs/ansi_up.js` & `alphaz-0.7.7.1/alphaz/templates/assets/js/libs/ansi_up.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/templates/assets/js/libs/jquery.min.js` & `alphaz-0.7.7.1/alphaz/templates/assets/js/libs/jquery.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/templates/assets/js/logs.js` & `alphaz-0.7.7.1/alphaz/templates/assets/js/logs.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/templates/home.html` & `alphaz-0.7.7.1/alphaz/templates/home.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/templates/logs.html` & `alphaz-0.7.7.1/alphaz/templates/logs.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/test.py` & `alphaz-0.7.7.1/alphaz/test.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/tests/api.py` & `alphaz-0.7.7.1/alphaz/tests/api.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/tests/configurations.py` & `alphaz-0.7.7.1/alphaz/tests/configurations.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/tests/database.py` & `alphaz-0.7.7.1/alphaz/tests/database.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/tests/utils.py` & `alphaz-0.7.7.1/alphaz/tests/utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/utils/api.py` & `alphaz-0.7.7.1/alphaz/utils/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 from core import core
 
 api = core.api
 API = core.api
 DB = core.db
 LOG = core.get_logger("api")
 
+ROUTES_DISABLED = core.config.get("api/routes_disabled", [])
+
 ROUTES = {}
 
 # Specify the debug panels you want
 # api.config['DEBUG_TB_PANELS'] = [ 'flask_debugtoolbar.panels.versions.VersionDebugPanel', 'flask_debugtoolbar.panels.timer.TimerDebugPanel', 'flask_debugtoolbar.panels.headers.HeaderDebugPanel', 'flask_debugtoolbar.panels.request_vars.RequestVarsDebugPanel', 'flask_debugtoolbar.panels.template.TemplateDebugPanel', 'flask_debugtoolbar.panels.sqlalchemy.SQLAlchemyDebugPanel', 'flask_debugtoolbar.panels.logger.LoggingPanel', 'flask_debugtoolbar.panels.profiler.ProfilerDebugPanel', 'flask_debugtoolbar_lineprofilerpanel.panels.LineProfilerPanel' ]
 # toolbar = flask_debugtoolbar.DebugToolbarExtension(api)
 
 ADMIN_USER_ID_PRIVATE = Parameter(
@@ -119,14 +121,16 @@
     mode: str | None = None,
     route_log: bool = True,
     access_strings: list[str] | list[Enum] = [],
     access_error_message: str | None = None,
     pagination: int | None = None,
 ):
     path = "/" + path if path[0] != "/" else path
+    if path in ROUTES_DISABLED:
+        return lambda x : x
 
     parameters = _process_parameters(path, parameters, pagination=pagination)
 
     def api_in(func):
         api.add_url_rule(path, methods=methods, view_func=func, endpoint=func.__name__)
 
         @api.endpoint(func.__name__)
```

### Comparing `alphaz-0.7.7/alphaz/utils/apm/ora.py` & `alphaz-0.7.7.1/alphaz/utils/apm/ora.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/utils/configuration.py` & `alphaz-0.7.7.1/alphaz/utils/configuration.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/utils/database/init.py` & `alphaz-0.7.7.1/alphaz/utils/database/init.py`

 * *Files 10% similar despite different names*

```diff
@@ -51,39 +51,14 @@
         raise AlphaException(
             f"In file {file_path} <ini> configuration must be of type <dict>"
         )
 
     for real_table_name, conf in ini.items():
         __process_table(core, bind, real_table_name, tables, file_path, conf)
 
-
-def __process_json_file(
-    core: AlphaCore, bind: str, file_path: str, tables: list[str]
-) -> None:
-    """
-    Process a JSON file for database initialization.
-
-    :param core: AlphaCore instance to work with.
-    :param bind: Bind name to work with.
-    :param file_path: Path to the JSON file containing the database initialization configuration.
-    :param tables: list of table names to process, None for all tables.
-    :raises AlphaException: If there is any issue with the provided configuration or file.
-    """
-    try:
-        data = {}
-        if os.path.exists(file_path):
-            with open(file_path, encoding="utf-8") as json_data_file:
-                data = json.load(json_data_file)
-    except Exception as ex:
-        raise AlphaException(f"Cannot read file {file_path}: {ex}")
-
-    for table_name, conf in data.items():
-        __process_table(core, bind, table_name, tables, file_path, conf)
-
-
 def __process_sql_file(core: AlphaCore, bind: str, file_path: str) -> None:
     """
     Process an SQL file for database initialization.
 
     :param core: AlphaCore instance to work with.
     :param bind: Bind name to work with.
     :param file_path: Path to the SQL file containing the database initialization statements.
@@ -250,39 +225,15 @@
             raise ValueError(f"Invalid data_type '{data_type}'")
 
         entries.append(entry)
 
     return entries
 
 
-def __process_databases_init(
-    core: AlphaCore,
-    bind: str,
-    file_path: str,
-    tables: list[str] | None = None,
-    file_type: str = "py",
-) -> None:
-    """
-    Process database initialization based on the given file type (Python, JSON, or SQL).
 
-    :param core: AlphaCore instance to work with.
-    :param bind: Bind name to work with.
-    :param file_path: Path to the file containing the database initialization configuration.
-    :param tables: list of table names to process, None for all tables.
-    :param file_type: Type of file to process (default is "py").
-    :raises AlphaException: If there is any issue with the provided configuration or file.
-    """
-    if file_type == "py":
-        __process_python_file(core, bind, file_path, tables)
-    elif file_type == "json":
-        __process_json_file(core, bind, file_path, tables)
-    elif file_type == "sql":
-        __process_sql_file(core, bind, file_path)
-    else:
-        raise ValueError(f"Unsupported file type '{file_type}'")
 
 
 def process_init_files(
     core: AlphaCore, binds: list[str], tables: list[str], init_databases_config: dict
 ):
     """Charge les fichiers d'initialisation en fonction des types de fichiers et du répertoire d'initialisation spécifié pour chaque type.
 
@@ -294,35 +245,56 @@
     """
     ini_types = {
         "json": {"key": "init_database_dir_json", "pattern": "*.json"},
         "py": {"key": "init_database_dir_py", "pattern": "*.py"},
         "sql": {"key": "init_database_dir_sql", "pattern": "*.sql"},
     }
 
+    
+
     for bind in binds:
         if not bind in init_databases_config:
             core.log.warning(
                 f"No initialisation configuration has been set in <databases> entry for {bind=}"
             )
             continue
+        tables_configs  = {}
+
+        bind_cf = init_databases_config[bind]
+        if type(bind_cf) == str and bind_cf.upper() in init_databases_config:
+            bind_cf = init_databases_config[bind_cf.upper()]
 
         for ini_type, cf_ini in ini_types.items():
-            bind_cf = init_databases_config[bind]
-            if type(bind_cf) == str and bind_cf in init_databases_config:
-                bind_cf = init_databases_config[bind_cf]
             if not cf_ini["key"] in bind_cf:
                 continue
 
             ini_dir = bind_cf[cf_ini["key"]]
             files = glob.glob(ini_dir + os.sep + cf_ini["pattern"])
 
             for file_path in files:
-                __process_databases_init(
-                    core, bind, file_path, tables, file_type=ini_type
-                )
+                if ini_type == "py":
+                    __process_python_file(core, bind, file_path, tables)
+                elif ini_type == "json":
+                    data = {}
+                    if os.path.exists(file_path):
+                        try:
+                            with open(file_path, encoding="utf-8") as json_data_file:
+                                data = json.load(json_data_file)
+                        except Exception as ex:
+                            raise AlphaException(f"Cannot read file {file_path}: {ex}")
+                    for d_t, conf in data.items():
+                        tables_configs[d_t] = conf
+                elif ini_type == "sql":
+                    __process_sql_file(core, bind, file_path)
+                else:
+                    raise ValueError(f"Unsupported file type '{ini_type}'")
+
+        for table in tables:
+            if table in tables_configs:
+                __process_table(core, bind, table, tables, file_path, tables_configs[table])
 
 
 def __normalize_tables(tables: list[str] | dict[str, str]) -> list[str]:
     """Normalise le paramètre 'tables' pour s'assurer qu'il est sous la forme d'un dictionnaire avec les noms des tables en majuscules.
 
     Args:
         tables (list[str]): Liste ou dictionnaire des noms des tables à traiter
```

### Comparing `alphaz-0.7.7/alphaz/utils/database_to_dataclass.py` & `alphaz-0.7.7.1/alphaz/utils/database_to_dataclass.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/utils/decorators.py` & `alphaz-0.7.7.1/alphaz/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/utils/ensure.py` & `alphaz-0.7.7.1/alphaz/utils/ensure.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/utils/init_database.py` & `alphaz-0.7.7.1/alphaz/utils/init_database.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/utils/mep.py` & `alphaz-0.7.7.1/alphaz/utils/mep.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/utils/screens.py` & `alphaz-0.7.7.1/alphaz/utils/screens.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/utils/selectionMenu.py` & `alphaz-0.7.7.1/alphaz/utils/selectionMenu.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/utils/tasks.py` & `alphaz-0.7.7.1/alphaz/utils/tasks.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/utils/tests.py` & `alphaz-0.7.7.1/alphaz/utils/tests.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/utils/time.py` & `alphaz-0.7.7.1/alphaz/utils/time.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz/utils/transactions.py` & `alphaz-0.7.7.1/alphaz/utils/transactions.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7/alphaz.egg-info/PKG-INFO` & `alphaz-0.7.7.1/alphaz.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,20 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: alphaz
-Version: 0.7.7
+Version: 0.7.7.1
 Summary: A package full of very nice tools
 Home-page: https://github.com/ZAurele/alphaz
+Download-URL: https://github.com/ZAurele/alphaz/archive/refs/tags/0.7.7.1.tar.gz
 Author: Aurèle
 Author-email: contact@aurele.eu
 License: MIT
-Download-URL: https://github.com/ZAurele/alphaz/archive/refs/tags/0.7.7.tar.gz
-Description: UNKNOWN
 Keywords: Flask,Json
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
+License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `alphaz-0.7.7/alphaz.egg-info/SOURCES.txt` & `alphaz-0.7.7.1/alphaz.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 alphaz/README.md
 alphaz/__init__.py
 alphaz/alphaz.bat
```

### Comparing `alphaz-0.7.7/setup.py` & `alphaz-0.7.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os, glob, re
 from datetime import date
 
 today = date.today()
 
 from setuptools import setup, find_packages
 
-version = "0.7.7"
+version = "0.7.7.1"
 
 excludes = [".git", ".vscode"]
 
 archives = glob.glob("dist/*")
 for archive in archives:
     os.remove(archive)
```

