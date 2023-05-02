# Comparing `tmp/ApiLogicServer-8.3.3.tar.gz` & `tmp/ApiLogicServer-8.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ApiLogicServer-8.3.3.tar", last modified: Sat Apr 29 22:01:05 2023, max compression
+gzip compressed data, was "ApiLogicServer-8.3.6.tar", last modified: Tue May  2 04:14:08 2023, max compression
```

## Comparing `ApiLogicServer-8.3.3.tar` & `ApiLogicServer-8.3.6.tar`

### file list

```diff
@@ -1,766 +1,777 @@
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.776017 ApiLogicServer-8.3.3/
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.566931 ApiLogicServer-8.3.3/ApiLogicServer.egg-info/
--rw-r--r--   0 val        (502) staff       (20)    14774 2023-04-29 22:01:05.000000 ApiLogicServer-8.3.3/ApiLogicServer.egg-info/PKG-INFO
--rw-r--r--   0 val        (502) staff       (20)    53981 2023-04-29 22:01:05.000000 ApiLogicServer-8.3.3/ApiLogicServer.egg-info/SOURCES.txt
--rw-r--r--   0 val        (502) staff       (20)        1 2023-04-29 22:01:05.000000 ApiLogicServer-8.3.3/ApiLogicServer.egg-info/dependency_links.txt
--rw-r--r--   0 val        (502) staff       (20)       66 2023-04-29 22:01:05.000000 ApiLogicServer-8.3.3/ApiLogicServer.egg-info/entry_points.txt
--rw-r--r--   0 val        (502) staff       (20)        1 2023-04-29 22:01:05.000000 ApiLogicServer-8.3.3/ApiLogicServer.egg-info/not-zip-safe
--rw-r--r--   0 val        (502) staff       (20)      585 2023-04-29 22:01:05.000000 ApiLogicServer-8.3.3/ApiLogicServer.egg-info/requires.txt
--rw-r--r--   0 val        (502) staff       (20)       21 2023-04-29 22:01:05.000000 ApiLogicServer-8.3.3/ApiLogicServer.egg-info/top_level.txt
--rw-r--r--   0 val        (502) staff       (20)     1485 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/LICENSE
--rw-r--r--   0 val        (502) staff       (20)      732 2023-04-23 23:14:50.000000 ApiLogicServer-8.3.3/MANIFEST.in
--rw-r--r--   0 val        (502) staff       (20)    14774 2023-04-29 22:01:05.775639 ApiLogicServer-8.3.3/PKG-INFO
--rw-r--r--   0 val        (502) staff       (20)    13785 2023-04-29 22:00:12.000000 ApiLogicServer-8.3.3/README.md
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.569055 ApiLogicServer-8.3.3/api_logic_server_cli/
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/__init__.py
--rw-r--r--   0 val        (502) staff       (20)    59911 2023-04-29 19:56:56.000000 ApiLogicServer-8.3.3/api_logic_server_cli/api_logic_server.py
--rw-r--r--   0 val        (502) staff       (20)      131 2023-04-29 21:44:24.000000 ApiLogicServer-8.3.3/api_logic_server_cli/api_logic_server_info.yaml
--rw-r--r--   0 val        (502) staff       (20)    33430 2023-03-10 20:22:39.000000 ApiLogicServer-8.3.3/api_logic_server_cli/cli.py
--rw-r--r--   0 val        (502) staff       (20)     1001 2023-04-02 18:24:38.000000 ApiLogicServer-8.3.3/api_logic_server_cli/cli_args_base.py
--rw-r--r--   0 val        (502) staff       (20)     3184 2023-04-02 23:08:24.000000 ApiLogicServer-8.3.3/api_logic_server_cli/cli_args_project.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.572547 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/
--rw-r--r--   0 val        (502) staff       (20)    10244 2023-01-26 18:43:59.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/.DS_Store
--rw-r--r--   0 val        (502) staff       (20)        0 2022-11-10 15:34:44.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.577545 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__pycache__/
--rw-r--r--   0 val        (502) staff       (20)      173 2022-11-10 15:35:23.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)      189 2023-02-26 22:48:45.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 val        (502) staff       (20)     2601 2022-11-18 17:28:18.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__pycache__/api_expose_api_models.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     3049 2023-02-05 16:19:43.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__pycache__/api_expose_api_models_creator.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     5300 2023-02-26 23:03:43.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__pycache__/api_expose_api_models_creator.cpython-311.pyc
--rw-r--r--   0 val        (502) staff       (20)     7174 2023-02-10 20:33:17.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__pycache__/api_logic_server_utils.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)    13492 2023-03-16 03:50:38.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__pycache__/api_logic_server_utils.cpython-311.pyc
--rw-r--r--   0 val        (502) staff       (20)    21342 2023-02-05 16:19:42.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__pycache__/model_creation_services.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)    35378 2023-02-26 22:48:45.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__pycache__/model_creation_services.cpython-311.pyc
--rw-r--r--   0 val        (502) staff       (20)     4053 2023-01-18 01:12:07.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__pycache__/multi_db_utils.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)    20087 2023-02-05 19:25:01.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__pycache__/ui_admin_creator.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)    37019 2023-02-26 23:03:43.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__pycache__/ui_admin_creator.cpython-311.pyc
--rw-r--r--   0 val        (502) staff       (20)     2274 2023-02-26 20:50:53.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__pycache__/uri_info.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     2617 2023-03-12 04:54:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__pycache__/uri_info.cpython-311.pyc
--rw-r--r--   0 val        (502) staff       (20)     5290 2023-02-05 02:48:17.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/api_expose_api_models_creator.py
--rw-r--r--   0 val        (502) staff       (20)    11423 2023-03-16 03:50:23.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/api_logic_server_utils.py
--rw-r--r--   0 val        (502) staff       (20)    34401 2023-02-05 02:48:22.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/model_creation_services.py
--rw-r--r--   0 val        (502) staff       (20)     6127 2023-01-18 01:12:06.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/multi_db_utilsZZ.txt
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.579977 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/
--rw-r--r--   0 val        (502) staff       (20)     6148 2023-01-22 18:56:43.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/.DS_Store
--rwxrwxrwx   0 val        (502) staff       (20)    15430 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/asset-manifest.json
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.580135 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/data/
--rwxrwxrwx   0 val        (502) staff       (20)  1145966 2023-01-15 08:58:09.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/data/customer.json
--rwxrwxrwx   0 val        (502) staff       (20)     3870 2023-01-15 08:58:09.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/favicon.ico
--rwxrwxrwx   0 val        (502) staff       (20)      692 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/index.html
--rwxrwxrwx   0 val        (502) staff       (20)     5347 2023-01-15 08:58:09.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/logo192.png
--rwxrwxrwx   0 val        (502) staff       (20)     9664 2023-01-15 08:58:09.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/logo512.png
--rwxrwxrwx   0 val        (502) staff       (20)      492 2023-01-15 08:58:09.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/manifest.json
--rwxrwxrwx   0 val        (502) staff       (20)       67 2023-01-15 08:58:09.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/robots.txt
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.559148 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.582444 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/
--rwxrwxrwx   0 val        (502) staff       (20)    86781 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/695.2b02568d.chunk.css
--rwxrwxrwx   0 val        (502) staff       (20)   166928 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/695.2b02568d.chunk.css.map
--rwxrwxrwx   0 val        (502) staff       (20)      211 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/main.a0c288b7.css
--rwxrwxrwx   0 val        (502) staff       (20)      516 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/main.a0c288b7.css.map
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.658366 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/
--rwxrwxrwx   0 val        (502) staff       (20)     1576 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1022.0747a719.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1022.0747a719.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     3197 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1022.0747a719.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     9011 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1062.9e2b1e6c.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)    21905 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1062.9e2b1e6c.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2921 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1069.16bec71d.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1069.16bec71d.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     7103 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1069.16bec71d.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     1004 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1074.2c3d927c.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1074.2c3d927c.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     2792 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1074.2c3d927c.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     7546 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1251.10ac0097.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1251.10ac0097.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    17381 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1251.10ac0097.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)    33520 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1258.94dead34.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)    71153 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1258.94dead34.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)    14043 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1295.179239a3.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)    36857 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1295.179239a3.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     5595 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1324.be7507c8.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)    14138 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1324.be7507c8.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     6135 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1431.d02260cd.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1431.d02260cd.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    14288 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1431.d02260cd.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2280 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1532.41e3c0c8.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1532.41e3c0c8.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     5953 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1532.41e3c0c8.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3747 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1619.31b6d6e8.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1619.31b6d6e8.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     8068 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1619.31b6d6e8.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     4407 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1690.e74e47c3.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1690.e74e47c3.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    10552 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1690.e74e47c3.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2156 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1989.ee922c62.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1989.ee922c62.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     5783 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1989.ee922c62.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)    11957 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2154.5c399961.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2154.5c399961.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    24504 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2154.5c399961.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     5499 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2402.e66e47e8.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2402.e66e47e8.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    13356 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2402.e66e47e8.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     4187 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2478.4e6b45fa.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)    10856 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2478.4e6b45fa.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     7001 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2526.c4309069.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)    17447 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2526.c4309069.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3591 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/254.1bc22866.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/254.1bc22866.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     8746 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/254.1bc22866.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3747 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2611.8815ae2b.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2611.8815ae2b.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     9475 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2611.8815ae2b.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3140 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2880.029aa44e.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2880.029aa44e.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     7634 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2880.029aa44e.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     4056 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2900.14a00390.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2900.14a00390.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     9168 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2900.14a00390.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     8184 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2909.28b39275.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2909.28b39275.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    18882 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2909.28b39275.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     4068 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3003.57cfe277.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3003.57cfe277.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     9104 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3003.57cfe277.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)    14317 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/312.3d69e408.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/312.3d69e408.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    32894 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/312.3d69e408.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3963 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3126.99b58416.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3126.99b58416.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     9547 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3126.99b58416.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3152 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3323.b47b9b1e.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3323.b47b9b1e.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     8052 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3323.b47b9b1e.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     8662 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3668.cd0becc2.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3668.cd0becc2.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    20172 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3668.cd0becc2.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     4982 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/369.0237ca8c.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/369.0237ca8c.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    13442 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/369.0237ca8c.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     6569 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3698.750e43d6.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3698.750e43d6.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    15183 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3698.750e43d6.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2002 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3766.d8eddcd9.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3766.d8eddcd9.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     4736 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3766.d8eddcd9.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2974 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3907.7b2efd62.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3907.7b2efd62.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     7499 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3907.7b2efd62.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     1967 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3955.f5434704.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3955.f5434704.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     5172 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3955.f5434704.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     5948 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4040.613bd8c0.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4040.613bd8c0.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    13558 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4040.613bd8c0.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)    10454 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4333.61aa216a.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4333.61aa216a.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    23458 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4333.61aa216a.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     1255 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/464.522c11f6.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/464.522c11f6.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     3229 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/464.522c11f6.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     4128 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4877.7cebca37.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4877.7cebca37.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    10303 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4877.7cebca37.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)    17096 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4900.19572072.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4900.19572072.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    31009 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4900.19572072.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     7760 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4969.ccedbf9b.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4969.ccedbf9b.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    18142 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4969.ccedbf9b.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     9800 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5133.71af5a54.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5133.71af5a54.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    21207 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5133.71af5a54.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3420 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/52.22a03ee6.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/52.22a03ee6.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     8828 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/52.22a03ee6.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3820 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5328.77d62d48.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)    10430 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5328.77d62d48.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)    41393 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5342.e36bdc43.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)   145206 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5342.e36bdc43.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     5605 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5419.3d10c516.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5419.3d10c516.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    13185 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5419.3d10c516.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     8412 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5507.c29076d8.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5507.c29076d8.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    19971 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5507.c29076d8.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     9916 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5540.d957a974.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5540.d957a974.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    22155 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5540.d957a974.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     6545 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5558.d0dc5575.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5558.d0dc5575.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    16602 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5558.d0dc5575.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     4681 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5571.ad570057.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5571.ad570057.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    11819 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5571.ad570057.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3545 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5672.f0c2440f.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5672.f0c2440f.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     8963 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5672.f0c2440f.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3710 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/608.84469af3.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/608.84469af3.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     9146 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/608.84469af3.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     1924 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6289.a7c21fba.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6289.a7c21fba.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     4864 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6289.a7c21fba.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     5069 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6304.ce792f5f.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6304.ce792f5f.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    11830 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6304.ce792f5f.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3092 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6384.8f33f789.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6384.8f33f789.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     8217 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6384.8f33f789.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2417 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6403.77f38472.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6403.77f38472.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     6013 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6403.77f38472.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     7472 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/651.bf520a75.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/651.bf520a75.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    16988 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/651.bf520a75.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2342 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6717.805e1882.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6717.805e1882.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     6267 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6717.805e1882.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)  3310604 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      576 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20) 10838575 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)    35620 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6965.381dbe04.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)   121512 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6965.381dbe04.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)    17547 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7117.b2e9eb70.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)    39845 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7117.b2e9eb70.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2594 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7294.6813eb1f.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7294.6813eb1f.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     6567 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7294.6813eb1f.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2814 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7299.20100701.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7299.20100701.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     7255 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7299.20100701.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)    18754 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7436.4e91a3a5.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7436.4e91a3a5.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    38065 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7436.4e91a3a5.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2736 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7497.f56048e1.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7497.f56048e1.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     7008 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7497.f56048e1.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2693 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7499.b216e9da.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7499.b216e9da.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     6865 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7499.b216e9da.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3378 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7615.f5af9bae.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7615.f5af9bae.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     8159 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7615.f5af9bae.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2709 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7713.6d02efa2.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7713.6d02efa2.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     6645 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7713.6d02efa2.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     4619 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/787.d5293104.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)    10592 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/787.d5293104.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     4203 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7894.f8f70466.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)    10608 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7894.f8f70466.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2559 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7952.29e2c950.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7952.29e2c950.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     6522 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7952.29e2c950.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     5926 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8184.741e3d56.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)    96741 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8184.741e3d56.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     1840 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8272.99aef5a5.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8272.99aef5a5.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     5116 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8272.99aef5a5.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     8013 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8347.649393e6.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8347.649393e6.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    19497 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8347.649393e6.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3725 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/839.87662037.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/839.87662037.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     9025 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/839.87662037.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3288 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8501.ea0cd3a2.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8501.ea0cd3a2.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     8254 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8501.ea0cd3a2.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2026 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8861.01a110f5.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8861.01a110f5.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     5528 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8861.01a110f5.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)    13558 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/907.7b650179.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/907.7b650179.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    26650 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/907.7b650179.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     9201 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9186.73a41896.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9186.73a41896.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    21765 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9186.73a41896.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     5069 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9200.d0bc8746.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9200.d0bc8746.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    11826 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9200.d0bc8746.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)    34921 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9214.5198dfc3.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)   119930 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9214.5198dfc3.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     4669 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9335.43329da2.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9335.43329da2.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    10814 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9335.43329da2.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     4316 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9357.e2f466b8.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9357.e2f466b8.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    10868 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9357.e2f466b8.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)    11414 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9361.e7bbdd03.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9361.e7bbdd03.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    24817 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9361.e7bbdd03.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2622 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9381.9495a14c.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)     7016 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9381.9495a14c.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     5259 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9432.e84dc193.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)    13615 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9432.e84dc193.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     7391 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9687.e1a38d25.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9687.e1a38d25.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    17258 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9687.e1a38d25.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     1986 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9845.3bb55d3c.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9845.3bb55d3c.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     4960 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9845.3bb55d3c.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3230 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9902.bfcd7f60.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9902.bfcd7f60.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     8177 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9902.bfcd7f60.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)  1384276 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js
--rwxrwxrwx   0 val        (502) staff       (20)     3014 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)  5552838 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js.map
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.662765 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/media/
--rwxrwxrwx   0 val        (502) staff       (20)    72504 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/media/codicon.b797181c93b3755f4fa1.ttf
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.667416 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.668102 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/basic_web_app/
--rw-r--r--   0 val        (502) staff       (20)       55 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/basic_web_app/.gitignore
--rw-r--r--   0 val        (502) staff       (20)      389 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/basic_web_app/README.rst
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.668635 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/basic_web_app/app/
--rw-r--r--   0 val        (502) staff       (20)      742 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/basic_web_app/app/__init__.py
--rw-r--r--   0 val        (502) staff       (20)      276 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/basic_web_app/app/models.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.668797 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/basic_web_app/app/templates/
--rw-r--r--   0 val        (502) staff       (20)      124 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/basic_web_app/app/templates/404.html
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.559458 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.559499 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/pt/
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.669150 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 val        (502) staff       (20)      483 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 val        (502) staff       (20)      727 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 val        (502) staff       (20)      938 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/basic_web_app/app/views.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.669474 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/basic_web_app/babel/
--rw-r--r--   0 val        (502) staff       (20)       64 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/basic_web_app/babel/babel.cfg
--rw-r--r--   0 val        (502) staff       (20)      662 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/basic_web_app/babel/messages.pot
--rw-r--r--   0 val        (502) staff       (20)     3669 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/basic_web_app/config.py
--rw-r--r--   0 val        (502) staff       (20)       68 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/basic_web_app/run.py
--rw-r--r--   0 val        (502) staff       (20)      556 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/create_admin.sh
--rw-r--r--   0 val        (502) staff       (20)      624 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/fab_config.py
--rw-r--r--   0 val        (502) staff       (20)     2683 2023-02-05 02:49:11.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/home.js
--rw-r--r--   0 val        (502) staff       (20)     3121 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/react_admin_component.js
--rw-r--r--   0 val        (502) staff       (20)    35694 2023-02-05 19:24:16.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/ui_admin_creator.py
--rw-r--r--   0 val        (502) staff       (20)     2252 2023-03-12 01:14:25.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/uri_info.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.685328 ApiLogicServer-8.3.3/api_logic_server_cli/database/
--rw-r--r--   0 val        (502) staff       (20)     6148 2022-12-22 22:39:55.000000 ApiLogicServer-8.3.3/api_logic_server_cli/database/.DS_Store
--rw-r--r--   0 val        (502) staff       (20)  1067008 2022-10-11 15:13:39.000000 ApiLogicServer-8.3.3/api_logic_server_cli/database/Chinook_Sqlite.sqlite
--rw-r--r--   0 val        (502) staff       (20)       60 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/database/__init__.py
--rw-r--r--   0 val        (502) staff       (20)    45056 2023-01-19 01:03:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/database/authentication.sqlite
--rw-r--r--   0 val        (502) staff       (20)   413696 2022-12-26 21:41:55.000000 ApiLogicServer-8.3.3/api_logic_server_cli/database/classicmodels.sqlite
--rw-r--r--   0 val        (502) staff       (20)      122 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/database/customize_models.py
--rw-r--r--   0 val        (502) staff       (20)    16384 2023-03-07 00:17:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/database/new.sqlite
--rw-r--r--   0 val        (502) staff       (20)   522240 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/database/nw-gold-plus.sqlite
--rw-r--r--   0 val        (502) staff       (20)   522240 2023-03-19 18:51:02.000000 ApiLogicServer-8.3.3/api_logic_server_cli/database/nw-gold.sqlite
--rw-r--r--   0 val        (502) staff       (20)   496640 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/database/nw.sqlite
--rw-r--r--   0 val        (502) staff       (20)    32768 2023-03-08 04:23:41.000000 ApiLogicServer-8.3.3/api_logic_server_cli/database/table_filters_tests.sqlite
--rw-r--r--   0 val        (502) staff       (20)       53 2023-03-08 15:53:51.000000 ApiLogicServer-8.3.3/api_logic_server_cli/database/table_filters_tests.yml
--rw-r--r--   0 val        (502) staff       (20)       23 2023-04-06 03:07:09.000000 ApiLogicServer-8.3.3/api_logic_server_cli/database/table_filters_tests_nw.yml
--rw-r--r--   0 val        (502) staff       (20)       25 2023-04-06 03:06:34.000000 ApiLogicServer-8.3.3/api_logic_server_cli/database/table_filters_tests_nw_1.yml
--rw-r--r--   0 val        (502) staff       (20)       21 2023-03-14 16:06:21.000000 ApiLogicServer-8.3.3/api_logic_server_cli/database/table_filters_tests_typical.yml
--rw-r--r--   0 val        (502) staff       (20)    16384 2022-12-31 01:13:31.000000 ApiLogicServer-8.3.3/api_logic_server_cli/database/todos.sqlite
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.703214 ApiLogicServer-8.3.3/api_logic_server_cli/docs/
--rw-r--r--   0 val        (502) staff       (20)     6148 2023-01-22 18:56:43.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/.DS_Store
--rw-r--r--   0 val        (502) staff       (20)     1251 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/API-Customize.md
--rw-r--r--   0 val        (502) staff       (20)     2647 2022-12-29 01:51:24.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/API.md
--rw-r--r--   0 val        (502) staff       (20)     3222 2022-12-21 16:33:05.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Admin-Customization.md
--rw-r--r--   0 val        (502) staff       (20)    18275 2023-03-10 04:52:51.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Admin-Tour.md
--rw-r--r--   0 val        (502) staff       (20)      384 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Architecture-What-Is.md
--rw-r--r--   0 val        (502) staff       (20)    12713 2022-11-22 02:48:15.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Architecture.md
--rw-r--r--   0 val        (502) staff       (20)    61944 2022-10-11 03:42:54.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Behave-Logic-Report.md
--rw-r--r--   0 val        (502) staff       (20)     3838 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Behave.md
--rw-r--r--   0 val        (502) staff       (20)     1994 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Create-ApiLogicProject.md
--rw-r--r--   0 val        (502) staff       (20)     5319 2022-12-21 20:29:28.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Data-Model-Classes.md
--rw-r--r--   0 val        (502) staff       (20)     2660 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Data-Model-Customization.md
--rw-r--r--   0 val        (502) staff       (20)     1114 2023-01-27 04:14:44.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Data-Model-Examples.md
--rw-r--r--   0 val        (502) staff       (20)      970 2022-10-03 02:15:43.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Data-Model-Keys.md
--rw-r--r--   0 val        (502) staff       (20)     3898 2023-01-06 02:59:38.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Data-Model-Multi.md
--rw-r--r--   0 val        (502) staff       (20)    13193 2023-03-12 01:14:31.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Database-Connectivity.md
--rw-r--r--   0 val        (502) staff       (20)     1241 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Execute.md
--rw-r--r--   0 val        (502) staff       (20)     3273 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/FAQ-Frameworks.md
--rw-r--r--   0 val        (502) staff       (20)      527 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/FAQ-Low-Code.md
--rw-r--r--   0 val        (502) staff       (20)     7036 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/FAQ-RETE.md
--rw-r--r--   0 val        (502) staff       (20)     1851 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/IDE-Customize.md
--rw-r--r--   0 val        (502) staff       (20)     7532 2023-01-20 15:50:43.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/IDE-Execute.md
--rw-r--r--   0 val        (502) staff       (20)     6368 2023-02-04 01:50:40.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Install-Eval-x.md
--rw-r--r--   0 val        (502) staff       (20)     8093 2023-01-09 21:17:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Install-Eval.md
--rw-r--r--   0 val        (502) staff       (20)     3390 2023-02-03 23:28:34.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Install-Express-x.md
--rw-r--r--   0 val        (502) staff       (20)     3539 2022-08-23 15:56:25.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Install-Express.md
--rw-r--r--   0 val        (502) staff       (20)      566 2022-11-30 17:57:34.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Install-psycopg2.md
--rw-r--r--   0 val        (502) staff       (20)      977 2022-11-17 04:40:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Install-pyodbc.md
--rw-r--r--   0 val        (502) staff       (20)     7135 2022-09-18 04:42:29.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Install.md
--rw-r--r--   0 val        (502) staff       (20)    13448 2023-02-05 02:54:14.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Internals-CLI.md
--rw-r--r--   0 val        (502) staff       (20)     6504 2022-12-01 16:51:37.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Internals.md
--rw-r--r--   0 val        (502) staff       (20)     3258 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Logic-Operation.md
--rw-r--r--   0 val        (502) staff       (20)    14729 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Logic-Tutorial.md
--rw-r--r--   0 val        (502) staff       (20)    10325 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Logic-Why.md
--rw-r--r--   0 val        (502) staff       (20)     3707 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Logic.md
--rw-r--r--   0 val        (502) staff       (20)     4205 2022-08-28 15:23:33.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Manage-GitHub.md
--rw-r--r--   0 val        (502) staff       (20)     3796 2022-12-28 03:43:06.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Project-Builders.md
--rw-r--r--   0 val        (502) staff       (20)     1957 2022-12-22 04:40:03.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Project-DevOps.md
--rw-r--r--   0 val        (502) staff       (20)     1930 2023-01-31 22:36:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Project-Env.md
--rw-r--r--   0 val        (502) staff       (20)     4936 2022-11-24 20:38:40.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Project-Execution.md
--rw-r--r--   0 val        (502) staff       (20)     2446 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Project-Rebuild.md
--rw-r--r--   0 val        (502) staff       (20)     2104 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Project-Structure.md
--rw-r--r--   0 val        (502) staff       (20)      773 2022-09-18 04:42:29.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Sample-Database.md
--rw-r--r--   0 val        (502) staff       (20)     2227 2023-02-14 23:54:00.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Security-Activation.md
--rw-------   0 val        (502) staff       (20)     1585 2023-01-21 01:47:08.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Security-Authentication-Provider.md
--rw-------   0 val        (502) staff       (20)     1470 2023-01-21 02:17:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Security-Authentication.md
--rw-r--r--   0 val        (502) staff       (20)     1922 2023-01-06 17:06:26.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Security-Authorization.md
--rw-r--r--   0 val        (502) staff       (20)     5277 2023-01-21 01:31:32.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Security-Overview.md
--rw-r--r--   0 val        (502) staff       (20)      155 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Tech--Notes.md
--rw-r--r--   0 val        (502) staff       (20)      237 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Tech-4GL.md
--rw-r--r--   0 val        (502) staff       (20)     7081 2022-11-24 00:40:19.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Tech-CodeSpaces.md
--rw-r--r--   0 val        (502) staff       (20)     3053 2022-12-06 21:43:43.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Tech-Conference-PyCon23-Talk.md
--rw-r--r--   0 val        (502) staff       (20)     3174 2022-12-06 18:38:49.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Tech-Conference-PyCon23-Tutorial.md
--rw-r--r--   0 val        (502) staff       (20)     5693 2022-12-05 19:50:10.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Tech-Conference.md
--rw-r--r--   0 val        (502) staff       (20)     3385 2022-11-07 18:45:42.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Tech-Docker.md
--rw-r--r--   0 val        (502) staff       (20)      815 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Tech-Install-Python.md
--rw-r--r--   0 val        (502) staff       (20)     1049 2022-10-03 16:52:30.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Tech-Proven.md
--rw-r--r--   0 val        (502) staff       (20)     2679 2022-12-07 04:30:27.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Tech-Python-311.md
--rw-r--r--   0 val        (502) staff       (20)     3728 2023-01-12 06:40:15.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Tech-Python.md
--rw-r--r--   0 val        (502) staff       (20)     3019 2022-10-21 23:29:01.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Tech-m1.md
--rw-r--r--   0 val        (502) staff       (20)     1644 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Tech-mkdocs-material.md
--rw-r--r--   0 val        (502) staff       (20)    12291 2022-10-08 18:23:10.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Troubleshooting.md
--rw-r--r--   0 val        (502) staff       (20)    15277 2023-04-27 02:31:04.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Tutorial.md
--rw-r--r--   0 val        (502) staff       (20)     6697 2022-12-02 18:42:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Working-With-Docker.md
--rw-r--r--   0 val        (502) staff       (20)     4031 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Working-with-Flask-AppBuilder.md
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.703499 ApiLogicServer-8.3.3/api_logic_server_cli/docs/assets/
--rw-r--r--   0 val        (502) staff       (20)     6148 2022-08-30 03:14:41.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/assets/.DS_Store
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.703978 ApiLogicServer-8.3.3/api_logic_server_cli/docs/assets/images/
--rw-r--r--   0 val        (502) staff       (20)     2362 2022-08-29 00:06:15.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/assets/images/bulb-icon.svg
--rw-r--r--   0 val        (502) staff       (20)     3482 2022-08-30 03:46:01.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/assets/images/lightbulb.svg
--rw-r--r--   0 val        (502) staff       (20)    15440 2023-02-06 03:49:29.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/index.md
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.704175 ApiLogicServer-8.3.3/api_logic_server_cli/docs/stylesheets/
--rw-r--r--   0 val        (502) staff       (20)      634 2022-08-30 03:44:15.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/stylesheets/extra.css
--rw-r--r--   0 val        (502) staff       (20)    11824 2023-02-11 04:16:18.000000 ApiLogicServer-8.3.3/api_logic_server_cli/extended_builder.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.705870 ApiLogicServer-8.3.3/api_logic_server_cli/fragments/
--rw-r--r--   0 val        (502) staff       (20)     1431 2023-02-05 02:48:13.000000 ApiLogicServer-8.3.3/api_logic_server_cli/fragments/Todo_modelsZZ.py.py
--rw-r--r--   0 val        (502) staff       (20)     1956 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/fragments/configZZ.py
--rw-r--r--   0 val        (502) staff       (20)       63 2022-10-01 16:17:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/fragments/db_typesZZ.txt
--rw-r--r--   0 val        (502) staff       (20)    12053 2023-02-05 02:48:09.000000 ApiLogicServer-8.3.3/api_logic_server_cli/fragments/modelsZZ.py
--rw-r--r--   0 val        (502) staff       (20)      888 2023-04-23 22:57:22.000000 ApiLogicServer-8.3.3/api_logic_server_cli/fragments/nw_virtual_attrs.py
--rw-r--r--   0 val        (502) staff       (20)      870 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/fragments/ui_basic_web_app_runZZ.py
--rw-r--r--   0 val        (502) staff       (20)     1006 2023-04-21 23:18:04.000000 ApiLogicServer-8.3.3/api_logic_server_cli/logging.yml
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.709620 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/
--rw-r--r--   0 val        (502) staff       (20)    10244 2023-04-26 02:43:32.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.DS_Store
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.710522 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.devcontainer/
--rw-r--r--   0 val        (502) staff       (20)      444 2023-02-05 02:50:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.devcontainer/For_VSCode.dockerfile
--rw-r--r--   0 val        (502) staff       (20)     1932 2023-02-05 21:44:41.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.devcontainer/devcontainer.json
--rw-r--r--   0 val        (502) staff       (20)      288 2023-01-08 18:52:09.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.devcontainer/setup.sh
--rw-r--r--   0 val        (502) staff       (20)      106 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.gitignore
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.710816 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.idea/
--rw-r--r--   0 val        (502) staff       (20)     6148 2023-02-14 05:32:37.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.idea/.DS_Store
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.712859 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.idea/runConfigurations/
--rw-r--r--   0 val        (502) staff       (20)     6148 2023-02-14 05:32:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.idea/runConfigurations/.DS_Store
--rw-r--r--   0 val        (502) staff       (20)     1127 2023-04-29 02:28:50.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.idea/runConfigurations/ApiLogicServer.xml
--rw-r--r--   0 val        (502) staff       (20)     1306 2022-04-03 03:00:44.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.idea/runConfigurations/Report_Behave_Logic.xml
--rw-r--r--   0 val        (502) staff       (20)     1196 2022-04-03 03:00:44.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.idea/runConfigurations/Run_Behave.xml
--rw-r--r--   0 val        (502) staff       (20)     1205 2022-04-03 03:00:44.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.idea/runConfigurations/Windows_Run_Behave.xml
--rw-r--r--   0 val        (502) staff       (20)     1193 2023-04-29 01:03:03.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.idea/runConfigurations/run___No_Security.xml
--rw-r--r--   0 val        (502) staff       (20)     2444 2023-04-29 01:03:22.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.idea/runConfigurations/run_docker.xml
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.713433 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.vscode/
--rw-r--r--   0 val        (502) staff       (20)     6518 2023-04-13 16:38:20.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.vscode/launch.json
--rw-r--r--   0 val        (502) staff       (20)      437 2023-04-13 04:29:56.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.vscode/settings.json
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.714628 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/api/
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/api/__init__.py
--rw-r--r--   0 val        (502) staff       (20)     2053 2023-04-26 02:48:17.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/api/customize_api.py
--rw-r--r--   0 val        (502) staff       (20)      316 2023-01-23 01:07:06.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/api/expose_api_models.py
--rw-r--r--   0 val        (502) staff       (20)      521 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/api/json_encoder.py
--rw-r--r--   0 val        (502) staff       (20)     2689 2023-04-29 21:17:10.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/api/readme_customize_api.md
--rw-r--r--   0 val        (502) staff       (20)    18920 2023-04-29 18:24:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/api_logic_server_run.py
--rw-r--r--   0 val        (502) staff       (20)     3131 2023-03-03 16:08:15.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/config.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.715529 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/database/
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/database/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.716256 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/database/alembic/
--rw-r--r--   0 val        (502) staff       (20)     2101 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/database/alembic/env.py
--rw-r--r--   0 val        (502) staff       (20)     1967 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/database/alembic/readme.md
--rw-r--r--   0 val        (502) staff       (20)      494 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/database/alembic/script.py.mako
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.716400 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/database/alembic/versions/
--rw-r--r--   0 val        (502) staff       (20)       60 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/database/alembic/versions/readme.md
--rw-r--r--   0 val        (502) staff       (20)     3027 2023-02-09 15:42:27.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/database/alembic.ini
--rw-r--r--   0 val        (502) staff       (20)      537 2023-01-28 17:53:13.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/database/bind_databases.py
--rw-r--r--   0 val        (502) staff       (20)      469 2023-01-23 01:14:38.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/database/customize_models.py
--rw-r--r--   0 val        (502) staff       (20)      139 2022-12-21 03:23:43.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/default.env
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.716580 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/devops/
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.717759 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/devops/docker/
--rw-r--r--   0 val        (502) staff       (20)     2381 2023-02-26 22:13:43.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/devops/docker/authdb_mysql.Dockerfile
--rw-r--r--   0 val        (502) staff       (20)     3643 2023-02-25 03:16:21.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/devops/docker/authdb_mysql.sql
--rw-r--r--   0 val        (502) staff       (20)      331 2023-04-02 15:52:20.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/devops/docker/build_image.dockerfile
--rw-r--r--   0 val        (502) staff       (20)     2079 2023-04-02 16:35:31.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/devops/docker/build_image.sh
--rw-r--r--   0 val        (502) staff       (20)      876 2023-01-07 21:19:34.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/devops/git_push_new_project.sh
--rw-r--r--   0 val        (502) staff       (20)     1475 2023-04-21 23:01:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/logging.yml
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.718322 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/logic/
--rw-r--r--   0 val        (502) staff       (20)      592 2023-04-26 02:47:32.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/logic/declare_logic.py
--rw-r--r--   0 val        (502) staff       (20)     5953 2023-04-27 00:49:20.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/logic/readme_declare_logic.md
--rw-r--r--   0 val        (502) staff       (20)      568 2023-03-04 03:52:49.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/mypy.ini
--rw-r--r--   0 val        (502) staff       (20)     3820 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/python_anywhere_wsgi.py
--rw-r--r--   0 val        (502) staff       (20)     7133 2023-04-29 21:44:21.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/readme.md
--rw-r--r--   0 val        (502) staff       (20)       14 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/requirements.txt
--rw-r--r--   0 val        (502) staff       (20)      801 2022-10-19 20:24:10.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/run.ps1
--rwxr-xr-x   0 val        (502) staff       (20)     1040 2022-11-09 16:08:44.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/run.sh
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.719092 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/
--rw-r--r--   0 val        (502) staff       (20)     6148 2023-01-22 18:56:43.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/.DS_Store
--rw-r--r--   0 val        (502) staff       (20)        0 2022-12-15 01:50:41.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.719768 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/
--rw-r--r--   0 val        (502) staff       (20)     6148 2022-12-18 05:06:14.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/.DS_Store
--rw-r--r--   0 val        (502) staff       (20)        0 2022-12-14 21:51:49.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.722043 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/
--rw-r--r--   0 val        (502) staff       (20)      173 2022-12-14 21:55:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)      928 2022-12-19 03:03:12.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/abstract_authentication_provider.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     1803 2022-12-18 03:38:13.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/authentication_models.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)      820 2022-12-16 14:20:29.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/db_auth.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     1392 2022-12-14 22:25:00.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/mem_auth.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     1024 2022-12-16 15:01:05.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/mem_auth_row.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     1619 2022-12-15 17:24:50.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/models.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)      580 2022-12-19 03:03:11.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/abstract_authentication_provider.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.722817 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/memory/
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.723085 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/memory/__pycache__/
--rw-r--r--   0 val        (502) staff       (20)     1493 2022-12-19 03:13:00.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/memory/__pycache__/auth_provider.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     4355 2023-01-24 04:07:34.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/memory/auth_provider.py
--rw-r--r--   0 val        (502) staff       (20)     2907 2023-01-24 04:07:34.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/memory/auth_provider_no_swagger.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.561468 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/sql/
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.723867 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/
--rw-r--r--   0 val        (502) staff       (20)     1215 2022-12-19 03:24:21.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/auth_provider.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     2262 2022-12-19 00:39:44.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/authentication_models.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)      839 2022-12-18 03:49:32.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/db_auth.cpython-310.pyc
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.724095 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/sql/sqlite/
--rw-r--r--   0 val        (502) staff       (20)     2165 2023-02-15 02:24:49.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/sql/sqlite/auth_provider.py
--rw-r--r--   0 val        (502) staff       (20)      587 2023-01-23 01:02:25.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/declare_security.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.724775 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/notes_temp/
--rw-r--r--   0 val        (502) staff       (20)     1403 2023-01-12 23:08:16.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/notes_temp/pip-freeze-th.txt
--rw-r--r--   0 val        (502) staff       (20)     1156 2023-01-12 23:08:16.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/notes_temp/pip-freeze.txt
--rw-r--r--   0 val        (502) staff       (20)     1364 2023-01-12 23:29:28.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/notes_temp/token.txt
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.725821 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/system/
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.726100 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/system/__pycache__/
--rw-r--r--   0 val        (502) staff       (20)     4665 2022-12-19 03:03:12.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/system/__pycache__/security_manager.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     3425 2023-03-03 16:56:43.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/system/authentication.py
--rw-r--r--   0 val        (502) staff       (20)     6004 2023-03-03 16:56:55.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/system/authorization.py
--rw-r--r--   0 val        (502) staff       (20)     1705 2023-02-13 15:35:11.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/system/custom_swagger.json
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.726381 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/templates/
--rw-r--r--   0 val        (502) staff       (20)     3765 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/templates/index.html
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.726567 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/test/
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/test/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.727351 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/test/api_logic_server_behave/
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/test/api_logic_server_behave/__init__.py
--rw-r--r--   0 val        (502) staff       (20)     9969 2022-11-29 03:36:44.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/test/api_logic_server_behave/behave_logic_report.py
--rw-r--r--   0 val        (502) staff       (20)     1026 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/test/api_logic_server_behave/behave_run.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.727611 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/
--rw-r--r--   0 val        (502) staff       (20)      414 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/about.feature
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.728091 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/steps/
--rw-r--r--   0 val        (502) staff       (20)      416 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/steps/about.py
--rw-r--r--   0 val        (502) staff       (20)     1518 2023-02-11 17:50:21.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/steps/test_utils.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.728953 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/
--rw-r--r--   0 val        (502) staff       (20)      147 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/Behave Logic Report Intro micro.md
--rw-r--r--   0 val        (502) staff       (20)     3707 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/Behave Logic Report Intro.md
--rw-r--r--   0 val        (502) staff       (20)    65295 2022-10-11 03:42:40.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/Behave Logic Report Sample.md
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.729936 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/test/basic/
--rw-r--r--   0 val        (502) staff       (20)      735 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/test/basic/server_test.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.730546 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/
--rw-r--r--   0 val        (502) staff       (20)    10244 2023-01-22 20:09:13.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/.DS_Store
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.731029 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/admin/
--rw-r--r--   0 val        (502) staff       (20)     6671 2023-03-19 18:44:09.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/admin/admin_loader.py
--rw-r--r--   0 val        (502) staff       (20)     2750 2023-02-05 02:50:52.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/admin/home.js
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.731325 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/
--rw-r--r--   0 val        (502) staff       (20)     6148 2022-11-26 23:48:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/.DS_Store
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.733319 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Employee/
--rw-r--r--   0 val        (502) staff       (20)     3778 2008-04-22 03:51:40.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Employee/andrew.jpg
--rw-r--r--   0 val        (502) staff       (20)     5404 2008-04-22 03:51:58.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Employee/anne.jpg
--rw-r--r--   0 val        (502) staff       (20)     3750 2008-04-22 03:48:16.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Employee/janet.jpg
--rw-r--r--   0 val        (502) staff       (20)     3715 2008-04-22 03:48:32.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Employee/laura.jpg
--rw-r--r--   0 val        (502) staff       (20)     3862 2008-04-22 03:48:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Employee/margaret.jpg
--rw-r--r--   0 val        (502) staff       (20)     4375 2008-04-22 03:49:14.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Employee/michael.jpg
--rw-r--r--   0 val        (502) staff       (20)     4425 2008-04-22 03:49:28.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Employee/nancy.jpg
--rw-r--r--   0 val        (502) staff       (20)     3737 2008-04-22 03:50:00.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Employee/robert.jpg
--rw-r--r--   0 val        (502) staff       (20)     3719 2008-04-22 03:50:34.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Employee/steven.jpg
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.734717 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Product/
--rw-r--r--   0 val        (502) staff       (20)     6054 2008-04-22 03:46:52.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Product/beverages.gif
--rw-r--r--   0 val        (502) staff       (20)     7324 2008-04-22 03:47:14.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Product/cereals.gif
--rw-r--r--   0 val        (502) staff       (20)     7751 2008-04-22 03:47:30.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Product/condiments.gif
--rw-r--r--   0 val        (502) staff       (20)     7022 2008-04-22 03:47:44.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Product/confections.gif
--rw-r--r--   0 val        (502) staff       (20)     6136 2008-04-22 03:47:58.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Product/diary.gif
--rw-r--r--   0 val        (502) staff       (20)     7268 2008-04-22 03:49:00.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Product/meat.gif
--rw-r--r--   0 val        (502) staff       (20)     7633 2008-04-22 03:49:44.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Product/produce.gif
--rw-r--r--   0 val        (502) staff       (20)     8469 2008-04-22 03:50:18.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Product/seafood.gif
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.734883 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/templates/
--rw-r--r--   0 val        (502) staff       (20)       26 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/templates/content.html
--rw-r--r--   0 val        (502) staff       (20)     9076 2023-03-24 00:43:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/util.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.737074 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/venv_setup/
--rwxr-xr-x   0 val        (502) staff       (20)     3116 2023-03-10 20:26:13.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/venv_setup/py.py
--rw-r--r--   0 val        (502) staff       (20)      738 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/venv_setup/readme_venv.md
--rw-r--r--   0 val        (502) staff       (20)      579 2023-03-03 02:36:32.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/venv_setup/requirements-no-cli.txt
--rw-r--r--   0 val        (502) staff       (20)      900 2023-02-05 02:50:56.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/venv_setup/venv-linux.sh
--rw-r--r--   0 val        (502) staff       (20)      698 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/venv_setup/venv.ps1
--rw-r--r--   0 val        (502) staff       (20)      893 2023-02-05 02:50:58.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/venv_setup/venv.sh
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.737885 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/
--rw-r--r--   0 val        (502) staff       (20)    10244 2023-01-22 18:56:43.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/.DS_Store
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.738499 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/api/
--rw-r--r--   0 val        (502) staff       (20)     8711 2023-02-13 15:35:11.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/api/customize_api.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.739429 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/api/multi-table-example/
--rw-r--r--   0 val        (502) staff       (20)    34142 2023-04-29 21:00:10.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/api/multi-table-example/multi-table.json
--rw-r--r--   0 val        (502) staff       (20)      650 2023-04-29 21:02:15.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/api/multi-table-example/multi-table.txt
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.740268 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/database/
--rw-r--r--   0 val        (502) staff       (20)     2662 2023-04-24 23:31:11.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/database/customize_models.py
--rw-r--r--   0 val        (502) staff       (20)      312 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/database/db_debug.py
--rw-r--r--   0 val        (502) staff       (20)        0 2022-11-16 19:24:28.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/database/nw-gold.sqlite
--rw-r--r--   0 val        (502) staff       (20)       29 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/database/restore_sample_db.sh
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.740526 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/logic/
--rw-r--r--   0 val        (502) staff       (20)    10650 2023-04-23 00:10:12.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/logic/declare_logic.py
--rw-r--r--   0 val        (502) staff       (20)      241 2023-04-29 21:06:51.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/readme.md
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.740820 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/security/
--rw-r--r--   0 val        (502) staff       (20)     1158 2023-02-14 15:54:30.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/security/declare_security.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.741157 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.741255 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.741827 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/
--rw-r--r--   0 val        (502) staff       (20)      187 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/about.feature
--rw-r--r--   0 val        (502) staff       (20)      285 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/api.feature
--rw-r--r--   0 val        (502) staff       (20)     1281 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/place_order.feature
--rw-r--r--   0 val        (502) staff       (20)      473 2023-04-23 23:42:07.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/salary_change.feature
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.742845 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/
--rw-r--r--   0 val        (502) staff       (20)      450 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/about.py
--rw-r--r--   0 val        (502) staff       (20)     2130 2023-01-14 03:27:19.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/api.py
--rw-r--r--   0 val        (502) staff       (20)    16642 2023-02-16 04:52:22.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/place_order.py
--rw-r--r--   0 val        (502) staff       (20)     4722 2023-04-23 23:41:49.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/salary_change.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.743111 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/
--rw-r--r--   0 val        (502) staff       (20)     4356 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/behave.log
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.744937 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/
--rw-r--r--   0 val        (502) staff       (20)     5070 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Alter_Item_Qty_to_exceed_.log
--rw-r--r--   0 val        (502) staff       (20)     2256 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Alter_Required_Date_-_adj.log
--rw-r--r--   0 val        (502) staff       (20)     8652 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Audit_Salary_Change.log
--rw-r--r--   0 val        (502) staff       (20)     6095 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Bad_Order_Custom_Service.log
--rw-r--r--   0 val        (502) staff       (20)     5794 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Good_Order_Custom_Service.log
--rw-r--r--   0 val        (502) staff       (20)     2568 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Raise_Must_be_Meaningful.log
--rw-r--r--   0 val        (502) staff       (20)     8481 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Reset_Shipped_-_adjust_lo.log
--rw-r--r--   0 val        (502) staff       (20)     8445 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Set_Shipped_-_adjust_logi.log
--rw-r--r--   0 val        (502) staff       (20)     2561 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Transaction_Processing.log
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.745723 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.747602 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/results/
--rw-r--r--   0 val        (502) staff       (20)     5070 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/results/ADJUST_test_-_OrderDetail.log
--rw-r--r--   0 val        (502) staff       (20)     8652 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/results/AUDIT_test_-_Emp_Sal.log
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/results/BEGIN.log
--rw-r--r--   0 val        (502) staff       (20)    16926 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/results/CASCADE_UPDATE_-_ShippedD.log
--rw-r--r--   0 val        (502) staff       (20)     6095 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/results/CUSTOM_SERVICE_Bad_Order.log
--rw-r--r--   0 val        (502) staff       (20)      840 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/results/DELETE_test_-_Cust.log
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/results/GET_self-reln_Dept-SubDep.log
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/results/GET_test_on_Order.log
--rw-r--r--   0 val        (502) staff       (20)     1381 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/results/PATCH_-_low_credit.log
--rw-r--r--   0 val        (502) staff       (20)      831 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/results/POST_test_-_Cust.log
--rw-r--r--   0 val        (502) staff       (20)     2256 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/results/PRUNE_test_-_ReqdDate.log
--rw-r--r--   0 val        (502) staff       (20)     8405 2023-03-10 20:26:58.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/server_startup_test.py
--rw-r--r--   0 val        (502) staff       (20)    13497 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/server_test.py
--rw-r--r--   0 val        (502) staff       (20)     1543 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/server_test.sh
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.747785 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/
--rw-r--r--   0 val        (502) staff       (20)     8196 2022-11-11 23:20:49.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/.DS_Store
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.748769 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/admin/
--rw-r--r--   0 val        (502) staff       (20)    17259 2023-04-24 23:38:28.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/admin/admin.yaml
--rw-r--r--   0 val        (502) staff       (20)     3443 2023-02-05 02:51:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/admin/home.js
--rw-r--r--   0 val        (502) staff       (20)     8798 2022-12-30 19:58:21.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/admin/multi_app_project.yaml
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.749175 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/
--rw-r--r--   0 val        (502) staff       (20)     6148 2022-11-11 23:17:05.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/.DS_Store
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.750904 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Category/
--rw-r--r--   0 val        (502) staff       (20)     6054 2008-04-22 03:46:52.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Category/beverages.gif
--rw-r--r--   0 val        (502) staff       (20)     7324 2008-04-22 03:47:14.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Category/cereals.gif
--rw-r--r--   0 val        (502) staff       (20)     7751 2008-04-22 03:47:30.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Category/condiments.gif
--rw-r--r--   0 val        (502) staff       (20)     7022 2008-04-22 03:47:44.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Category/confections.gif
--rw-r--r--   0 val        (502) staff       (20)     6136 2008-04-22 03:47:58.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Category/diary.gif
--rw-r--r--   0 val        (502) staff       (20)     7268 2008-04-22 03:49:00.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Category/meat.gif
--rw-r--r--   0 val        (502) staff       (20)     7633 2008-04-22 03:49:44.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Category/produce.gif
--rw-r--r--   0 val        (502) staff       (20)     8469 2008-04-22 03:50:18.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Category/seafood.gif
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.752387 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Employee/
--rw-r--r--   0 val        (502) staff       (20)     3719 2008-04-22 03:50:34.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Employee/buchanan.jpg
--rw-r--r--   0 val        (502) staff       (20)     3715 2008-04-22 03:48:32.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Employee/callahan.jpg
--rw-r--r--   0 val        (502) staff       (20)     4425 2008-04-22 03:49:28.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Employee/davolio.jpg
--rw-r--r--   0 val        (502) staff       (20)     5404 2008-04-22 03:51:58.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Employee/dodsworth.jpg
--rw-r--r--   0 val        (502) staff       (20)     3778 2008-04-22 03:51:40.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Employee/fuller.jpg
--rw-r--r--   0 val        (502) staff       (20)     3737 2008-04-22 03:50:00.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Employee/king.jpg
--rw-r--r--   0 val        (502) staff       (20)     3750 2008-04-22 03:48:16.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Employee/leverling.jpg
--rw-r--r--   0 val        (502) staff       (20)     3862 2008-04-22 03:48:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Employee/peacock.jpg
--rw-r--r--   0 val        (502) staff       (20)     4375 2008-04-22 03:49:14.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Employee/suyama.jpg
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.752574 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw_no_cust/
--rw-r--r--   0 val        (502) staff       (20)     5431 2023-02-05 02:51:56.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw_no_cust/readme.md
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.754309 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/
--rw-r--r--   0 val        (502) staff       (20)     6148 2023-02-14 06:04:24.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.DS_Store
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.755904 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.devcontainer/
--rw-r--r--   0 val        (502) staff       (20)      446 2023-02-05 02:55:30.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.devcontainer/For_VSCode.dockerfile
--rw-r--r--   0 val        (502) staff       (20)     1932 2023-02-05 02:52:45.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.devcontainer/devcontainer.json
--rw-r--r--   0 val        (502) staff       (20)      288 2023-01-25 20:14:39.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.devcontainer/setup.sh
--rw-r--r--   0 val        (502) staff       (20)      215 2023-01-25 20:14:39.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.gitignore
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.756150 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.idea/
--rw-r--r--   0 val        (502) staff       (20)     6148 2023-02-14 06:05:31.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.idea/.DS_Store
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.758823 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.idea/runConfigurations/
--rw-r--r--   0 val        (502) staff       (20)     6148 2023-02-14 05:30:57.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.idea/runConfigurations/.DS_Store
--rw-r--r--   0 val        (502) staff       (20)     1141 2023-02-14 05:35:26.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.idea/runConfigurations/1__Basic_App.xml
--rw-r--r--   0 val        (502) staff       (20)     1162 2023-02-14 05:07:31.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.idea/runConfigurations/2__ApiLogicProject.xml
--rw-r--r--   0 val        (502) staff       (20)     1174 2023-02-14 05:17:54.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.idea/runConfigurations/3__ApiLogicProject_Logic.xml
--rw-r--r--   0 val        (502) staff       (20)     1148 2023-02-14 05:35:26.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Execute_chinook.xml
--rw-r--r--   0 val        (502) staff       (20)     1160 2023-02-14 05:35:26.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Execute_classicmodels.xml
--rw-r--r--   0 val        (502) staff       (20)     1142 2023-02-14 05:16:08.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Execute_todo.xml
--rw-r--r--   0 val        (502) staff       (20)     1204 2023-02-14 05:54:42.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Run_Behave.xml
--rw-r--r--   0 val        (502) staff       (20)     1386 2023-02-14 05:54:42.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Run_Behave_Logic_Report.xml
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.759488 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.vscode/
--rw-r--r--   0 val        (502) staff       (20)     5986 2023-04-13 16:51:25.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.vscode/launch.json
--rw-r--r--   0 val        (502) staff       (20)      100 2023-01-25 20:14:39.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.vscode/settings.json
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.761554 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/
--rw-r--r--   0 val        (502) staff       (20)     6148 2023-02-27 01:16:56.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/.DS_Store
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.762950 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/
--rw-r--r--   0 val        (502) staff       (20)     1238 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/config.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     3435 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/flask.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     3970 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/flask_basic.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     3439 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/raw_flask.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     5965 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/util.cpython-310.pyc
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.763099 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/api/
--rw-r--r--   0 val        (502) staff       (20)     2895 2023-02-28 05:23:15.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/api/end_points.py
--rw-r--r--   0 val        (502) staff       (20)     2058 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/config.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.764738 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.765018 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/__pycache__/
--rw-r--r--   0 val        (502) staff       (20)     8571 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/__pycache__/models.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)   522240 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/db.sqlite
--rw-r--r--   0 val        (502) staff       (20)     1400 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/logging.yml
--rw-r--r--   0 val        (502) staff       (20)    11838 2023-01-28 17:14:40.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/models.py
--rw-r--r--   0 val        (502) staff       (20)     1452 2023-02-27 23:00:55.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/flask_basic.py
--rw-r--r--   0 val        (502) staff       (20)     1400 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/logging.yml
--rw-r--r--   0 val        (502) staff       (20)     3530 2023-02-28 05:20:39.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/readme.md
--rw-r--r--   0 val        (502) staff       (20)     7699 2023-02-13 15:35:11.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/util.py
--rw-r--r--   0 val        (502) staff       (20)    21134 2023-04-14 00:57:12.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/readme.md
--rw-r--r--   0 val        (502) staff       (20)       14 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/requirements.txt
--rw-r--r--   0 val        (502) staff       (20)   522240 2023-04-02 02:53:45.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/sample_db.sqlite
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.766602 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/
--rw-r--r--   0 val        (502) staff       (20)     6148 2023-01-22 18:56:43.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/.DS_Store
--rw-r--r--   0 val        (502) staff       (20)      369 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/Readme.md
--rw-r--r--   0 val        (502) staff       (20)        0 2023-01-03 23:29:33.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.768327 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/
--rw-r--r--   0 val        (502) staff       (20)      175 2023-01-03 23:29:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)      191 2023-02-26 22:48:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 val        (502) staff       (20)     8054 2022-11-17 03:31:49.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/expose_existing_callable.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)    14080 2023-02-17 01:02:20.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/sqlacodegen_wrapper.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)    21445 2023-04-29 17:29:36.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/sqlacodegen_wrapper.cpython-311.pyc
--rw-r--r--   0 val        (502) staff       (20)     1755 2023-02-01 19:08:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/uri_info.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)    53944 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/console_log.txt
--rw-r--r--   0 val        (502) staff       (20)       54 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/requirements.txt
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.769702 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/
--rw-r--r--   0 val        (502) staff       (20)     1850 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/.travis.yml
--rw-r--r--   0 val        (502) staff       (20)     2593 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/CHANGES.rst
--rw-r--r--   0 val        (502) staff       (20)     3865 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/README.rst
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.770127 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/__pycache__/
--rw-r--r--   0 val        (502) staff       (20)      183 2022-08-15 21:21:51.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)      203 2023-02-26 22:48:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 val        (502) staff       (20)       87 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/pyproject.toml
--rw-r--r--   0 val        (502) staff       (20)     1399 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/setup.cfg
--rw-r--r--   0 val        (502) staff       (20)      196 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/setup.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.771042 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.772280 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/
--rw-r--r--   0 val        (502) staff       (20)      195 2022-08-15 21:21:51.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)      215 2023-02-26 22:48:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 val        (502) staff       (20)    32358 2023-02-05 16:19:43.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/codegen.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)    74447 2023-04-06 14:36:23.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/codegen.cpython-311.pyc
--rw-r--r--   0 val        (502) staff       (20)    58988 2023-04-06 14:31:39.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/codegen.py
--rw-r--r--   0 val        (502) staff       (20)     3252 2022-11-18 19:19:33.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/main.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.772893 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/tests/
--rw-r--r--   0 val        (502) staff       (20)    33384 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/tests/test_codegen.py
--rw-r--r--   0 val        (502) staff       (20)      440 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/tox.ini
--rwxr-xr-x   0 val        (502) staff       (20)    17236 2023-04-29 17:29:32.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen_wrapper.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.775255 ApiLogicServer-8.3.3/api_logic_server_cli/templates/
--rw-r--r--   0 val        (502) staff       (20)    14864 2023-03-29 21:47:30.000000 ApiLogicServer-8.3.3/api_logic_server_cli/templates/admin.yaml
--rw-r--r--   0 val        (502) staff       (20)     1221 2023-03-29 20:25:21.000000 ApiLogicServer-8.3.3/api_logic_server_cli/templates/app_fiddle.md
--rw-r--r--   0 val        (502) staff       (20)     3322 2023-04-13 17:12:40.000000 ApiLogicServer-8.3.3/api_logic_server_cli/templates/app_fiddle.txt
--rw-r--r--   0 val        (502) staff       (20)     3765 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/templates/index.html
--rw-r--r--   0 val        (502) staff       (20)      900 2023-01-19 01:43:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/templates/login_endpoint.txt
--rw-r--r--   0 val        (502) staff       (20)      205 2023-01-19 01:44:07.000000 ApiLogicServer-8.3.3/api_logic_server_cli/templates/login_endpoint_imports.txt
--rw-r--r--   0 val        (502) staff       (20)       38 2023-04-29 22:01:05.776079 ApiLogicServer-8.3.3/setup.cfg
--rw-r--r--   0 val        (502) staff       (20)     3521 2023-04-26 19:16:06.000000 ApiLogicServer-8.3.3/setup.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.728937 ApiLogicServer-8.3.6/
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.507710 ApiLogicServer-8.3.6/ApiLogicServer.egg-info/
+-rw-r--r--   0 val        (502) staff       (20)    14816 2023-05-02 04:14:08.000000 ApiLogicServer-8.3.6/ApiLogicServer.egg-info/PKG-INFO
+-rw-r--r--   0 val        (502) staff       (20)    54435 2023-05-02 04:14:08.000000 ApiLogicServer-8.3.6/ApiLogicServer.egg-info/SOURCES.txt
+-rw-r--r--   0 val        (502) staff       (20)        1 2023-05-02 04:14:08.000000 ApiLogicServer-8.3.6/ApiLogicServer.egg-info/dependency_links.txt
+-rw-r--r--   0 val        (502) staff       (20)       66 2023-05-02 04:14:08.000000 ApiLogicServer-8.3.6/ApiLogicServer.egg-info/entry_points.txt
+-rw-r--r--   0 val        (502) staff       (20)        1 2023-05-02 04:14:08.000000 ApiLogicServer-8.3.6/ApiLogicServer.egg-info/not-zip-safe
+-rw-r--r--   0 val        (502) staff       (20)      585 2023-05-02 04:14:08.000000 ApiLogicServer-8.3.6/ApiLogicServer.egg-info/requires.txt
+-rw-r--r--   0 val        (502) staff       (20)       21 2023-05-02 04:14:08.000000 ApiLogicServer-8.3.6/ApiLogicServer.egg-info/top_level.txt
+-rw-r--r--   0 val        (502) staff       (20)     1485 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/LICENSE
+-rw-r--r--   0 val        (502) staff       (20)      804 2023-05-02 03:36:56.000000 ApiLogicServer-8.3.6/MANIFEST.in
+-rw-r--r--   0 val        (502) staff       (20)    14816 2023-05-02 04:14:08.728664 ApiLogicServer-8.3.6/PKG-INFO
+-rw-r--r--   0 val        (502) staff       (20)    13827 2023-05-02 04:03:01.000000 ApiLogicServer-8.3.6/README.md
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.509731 ApiLogicServer-8.3.6/api_logic_server_cli/
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/__init__.py
+-rw-r--r--   0 val        (502) staff       (20)    60440 2023-05-02 04:02:22.000000 ApiLogicServer-8.3.6/api_logic_server_cli/api_logic_server.py
+-rw-r--r--   0 val        (502) staff       (20)      124 2023-05-02 04:11:59.000000 ApiLogicServer-8.3.6/api_logic_server_cli/api_logic_server_info.yaml
+-rw-r--r--   0 val        (502) staff       (20)    33430 2023-03-10 20:22:39.000000 ApiLogicServer-8.3.6/api_logic_server_cli/cli.py
+-rw-r--r--   0 val        (502) staff       (20)     1001 2023-04-02 18:24:38.000000 ApiLogicServer-8.3.6/api_logic_server_cli/cli_args_base.py
+-rw-r--r--   0 val        (502) staff       (20)     3184 2023-04-02 23:08:24.000000 ApiLogicServer-8.3.6/api_logic_server_cli/cli_args_project.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.512921 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/
+-rw-r--r--   0 val        (502) staff       (20)    10244 2023-01-26 18:43:59.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/.DS_Store
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-11-10 15:34:44.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.517871 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__pycache__/
+-rw-r--r--   0 val        (502) staff       (20)      173 2022-11-10 15:35:23.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)      189 2023-02-26 22:48:45.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 val        (502) staff       (20)     2601 2022-11-18 17:28:18.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__pycache__/api_expose_api_models.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     3049 2023-02-05 16:19:43.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__pycache__/api_expose_api_models_creator.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     5300 2023-02-26 23:03:43.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__pycache__/api_expose_api_models_creator.cpython-311.pyc
+-rw-r--r--   0 val        (502) staff       (20)     7174 2023-02-10 20:33:17.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__pycache__/api_logic_server_utils.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)    13709 2023-05-02 02:08:40.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__pycache__/api_logic_server_utils.cpython-311.pyc
+-rw-r--r--   0 val        (502) staff       (20)    21342 2023-02-05 16:19:42.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__pycache__/model_creation_services.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)    35378 2023-02-26 22:48:45.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__pycache__/model_creation_services.cpython-311.pyc
+-rw-r--r--   0 val        (502) staff       (20)     4053 2023-01-18 01:12:07.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__pycache__/multi_db_utils.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)    20087 2023-02-05 19:25:01.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__pycache__/ui_admin_creator.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)    37019 2023-02-26 23:03:43.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__pycache__/ui_admin_creator.cpython-311.pyc
+-rw-r--r--   0 val        (502) staff       (20)     2274 2023-02-26 20:50:53.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__pycache__/uri_info.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     2617 2023-03-12 04:54:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__pycache__/uri_info.cpython-311.pyc
+-rw-r--r--   0 val        (502) staff       (20)     5290 2023-02-05 02:48:17.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/api_expose_api_models_creator.py
+-rw-r--r--   0 val        (502) staff       (20)    11680 2023-05-02 02:02:21.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/api_logic_server_utils.py
+-rw-r--r--   0 val        (502) staff       (20)    34401 2023-02-05 02:48:22.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/model_creation_services.py
+-rw-r--r--   0 val        (502) staff       (20)     6127 2023-01-18 01:12:06.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/multi_db_utilsZZ.txt
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.519954 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2023-01-22 18:56:43.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/.DS_Store
+-rwxrwxrwx   0 val        (502) staff       (20)    15430 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/asset-manifest.json
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.520143 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/data/
+-rwxrwxrwx   0 val        (502) staff       (20)  1145966 2023-01-15 08:58:09.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/data/customer.json
+-rwxrwxrwx   0 val        (502) staff       (20)     3870 2023-01-15 08:58:09.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/favicon.ico
+-rwxrwxrwx   0 val        (502) staff       (20)      692 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/index.html
+-rwxrwxrwx   0 val        (502) staff       (20)     5347 2023-01-15 08:58:09.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/logo192.png
+-rwxrwxrwx   0 val        (502) staff       (20)     9664 2023-01-15 08:58:09.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/logo512.png
+-rwxrwxrwx   0 val        (502) staff       (20)      492 2023-01-15 08:58:09.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/manifest.json
+-rwxrwxrwx   0 val        (502) staff       (20)       67 2023-01-15 08:58:09.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/robots.txt
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.499500 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.522549 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/
+-rwxrwxrwx   0 val        (502) staff       (20)    86781 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/695.2b02568d.chunk.css
+-rwxrwxrwx   0 val        (502) staff       (20)   166928 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/695.2b02568d.chunk.css.map
+-rwxrwxrwx   0 val        (502) staff       (20)      211 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/main.a0c288b7.css
+-rwxrwxrwx   0 val        (502) staff       (20)      516 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/main.a0c288b7.css.map
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.602635 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/
+-rwxrwxrwx   0 val        (502) staff       (20)     1576 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1022.0747a719.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1022.0747a719.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     3197 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1022.0747a719.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     9011 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1062.9e2b1e6c.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)    21905 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1062.9e2b1e6c.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2921 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1069.16bec71d.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1069.16bec71d.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     7103 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1069.16bec71d.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     1004 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1074.2c3d927c.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1074.2c3d927c.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     2792 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1074.2c3d927c.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     7546 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1251.10ac0097.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1251.10ac0097.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    17381 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1251.10ac0097.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)    33520 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1258.94dead34.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)    71153 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1258.94dead34.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)    14043 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1295.179239a3.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)    36857 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1295.179239a3.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     5595 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1324.be7507c8.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)    14138 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1324.be7507c8.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     6135 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1431.d02260cd.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1431.d02260cd.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    14288 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1431.d02260cd.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2280 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1532.41e3c0c8.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1532.41e3c0c8.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     5953 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1532.41e3c0c8.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3747 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1619.31b6d6e8.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1619.31b6d6e8.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     8068 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1619.31b6d6e8.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     4407 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1690.e74e47c3.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1690.e74e47c3.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    10552 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1690.e74e47c3.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2156 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1989.ee922c62.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1989.ee922c62.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     5783 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1989.ee922c62.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)    11957 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2154.5c399961.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2154.5c399961.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    24504 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2154.5c399961.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     5499 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2402.e66e47e8.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2402.e66e47e8.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    13356 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2402.e66e47e8.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     4187 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2478.4e6b45fa.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)    10856 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2478.4e6b45fa.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     7001 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2526.c4309069.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)    17447 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2526.c4309069.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3591 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/254.1bc22866.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/254.1bc22866.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     8746 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/254.1bc22866.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3747 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2611.8815ae2b.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2611.8815ae2b.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     9475 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2611.8815ae2b.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3140 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2880.029aa44e.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2880.029aa44e.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     7634 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2880.029aa44e.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     4056 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2900.14a00390.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2900.14a00390.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     9168 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2900.14a00390.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     8184 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2909.28b39275.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2909.28b39275.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    18882 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2909.28b39275.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     4068 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3003.57cfe277.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3003.57cfe277.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     9104 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3003.57cfe277.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)    14317 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/312.3d69e408.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/312.3d69e408.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    32894 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/312.3d69e408.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3963 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3126.99b58416.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3126.99b58416.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     9547 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3126.99b58416.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3152 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3323.b47b9b1e.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3323.b47b9b1e.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     8052 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3323.b47b9b1e.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     8662 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3668.cd0becc2.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3668.cd0becc2.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    20172 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3668.cd0becc2.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     4982 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/369.0237ca8c.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/369.0237ca8c.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    13442 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/369.0237ca8c.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     6569 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3698.750e43d6.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3698.750e43d6.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    15183 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3698.750e43d6.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2002 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3766.d8eddcd9.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3766.d8eddcd9.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     4736 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3766.d8eddcd9.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2974 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3907.7b2efd62.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3907.7b2efd62.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     7499 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3907.7b2efd62.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     1967 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3955.f5434704.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3955.f5434704.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     5172 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3955.f5434704.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     5948 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4040.613bd8c0.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4040.613bd8c0.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    13558 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4040.613bd8c0.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)    10454 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4333.61aa216a.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4333.61aa216a.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    23458 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4333.61aa216a.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     1255 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/464.522c11f6.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/464.522c11f6.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     3229 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/464.522c11f6.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     4128 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4877.7cebca37.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4877.7cebca37.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    10303 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4877.7cebca37.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)    17096 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4900.19572072.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4900.19572072.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    31009 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4900.19572072.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     7760 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4969.ccedbf9b.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4969.ccedbf9b.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    18142 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4969.ccedbf9b.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     9800 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5133.71af5a54.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5133.71af5a54.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    21207 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5133.71af5a54.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3420 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/52.22a03ee6.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/52.22a03ee6.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     8828 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/52.22a03ee6.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3820 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5328.77d62d48.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)    10430 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5328.77d62d48.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)    41393 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5342.e36bdc43.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)   145206 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5342.e36bdc43.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     5605 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5419.3d10c516.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5419.3d10c516.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    13185 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5419.3d10c516.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     8412 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5507.c29076d8.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5507.c29076d8.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    19971 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5507.c29076d8.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     9916 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5540.d957a974.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5540.d957a974.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    22155 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5540.d957a974.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     6545 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5558.d0dc5575.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5558.d0dc5575.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    16602 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5558.d0dc5575.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     4681 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5571.ad570057.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5571.ad570057.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    11819 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5571.ad570057.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3545 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5672.f0c2440f.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5672.f0c2440f.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     8963 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5672.f0c2440f.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3710 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/608.84469af3.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/608.84469af3.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     9146 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/608.84469af3.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     1924 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6289.a7c21fba.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6289.a7c21fba.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     4864 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6289.a7c21fba.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     5069 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6304.ce792f5f.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6304.ce792f5f.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    11830 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6304.ce792f5f.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3092 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6384.8f33f789.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6384.8f33f789.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     8217 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6384.8f33f789.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2417 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6403.77f38472.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6403.77f38472.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     6013 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6403.77f38472.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     7472 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/651.bf520a75.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/651.bf520a75.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    16988 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/651.bf520a75.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2342 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6717.805e1882.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6717.805e1882.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     6267 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6717.805e1882.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)  3310604 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      576 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20) 10838575 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)    35620 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6965.381dbe04.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)   121512 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6965.381dbe04.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)    17547 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7117.b2e9eb70.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)    39845 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7117.b2e9eb70.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2594 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7294.6813eb1f.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7294.6813eb1f.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     6567 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7294.6813eb1f.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2814 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7299.20100701.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7299.20100701.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     7255 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7299.20100701.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)    18754 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7436.4e91a3a5.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7436.4e91a3a5.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    38065 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7436.4e91a3a5.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2736 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7497.f56048e1.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7497.f56048e1.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     7008 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7497.f56048e1.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2693 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7499.b216e9da.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7499.b216e9da.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     6865 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7499.b216e9da.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3378 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7615.f5af9bae.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7615.f5af9bae.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     8159 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7615.f5af9bae.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2709 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7713.6d02efa2.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7713.6d02efa2.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     6645 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7713.6d02efa2.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     4619 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/787.d5293104.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)    10592 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/787.d5293104.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     4203 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7894.f8f70466.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)    10608 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7894.f8f70466.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2559 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7952.29e2c950.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7952.29e2c950.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     6522 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7952.29e2c950.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     5926 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8184.741e3d56.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)    96741 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8184.741e3d56.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     1840 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8272.99aef5a5.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8272.99aef5a5.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     5116 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8272.99aef5a5.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     8013 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8347.649393e6.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8347.649393e6.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    19497 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8347.649393e6.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3725 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/839.87662037.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/839.87662037.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     9025 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/839.87662037.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3288 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8501.ea0cd3a2.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8501.ea0cd3a2.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     8254 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8501.ea0cd3a2.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2026 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8861.01a110f5.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8861.01a110f5.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     5528 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8861.01a110f5.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)    13558 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/907.7b650179.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/907.7b650179.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    26650 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/907.7b650179.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     9201 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9186.73a41896.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9186.73a41896.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    21765 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9186.73a41896.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     5069 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9200.d0bc8746.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9200.d0bc8746.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    11826 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9200.d0bc8746.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)    34921 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9214.5198dfc3.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)   119930 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9214.5198dfc3.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     4669 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9335.43329da2.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9335.43329da2.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    10814 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9335.43329da2.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     4316 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9357.e2f466b8.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9357.e2f466b8.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    10868 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9357.e2f466b8.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)    11414 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9361.e7bbdd03.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9361.e7bbdd03.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    24817 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9361.e7bbdd03.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2622 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9381.9495a14c.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)     7016 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9381.9495a14c.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     5259 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9432.e84dc193.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)    13615 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9432.e84dc193.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     7391 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9687.e1a38d25.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9687.e1a38d25.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    17258 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9687.e1a38d25.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     1986 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9845.3bb55d3c.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9845.3bb55d3c.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     4960 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9845.3bb55d3c.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3230 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9902.bfcd7f60.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9902.bfcd7f60.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     8177 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9902.bfcd7f60.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)  1384276 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js
+-rwxrwxrwx   0 val        (502) staff       (20)     3014 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)  5552838 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js.map
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.607377 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/media/
+-rwxrwxrwx   0 val        (502) staff       (20)    72504 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/media/codicon.b797181c93b3755f4fa1.ttf
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.613021 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.613691 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/basic_web_app/
+-rw-r--r--   0 val        (502) staff       (20)       55 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/basic_web_app/.gitignore
+-rw-r--r--   0 val        (502) staff       (20)      389 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/basic_web_app/README.rst
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.614189 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/basic_web_app/app/
+-rw-r--r--   0 val        (502) staff       (20)      742 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/basic_web_app/app/__init__.py
+-rw-r--r--   0 val        (502) staff       (20)      276 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/basic_web_app/app/models.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.614374 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/basic_web_app/app/templates/
+-rw-r--r--   0 val        (502) staff       (20)      124 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/basic_web_app/app/templates/404.html
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.499833 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.499878 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/pt/
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.614743 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 val        (502) staff       (20)      483 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 val        (502) staff       (20)      727 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 val        (502) staff       (20)      938 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/basic_web_app/app/views.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.615321 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/basic_web_app/babel/
+-rw-r--r--   0 val        (502) staff       (20)       64 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/basic_web_app/babel/babel.cfg
+-rw-r--r--   0 val        (502) staff       (20)      662 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/basic_web_app/babel/messages.pot
+-rw-r--r--   0 val        (502) staff       (20)     3669 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/basic_web_app/config.py
+-rw-r--r--   0 val        (502) staff       (20)       68 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/basic_web_app/run.py
+-rw-r--r--   0 val        (502) staff       (20)      556 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/create_admin.sh
+-rw-r--r--   0 val        (502) staff       (20)      624 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/fab_config.py
+-rw-r--r--   0 val        (502) staff       (20)     2683 2023-02-05 02:49:11.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/home.js
+-rw-r--r--   0 val        (502) staff       (20)     3121 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/react_admin_component.js
+-rw-r--r--   0 val        (502) staff       (20)    35694 2023-02-05 19:24:16.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/ui_admin_creator.py
+-rw-r--r--   0 val        (502) staff       (20)     2252 2023-03-12 01:14:25.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/uri_info.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.638965 ApiLogicServer-8.3.6/api_logic_server_cli/database/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2022-12-22 22:39:55.000000 ApiLogicServer-8.3.6/api_logic_server_cli/database/.DS_Store
+-rw-r--r--   0 val        (502) staff       (20)  1067008 2022-10-11 15:13:39.000000 ApiLogicServer-8.3.6/api_logic_server_cli/database/Chinook_Sqlite.sqlite
+-rw-r--r--   0 val        (502) staff       (20)       60 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/database/__init__.py
+-rw-r--r--   0 val        (502) staff       (20)   545792 2023-05-02 01:22:02.000000 ApiLogicServer-8.3.6/api_logic_server_cli/database/allocation.sqlite
+-rw-r--r--   0 val        (502) staff       (20)    45056 2023-01-19 01:03:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/database/authentication.sqlite
+-rw-r--r--   0 val        (502) staff       (20)   413696 2022-12-26 21:41:55.000000 ApiLogicServer-8.3.6/api_logic_server_cli/database/classicmodels.sqlite
+-rw-r--r--   0 val        (502) staff       (20)      122 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/database/customize_models.py
+-rw-r--r--   0 val        (502) staff       (20)    16384 2023-03-07 00:17:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/database/new.sqlite
+-rw-r--r--   0 val        (502) staff       (20)   522240 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/database/nw-gold-plus.sqlite
+-rw-r--r--   0 val        (502) staff       (20)   522240 2023-03-19 18:51:02.000000 ApiLogicServer-8.3.6/api_logic_server_cli/database/nw-gold.sqlite
+-rw-r--r--   0 val        (502) staff       (20)   496640 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/database/nw.sqlite
+-rw-r--r--   0 val        (502) staff       (20)    32768 2023-03-08 04:23:41.000000 ApiLogicServer-8.3.6/api_logic_server_cli/database/table_filters_tests.sqlite
+-rw-r--r--   0 val        (502) staff       (20)       53 2023-03-08 15:53:51.000000 ApiLogicServer-8.3.6/api_logic_server_cli/database/table_filters_tests.yml
+-rw-r--r--   0 val        (502) staff       (20)       23 2023-04-06 03:07:09.000000 ApiLogicServer-8.3.6/api_logic_server_cli/database/table_filters_tests_nw.yml
+-rw-r--r--   0 val        (502) staff       (20)       25 2023-04-06 03:06:34.000000 ApiLogicServer-8.3.6/api_logic_server_cli/database/table_filters_tests_nw_1.yml
+-rw-r--r--   0 val        (502) staff       (20)       21 2023-03-14 16:06:21.000000 ApiLogicServer-8.3.6/api_logic_server_cli/database/table_filters_tests_typical.yml
+-rw-r--r--   0 val        (502) staff       (20)    16384 2022-12-31 01:13:31.000000 ApiLogicServer-8.3.6/api_logic_server_cli/database/todos.sqlite
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.656863 ApiLogicServer-8.3.6/api_logic_server_cli/docs/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2023-01-22 18:56:43.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/.DS_Store
+-rw-r--r--   0 val        (502) staff       (20)     1251 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/API-Customize.md
+-rw-r--r--   0 val        (502) staff       (20)     2647 2022-12-29 01:51:24.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/API.md
+-rw-r--r--   0 val        (502) staff       (20)     3222 2022-12-21 16:33:05.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Admin-Customization.md
+-rw-r--r--   0 val        (502) staff       (20)    18275 2023-03-10 04:52:51.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Admin-Tour.md
+-rw-r--r--   0 val        (502) staff       (20)      384 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Architecture-What-Is.md
+-rw-r--r--   0 val        (502) staff       (20)    12713 2022-11-22 02:48:15.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Architecture.md
+-rw-r--r--   0 val        (502) staff       (20)    61944 2022-10-11 03:42:54.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Behave-Logic-Report.md
+-rw-r--r--   0 val        (502) staff       (20)     3838 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Behave.md
+-rw-r--r--   0 val        (502) staff       (20)     1994 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Create-ApiLogicProject.md
+-rw-r--r--   0 val        (502) staff       (20)     5319 2022-12-21 20:29:28.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Data-Model-Classes.md
+-rw-r--r--   0 val        (502) staff       (20)     2660 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Data-Model-Customization.md
+-rw-r--r--   0 val        (502) staff       (20)     1114 2023-01-27 04:14:44.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Data-Model-Examples.md
+-rw-r--r--   0 val        (502) staff       (20)      970 2022-10-03 02:15:43.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Data-Model-Keys.md
+-rw-r--r--   0 val        (502) staff       (20)     3898 2023-01-06 02:59:38.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Data-Model-Multi.md
+-rw-r--r--   0 val        (502) staff       (20)    13193 2023-03-12 01:14:31.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Database-Connectivity.md
+-rw-r--r--   0 val        (502) staff       (20)     1241 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Execute.md
+-rw-r--r--   0 val        (502) staff       (20)     3273 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/FAQ-Frameworks.md
+-rw-r--r--   0 val        (502) staff       (20)      527 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/FAQ-Low-Code.md
+-rw-r--r--   0 val        (502) staff       (20)     7036 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/FAQ-RETE.md
+-rw-r--r--   0 val        (502) staff       (20)     1851 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/IDE-Customize.md
+-rw-r--r--   0 val        (502) staff       (20)     7532 2023-01-20 15:50:43.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/IDE-Execute.md
+-rw-r--r--   0 val        (502) staff       (20)     6368 2023-02-04 01:50:40.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Install-Eval-x.md
+-rw-r--r--   0 val        (502) staff       (20)     8093 2023-01-09 21:17:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Install-Eval.md
+-rw-r--r--   0 val        (502) staff       (20)     3390 2023-02-03 23:28:34.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Install-Express-x.md
+-rw-r--r--   0 val        (502) staff       (20)     3539 2022-08-23 15:56:25.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Install-Express.md
+-rw-r--r--   0 val        (502) staff       (20)      566 2022-11-30 17:57:34.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Install-psycopg2.md
+-rw-r--r--   0 val        (502) staff       (20)      977 2022-11-17 04:40:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Install-pyodbc.md
+-rw-r--r--   0 val        (502) staff       (20)     7135 2022-09-18 04:42:29.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Install.md
+-rw-r--r--   0 val        (502) staff       (20)    13448 2023-02-05 02:54:14.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Internals-CLI.md
+-rw-r--r--   0 val        (502) staff       (20)     6504 2022-12-01 16:51:37.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Internals.md
+-rw-r--r--   0 val        (502) staff       (20)     3258 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Logic-Operation.md
+-rw-r--r--   0 val        (502) staff       (20)    14729 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Logic-Tutorial.md
+-rw-r--r--   0 val        (502) staff       (20)    10325 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Logic-Why.md
+-rw-r--r--   0 val        (502) staff       (20)     3707 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Logic.md
+-rw-r--r--   0 val        (502) staff       (20)     4205 2022-08-28 15:23:33.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Manage-GitHub.md
+-rw-r--r--   0 val        (502) staff       (20)     3796 2022-12-28 03:43:06.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Project-Builders.md
+-rw-r--r--   0 val        (502) staff       (20)     1957 2022-12-22 04:40:03.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Project-DevOps.md
+-rw-r--r--   0 val        (502) staff       (20)     1930 2023-01-31 22:36:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Project-Env.md
+-rw-r--r--   0 val        (502) staff       (20)     4936 2022-11-24 20:38:40.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Project-Execution.md
+-rw-r--r--   0 val        (502) staff       (20)     2446 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Project-Rebuild.md
+-rw-r--r--   0 val        (502) staff       (20)     2104 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Project-Structure.md
+-rw-r--r--   0 val        (502) staff       (20)      773 2022-09-18 04:42:29.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Sample-Database.md
+-rw-r--r--   0 val        (502) staff       (20)     2227 2023-02-14 23:54:00.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Security-Activation.md
+-rw-------   0 val        (502) staff       (20)     1585 2023-01-21 01:47:08.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Security-Authentication-Provider.md
+-rw-------   0 val        (502) staff       (20)     1470 2023-01-21 02:17:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Security-Authentication.md
+-rw-r--r--   0 val        (502) staff       (20)     1922 2023-01-06 17:06:26.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Security-Authorization.md
+-rw-r--r--   0 val        (502) staff       (20)     5277 2023-01-21 01:31:32.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Security-Overview.md
+-rw-r--r--   0 val        (502) staff       (20)      155 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Tech--Notes.md
+-rw-r--r--   0 val        (502) staff       (20)      237 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Tech-4GL.md
+-rw-r--r--   0 val        (502) staff       (20)     7081 2022-11-24 00:40:19.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Tech-CodeSpaces.md
+-rw-r--r--   0 val        (502) staff       (20)     3053 2022-12-06 21:43:43.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Tech-Conference-PyCon23-Talk.md
+-rw-r--r--   0 val        (502) staff       (20)     3174 2022-12-06 18:38:49.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Tech-Conference-PyCon23-Tutorial.md
+-rw-r--r--   0 val        (502) staff       (20)     5693 2022-12-05 19:50:10.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Tech-Conference.md
+-rw-r--r--   0 val        (502) staff       (20)     3385 2022-11-07 18:45:42.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Tech-Docker.md
+-rw-r--r--   0 val        (502) staff       (20)      815 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Tech-Install-Python.md
+-rw-r--r--   0 val        (502) staff       (20)     1049 2022-10-03 16:52:30.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Tech-Proven.md
+-rw-r--r--   0 val        (502) staff       (20)     2679 2022-12-07 04:30:27.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Tech-Python-311.md
+-rw-r--r--   0 val        (502) staff       (20)     3728 2023-01-12 06:40:15.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Tech-Python.md
+-rw-r--r--   0 val        (502) staff       (20)     3019 2022-10-21 23:29:01.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Tech-m1.md
+-rw-r--r--   0 val        (502) staff       (20)     1644 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Tech-mkdocs-material.md
+-rw-r--r--   0 val        (502) staff       (20)    12291 2022-10-08 18:23:10.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Troubleshooting.md
+-rw-r--r--   0 val        (502) staff       (20)    15277 2023-04-27 02:31:04.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Tutorial.md
+-rw-r--r--   0 val        (502) staff       (20)     6697 2022-12-02 18:42:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Working-With-Docker.md
+-rw-r--r--   0 val        (502) staff       (20)     4031 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Working-with-Flask-AppBuilder.md
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.657168 ApiLogicServer-8.3.6/api_logic_server_cli/docs/assets/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2022-08-30 03:14:41.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/assets/.DS_Store
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.657694 ApiLogicServer-8.3.6/api_logic_server_cli/docs/assets/images/
+-rw-r--r--   0 val        (502) staff       (20)     2362 2022-08-29 00:06:15.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/assets/images/bulb-icon.svg
+-rw-r--r--   0 val        (502) staff       (20)     3482 2022-08-30 03:46:01.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/assets/images/lightbulb.svg
+-rw-r--r--   0 val        (502) staff       (20)    15440 2023-02-06 03:49:29.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/index.md
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.657946 ApiLogicServer-8.3.6/api_logic_server_cli/docs/stylesheets/
+-rw-r--r--   0 val        (502) staff       (20)      634 2022-08-30 03:44:15.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/stylesheets/extra.css
+-rw-r--r--   0 val        (502) staff       (20)    11824 2023-02-11 04:16:18.000000 ApiLogicServer-8.3.6/api_logic_server_cli/extended_builder.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.659685 ApiLogicServer-8.3.6/api_logic_server_cli/fragments/
+-rw-r--r--   0 val        (502) staff       (20)     1431 2023-02-05 02:48:13.000000 ApiLogicServer-8.3.6/api_logic_server_cli/fragments/Todo_modelsZZ.py.py
+-rw-r--r--   0 val        (502) staff       (20)     1956 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/fragments/configZZ.py
+-rw-r--r--   0 val        (502) staff       (20)       63 2022-10-01 16:17:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/fragments/db_typesZZ.txt
+-rw-r--r--   0 val        (502) staff       (20)    12053 2023-02-05 02:48:09.000000 ApiLogicServer-8.3.6/api_logic_server_cli/fragments/modelsZZ.py
+-rw-r--r--   0 val        (502) staff       (20)      888 2023-04-23 22:57:22.000000 ApiLogicServer-8.3.6/api_logic_server_cli/fragments/nw_virtual_attrs.py
+-rw-r--r--   0 val        (502) staff       (20)      870 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/fragments/ui_basic_web_app_runZZ.py
+-rw-r--r--   0 val        (502) staff       (20)     1006 2023-04-21 23:18:04.000000 ApiLogicServer-8.3.6/api_logic_server_cli/logging.yml
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.663139 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/
+-rw-r--r--   0 val        (502) staff       (20)    10244 2023-04-26 02:43:32.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.DS_Store
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.663923 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.devcontainer/
+-rw-r--r--   0 val        (502) staff       (20)      444 2023-02-05 02:50:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.devcontainer/For_VSCode.dockerfile
+-rw-r--r--   0 val        (502) staff       (20)     1932 2023-02-05 21:44:41.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.devcontainer/devcontainer.json
+-rw-r--r--   0 val        (502) staff       (20)      288 2023-01-08 18:52:09.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.devcontainer/setup.sh
+-rw-r--r--   0 val        (502) staff       (20)      106 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.gitignore
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.664187 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.idea/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2023-02-14 05:32:37.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.idea/.DS_Store
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.665917 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.idea/runConfigurations/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2023-02-14 05:32:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.idea/runConfigurations/.DS_Store
+-rw-r--r--   0 val        (502) staff       (20)     1127 2023-04-29 02:28:50.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.idea/runConfigurations/ApiLogicServer.xml
+-rw-r--r--   0 val        (502) staff       (20)     1306 2022-04-03 03:00:44.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.idea/runConfigurations/Report_Behave_Logic.xml
+-rw-r--r--   0 val        (502) staff       (20)     1196 2022-04-03 03:00:44.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.idea/runConfigurations/Run_Behave.xml
+-rw-r--r--   0 val        (502) staff       (20)     1205 2022-04-03 03:00:44.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.idea/runConfigurations/Windows_Run_Behave.xml
+-rw-r--r--   0 val        (502) staff       (20)     1193 2023-04-29 01:03:03.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.idea/runConfigurations/run___No_Security.xml
+-rw-r--r--   0 val        (502) staff       (20)     2444 2023-04-29 01:03:22.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.idea/runConfigurations/run_docker.xml
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.666439 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.vscode/
+-rw-r--r--   0 val        (502) staff       (20)     6518 2023-04-13 16:38:20.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.vscode/launch.json
+-rw-r--r--   0 val        (502) staff       (20)      437 2023-04-13 04:29:56.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.vscode/settings.json
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.667442 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/api/
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/api/__init__.py
+-rw-r--r--   0 val        (502) staff       (20)     2053 2023-04-26 02:48:17.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/api/customize_api.py
+-rw-r--r--   0 val        (502) staff       (20)      316 2023-01-23 01:07:06.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/api/expose_api_models.py
+-rw-r--r--   0 val        (502) staff       (20)      521 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/api/json_encoder.py
+-rw-r--r--   0 val        (502) staff       (20)     2689 2023-04-29 21:17:10.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/api/readme_customize_api.md
+-rw-r--r--   0 val        (502) staff       (20)    18920 2023-04-29 18:24:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/api_logic_server_run.py
+-rw-r--r--   0 val        (502) staff       (20)     3131 2023-03-03 16:08:15.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/config.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.668241 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/database/
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/database/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.669001 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/database/alembic/
+-rw-r--r--   0 val        (502) staff       (20)     2101 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/database/alembic/env.py
+-rw-r--r--   0 val        (502) staff       (20)     1967 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/database/alembic/readme.md
+-rw-r--r--   0 val        (502) staff       (20)      494 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/database/alembic/script.py.mako
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.669173 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/database/alembic/versions/
+-rw-r--r--   0 val        (502) staff       (20)       60 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/database/alembic/versions/readme.md
+-rw-r--r--   0 val        (502) staff       (20)     3027 2023-02-09 15:42:27.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/database/alembic.ini
+-rw-r--r--   0 val        (502) staff       (20)      537 2023-01-28 17:53:13.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/database/bind_databases.py
+-rw-r--r--   0 val        (502) staff       (20)      469 2023-01-23 01:14:38.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/database/customize_models.py
+-rw-r--r--   0 val        (502) staff       (20)      139 2022-12-21 03:23:43.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/default.env
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.669347 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/devops/
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.670416 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/devops/docker/
+-rw-r--r--   0 val        (502) staff       (20)     2381 2023-02-26 22:13:43.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/devops/docker/authdb_mysql.Dockerfile
+-rw-r--r--   0 val        (502) staff       (20)     3643 2023-02-25 03:16:21.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/devops/docker/authdb_mysql.sql
+-rw-r--r--   0 val        (502) staff       (20)      331 2023-04-02 15:52:20.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/devops/docker/build_image.dockerfile
+-rw-r--r--   0 val        (502) staff       (20)     2079 2023-04-02 16:35:31.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/devops/docker/build_image.sh
+-rw-r--r--   0 val        (502) staff       (20)      876 2023-01-07 21:19:34.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/devops/git_push_new_project.sh
+-rw-r--r--   0 val        (502) staff       (20)     1475 2023-04-21 23:01:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/logging.yml
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.670906 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/logic/
+-rw-r--r--   0 val        (502) staff       (20)      592 2023-04-26 02:47:32.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/logic/declare_logic.py
+-rw-r--r--   0 val        (502) staff       (20)     5953 2023-04-27 00:49:20.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/logic/readme_declare_logic.md
+-rw-r--r--   0 val        (502) staff       (20)      568 2023-03-04 03:52:49.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/mypy.ini
+-rw-r--r--   0 val        (502) staff       (20)     3820 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/python_anywhere_wsgi.py
+-rw-r--r--   0 val        (502) staff       (20)     7196 2023-05-01 21:36:23.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/readme.md
+-rw-r--r--   0 val        (502) staff       (20)       14 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/requirements.txt
+-rw-r--r--   0 val        (502) staff       (20)      801 2022-10-19 20:24:10.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/run.ps1
+-rwxr-xr-x   0 val        (502) staff       (20)     1040 2022-11-09 16:08:44.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/run.sh
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.671676 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2023-01-22 18:56:43.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/.DS_Store
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-12-15 01:50:41.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.672309 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2022-12-18 05:06:14.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/.DS_Store
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-12-14 21:51:49.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.674009 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/
+-rw-r--r--   0 val        (502) staff       (20)      173 2022-12-14 21:55:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)      928 2022-12-19 03:03:12.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/abstract_authentication_provider.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     1803 2022-12-18 03:38:13.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/authentication_models.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)      820 2022-12-16 14:20:29.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/db_auth.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     1392 2022-12-14 22:25:00.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/mem_auth.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     1024 2022-12-16 15:01:05.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/mem_auth_row.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     1619 2022-12-15 17:24:50.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/models.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)      580 2022-12-19 03:03:11.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/abstract_authentication_provider.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.674506 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/memory/
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.674759 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/memory/__pycache__/
+-rw-r--r--   0 val        (502) staff       (20)     1493 2022-12-19 03:13:00.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/memory/__pycache__/auth_provider.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     4355 2023-01-24 04:07:34.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/memory/auth_provider.py
+-rw-r--r--   0 val        (502) staff       (20)     2907 2023-01-24 04:07:34.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/memory/auth_provider_no_swagger.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.501621 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/sql/
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.675474 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/
+-rw-r--r--   0 val        (502) staff       (20)     1215 2022-12-19 03:24:21.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/auth_provider.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     2262 2022-12-19 00:39:44.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/authentication_models.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)      839 2022-12-18 03:49:32.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/db_auth.cpython-310.pyc
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.675708 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/sql/sqlite/
+-rw-r--r--   0 val        (502) staff       (20)     2165 2023-02-15 02:24:49.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/sql/sqlite/auth_provider.py
+-rw-r--r--   0 val        (502) staff       (20)      587 2023-01-23 01:02:25.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/declare_security.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.676388 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/notes_temp/
+-rw-r--r--   0 val        (502) staff       (20)     1403 2023-01-12 23:08:16.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/notes_temp/pip-freeze-th.txt
+-rw-r--r--   0 val        (502) staff       (20)     1156 2023-01-12 23:08:16.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/notes_temp/pip-freeze.txt
+-rw-r--r--   0 val        (502) staff       (20)     1364 2023-01-12 23:29:28.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/notes_temp/token.txt
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.677251 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/system/
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.677538 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/system/__pycache__/
+-rw-r--r--   0 val        (502) staff       (20)     4665 2022-12-19 03:03:12.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/system/__pycache__/security_manager.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     3425 2023-03-03 16:56:43.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/system/authentication.py
+-rw-r--r--   0 val        (502) staff       (20)     6004 2023-03-03 16:56:55.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/system/authorization.py
+-rw-r--r--   0 val        (502) staff       (20)     1705 2023-02-13 15:35:11.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/system/custom_swagger.json
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.677815 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/templates/
+-rw-r--r--   0 val        (502) staff       (20)     3765 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/templates/index.html
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.677966 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/test/
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/test/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.678483 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/test/api_logic_server_behave/
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/test/api_logic_server_behave/__init__.py
+-rw-r--r--   0 val        (502) staff       (20)     9969 2022-11-29 03:36:44.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/test/api_logic_server_behave/behave_logic_report.py
+-rw-r--r--   0 val        (502) staff       (20)     1026 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/test/api_logic_server_behave/behave_run.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.678660 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/
+-rw-r--r--   0 val        (502) staff       (20)      414 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/about.feature
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.679034 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/steps/
+-rw-r--r--   0 val        (502) staff       (20)      416 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/steps/about.py
+-rw-r--r--   0 val        (502) staff       (20)     1518 2023-02-11 17:50:21.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/steps/test_utils.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.679596 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/
+-rw-r--r--   0 val        (502) staff       (20)      147 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/Behave Logic Report Intro micro.md
+-rw-r--r--   0 val        (502) staff       (20)     3707 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/Behave Logic Report Intro.md
+-rw-r--r--   0 val        (502) staff       (20)    65295 2022-10-11 03:42:40.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/Behave Logic Report Sample.md
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.680395 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/test/basic/
+-rw-r--r--   0 val        (502) staff       (20)      735 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/test/basic/server_test.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.680927 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/
+-rw-r--r--   0 val        (502) staff       (20)    10244 2023-01-22 20:09:13.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/.DS_Store
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.681290 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/admin/
+-rw-r--r--   0 val        (502) staff       (20)     6671 2023-03-19 18:44:09.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/admin/admin_loader.py
+-rw-r--r--   0 val        (502) staff       (20)     2750 2023-02-05 02:50:52.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/admin/home.js
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.681550 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2022-11-26 23:48:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/.DS_Store
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.683307 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Employee/
+-rw-r--r--   0 val        (502) staff       (20)     3778 2008-04-22 03:51:40.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Employee/andrew.jpg
+-rw-r--r--   0 val        (502) staff       (20)     5404 2008-04-22 03:51:58.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Employee/anne.jpg
+-rw-r--r--   0 val        (502) staff       (20)     3750 2008-04-22 03:48:16.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Employee/janet.jpg
+-rw-r--r--   0 val        (502) staff       (20)     3715 2008-04-22 03:48:32.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Employee/laura.jpg
+-rw-r--r--   0 val        (502) staff       (20)     3862 2008-04-22 03:48:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Employee/margaret.jpg
+-rw-r--r--   0 val        (502) staff       (20)     4375 2008-04-22 03:49:14.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Employee/michael.jpg
+-rw-r--r--   0 val        (502) staff       (20)     4425 2008-04-22 03:49:28.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Employee/nancy.jpg
+-rw-r--r--   0 val        (502) staff       (20)     3737 2008-04-22 03:50:00.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Employee/robert.jpg
+-rw-r--r--   0 val        (502) staff       (20)     3719 2008-04-22 03:50:34.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Employee/steven.jpg
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.684635 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Product/
+-rw-r--r--   0 val        (502) staff       (20)     6054 2008-04-22 03:46:52.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Product/beverages.gif
+-rw-r--r--   0 val        (502) staff       (20)     7324 2008-04-22 03:47:14.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Product/cereals.gif
+-rw-r--r--   0 val        (502) staff       (20)     7751 2008-04-22 03:47:30.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Product/condiments.gif
+-rw-r--r--   0 val        (502) staff       (20)     7022 2008-04-22 03:47:44.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Product/confections.gif
+-rw-r--r--   0 val        (502) staff       (20)     6136 2008-04-22 03:47:58.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Product/diary.gif
+-rw-r--r--   0 val        (502) staff       (20)     7268 2008-04-22 03:49:00.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Product/meat.gif
+-rw-r--r--   0 val        (502) staff       (20)     7633 2008-04-22 03:49:44.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Product/produce.gif
+-rw-r--r--   0 val        (502) staff       (20)     8469 2008-04-22 03:50:18.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Product/seafood.gif
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.684784 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/templates/
+-rw-r--r--   0 val        (502) staff       (20)       26 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/templates/content.html
+-rw-r--r--   0 val        (502) staff       (20)     9076 2023-03-24 00:43:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/util.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.686333 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/venv_setup/
+-rwxr-xr-x   0 val        (502) staff       (20)     3116 2023-03-10 20:26:13.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/venv_setup/py.py
+-rw-r--r--   0 val        (502) staff       (20)      738 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/venv_setup/readme_venv.md
+-rw-r--r--   0 val        (502) staff       (20)      579 2023-03-03 02:36:32.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/venv_setup/requirements-no-cli.txt
+-rw-r--r--   0 val        (502) staff       (20)      900 2023-02-05 02:50:56.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/venv_setup/venv-linux.sh
+-rw-r--r--   0 val        (502) staff       (20)      698 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/venv_setup/venv.ps1
+-rw-r--r--   0 val        (502) staff       (20)      893 2023-02-05 02:50:58.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/venv_setup/venv.sh
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.686886 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_allocation/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2023-05-02 02:53:53.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_allocation/.DS_Store
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.688462 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_allocation/images/
+-rw-r--r--   0 val        (502) staff       (20)   670261 2023-05-02 02:18:30.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_allocation/images/db.png
+-rw-r--r--   0 val        (502) staff       (20)  1035433 2023-05-02 02:18:30.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_allocation/images/logic-diagram.png
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.689976 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_allocation/logic/
+-rw-r--r--   0 val        (502) staff       (20)     1398 2023-05-02 01:22:37.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_allocation/logic/declare_logic.py
+-rw-r--r--   0 val        (502) staff       (20)     7982 2023-05-02 04:11:55.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_allocation/readme-allocation.md
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.690104 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_allocation/test/
+-rw-r--r--   0 val        (502) staff       (20)      583 2023-05-02 01:22:37.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_allocation/test/test.sh
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.690670 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/
+-rw-r--r--   0 val        (502) staff       (20)    10244 2023-01-22 18:56:43.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/.DS_Store
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.690901 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/api/
+-rw-r--r--   0 val        (502) staff       (20)     8711 2023-02-13 15:35:11.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/api/customize_api.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.691691 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/api/multi-table-example/
+-rw-r--r--   0 val        (502) staff       (20)    34142 2023-04-29 21:00:10.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/api/multi-table-example/multi-table.json
+-rw-r--r--   0 val        (502) staff       (20)      650 2023-04-29 21:02:15.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/api/multi-table-example/multi-table.txt
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.692616 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/database/
+-rw-r--r--   0 val        (502) staff       (20)     2664 2023-05-01 21:01:40.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/database/customize_models.py
+-rw-r--r--   0 val        (502) staff       (20)      312 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/database/db_debug.py
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-11-16 19:24:28.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/database/nw-gold.sqlite
+-rw-r--r--   0 val        (502) staff       (20)       29 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/database/restore_sample_db.sh
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.692864 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/logic/
+-rw-r--r--   0 val        (502) staff       (20)    10650 2023-04-23 00:10:12.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/logic/declare_logic.py
+-rw-r--r--   0 val        (502) staff       (20)      241 2023-04-29 21:06:51.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/readme.md
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.693122 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/security/
+-rw-r--r--   0 val        (502) staff       (20)     1158 2023-02-14 15:54:30.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/security/declare_security.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.693341 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.693427 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.694015 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/
+-rw-r--r--   0 val        (502) staff       (20)      187 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/about.feature
+-rw-r--r--   0 val        (502) staff       (20)      285 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/api.feature
+-rw-r--r--   0 val        (502) staff       (20)     1281 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/place_order.feature
+-rw-r--r--   0 val        (502) staff       (20)      473 2023-04-23 23:42:07.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/salary_change.feature
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.695081 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/
+-rw-r--r--   0 val        (502) staff       (20)      450 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/about.py
+-rw-r--r--   0 val        (502) staff       (20)     2130 2023-01-14 03:27:19.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/api.py
+-rw-r--r--   0 val        (502) staff       (20)    16642 2023-02-16 04:52:22.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/place_order.py
+-rw-r--r--   0 val        (502) staff       (20)     4722 2023-04-23 23:41:49.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/salary_change.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.695381 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/
+-rw-r--r--   0 val        (502) staff       (20)     4356 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/behave.log
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.697007 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/
+-rw-r--r--   0 val        (502) staff       (20)     5070 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Alter_Item_Qty_to_exceed_.log
+-rw-r--r--   0 val        (502) staff       (20)     2256 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Alter_Required_Date_-_adj.log
+-rw-r--r--   0 val        (502) staff       (20)     8652 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Audit_Salary_Change.log
+-rw-r--r--   0 val        (502) staff       (20)     6095 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Bad_Order_Custom_Service.log
+-rw-r--r--   0 val        (502) staff       (20)     5794 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Good_Order_Custom_Service.log
+-rw-r--r--   0 val        (502) staff       (20)     2568 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Raise_Must_be_Meaningful.log
+-rw-r--r--   0 val        (502) staff       (20)     8481 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Reset_Shipped_-_adjust_lo.log
+-rw-r--r--   0 val        (502) staff       (20)     8445 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Set_Shipped_-_adjust_logi.log
+-rw-r--r--   0 val        (502) staff       (20)     2561 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Transaction_Processing.log
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.697668 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.699152 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/results/
+-rw-r--r--   0 val        (502) staff       (20)     5070 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/results/ADJUST_test_-_OrderDetail.log
+-rw-r--r--   0 val        (502) staff       (20)     8652 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/results/AUDIT_test_-_Emp_Sal.log
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/results/BEGIN.log
+-rw-r--r--   0 val        (502) staff       (20)    16926 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/results/CASCADE_UPDATE_-_ShippedD.log
+-rw-r--r--   0 val        (502) staff       (20)     6095 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/results/CUSTOM_SERVICE_Bad_Order.log
+-rw-r--r--   0 val        (502) staff       (20)      840 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/results/DELETE_test_-_Cust.log
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/results/GET_self-reln_Dept-SubDep.log
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/results/GET_test_on_Order.log
+-rw-r--r--   0 val        (502) staff       (20)     1381 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/results/PATCH_-_low_credit.log
+-rw-r--r--   0 val        (502) staff       (20)      831 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/results/POST_test_-_Cust.log
+-rw-r--r--   0 val        (502) staff       (20)     2256 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/results/PRUNE_test_-_ReqdDate.log
+-rw-r--r--   0 val        (502) staff       (20)     8405 2023-03-10 20:26:58.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/server_startup_test.py
+-rw-r--r--   0 val        (502) staff       (20)    13497 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/server_test.py
+-rw-r--r--   0 val        (502) staff       (20)     1543 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/server_test.sh
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.699309 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/
+-rw-r--r--   0 val        (502) staff       (20)     8196 2022-11-11 23:20:49.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/.DS_Store
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.700192 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/admin/
+-rw-r--r--   0 val        (502) staff       (20)    17259 2023-04-24 23:38:28.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/admin/admin.yaml
+-rw-r--r--   0 val        (502) staff       (20)     3443 2023-02-05 02:51:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/admin/home.js
+-rw-r--r--   0 val        (502) staff       (20)     8798 2022-12-30 19:58:21.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/admin/multi_app_project.yaml
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.700577 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2022-11-11 23:17:05.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/.DS_Store
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.702294 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Category/
+-rw-r--r--   0 val        (502) staff       (20)     6054 2008-04-22 03:46:52.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Category/beverages.gif
+-rw-r--r--   0 val        (502) staff       (20)     7324 2008-04-22 03:47:14.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Category/cereals.gif
+-rw-r--r--   0 val        (502) staff       (20)     7751 2008-04-22 03:47:30.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Category/condiments.gif
+-rw-r--r--   0 val        (502) staff       (20)     7022 2008-04-22 03:47:44.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Category/confections.gif
+-rw-r--r--   0 val        (502) staff       (20)     6136 2008-04-22 03:47:58.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Category/diary.gif
+-rw-r--r--   0 val        (502) staff       (20)     7268 2008-04-22 03:49:00.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Category/meat.gif
+-rw-r--r--   0 val        (502) staff       (20)     7633 2008-04-22 03:49:44.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Category/produce.gif
+-rw-r--r--   0 val        (502) staff       (20)     8469 2008-04-22 03:50:18.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Category/seafood.gif
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.703628 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Employee/
+-rw-r--r--   0 val        (502) staff       (20)     3719 2008-04-22 03:50:34.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Employee/buchanan.jpg
+-rw-r--r--   0 val        (502) staff       (20)     3715 2008-04-22 03:48:32.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Employee/callahan.jpg
+-rw-r--r--   0 val        (502) staff       (20)     4425 2008-04-22 03:49:28.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Employee/davolio.jpg
+-rw-r--r--   0 val        (502) staff       (20)     5404 2008-04-22 03:51:58.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Employee/dodsworth.jpg
+-rw-r--r--   0 val        (502) staff       (20)     3778 2008-04-22 03:51:40.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Employee/fuller.jpg
+-rw-r--r--   0 val        (502) staff       (20)     3737 2008-04-22 03:50:00.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Employee/king.jpg
+-rw-r--r--   0 val        (502) staff       (20)     3750 2008-04-22 03:48:16.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Employee/leverling.jpg
+-rw-r--r--   0 val        (502) staff       (20)     3862 2008-04-22 03:48:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Employee/peacock.jpg
+-rw-r--r--   0 val        (502) staff       (20)     4375 2008-04-22 03:49:14.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Employee/suyama.jpg
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.703770 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw_no_cust/
+-rw-r--r--   0 val        (502) staff       (20)     5431 2023-02-05 02:51:56.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw_no_cust/readme.md
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.705211 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2023-02-14 06:04:24.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.DS_Store
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.706957 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.devcontainer/
+-rw-r--r--   0 val        (502) staff       (20)      446 2023-02-05 02:55:30.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.devcontainer/For_VSCode.dockerfile
+-rw-r--r--   0 val        (502) staff       (20)     1932 2023-02-05 02:52:45.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.devcontainer/devcontainer.json
+-rw-r--r--   0 val        (502) staff       (20)      288 2023-01-25 20:14:39.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.devcontainer/setup.sh
+-rw-r--r--   0 val        (502) staff       (20)      215 2023-01-25 20:14:39.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.gitignore
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.707251 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.idea/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2023-02-14 06:05:31.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.idea/.DS_Store
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.710227 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.idea/runConfigurations/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2023-02-14 05:30:57.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.idea/runConfigurations/.DS_Store
+-rw-r--r--   0 val        (502) staff       (20)     1141 2023-02-14 05:35:26.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.idea/runConfigurations/1__Basic_App.xml
+-rw-r--r--   0 val        (502) staff       (20)     1162 2023-02-14 05:07:31.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.idea/runConfigurations/2__ApiLogicProject.xml
+-rw-r--r--   0 val        (502) staff       (20)     1174 2023-02-14 05:17:54.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.idea/runConfigurations/3__ApiLogicProject_Logic.xml
+-rw-r--r--   0 val        (502) staff       (20)     1148 2023-02-14 05:35:26.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Execute_chinook.xml
+-rw-r--r--   0 val        (502) staff       (20)     1160 2023-02-14 05:35:26.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Execute_classicmodels.xml
+-rw-r--r--   0 val        (502) staff       (20)     1142 2023-02-14 05:16:08.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Execute_todo.xml
+-rw-r--r--   0 val        (502) staff       (20)     1204 2023-02-14 05:54:42.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Run_Behave.xml
+-rw-r--r--   0 val        (502) staff       (20)     1386 2023-02-14 05:54:42.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Run_Behave_Logic_Report.xml
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.710840 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.vscode/
+-rw-r--r--   0 val        (502) staff       (20)     5986 2023-04-13 16:51:25.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.vscode/launch.json
+-rw-r--r--   0 val        (502) staff       (20)      100 2023-01-25 20:14:39.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.vscode/settings.json
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.712564 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2023-02-27 01:16:56.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/.DS_Store
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.713627 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/
+-rw-r--r--   0 val        (502) staff       (20)     1238 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/config.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     3435 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/flask.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     3970 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/flask_basic.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     3439 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/raw_flask.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     5965 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/util.cpython-310.pyc
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.713810 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/api/
+-rw-r--r--   0 val        (502) staff       (20)     2895 2023-02-28 05:23:15.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/api/end_points.py
+-rw-r--r--   0 val        (502) staff       (20)     2058 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/config.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.715365 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.715656 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/__pycache__/
+-rw-r--r--   0 val        (502) staff       (20)     8571 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/__pycache__/models.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)   522240 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/db.sqlite
+-rw-r--r--   0 val        (502) staff       (20)     1400 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/logging.yml
+-rw-r--r--   0 val        (502) staff       (20)    11838 2023-01-28 17:14:40.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/models.py
+-rw-r--r--   0 val        (502) staff       (20)     1452 2023-02-27 23:00:55.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/flask_basic.py
+-rw-r--r--   0 val        (502) staff       (20)     1400 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/logging.yml
+-rw-r--r--   0 val        (502) staff       (20)     3530 2023-02-28 05:20:39.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/readme.md
+-rw-r--r--   0 val        (502) staff       (20)     7699 2023-02-13 15:35:11.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/util.py
+-rw-r--r--   0 val        (502) staff       (20)    21134 2023-04-14 00:57:12.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/readme.md
+-rw-r--r--   0 val        (502) staff       (20)       14 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/requirements.txt
+-rw-r--r--   0 val        (502) staff       (20)   522240 2023-04-02 02:53:45.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/sample_db.sqlite
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.717265 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2023-01-22 18:56:43.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/.DS_Store
+-rw-r--r--   0 val        (502) staff       (20)      369 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/Readme.md
+-rw-r--r--   0 val        (502) staff       (20)        0 2023-01-03 23:29:33.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.721291 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/
+-rw-r--r--   0 val        (502) staff       (20)      175 2023-01-03 23:29:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)      191 2023-02-26 22:48:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 val        (502) staff       (20)     8054 2022-11-17 03:31:49.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/expose_existing_callable.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)    14080 2023-02-17 01:02:20.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/sqlacodegen_wrapper.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)    21445 2023-04-29 17:29:36.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/sqlacodegen_wrapper.cpython-311.pyc
+-rw-r--r--   0 val        (502) staff       (20)     1755 2023-02-01 19:08:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/uri_info.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)    53944 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/console_log.txt
+-rw-r--r--   0 val        (502) staff       (20)       54 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/requirements.txt
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.722688 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/
+-rw-r--r--   0 val        (502) staff       (20)     1850 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/.travis.yml
+-rw-r--r--   0 val        (502) staff       (20)     2593 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/CHANGES.rst
+-rw-r--r--   0 val        (502) staff       (20)     3865 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/README.rst
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.723184 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/__pycache__/
+-rw-r--r--   0 val        (502) staff       (20)      183 2022-08-15 21:21:51.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)      203 2023-02-26 22:48:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 val        (502) staff       (20)       87 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/pyproject.toml
+-rw-r--r--   0 val        (502) staff       (20)     1399 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/setup.cfg
+-rw-r--r--   0 val        (502) staff       (20)      196 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/setup.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.724239 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.725479 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/
+-rw-r--r--   0 val        (502) staff       (20)      195 2022-08-15 21:21:51.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)      215 2023-02-26 22:48:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 val        (502) staff       (20)    32358 2023-02-05 16:19:43.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/codegen.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)    74447 2023-04-06 14:36:23.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/codegen.cpython-311.pyc
+-rw-r--r--   0 val        (502) staff       (20)    58988 2023-04-06 14:31:39.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/codegen.py
+-rw-r--r--   0 val        (502) staff       (20)     3252 2022-11-18 19:19:33.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/main.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.726084 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/tests/
+-rw-r--r--   0 val        (502) staff       (20)    33384 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/tests/test_codegen.py
+-rw-r--r--   0 val        (502) staff       (20)      440 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/tox.ini
+-rwxr-xr-x   0 val        (502) staff       (20)    17236 2023-04-29 17:29:32.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen_wrapper.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.728259 ApiLogicServer-8.3.6/api_logic_server_cli/templates/
+-rw-r--r--   0 val        (502) staff       (20)    14864 2023-03-29 21:47:30.000000 ApiLogicServer-8.3.6/api_logic_server_cli/templates/admin.yaml
+-rw-r--r--   0 val        (502) staff       (20)     1221 2023-03-29 20:25:21.000000 ApiLogicServer-8.3.6/api_logic_server_cli/templates/app_fiddle.md
+-rw-r--r--   0 val        (502) staff       (20)     3322 2023-04-13 17:12:40.000000 ApiLogicServer-8.3.6/api_logic_server_cli/templates/app_fiddle.txt
+-rw-r--r--   0 val        (502) staff       (20)     3765 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/templates/index.html
+-rw-r--r--   0 val        (502) staff       (20)      900 2023-01-19 01:43:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/templates/login_endpoint.txt
+-rw-r--r--   0 val        (502) staff       (20)      205 2023-01-19 01:44:07.000000 ApiLogicServer-8.3.6/api_logic_server_cli/templates/login_endpoint_imports.txt
+-rw-r--r--   0 val        (502) staff       (20)       38 2023-05-02 04:14:08.728977 ApiLogicServer-8.3.6/setup.cfg
+-rw-r--r--   0 val        (502) staff       (20)     3521 2023-04-26 19:16:06.000000 ApiLogicServer-8.3.6/setup.py
```

### Comparing `ApiLogicServer-8.3.3/ApiLogicServer.egg-info/PKG-INFO` & `ApiLogicServer-8.3.6/ApiLogicServer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ApiLogicServer
-Version: 8.3.3
+Version: 8.3.6
 Summary: Create JSON:API and Web App from database, with LogicBank -- 40X more concise, Python for extensibility.
 Home-page: https://github.com/valhuber/ApiLogicServer
 Author: Val Huber
 Author-email: valjhuber@gmail.com
 License: BSD
 Project-URL: Docs, https://valhuber.github.io/ApiLogicServer/
 Platform: any
@@ -263,14 +263,16 @@
 
 
 [^1]:
     See the [FAQ for Low Code](FAQ-Low-Code)
 
 ### Change Log
 
+05/01/2023 - 08.03.06: allocation sample
+
 04/29/2023 - 08.03.03: restore missing debug info for open database failures
 
 04/26/2023 - 08.03.00: virt attrs (Issue 56), safrs 3.0.2, LogicBank 1.8.4, project readme updates
 
 04/13/2023 - 08.02.00: integratedConsole, logic logging (66), table relns fix (65)
 
 03/23/2023 - 08.01.15: table filters, cloud debug additions, issue 59, 62-4
```

### Comparing `ApiLogicServer-8.3.3/ApiLogicServer.egg-info/SOURCES.txt` & `ApiLogicServer-8.3.6/ApiLogicServer.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -314,14 +314,15 @@
 api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/pt/LC_MESSAGES/messages.mo
 api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/pt/LC_MESSAGES/messages.po
 api_logic_server_cli/create_from_model/templates/basic_web_app/babel/babel.cfg
 api_logic_server_cli/create_from_model/templates/basic_web_app/babel/messages.pot
 api_logic_server_cli/database/.DS_Store
 api_logic_server_cli/database/Chinook_Sqlite.sqlite
 api_logic_server_cli/database/__init__.py
+api_logic_server_cli/database/allocation.sqlite
 api_logic_server_cli/database/authentication.sqlite
 api_logic_server_cli/database/classicmodels.sqlite
 api_logic_server_cli/database/customize_models.py
 api_logic_server_cli/database/new.sqlite
 api_logic_server_cli/database/nw-gold-plus.sqlite
 api_logic_server_cli/database/nw-gold.sqlite
 api_logic_server_cli/database/nw.sqlite
@@ -517,14 +518,20 @@
 api_logic_server_cli/project_prototype/ui/templates/content.html
 api_logic_server_cli/project_prototype/venv_setup/py.py
 api_logic_server_cli/project_prototype/venv_setup/readme_venv.md
 api_logic_server_cli/project_prototype/venv_setup/requirements-no-cli.txt
 api_logic_server_cli/project_prototype/venv_setup/venv-linux.sh
 api_logic_server_cli/project_prototype/venv_setup/venv.ps1
 api_logic_server_cli/project_prototype/venv_setup/venv.sh
+api_logic_server_cli/project_prototype_allocation/.DS_Store
+api_logic_server_cli/project_prototype_allocation/readme-allocation.md
+api_logic_server_cli/project_prototype_allocation/images/db.png
+api_logic_server_cli/project_prototype_allocation/images/logic-diagram.png
+api_logic_server_cli/project_prototype_allocation/logic/declare_logic.py
+api_logic_server_cli/project_prototype_allocation/test/test.sh
 api_logic_server_cli/project_prototype_nw/.DS_Store
 api_logic_server_cli/project_prototype_nw/readme.md
 api_logic_server_cli/project_prototype_nw/api/customize_api.py
 api_logic_server_cli/project_prototype_nw/api/multi-table-example/multi-table.json
 api_logic_server_cli/project_prototype_nw/api/multi-table-example/multi-table.txt
 api_logic_server_cli/project_prototype_nw/database/customize_models.py
 api_logic_server_cli/project_prototype_nw/database/db_debug.py
```

### Comparing `ApiLogicServer-8.3.3/ApiLogicServer.egg-info/requires.txt` & `ApiLogicServer-8.3.6/ApiLogicServer.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/LICENSE` & `ApiLogicServer-8.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/MANIFEST.in` & `ApiLogicServer-8.3.6/MANIFEST.in`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 recursive-include api_logic_server_cli/project_prototype *.*
 recursive-include api_logic_server_cli/project_prototype_nw *.*
 recursive-include api_logic_server_cli/project_prototype_nw_no_cust *.*
+recursive-include api_logic_server_cli/project_prototype_allocation *.*
 recursive-include api_logic_server_cli/project_tutorial *.*
 recursive-include api_logic_server_cli/sqlacodegen_wrapper *.*
 recursive-include api_logic_server_cli/create_from_model *.*
 recursive-include api_logic_server_cli/database *.*
 recursive-include api_logic_server_cli/templates *.*
 recursive-include api_logic_server_cli/docs *.*
 recursive-include api_logic_server_cli/fragments *.*
```

### Comparing `ApiLogicServer-8.3.3/PKG-INFO` & `ApiLogicServer-8.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ApiLogicServer
-Version: 8.3.3
+Version: 8.3.6
 Summary: Create JSON:API and Web App from database, with LogicBank -- 40X more concise, Python for extensibility.
 Home-page: https://github.com/valhuber/ApiLogicServer
 Author: Val Huber
 Author-email: valjhuber@gmail.com
 License: BSD
 Project-URL: Docs, https://valhuber.github.io/ApiLogicServer/
 Platform: any
@@ -263,14 +263,16 @@
 
 
 [^1]:
     See the [FAQ for Low Code](FAQ-Low-Code)
 
 ### Change Log
 
+05/01/2023 - 08.03.06: allocation sample
+
 04/29/2023 - 08.03.03: restore missing debug info for open database failures
 
 04/26/2023 - 08.03.00: virt attrs (Issue 56), safrs 3.0.2, LogicBank 1.8.4, project readme updates
 
 04/13/2023 - 08.02.00: integratedConsole, logic logging (66), table relns fix (65)
 
 03/23/2023 - 08.01.15: table filters, cloud debug additions, issue 59, 62-4
```

### Comparing `ApiLogicServer-8.3.3/README.md` & `ApiLogicServer-8.3.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -239,14 +239,16 @@
 
 
 [^1]:
     See the [FAQ for Low Code](FAQ-Low-Code)
 
 ### Change Log
 
+05/01/2023 - 08.03.06: allocation sample
+
 04/29/2023 - 08.03.03: restore missing debug info for open database failures
 
 04/26/2023 - 08.03.00: virt attrs (Issue 56), safrs 3.0.2, LogicBank 1.8.4, project readme updates
 
 04/13/2023 - 08.02.00: integratedConsole, logic logging (66), table relns fix (65)
 
 03/23/2023 - 08.01.15: table filters, cloud debug additions, issue 59, 62-4
```

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/api_logic_server.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/api_logic_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,18 @@
         * api/expose_api_models.py for a safrs api  - using introspected models.py
     * Special provisions for NW Sample, to show customizations.
     * See end for key module map quick links...
 
 Called from api_logic_server_cli.py, by instantiating the ProjectRun object.
 '''
 
-__version__ = "08.03.03"
+__version__ = "08.03.06"
 recent_changes = \
     f'\n\nRecent Changes:\n' +\
+    "\t05/01/2023 - 08.03.06: allocation sample \n"\
     "\t04/29/2023 - 08.03.03: connect error reporting, startup logging \n"\
     "\t04/26/2023 - 08.03.00: virt attrs (Issue 56), safrs 3.0.2, readme updates, LogicBank 1.8.4 \n"\
     "\t04/13/2023 - 08.02.00: integratedConsole, logic logging (66), table relns fix (65) \n"\
     "\t04/06/2023 - 08.01.24: create_image, bugfix for excluded table relationships \n"\
     "\t03/23/2023 - 08.01.15: cloud debug additions, issue 59, 62-4, table filters \n"\
     "\t03/05/2023 - 08.01.04: python 3.11.2, Werkzeug==2.2.3, mypy initial, logicbank 1.8.3 \n"\
     "\t02/15/2023 - 08.00.01: Declarative Authorization and Authentication, Werkzeug==2.2.3 \n"\
@@ -237,14 +238,16 @@
     """
     clone prototype to  project directory, copy sqlite db, and remove git folder
 
     update config.py - SQLALCHEMY_DATABASE_URI
 
     if nw/nw+, inject sample logic/declare_logic and api/customize_api.
 
+    nw, allocation etc databases are resolved in api_logic_server_utils.get_abs_db_url()
+
     :param project a ProjectRun
     :param msg log.debuged, such as Create Project:
     :return: return_abs_db_url (e.g., reflects sqlite copy to project/database dir)
     """
 
     import tempfile
     cloned_from = project.from_git
@@ -299,14 +302,20 @@
             log.debug(".. ..Copy in nw customizations: logic, custom api, readme, tests, admin app")
             nw_dir = (Path(api_logic_server_dir_str)).\
                 joinpath('project_prototype_nw')  # /Users/val/dev/ApiLogicServer/api_logic_server_cli/project_prototype
             recursive_overwrite(nw_dir, project.project_directory)
 
             create_nw_tutorial(project.project_directory, api_logic_server_dir_str)
 
+        if project.db_url in ["allocation"]:
+            log.debug(".. ..Copy in allocation customizations: readme, logic, tests")
+            nw_dir = (Path(api_logic_server_dir_str)).\
+                joinpath('project_prototype_allocation')  # /Users/val/dev/ApiLogicServer/project_prototype_allocation
+            recursive_overwrite(nw_dir, project.project_directory)
+
         if project.nw_db_status in ["nw-"]:
             log.debug(".. ..Copy in nw- customizations: readme, perform_customizations")
             nw_dir = (Path(api_logic_server_dir_str)).\
                 joinpath('project_prototype_nw_no_cust')  # /Users/val/dev/ApiLogicServer/project_prototype_nw_no_cust
             recursive_overwrite(nw_dir, project.project_directory)
 
         create_utils.replace_string_in_file(search_for="creation-date",
@@ -1173,20 +1182,20 @@
         ctl-l (^l) for last edit
     """
     import create_from_model.ui_admin_creator as ui_admin_creator
     import create_from_model.api_expose_api_models_creator as api_expose_api_models_creator
     import sqlacodegen_wrapper.sqlacodegen_wrapper as sqlacodegen_wrapper
 
     ProjectRun.create_project()                             # main driver, calls...
+    create_utils.get_abs_db_url()                           # nw set here, dbname, db abbrevs
     create_project_with_nw_samples()                        # clone project, overlay nw
     model_creation_services = ModelCreationServices()       # creates resource_list (python db model); ctor calls...
     def and_the_ctor_calls():
         sqlacodegen_wrapper.create_models_py({})            # creates models.py via *sqlacodegen*
         sqlacodegen_wrapper.CodeGenerator.render_class()    # sqlacodegen - creates models_py as string
         model_creation_services.create_resource_list()      # creates resource_list via *dynamic import* of models.py
     invoke_creators(model_creation_services)                # creates api & ui, via create_from_model...
     api_expose_api_models_creator.create()                  # creates api/expose_api_models.py, key input to SAFRS        
     ui_admin_creator.create()                               # creates ui/admin/admin.yaml from resource_list
-    create_utils.get_abs_db_url()                           # nw set here, dbname
     ProjectRun.update_config_and_copy_sqlite_db()           # adds db (model, binds, api, app) to curr project
     ProjectRun.add_sqlite_security()                        # add_db(auth), adds nw declare_security, upd config
     ProjectRun.tutorial()                                   # creates basic, nw, nw + cust
```

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/cli.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/cli.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/cli_args_base.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/cli_args_base.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/cli_args_project.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/cli_args_project.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/.DS_Store` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__pycache__/api_expose_api_models.cpython-310.pyc` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__pycache__/api_expose_api_models.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__pycache__/api_expose_api_models_creator.cpython-310.pyc` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__pycache__/api_expose_api_models_creator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__pycache__/api_expose_api_models_creator.cpython-311.pyc` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__pycache__/api_expose_api_models_creator.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__pycache__/api_logic_server_utils.cpython-310.pyc` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__pycache__/api_logic_server_utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__pycache__/api_logic_server_utils.cpython-311.pyc` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__pycache__/api_logic_server_utils.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xff911264 (Thu Mar 16 03:50:23 2023 UTC)
-files sz: 11423
+moddate:  0x2d6f5064 (Tue May  2 02:02:21 2023 UTC)
+files sz: 11680
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 9
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064016c025a02640064
@@ -81,75 +81,75 @@
     63         124 LOAD_CONST               9 ('project')
                126 LOAD_NAME                8 (Project)
                128 BUILD_TUPLE              2
                130 LOAD_CONST              10 (<code object get_abs_db_url, file "/Users/val/dev/ApiLogicServer/api_logic_server_cli/create_from_model/api_logic_server_utils.py", line 63>)
                132 MAKE_FUNCTION            4 (annotations)
                134 STORE_NAME              16 (get_abs_db_url)
    
-   135         136 LOAD_CONST               6 ('return')
+   138         136 LOAD_CONST               6 ('return')
                138 LOAD_NAME               13 (str)
                140 BUILD_TUPLE              2
-               142 LOAD_CONST              11 (<code object get_api_logic_server_dir, file "/Users/val/dev/ApiLogicServer/api_logic_server_cli/create_from_model/api_logic_server_utils.py", line 135>)
+               142 LOAD_CONST              11 (<code object get_api_logic_server_dir, file "/Users/val/dev/ApiLogicServer/api_logic_server_cli/create_from_model/api_logic_server_utils.py", line 138>)
                144 MAKE_FUNCTION            4 (annotations)
                146 STORE_NAME              17 (get_api_logic_server_dir)
    
-   145         148 LOAD_CONST              12 ('search_for')
+   148         148 LOAD_CONST              12 ('search_for')
                150 LOAD_NAME               13 (str)
                152 LOAD_CONST              13 ('in_file')
                154 LOAD_NAME               13 (str)
                156 LOAD_CONST               6 ('return')
                158 LOAD_NAME               18 (bool)
                160 BUILD_TUPLE              6
-               162 LOAD_CONST              14 (<code object does_file_contain, file "/Users/val/dev/ApiLogicServer/api_logic_server_cli/create_from_model/api_logic_server_utils.py", line 145>)
+               162 LOAD_CONST              14 (<code object does_file_contain, file "/Users/val/dev/ApiLogicServer/api_logic_server_cli/create_from_model/api_logic_server_utils.py", line 148>)
                164 MAKE_FUNCTION            4 (annotations)
                166 STORE_NAME              19 (does_file_contain)
    
-   157         168 LOAD_CONST              12 ('search_for')
+   160         168 LOAD_CONST              12 ('search_for')
                170 LOAD_NAME               13 (str)
                172 LOAD_CONST              15 ('replace_with')
                174 LOAD_NAME               13 (str)
                176 LOAD_CONST              13 ('in_file')
                178 LOAD_NAME               13 (str)
                180 BUILD_TUPLE              6
-               182 LOAD_CONST              16 (<code object replace_string_in_file, file "/Users/val/dev/ApiLogicServer/api_logic_server_cli/create_from_model/api_logic_server_utils.py", line 157>)
+               182 LOAD_CONST              16 (<code object replace_string_in_file, file "/Users/val/dev/ApiLogicServer/api_logic_server_cli/create_from_model/api_logic_server_utils.py", line 160>)
                184 MAKE_FUNCTION            4 (annotations)
                186 STORE_NAME              20 (replace_string_in_file)
    
-   165         188 LOAD_CONST              29 ((False,))
+   168         188 LOAD_CONST              29 ((False,))
                190 LOAD_CONST              18 ('lines')
                192 LOAD_NAME               13 (str)
                194 LOAD_CONST              19 ('at')
                196 LOAD_NAME               13 (str)
                198 LOAD_CONST              20 ('file_name')
                200 LOAD_NAME               13 (str)
                202 LOAD_CONST              21 ('after')
                204 LOAD_NAME               18 (bool)
                206 BUILD_TUPLE              8
-               208 LOAD_CONST              22 (<code object insert_lines_at, file "/Users/val/dev/ApiLogicServer/api_logic_server_cli/create_from_model/api_logic_server_utils.py", line 165>)
+               208 LOAD_CONST              22 (<code object insert_lines_at, file "/Users/val/dev/ApiLogicServer/api_logic_server_cli/create_from_model/api_logic_server_utils.py", line 168>)
                210 MAKE_FUNCTION            5 (defaults, annotations)
                212 STORE_NAME              21 (insert_lines_at)
    
-   185         214 LOAD_CONST               6 ('return')
+   188         214 LOAD_CONST               6 ('return')
                216 LOAD_NAME               13 (str)
                218 BUILD_TUPLE              2
-               220 LOAD_CONST              23 (<code object find_valid_python_name, file "/Users/val/dev/ApiLogicServer/api_logic_server_cli/create_from_model/api_logic_server_utils.py", line 185>)
+               220 LOAD_CONST              23 (<code object find_valid_python_name, file "/Users/val/dev/ApiLogicServer/api_logic_server_cli/create_from_model/api_logic_server_utils.py", line 188>)
                222 MAKE_FUNCTION            4 (annotations)
                224 STORE_NAME              22 (find_valid_python_name)
    
-   207         226 LOAD_CONST              30 ((None, '', False))
+   210         226 LOAD_CONST              30 ((None, '', False))
                228 LOAD_CONST              25 ('cmd')
                230 LOAD_NAME               13 (str)
                232 LOAD_CONST              26 ('msg')
                234 LOAD_NAME               13 (str)
                236 LOAD_CONST              27 ('new_line')
                238 LOAD_NAME               18 (bool)
                240 LOAD_CONST               6 ('return')
                242 LOAD_NAME               13 (str)
                244 BUILD_TUPLE              8
-               246 LOAD_CONST              28 (<code object run_command, file "/Users/val/dev/ApiLogicServer/api_logic_server_cli/create_from_model/api_logic_server_utils.py", line 207>)
+               246 LOAD_CONST              28 (<code object run_command, file "/Users/val/dev/ApiLogicServer/api_logic_server_cli/create_from_model/api_logic_server_utils.py", line 210>)
                248 MAKE_FUNCTION            5 (defaults, annotations)
                250 STORE_NAME              23 (run_command)
                252 LOAD_CONST               1 (None)
                254 RETURN_VALUE
    consts
       0
       None
@@ -397,65 +397,68 @@
             0000000000000000006404a6010000ab0100000000000000007201090009
             007c016a0000000000000000007c016a0700000000000000006401640564
             0666047600724d64077405000000000000000000007c016a080000000000
             000000a00500000000000000000000000000000000000000006408a60100
             00ab010000000000000000a6010000ab0100000000000000009b009d027d
             0364057d02741200000000000000000000a00a0000000000000000000000
             0000000000000000007c009b0064097c039b009d03a6010000ab01000000
-            0000000000010090026ece7c016a000000000000000000640a6b02000000
+            0000000000010090036e057c016a000000000000000000640a6b02000000
             00722e64077405000000000000000000007c016a080000000000000000a0
             0500000000000000000000000000000000000000006408a6010000ab0100
             00000000000000a6010000ab0100000000000000009b009d027d03640a7d
-            0290026e957c016a000000000000000000640b6b0200000000722e640774
+            0290026ecc7c016a000000000000000000640b6b0200000000722e640774
             05000000000000000000007c016a080000000000000000a0050000000000
             000000000000000000000000000000640ca6010000ab0100000000000000
-            00a6010000ab0100000000000000009b009d027d03640a7d0290026e5c7c
+            00a6010000ab0100000000000000009b009d027d03640a7d0290026e937c
             016a000000000000000000640d6b0200000000724d640774050000000000
             00000000007c016a080000000000000000a0050000000000000000000000
             000000000000000000640ea6010000ab010000000000000000a6010000ab
             0100000000000000009b009d027d03640d7d027412000000000000000000
             00a00a00000000000000000000000000000000000000007c009b0064097c
-            039b009d03a6010000ab010000000000000000010090026e047c016a0000
+            039b009d03a6010000ab010000000000000000010090026e3b7c016a0000
             00000000000000640f6b0200000000730b7c016a00000000000000000064
             106b0200000000722c64077405000000000000000000007c016a08000000
             0000000000a00500000000000000000000000000000000000000006411a6
             010000ab010000000000000000a6010000ab0100000000000000009b009d
-            027d0390016ec27c016a00000000000000000064126b0200000000722c64
+            027d0390016ef97c016a00000000000000000064126b0200000000722c64
             077405000000000000000000007c016a080000000000000000a005000000
             00000000000000000000000000000000006413a6010000ab010000000000
-            000000a6010000ab0100000000000000009b009d027d0390016e8b7c016a
+            000000a6010000ab0100000000000000009b009d027d0390016ec27c016a
             00000000000000000064146b0200000000730b7c016a0000000000000000
             0064156b0200000000722c64077405000000000000000000007c016a0800
             00000000000000a005000000000000000000000000000000000000000064
             16a6010000ab010000000000000000a6010000ab0100000000000000009b
-            009d027d0390016e497c016a00000000000000000064176b020000000072
+            009d027d0390016e807c016a00000000000000000064176b020000000072
             2c64077405000000000000000000007c016a080000000000000000a00500
             000000000000000000000000000000000000006418a6010000ab01000000
-            0000000000a6010000ab0100000000000000009b009d027d0390016e127c
-            016a00000000000000000064196b0200000000722b640774050000000000
+            0000000000a6010000ab0100000000000000009b009d027d0390016e497c
+            016a00000000000000000064196b0200000000722c640774050000000000
             00000000007c016a080000000000000000a0050000000000000000000000
             000000000000000000641aa6010000ab010000000000000000a6010000ab
-            0100000000000000009b009d027d036edc7c016a00000000000000000064
-            1b6b0200000000722b64077405000000000000000000007c016a08000000
-            0000000000a0050000000000000000000000000000000000000000641ca6
-            010000ab010000000000000000a6010000ab0100000000000000009b009d
-            027d036ea67c016a000000000000000000a0010000000000000000000000
-            0000000000000000006407a6010000ab01000000000000000072367c016a
-            000000000000000000641d7417000000000000000000007c016a00000000
-            0000000000a6010000ab0100000000000000008502190000000000000000
-            007d057419000000000000000000007c05a6010000ab0100000000000000
-            007d0364077c037a0000007d036e567c016a000000000000000000a00100
-            00000000000000000000000000000000000000641ea6010000ab01000000
-            00000000007203641f7d036e397c016a000000000000000000a001000000
-            00000000000000000000000000000000006420a6010000ab010000000000
-            000000720364217d036e1c7c016a000000000000000000a0010000000000
-            0000000000000000000000000000006422a6010000ab0100000000000000
-            00720264237d0364247d067c016a0d000000000000000064016b03000000
-            00720d7c016a0d000000000000000064257a00000064247a0000007d067c
-            037c027c0666035300
+            0100000000000000009b009d027d0390016e127c016a0000000000000000
+            00641b6b0200000000722b64077405000000000000000000007c016a0800
+            00000000000000a005000000000000000000000000000000000000000064
+            1ca6010000ab010000000000000000a6010000ab0100000000000000009b
+            009d027d036edc7c016a000000000000000000641d6b0200000000722b64
+            077405000000000000000000007c016a080000000000000000a005000000
+            0000000000000000000000000000000000641ea6010000ab010000000000
+            000000a6010000ab0100000000000000009b009d027d036ea67c016a0000
+            00000000000000a001000000000000000000000000000000000000000064
+            07a6010000ab01000000000000000072367c016a00000000000000000064
+            1f7417000000000000000000007c016a000000000000000000a6010000ab
+            0100000000000000008502190000000000000000007d0574190000000000
+            00000000007c05a6010000ab0100000000000000007d0364077c037a0000
+            007d036e567c016a000000000000000000a0010000000000000000000000
+            0000000000000000006420a6010000ab010000000000000000720364217d
+            036e397c016a000000000000000000a00100000000000000000000000000
+            000000000000006422a6010000ab010000000000000000720364237d036e
+            1c7c016a000000000000000000a001000000000000000000000000000000
+            00000000006424a6010000ab010000000000000000720264257d0364267d
+            067c016a0d000000000000000064016b0300000000720d7c016a0d000000
+            000000000064277a00000064267a0000007d067c037c027c0666035300
           63           0 RESUME                   0
          
           75           2 LOAD_CONST               1 ('')
                        4 STORE_FAST               2 (rtn_nw_db_status)
          
           76           6 LOAD_FAST                1 (project)
                        8 LOAD_ATTR                0 (db_url)
@@ -526,346 +529,368 @@
                      384 FORMAT_VALUE             0
                      386 BUILD_STRING             2
                      388 STORE_FAST               3 (rtn_abs_db_url)
          
           95         390 LOAD_CONST               5 ('nw')
                      392 STORE_FAST               2 (rtn_nw_db_status)
          
-          96         394 LOAD_GLOBAL             18 (log)
+          97         394 LOAD_GLOBAL             18 (log)
                      406 LOAD_METHOD             10 (debug)
                      428 LOAD_FAST                0 (msg)
                      430 FORMAT_VALUE             0
                      432 LOAD_CONST               9 (' from: ')
                      434 LOAD_FAST                3 (rtn_abs_db_url)
                      436 FORMAT_VALUE             0
                      438 BUILD_STRING             3
                      440 PRECALL                  1
                      444 CALL                     1
                      454 POP_TOP
-                     456 EXTENDED_ARG             2
-                     458 JUMP_FORWARD           718 (to 1896)
+                     456 EXTENDED_ARG             3
+                     458 JUMP_FORWARD           773 (to 2006)
          
-          97     >>  460 LOAD_FAST                1 (project)
+          98     >>  460 LOAD_FAST                1 (project)
                      462 LOAD_ATTR                0 (db_url)
                      472 LOAD_CONST              10 ('nw-')
                      474 COMPARE_OP               2 (==)
                      480 POP_JUMP_FORWARD_IF_FALSE    46 (to 574)
          
-          98         482 LOAD_CONST               7 ('sqlite:///')
+          99         482 LOAD_CONST               7 ('sqlite:///')
                      484 LOAD_GLOBAL              5 (NULL + str)
                      496 LOAD_FAST                1 (project)
                      498 LOAD_ATTR                8 (api_logic_server_dir_path)
                      508 LOAD_METHOD              5 (joinpath)
                      530 LOAD_CONST               8 ('database/nw-gold.sqlite')
                      532 PRECALL                  1
                      536 CALL                     1
                      546 PRECALL                  1
                      550 CALL                     1
                      560 FORMAT_VALUE             0
                      562 BUILD_STRING             2
                      564 STORE_FAST               3 (rtn_abs_db_url)
          
-          99         566 LOAD_CONST              10 ('nw-')
+         100         566 LOAD_CONST              10 ('nw-')
                      568 STORE_FAST               2 (rtn_nw_db_status)
                      570 EXTENDED_ARG             2
-                     572 JUMP_FORWARD           661 (to 1896)
+                     572 JUMP_FORWARD           716 (to 2006)
          
-         100     >>  574 LOAD_FAST                1 (project)
+         101     >>  574 LOAD_FAST                1 (project)
                      576 LOAD_ATTR                0 (db_url)
                      586 LOAD_CONST              11 ('nw--')
                      588 COMPARE_OP               2 (==)
                      594 POP_JUMP_FORWARD_IF_FALSE    46 (to 688)
          
-         101         596 LOAD_CONST               7 ('sqlite:///')
+         102         596 LOAD_CONST               7 ('sqlite:///')
                      598 LOAD_GLOBAL              5 (NULL + str)
                      610 LOAD_FAST                1 (project)
                      612 LOAD_ATTR                8 (api_logic_server_dir_path)
                      622 LOAD_METHOD              5 (joinpath)
                      644 LOAD_CONST              12 ('database/nw.sqlite')
                      646 PRECALL                  1
                      650 CALL                     1
                      660 PRECALL                  1
                      664 CALL                     1
                      674 FORMAT_VALUE             0
                      676 BUILD_STRING             2
                      678 STORE_FAST               3 (rtn_abs_db_url)
          
-         102         680 LOAD_CONST              10 ('nw-')
+         103         680 LOAD_CONST              10 ('nw-')
                      682 STORE_FAST               2 (rtn_nw_db_status)
                      684 EXTENDED_ARG             2
-                     686 JUMP_FORWARD           604 (to 1896)
+                     686 JUMP_FORWARD           659 (to 2006)
          
-         103     >>  688 LOAD_FAST                1 (project)
+         104     >>  688 LOAD_FAST                1 (project)
                      690 LOAD_ATTR                0 (db_url)
                      700 LOAD_CONST              13 ('nw+')
                      702 COMPARE_OP               2 (==)
                      708 POP_JUMP_FORWARD_IF_FALSE    77 (to 864)
          
-         104         710 LOAD_CONST               7 ('sqlite:///')
+         105         710 LOAD_CONST               7 ('sqlite:///')
                      712 LOAD_GLOBAL              5 (NULL + str)
                      724 LOAD_FAST                1 (project)
                      726 LOAD_ATTR                8 (api_logic_server_dir_path)
                      736 LOAD_METHOD              5 (joinpath)
                      758 LOAD_CONST              14 ('database/nw-gold-plus.sqlite')
                      760 PRECALL                  1
                      764 CALL                     1
                      774 PRECALL                  1
                      778 CALL                     1
                      788 FORMAT_VALUE             0
                      790 BUILD_STRING             2
                      792 STORE_FAST               3 (rtn_abs_db_url)
          
-         105         794 LOAD_CONST              13 ('nw+')
+         106         794 LOAD_CONST              13 ('nw+')
                      796 STORE_FAST               2 (rtn_nw_db_status)
          
-         106         798 LOAD_GLOBAL             18 (log)
+         107         798 LOAD_GLOBAL             18 (log)
                      810 LOAD_METHOD             10 (debug)
                      832 LOAD_FAST                0 (msg)
                      834 FORMAT_VALUE             0
                      836 LOAD_CONST               9 (' from: ')
                      838 LOAD_FAST                3 (rtn_abs_db_url)
                      840 FORMAT_VALUE             0
                      842 BUILD_STRING             3
                      844 PRECALL                  1
                      848 CALL                     1
                      858 POP_TOP
                      860 EXTENDED_ARG             2
-                     862 JUMP_FORWARD           516 (to 1896)
+                     862 JUMP_FORWARD           571 (to 2006)
          
-         107     >>  864 LOAD_FAST                1 (project)
+         108     >>  864 LOAD_FAST                1 (project)
                      866 LOAD_ATTR                0 (db_url)
                      876 LOAD_CONST              15 ('auth')
                      878 COMPARE_OP               2 (==)
                      884 POP_JUMP_FORWARD_IF_TRUE    11 (to 908)
                      886 LOAD_FAST                1 (project)
                      888 LOAD_ATTR                0 (db_url)
                      898 LOAD_CONST              16 ('authorization')
                      900 COMPARE_OP               2 (==)
                      906 POP_JUMP_FORWARD_IF_FALSE    44 (to 996)
          
-         108     >>  908 LOAD_CONST               7 ('sqlite:///')
+         109     >>  908 LOAD_CONST               7 ('sqlite:///')
                      910 LOAD_GLOBAL              5 (NULL + str)
                      922 LOAD_FAST                1 (project)
                      924 LOAD_ATTR                8 (api_logic_server_dir_path)
                      934 LOAD_METHOD              5 (joinpath)
                      956 LOAD_CONST              17 ('database/authentication.sqlite')
                      958 PRECALL                  1
                      962 CALL                     1
                      972 PRECALL                  1
                      976 CALL                     1
                      986 FORMAT_VALUE             0
                      988 BUILD_STRING             2
                      990 STORE_FAST               3 (rtn_abs_db_url)
                      992 EXTENDED_ARG             1
-                     994 JUMP_FORWARD           450 (to 1896)
+                     994 JUMP_FORWARD           505 (to 2006)
          
-         109     >>  996 LOAD_FAST                1 (project)
+         110     >>  996 LOAD_FAST                1 (project)
                      998 LOAD_ATTR                0 (db_url)
                     1008 LOAD_CONST              18 ('chinook')
                     1010 COMPARE_OP               2 (==)
                     1016 POP_JUMP_FORWARD_IF_FALSE    44 (to 1106)
          
-         110        1018 LOAD_CONST               7 ('sqlite:///')
+         111        1018 LOAD_CONST               7 ('sqlite:///')
                     1020 LOAD_GLOBAL              5 (NULL + str)
                     1032 LOAD_FAST                1 (project)
                     1034 LOAD_ATTR                8 (api_logic_server_dir_path)
                     1044 LOAD_METHOD              5 (joinpath)
                     1066 LOAD_CONST              19 ('database/Chinook_Sqlite.sqlite')
                     1068 PRECALL                  1
                     1072 CALL                     1
                     1082 PRECALL                  1
                     1086 CALL                     1
                     1096 FORMAT_VALUE             0
                     1098 BUILD_STRING             2
                     1100 STORE_FAST               3 (rtn_abs_db_url)
                     1102 EXTENDED_ARG             1
-                    1104 JUMP_FORWARD           395 (to 1896)
+                    1104 JUMP_FORWARD           450 (to 2006)
          
-         111     >> 1106 LOAD_FAST                1 (project)
+         112     >> 1106 LOAD_FAST                1 (project)
                     1108 LOAD_ATTR                0 (db_url)
                     1118 LOAD_CONST              20 ('todo')
                     1120 COMPARE_OP               2 (==)
                     1126 POP_JUMP_FORWARD_IF_TRUE    11 (to 1150)
                     1128 LOAD_FAST                1 (project)
                     1130 LOAD_ATTR                0 (db_url)
                     1140 LOAD_CONST              21 ('todos')
                     1142 COMPARE_OP               2 (==)
                     1148 POP_JUMP_FORWARD_IF_FALSE    44 (to 1238)
          
-         112     >> 1150 LOAD_CONST               7 ('sqlite:///')
+         113     >> 1150 LOAD_CONST               7 ('sqlite:///')
                     1152 LOAD_GLOBAL              5 (NULL + str)
                     1164 LOAD_FAST                1 (project)
                     1166 LOAD_ATTR                8 (api_logic_server_dir_path)
                     1176 LOAD_METHOD              5 (joinpath)
                     1198 LOAD_CONST              22 ('database/todos.sqlite')
                     1200 PRECALL                  1
                     1204 CALL                     1
                     1214 PRECALL                  1
                     1218 CALL                     1
                     1228 FORMAT_VALUE             0
                     1230 BUILD_STRING             2
                     1232 STORE_FAST               3 (rtn_abs_db_url)
                     1234 EXTENDED_ARG             1
-                    1236 JUMP_FORWARD           329 (to 1896)
+                    1236 JUMP_FORWARD           384 (to 2006)
          
-         113     >> 1238 LOAD_FAST                1 (project)
+         114     >> 1238 LOAD_FAST                1 (project)
                     1240 LOAD_ATTR                0 (db_url)
                     1250 LOAD_CONST              23 ('new')
                     1252 COMPARE_OP               2 (==)
                     1258 POP_JUMP_FORWARD_IF_FALSE    44 (to 1348)
          
-         114        1260 LOAD_CONST               7 ('sqlite:///')
+         115        1260 LOAD_CONST               7 ('sqlite:///')
                     1262 LOAD_GLOBAL              5 (NULL + str)
                     1274 LOAD_FAST                1 (project)
                     1276 LOAD_ATTR                8 (api_logic_server_dir_path)
                     1286 LOAD_METHOD              5 (joinpath)
                     1308 LOAD_CONST              24 ('database/new.sqlite')
                     1310 PRECALL                  1
                     1314 CALL                     1
                     1324 PRECALL                  1
                     1328 CALL                     1
                     1338 FORMAT_VALUE             0
                     1340 BUILD_STRING             2
                     1342 STORE_FAST               3 (rtn_abs_db_url)
                     1344 EXTENDED_ARG             1
-                    1346 JUMP_FORWARD           274 (to 1896)
+                    1346 JUMP_FORWARD           329 (to 2006)
          
-         115     >> 1348 LOAD_FAST                1 (project)
+         116     >> 1348 LOAD_FAST                1 (project)
                     1350 LOAD_ATTR                0 (db_url)
                     1360 LOAD_CONST              25 ('table_filters_tests')
                     1362 COMPARE_OP               2 (==)
-                    1368 POP_JUMP_FORWARD_IF_FALSE    43 (to 1456)
+                    1368 POP_JUMP_FORWARD_IF_FALSE    44 (to 1458)
          
-         116        1370 LOAD_CONST               7 ('sqlite:///')
+         117        1370 LOAD_CONST               7 ('sqlite:///')
                     1372 LOAD_GLOBAL              5 (NULL + str)
                     1384 LOAD_FAST                1 (project)
                     1386 LOAD_ATTR                8 (api_logic_server_dir_path)
                     1396 LOAD_METHOD              5 (joinpath)
                     1418 LOAD_CONST              26 ('database/table_filters_tests.sqlite')
                     1420 PRECALL                  1
                     1424 CALL                     1
                     1434 PRECALL                  1
                     1438 CALL                     1
                     1448 FORMAT_VALUE             0
                     1450 BUILD_STRING             2
                     1452 STORE_FAST               3 (rtn_abs_db_url)
-                    1454 JUMP_FORWARD           220 (to 1896)
+                    1454 EXTENDED_ARG             1
+                    1456 JUMP_FORWARD           274 (to 2006)
          
-         117     >> 1456 LOAD_FAST                1 (project)
-                    1458 LOAD_ATTR                0 (db_url)
-                    1468 LOAD_CONST              27 ('classicmodels')
-                    1470 COMPARE_OP               2 (==)
-                    1476 POP_JUMP_FORWARD_IF_FALSE    43 (to 1564)
-         
-         118        1478 LOAD_CONST               7 ('sqlite:///')
-                    1480 LOAD_GLOBAL              5 (NULL + str)
-                    1492 LOAD_FAST                1 (project)
-                    1494 LOAD_ATTR                8 (api_logic_server_dir_path)
-                    1504 LOAD_METHOD              5 (joinpath)
-                    1526 LOAD_CONST              28 ('database/classicmodels.sqlite')
-                    1528 PRECALL                  1
-                    1532 CALL                     1
-                    1542 PRECALL                  1
-                    1546 CALL                     1
-                    1556 FORMAT_VALUE             0
-                    1558 BUILD_STRING             2
-                    1560 STORE_FAST               3 (rtn_abs_db_url)
-                    1562 JUMP_FORWARD           166 (to 1896)
-         
-         119     >> 1564 LOAD_FAST                1 (project)
-                    1566 LOAD_ATTR                0 (db_url)
-                    1576 LOAD_METHOD              1 (startswith)
-                    1598 LOAD_CONST               7 ('sqlite:///')
-                    1600 PRECALL                  1
-                    1604 CALL                     1
-                    1614 POP_JUMP_FORWARD_IF_FALSE    54 (to 1724)
-         
-         120        1616 LOAD_FAST                1 (project)
-                    1618 LOAD_ATTR                0 (db_url)
-                    1628 LOAD_CONST              29 (10)
-                    1630 LOAD_GLOBAL             23 (NULL + len)
-                    1642 LOAD_FAST                1 (project)
-                    1644 LOAD_ATTR                0 (db_url)
-                    1654 PRECALL                  1
-                    1658 CALL                     1
-                    1668 BUILD_SLICE              2
-                    1670 BINARY_SUBSCR
-                    1680 STORE_FAST               5 (url)
-         
-         121        1682 LOAD_GLOBAL             25 (NULL + abspath)
-                    1694 LOAD_FAST                5 (url)
-                    1696 PRECALL                  1
-                    1700 CALL                     1
-                    1710 STORE_FAST               3 (rtn_abs_db_url)
-         
-         122        1712 LOAD_CONST               7 ('sqlite:///')
-                    1714 LOAD_FAST                3 (rtn_abs_db_url)
-                    1716 BINARY_OP                0 (+)
-                    1720 STORE_FAST               3 (rtn_abs_db_url)
-                    1722 JUMP_FORWARD            86 (to 1896)
-         
-         123     >> 1724 LOAD_FAST                1 (project)
-                    1726 LOAD_ATTR                0 (db_url)
-                    1736 LOAD_METHOD              1 (startswith)
-                    1758 LOAD_CONST              30 ('sqlsvr-sample')
-                    1760 PRECALL                  1
-                    1764 CALL                     1
-                    1774 POP_JUMP_FORWARD_IF_FALSE     3 (to 1782)
-         
-         124        1776 LOAD_CONST              31 ('mssql+pyodbc://sa:Posey3861@localhost:1433/SampleDB?driver=ODBC+Driver+18+for+SQL+Server&trusted_connection=no&Encrypt=no')
-                    1778 STORE_FAST               3 (rtn_abs_db_url)
-                    1780 JUMP_FORWARD            57 (to 1896)
-         
-         125     >> 1782 LOAD_FAST                1 (project)
-                    1784 LOAD_ATTR                0 (db_url)
-                    1794 LOAD_METHOD              1 (startswith)
-                    1816 LOAD_CONST              32 ('sqlsvr-nwlogic')
-                    1818 PRECALL                  1
-                    1822 CALL                     1
-                    1832 POP_JUMP_FORWARD_IF_FALSE     3 (to 1840)
-         
-         126        1834 LOAD_CONST              33 ('mssql+pyodbc://sa:Posey3861@localhost:1433/nwlogic?driver=ODBC+Driver+18+for+SQL+Server&trusted_connection=no&Encrypt=no')
-                    1836 STORE_FAST               3 (rtn_abs_db_url)
-                    1838 JUMP_FORWARD            28 (to 1896)
-         
-         127     >> 1840 LOAD_FAST                1 (project)
-                    1842 LOAD_ATTR                0 (db_url)
-                    1852 LOAD_METHOD              1 (startswith)
-                    1874 LOAD_CONST              34 ('sqlsvr-nw')
-                    1876 PRECALL                  1
-                    1880 CALL                     1
-                    1890 POP_JUMP_FORWARD_IF_FALSE     2 (to 1896)
-         
-         128        1892 LOAD_CONST              35 ('mssql+pyodbc://sa:Posey3861@localhost:1433/NORTHWND?driver=ODBC+Driver+18+for+SQL+Server&trusted_connection=no&Encrypt=no')
-                    1894 STORE_FAST               3 (rtn_abs_db_url)
-         
-         129     >> 1896 LOAD_CONST              36 ('models.py')
-                    1898 STORE_FAST               6 (model_file_name)
-         
-         130        1900 LOAD_FAST                1 (project)
-                    1902 LOAD_ATTR               13 (bind_key)
-                    1912 LOAD_CONST               1 ('')
-                    1914 COMPARE_OP               3 (!=)
-                    1920 POP_JUMP_FORWARD_IF_FALSE    13 (to 1948)
-         
-         131        1922 LOAD_FAST                1 (project)
-                    1924 LOAD_ATTR               13 (bind_key)
-                    1934 LOAD_CONST              37 ('_')
-                    1936 BINARY_OP                0 (+)
-                    1940 LOAD_CONST              36 ('models.py')
-                    1942 BINARY_OP                0 (+)
-                    1946 STORE_FAST               6 (model_file_name)
-         
-         132     >> 1948 LOAD_FAST                3 (rtn_abs_db_url)
-                    1950 LOAD_FAST                2 (rtn_nw_db_status)
-                    1952 LOAD_FAST                6 (model_file_name)
-                    1954 BUILD_TUPLE              3
-                    1956 RETURN_VALUE
+         118     >> 1458 LOAD_FAST                1 (project)
+                    1460 LOAD_ATTR                0 (db_url)
+                    1470 LOAD_CONST              27 ('classicmodels')
+                    1472 COMPARE_OP               2 (==)
+                    1478 POP_JUMP_FORWARD_IF_FALSE    43 (to 1566)
+         
+         119        1480 LOAD_CONST               7 ('sqlite:///')
+                    1482 LOAD_GLOBAL              5 (NULL + str)
+                    1494 LOAD_FAST                1 (project)
+                    1496 LOAD_ATTR                8 (api_logic_server_dir_path)
+                    1506 LOAD_METHOD              5 (joinpath)
+                    1528 LOAD_CONST              28 ('database/classicmodels.sqlite')
+                    1530 PRECALL                  1
+                    1534 CALL                     1
+                    1544 PRECALL                  1
+                    1548 CALL                     1
+                    1558 FORMAT_VALUE             0
+                    1560 BUILD_STRING             2
+                    1562 STORE_FAST               3 (rtn_abs_db_url)
+                    1564 JUMP_FORWARD           220 (to 2006)
+         
+         120     >> 1566 LOAD_FAST                1 (project)
+                    1568 LOAD_ATTR                0 (db_url)
+                    1578 LOAD_CONST              29 ('allocation')
+                    1580 COMPARE_OP               2 (==)
+                    1586 POP_JUMP_FORWARD_IF_FALSE    43 (to 1674)
+         
+         121        1588 LOAD_CONST               7 ('sqlite:///')
+                    1590 LOAD_GLOBAL              5 (NULL + str)
+                    1602 LOAD_FAST                1 (project)
+                    1604 LOAD_ATTR                8 (api_logic_server_dir_path)
+                    1614 LOAD_METHOD              5 (joinpath)
+                    1636 LOAD_CONST              30 ('database/allocation.sqlite')
+                    1638 PRECALL                  1
+                    1642 CALL                     1
+                    1652 PRECALL                  1
+                    1656 CALL                     1
+                    1666 FORMAT_VALUE             0
+                    1668 BUILD_STRING             2
+                    1670 STORE_FAST               3 (rtn_abs_db_url)
+                    1672 JUMP_FORWARD           166 (to 2006)
+         
+         122     >> 1674 LOAD_FAST                1 (project)
+                    1676 LOAD_ATTR                0 (db_url)
+                    1686 LOAD_METHOD              1 (startswith)
+                    1708 LOAD_CONST               7 ('sqlite:///')
+                    1710 PRECALL                  1
+                    1714 CALL                     1
+                    1724 POP_JUMP_FORWARD_IF_FALSE    54 (to 1834)
+         
+         123        1726 LOAD_FAST                1 (project)
+                    1728 LOAD_ATTR                0 (db_url)
+                    1738 LOAD_CONST              31 (10)
+                    1740 LOAD_GLOBAL             23 (NULL + len)
+                    1752 LOAD_FAST                1 (project)
+                    1754 LOAD_ATTR                0 (db_url)
+                    1764 PRECALL                  1
+                    1768 CALL                     1
+                    1778 BUILD_SLICE              2
+                    1780 BINARY_SUBSCR
+                    1790 STORE_FAST               5 (url)
+         
+         124        1792 LOAD_GLOBAL             25 (NULL + abspath)
+                    1804 LOAD_FAST                5 (url)
+                    1806 PRECALL                  1
+                    1810 CALL                     1
+                    1820 STORE_FAST               3 (rtn_abs_db_url)
+         
+         125        1822 LOAD_CONST               7 ('sqlite:///')
+                    1824 LOAD_FAST                3 (rtn_abs_db_url)
+                    1826 BINARY_OP                0 (+)
+                    1830 STORE_FAST               3 (rtn_abs_db_url)
+                    1832 JUMP_FORWARD            86 (to 2006)
+         
+         126     >> 1834 LOAD_FAST                1 (project)
+                    1836 LOAD_ATTR                0 (db_url)
+                    1846 LOAD_METHOD              1 (startswith)
+                    1868 LOAD_CONST              32 ('sqlsvr-sample')
+                    1870 PRECALL                  1
+                    1874 CALL                     1
+                    1884 POP_JUMP_FORWARD_IF_FALSE     3 (to 1892)
+         
+         127        1886 LOAD_CONST              33 ('mssql+pyodbc://sa:Posey3861@localhost:1433/SampleDB?driver=ODBC+Driver+18+for+SQL+Server&trusted_connection=no&Encrypt=no')
+                    1888 STORE_FAST               3 (rtn_abs_db_url)
+                    1890 JUMP_FORWARD            57 (to 2006)
+         
+         128     >> 1892 LOAD_FAST                1 (project)
+                    1894 LOAD_ATTR                0 (db_url)
+                    1904 LOAD_METHOD              1 (startswith)
+                    1926 LOAD_CONST              34 ('sqlsvr-nwlogic')
+                    1928 PRECALL                  1
+                    1932 CALL                     1
+                    1942 POP_JUMP_FORWARD_IF_FALSE     3 (to 1950)
+         
+         129        1944 LOAD_CONST              35 ('mssql+pyodbc://sa:Posey3861@localhost:1433/nwlogic?driver=ODBC+Driver+18+for+SQL+Server&trusted_connection=no&Encrypt=no')
+                    1946 STORE_FAST               3 (rtn_abs_db_url)
+                    1948 JUMP_FORWARD            28 (to 2006)
+         
+         130     >> 1950 LOAD_FAST                1 (project)
+                    1952 LOAD_ATTR                0 (db_url)
+                    1962 LOAD_METHOD              1 (startswith)
+                    1984 LOAD_CONST              36 ('sqlsvr-nw')
+                    1986 PRECALL                  1
+                    1990 CALL                     1
+                    2000 POP_JUMP_FORWARD_IF_FALSE     2 (to 2006)
+         
+         131        2002 LOAD_CONST              37 ('mssql+pyodbc://sa:Posey3861@localhost:1433/NORTHWND?driver=ODBC+Driver+18+for+SQL+Server&trusted_connection=no&Encrypt=no')
+                    2004 STORE_FAST               3 (rtn_abs_db_url)
+         
+         132     >> 2006 LOAD_CONST              38 ('models.py')
+                    2008 STORE_FAST               6 (model_file_name)
+         
+         133        2010 LOAD_FAST                1 (project)
+                    2012 LOAD_ATTR               13 (bind_key)
+                    2022 LOAD_CONST               1 ('')
+                    2024 COMPARE_OP               3 (!=)
+                    2030 POP_JUMP_FORWARD_IF_FALSE    13 (to 2058)
+         
+         134        2032 LOAD_FAST                1 (project)
+                    2034 LOAD_ATTR               13 (bind_key)
+                    2044 LOAD_CONST              39 ('_')
+                    2046 BINARY_OP                0 (+)
+                    2050 LOAD_CONST              38 ('models.py')
+                    2052 BINARY_OP                0 (+)
+                    2056 STORE_FAST               6 (model_file_name)
+         
+         135     >> 2058 LOAD_FAST                3 (rtn_abs_db_url)
+                    2060 LOAD_FAST                2 (rtn_nw_db_status)
+                    2062 LOAD_FAST                6 (model_file_name)
+                    2064 BUILD_TUPLE              3
+                    2066 RETURN_VALUE
          consts
-            "\n    non-relative db location - we work with this\n\n    handle db_url abbreviations (nw, nw-, todo etc)\n\n    but NB: we copy sqlite db to <project>/database - see create_project_with_nw_samples (below)\n\n    also: compute physical nw db name (usually nw-gold) to be used for copy\n\n    returns abs_db_url, nw_db_status - the real url (e.g., for nw), and whether it's really nw, and model_file_name\n    "
+            "\n    non-relative db location - we work with this\n\n    handle db_url abbreviations (nw, nw-, todo, allocation, etc)\n\n    but NB: we copy sqlite db to <project>/database - see create_project_with_nw_samples (below)\n\n    also: compute physical nw db name (usually nw-gold) to be used for copy\n\n    returns abs_db_url, nw_db_status - the real url (e.g., for nw), and whether it's really nw, and model_file_name\n    "
             ''
             '{install}'
             'database'
             'SqlServer-arm'
             'nw'
             'sqlite:///nw.sqlite'
             'sqlite:///'
@@ -886,14 +911,16 @@
             'database/todos.sqlite'
             'new'
             'database/new.sqlite'
             'table_filters_tests'
             'database/table_filters_tests.sqlite'
             'classicmodels'
             'database/classicmodels.sqlite'
+            'allocation'
+            'database/allocation.sqlite'
             10
             'sqlsvr-sample'
             'mssql+pyodbc://sa:Posey3861@localhost:1433/SampleDB?driver=ODBC+Driver+18+for+SQL+Server&trusted_connection=no&Encrypt=no'
             'sqlsvr-nwlogic'
             'mssql+pyodbc://sa:Posey3861@localhost:1433/nwlogic?driver=ODBC+Driver+18+for+SQL+Server&trusted_connection=no&Encrypt=no'
             'sqlsvr-nw'
             'mssql+pyodbc://sa:Posey3861@localhost:1433/NORTHWND?driver=ODBC+Driver+18+for+SQL+Server&trusted_connection=no&Encrypt=no'
@@ -903,58 +930,58 @@
          varnames   ('msg', 'project', 'rtn_nw_db_status', 'rtn_abs_db_url', 'install_db', 'url', 'model_file_name')
          freevars   ()
          cellvars   ()
          filename   '/Users/val/dev/ApiLogicServer/api_logic_server_cli/create_from_model/api_logic_server_utils.py'
          name       'get_abs_db_url'
          firstlineno 63
          lnotab
-            0x020c04010e032a0176012c012a01020202082401540104014201160154
+            0x020c04010e032a0176012c012a01020202082401540104024201160154
             01080116015401080116015401040142012c015801160158012c01580116
-            0158011601560116015601340142011e010c013401060134010601340104
-            01040116011a01
+            015801160158011601560116015601340142011e010c0134010601340106
+            0134010401040116011a01
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 3
          flags     : 3
          code
             0x9700740100000000000000000000740200000000000000000000a60100
             00ab0100000000000000007d007c006a0200000000000000007d017c016a
             0200000000000000007d017407000000000000000000007c01a6010000ab
             0100000000000000005300
-         135           0 RESUME                   0
+         138           0 RESUME                   0
          
-         139           2 LOAD_GLOBAL              1 (NULL + Path)
+         142           2 LOAD_GLOBAL              1 (NULL + Path)
                       14 LOAD_GLOBAL              2 (__file__)
                       26 PRECALL                  1
                       30 CALL                     1
                       40 STORE_FAST               0 (path)
          
-         140          42 LOAD_FAST                0 (path)
+         143          42 LOAD_FAST                0 (path)
                       44 LOAD_ATTR                2 (parent)
                       54 STORE_FAST               1 (parent_path)
          
-         141          56 LOAD_FAST                1 (parent_path)
+         144          56 LOAD_FAST                1 (parent_path)
                       58 LOAD_ATTR                2 (parent)
                       68 STORE_FAST               1 (parent_path)
          
-         142          70 LOAD_GLOBAL              7 (NULL + str)
+         145          70 LOAD_GLOBAL              7 (NULL + str)
                       82 LOAD_FAST                1 (parent_path)
                       84 PRECALL                  1
                       88 CALL                     1
                       98 RETURN_VALUE
          consts
             '\n    :return: ApiLogicServer dir, eg, /Users/val/dev/ApiLogicServer\n    '
          names      ('Path', '__file__', 'parent', 'str')
          varnames   ('path', 'parent_path')
          freevars   ()
          cellvars   ()
          filename   '/Users/val/dev/ApiLogicServer/api_logic_server_cli/create_from_model/api_logic_server_utils.py'
          name       'get_api_logic_server_dir'
-         firstlineno 135
+         firstlineno 138
          lnotab 0x020428010e010e01
       'search_for'
       'in_file'
       code
          argcount  : 2
          nlocals   : 7
          stacksize : 6
@@ -962,57 +989,57 @@
          code
             0x97007401000000000000000000007c016401a6020000ab020000000000
             00000035007d027c02a00100000000000000000000000000000000000000
             00a6000000ab0000000000000000007d0364027d0464037d057c0344005d
             0a7d067c007c067600720464047d0401006e018c0b7c0463026405640564
             05a6020000ab020000000000000000010053002300310073047702780359
             007701010059000100010064055300
-         145           0 RESUME                   0
+         148           0 RESUME                   0
          
-         147           2 LOAD_GLOBAL              1 (NULL + open)
+         150           2 LOAD_GLOBAL              1 (NULL + open)
                       14 LOAD_FAST                1 (in_file)
                       16 LOAD_CONST               1 ('r+')
                       18 PRECALL                  2
                       22 CALL                     2
                       32 BEFORE_WITH
                       34 STORE_FAST               2 (fp)
          
-         148          36 LOAD_FAST                2 (fp)
+         151          36 LOAD_FAST                2 (fp)
                       38 LOAD_METHOD              1 (readlines)
                       60 PRECALL                  0
                       64 CALL                     0
                       74 STORE_FAST               3 (file_lines)
          
-         149          76 LOAD_CONST               2 (False)
+         152          76 LOAD_CONST               2 (False)
                       78 STORE_FAST               4 (found)
          
-         150          80 LOAD_CONST               3 (0)
+         153          80 LOAD_CONST               3 (0)
                       82 STORE_FAST               5 (insert_line)
          
-         151          84 LOAD_FAST                3 (file_lines)
+         154          84 LOAD_FAST                3 (file_lines)
                       86 GET_ITER
                  >>   88 FOR_ITER                10 (to 110)
                       90 STORE_FAST               6 (each_line)
          
-         152          92 LOAD_FAST                0 (search_for)
+         155          92 LOAD_FAST                0 (search_for)
                       94 LOAD_FAST                6 (each_line)
                       96 CONTAINS_OP              0
                       98 POP_JUMP_FORWARD_IF_FALSE     4 (to 108)
          
-         153         100 LOAD_CONST               4 (True)
+         156         100 LOAD_CONST               4 (True)
                      102 STORE_FAST               4 (found)
          
-         154         104 POP_TOP
+         157         104 POP_TOP
                      106 JUMP_FORWARD             1 (to 110)
          
-         152     >>  108 JUMP_BACKWARD           11 (to 88)
+         155     >>  108 JUMP_BACKWARD           11 (to 88)
          
-         155     >>  110 LOAD_FAST                4 (found)
+         158     >>  110 LOAD_FAST                4 (found)
          
-         147         112 SWAP                     2
+         150         112 SWAP                     2
                      114 LOAD_CONST               5 (None)
                      116 LOAD_CONST               5 (None)
                      118 LOAD_CONST               5 (None)
                      120 PRECALL                  2
                      124 CALL                     2
                      134 POP_TOP
                      136 RETURN_VALUE
@@ -1042,15 +1069,15 @@
             None
          names      ('open', 'readlines')
          varnames   ('search_for', 'in_file', 'fp', 'file_lines', 'found', 'insert_line', 'each_line')
          freevars   ()
          cellvars   ()
          filename   '/Users/val/dev/ApiLogicServer/api_logic_server_cli/create_from_model/api_logic_server_utils.py'
          name       'does_file_contain'
-         firstlineno 145
+         firstlineno 148
          lnotab 0x0202220128010401040108010801040104fe020302f8
       'replace_with'
       code
          argcount  : 3
          nlocals   : 5
          stacksize : 6
          flags     : 3
@@ -1061,39 +1088,39 @@
             00000000000000000000007c007c01a6020000ab0200000000000000007d
             04640064006400a6020000ab02000000000000000001006e0b2300310073
             04770278035900770101005900010001007401000000000000000000007c
             026402a6020000ab02000000000000000035007d037c03a0030000000000
             0000000000000000000000000000007c04a6010000ab0100000000000000
             000100640064006400a6020000ab02000000000000000001006400530023
             00310073047702780359007701010059000100010064005300
-         157           0 RESUME                   0
+         160           0 RESUME                   0
          
-         158           2 LOAD_GLOBAL              1 (NULL + open)
+         161           2 LOAD_GLOBAL              1 (NULL + open)
                       14 LOAD_FAST                2 (in_file)
                       16 LOAD_CONST               1 ('r')
                       18 PRECALL                  2
                       22 CALL                     2
                       32 BEFORE_WITH
                       34 STORE_FAST               3 (file)
          
-         159          36 LOAD_FAST                3 (file)
+         162          36 LOAD_FAST                3 (file)
                       38 LOAD_METHOD              1 (read)
                       60 PRECALL                  0
                       64 CALL                     0
                       74 STORE_FAST               4 (file_data)
          
-         160          76 LOAD_FAST                4 (file_data)
+         163          76 LOAD_FAST                4 (file_data)
                       78 LOAD_METHOD              2 (replace)
                      100 LOAD_FAST                0 (search_for)
                      102 LOAD_FAST                1 (replace_with)
                      104 PRECALL                  2
                      108 CALL                     2
                      118 STORE_FAST               4 (file_data)
          
-         158         120 LOAD_CONST               0 (None)
+         161         120 LOAD_CONST               0 (None)
                      122 LOAD_CONST               0 (None)
                      124 LOAD_CONST               0 (None)
                      126 PRECALL                  2
                      130 CALL                     2
                      140 POP_TOP
                      142 JUMP_FORWARD            11 (to 166)
                  >>  144 PUSH_EXC_INFO
@@ -1104,30 +1131,30 @@
                      154 POP_EXCEPT
                      156 RERAISE                  1
                  >>  158 POP_TOP
                      160 POP_EXCEPT
                      162 POP_TOP
                      164 POP_TOP
          
-         161     >>  166 LOAD_GLOBAL              1 (NULL + open)
+         164     >>  166 LOAD_GLOBAL              1 (NULL + open)
                      178 LOAD_FAST                2 (in_file)
                      180 LOAD_CONST               2 ('w')
                      182 PRECALL                  2
                      186 CALL                     2
                      196 BEFORE_WITH
                      198 STORE_FAST               3 (file)
          
-         162         200 LOAD_FAST                3 (file)
+         165         200 LOAD_FAST                3 (file)
                      202 LOAD_METHOD              3 (write)
                      224 LOAD_FAST                4 (file_data)
                      226 PRECALL                  1
                      230 CALL                     1
                      240 POP_TOP
          
-         161         242 LOAD_CONST               0 (None)
+         164         242 LOAD_CONST               0 (None)
                      244 LOAD_CONST               0 (None)
                      246 LOAD_CONST               0 (None)
                      248 PRECALL                  2
                      252 CALL                     2
                      262 POP_TOP
                      264 LOAD_CONST               0 (None)
                      266 RETURN_VALUE
@@ -1157,15 +1184,15 @@
             'w'
          names      ('open', 'read', 'replace', 'write')
          varnames   ('search_for', 'replace_with', 'in_file', 'file', 'file_data')
          freevars   ()
          cellvars   ()
          filename   '/Users/val/dev/ApiLogicServer/api_logic_server_cli/create_from_model/api_logic_server_utils.py'
          name       'replace_string_in_file'
-         firstlineno 157
+         firstlineno 160
          lnotab 0x0201220128012cfe2e0322012aff
       False
       'lines'
       'at'
       'file_name'
       'after'
       code
@@ -1182,101 +1209,101 @@
             01000000000000000082017c0372057c0764057a0000007d077c05a00300
             000000000000000000000000000000000000007c077c00a6020000ab0200
             0000000000000001007c04a0040000000000000000000000000000000000
             0000006403a6010000ab01000000000000000001007c04a0050000000000
             0000000000000000000000000000007c05a6010000ab0100000000000000
             000100640764076407a6020000ab02000000000000000001006407530023
             00310073047702780359007701010059000100010064075300
-         165           0 RESUME                   0
+         168           0 RESUME                   0
          
-         167           2 LOAD_GLOBAL              1 (NULL + open)
+         170           2 LOAD_GLOBAL              1 (NULL + open)
                       14 LOAD_FAST                2 (file_name)
                       16 LOAD_CONST               1 ('r+')
                       18 PRECALL                  2
                       22 CALL                     2
                       32 BEFORE_WITH
                       34 STORE_FAST               4 (fp)
          
-         168          36 LOAD_FAST                4 (fp)
+         171          36 LOAD_FAST                4 (fp)
                       38 LOAD_METHOD              1 (readlines)
                       60 PRECALL                  0
                       64 CALL                     0
                       74 STORE_FAST               5 (file_lines)
          
-         169          76 LOAD_CONST               2 (False)
+         172          76 LOAD_CONST               2 (False)
                       78 STORE_FAST               6 (found)
          
-         170          80 LOAD_CONST               3 (0)
+         173          80 LOAD_CONST               3 (0)
                       82 STORE_FAST               7 (insert_line)
          
-         171          84 LOAD_FAST                5 (file_lines)
+         174          84 LOAD_FAST                5 (file_lines)
                       86 GET_ITER
                  >>   88 FOR_ITER                15 (to 120)
                       90 STORE_FAST               8 (each_line)
          
-         172          92 LOAD_FAST                1 (at)
+         175          92 LOAD_FAST                1 (at)
                       94 LOAD_FAST                8 (each_line)
                       96 CONTAINS_OP              0
                       98 POP_JUMP_FORWARD_IF_FALSE     4 (to 108)
          
-         173         100 LOAD_CONST               4 (True)
+         176         100 LOAD_CONST               4 (True)
                      102 STORE_FAST               6 (found)
          
-         174         104 POP_TOP
+         177         104 POP_TOP
                      106 JUMP_FORWARD             6 (to 120)
          
-         175     >>  108 LOAD_FAST                7 (insert_line)
+         178     >>  108 LOAD_FAST                7 (insert_line)
                      110 LOAD_CONST               5 (1)
                      112 BINARY_OP               13 (+=)
                      116 STORE_FAST               7 (insert_line)
                      118 JUMP_BACKWARD           16 (to 88)
          
-         176     >>  120 LOAD_FAST                6 (found)
+         179     >>  120 LOAD_FAST                6 (found)
                      122 POP_JUMP_FORWARD_IF_TRUE    18 (to 160)
          
-         177         124 LOAD_GLOBAL              5 (NULL + Exception)
+         180         124 LOAD_GLOBAL              5 (NULL + Exception)
                      136 LOAD_CONST               6 ('Internal error - unable to find insert: ')
                      138 LOAD_FAST                1 (at)
                      140 FORMAT_VALUE             0
                      142 BUILD_STRING             2
                      144 PRECALL                  1
                      148 CALL                     1
                      158 RAISE_VARARGS            1
          
-         178     >>  160 LOAD_FAST                3 (after)
+         181     >>  160 LOAD_FAST                3 (after)
                      162 POP_JUMP_FORWARD_IF_FALSE     5 (to 174)
          
-         179         164 LOAD_FAST                7 (insert_line)
+         182         164 LOAD_FAST                7 (insert_line)
                      166 LOAD_CONST               5 (1)
                      168 BINARY_OP                0 (+)
                      172 STORE_FAST               7 (insert_line)
          
-         180     >>  174 LOAD_FAST                5 (file_lines)
+         183     >>  174 LOAD_FAST                5 (file_lines)
                      176 LOAD_METHOD              3 (insert)
                      198 LOAD_FAST                7 (insert_line)
                      200 LOAD_FAST                0 (lines)
                      202 PRECALL                  2
                      206 CALL                     2
                      216 POP_TOP
          
-         181         218 LOAD_FAST                4 (fp)
+         184         218 LOAD_FAST                4 (fp)
                      220 LOAD_METHOD              4 (seek)
                      242 LOAD_CONST               3 (0)
                      244 PRECALL                  1
                      248 CALL                     1
                      258 POP_TOP
          
-         182         260 LOAD_FAST                4 (fp)
+         185         260 LOAD_FAST                4 (fp)
                      262 LOAD_METHOD              5 (writelines)
                      284 LOAD_FAST                5 (file_lines)
                      286 PRECALL                  1
                      290 CALL                     1
                      300 POP_TOP
          
-         167         302 LOAD_CONST               7 (None)
+         170         302 LOAD_CONST               7 (None)
                      304 LOAD_CONST               7 (None)
                      306 LOAD_CONST               7 (None)
                      308 PRECALL                  2
                      312 CALL                     2
                      322 POP_TOP
                      324 LOAD_CONST               7 (None)
                      326 RETURN_VALUE
@@ -1308,15 +1335,15 @@
             None
          names      ('open', 'readlines', 'Exception', 'insert', 'seek', 'writelines')
          varnames   ('lines', 'at', 'file_name', 'after', 'fp', 'file_lines', 'found', 'insert_line', 'each_line')
          freevars   ()
          cellvars   ()
          filename   '/Users/val/dev/ApiLogicServer/api_logic_server_cli/create_from_model/api_logic_server_utils.py'
          name       'insert_lines_at'
-         firstlineno 165
+         firstlineno 168
          lnotab
             0x0202220128010401040108010801040104010c010401240104010a012c
             012a012af1
       code
          argcount  : 0
          nlocals   : 4
          stacksize : 6
@@ -1327,103 +1354,103 @@
             030000ab0300000000000000007d016e5723007406000000000000000000
             002400724a7d0264017d0009007401000000000000000000006a01000000
             0000000000640564037400000000000000000000006a0200000000000000
             00ac04a6030000ab0300000000000000007d016e19230074060000000000
             00000000002400720c7d0364017d00590064067d037e036e0864067d037e
             037701770078035900770164037d00590064067d027e026e0864067d027e
             02770177007803590077017c0072026407530064085300
-         185           0 RESUME                   0
+         188           0 RESUME                   0
          
-         191           2 LOAD_CONST               1 (False)
+         194           2 LOAD_CONST               1 (False)
                        4 STORE_FAST               0 (python3_worked)
          
-         192           6 NOP
+         195           6 NOP
          
-         193           8 LOAD_GLOBAL              1 (NULL + subprocess)
+         196           8 LOAD_GLOBAL              1 (NULL + subprocess)
                       20 LOAD_ATTR                1 (check_output)
                       30 LOAD_CONST               2 ('python --version')
                       32 LOAD_CONST               3 (True)
                       34 LOAD_GLOBAL              0 (subprocess)
                       46 LOAD_ATTR                2 (STDOUT)
                       56 KW_NAMES                 4
                       58 PRECALL                  3
                       62 CALL                     3
                       72 STORE_FAST               1 (result_b)
                       74 JUMP_FORWARD            87 (to 250)
                  >>   76 PUSH_EXC_INFO
          
-         194          78 LOAD_GLOBAL              6 (Exception)
+         197          78 LOAD_GLOBAL              6 (Exception)
                       90 CHECK_EXC_MATCH
                       92 POP_JUMP_FORWARD_IF_FALSE    74 (to 242)
                       94 STORE_FAST               2 (e)
          
-         195          96 LOAD_CONST               1 (False)
+         198          96 LOAD_CONST               1 (False)
                       98 STORE_FAST               0 (python3_worked)
          
-         196         100 NOP
+         199         100 NOP
          
-         197         102 LOAD_GLOBAL              1 (NULL + subprocess)
+         200         102 LOAD_GLOBAL              1 (NULL + subprocess)
                      114 LOAD_ATTR                1 (check_output)
                      124 LOAD_CONST               5 ('python3 --version')
                      126 LOAD_CONST               3 (True)
                      128 LOAD_GLOBAL              0 (subprocess)
                      140 LOAD_ATTR                2 (STDOUT)
                      150 KW_NAMES                 4
                      152 PRECALL                  3
                      156 CALL                     3
                      166 STORE_FAST               1 (result_b)
                      168 JUMP_FORWARD            25 (to 220)
                  >>  170 PUSH_EXC_INFO
          
-         198         172 LOAD_GLOBAL              6 (Exception)
+         201         172 LOAD_GLOBAL              6 (Exception)
                      184 CHECK_EXC_MATCH
                      186 POP_JUMP_FORWARD_IF_FALSE    12 (to 212)
                      188 STORE_FAST               3 (e1)
          
-         199         190 LOAD_CONST               1 (False)
+         202         190 LOAD_CONST               1 (False)
                      192 STORE_FAST               0 (python3_worked)
                      194 POP_EXCEPT
                      196 LOAD_CONST               6 (None)
                      198 STORE_FAST               3 (e1)
                      200 DELETE_FAST              3 (e1)
                      202 JUMP_FORWARD             8 (to 220)
                  >>  204 LOAD_CONST               6 (None)
                      206 STORE_FAST               3 (e1)
                      208 DELETE_FAST              3 (e1)
                      210 RERAISE                  1
          
-         198     >>  212 RERAISE                  0
+         201     >>  212 RERAISE                  0
                  >>  214 COPY                     3
                      216 POP_EXCEPT
                      218 RERAISE                  1
          
-         200     >>  220 LOAD_CONST               3 (True)
+         203     >>  220 LOAD_CONST               3 (True)
                      222 STORE_FAST               0 (python3_worked)
                      224 POP_EXCEPT
                      226 LOAD_CONST               6 (None)
                      228 STORE_FAST               2 (e)
                      230 DELETE_FAST              2 (e)
                      232 JUMP_FORWARD             8 (to 250)
                  >>  234 LOAD_CONST               6 (None)
                      236 STORE_FAST               2 (e)
                      238 DELETE_FAST              2 (e)
                      240 RERAISE                  1
          
-         194     >>  242 RERAISE                  0
+         197     >>  242 RERAISE                  0
                  >>  244 COPY                     3
                      246 POP_EXCEPT
                      248 RERAISE                  1
          
-         201     >>  250 LOAD_FAST                0 (python3_worked)
+         204     >>  250 LOAD_FAST                0 (python3_worked)
                      252 POP_JUMP_FORWARD_IF_FALSE     2 (to 258)
          
-         202         254 LOAD_CONST               7 ('python3')
+         205         254 LOAD_CONST               7 ('python3')
                      256 RETURN_VALUE
          
-         204     >>  258 LOAD_CONST               8 ('python')
+         207     >>  258 LOAD_CONST               8 ('python')
                      260 RETURN_VALUE
          ExceptionTable:
            8 to 72 -> 76 [0]
            76 to 94 -> 244 [1] lasti
            96 to 98 -> 234 [1] lasti
            102 to 166 -> 170 [1]
            168 to 168 -> 234 [1] lasti
@@ -1445,15 +1472,15 @@
             'python'
          names      ('subprocess', 'check_output', 'STDOUT', 'Exception')
          varnames   ('python3_worked', 'result_b', 'e', 'e1')
          freevars   ()
          cellvars   ()
          filename   '/Users/val/dev/ApiLogicServer/api_logic_server_cli/create_from_model/api_logic_server_utils.py'
          name       'find_valid_python_name'
-         firstlineno 185
+         firstlineno 188
          lnotab
             0x02060401020146011201040102014601120116ff080216fa0807040104
             02
       ''
       'cmd'
       'msg'
       'new_line'
@@ -1487,204 +1514,204 @@
             00000000007c0ba6010000ab01000000000000000064107a0a0000850219
             0000000000000000007d0b6411741b000000000000000000007c00a60100
             00ab0100000000000000007a0a00007d0c64067c0c7a0500007d0d7c0264
             056b020000000072016e307c0b64026b0300000000722a7c0b64126b0300
             0000007224740600000000000000000000a0040000000000000000000000
             0000000000000000007c059b0064067c009b0064137c0d9b007c0b9b009d
             06a6010000ab01000000000000000001007c0b5300
-         207           0 RESUME                   0
+         210           0 RESUME                   0
          
-         215           2 LOAD_FAST                0 (cmd)
+         218           2 LOAD_FAST                0 (cmd)
                        4 LOAD_METHOD              0 (startswith)
                       26 LOAD_CONST               1 ('python')
                       28 PRECALL                  1
                       32 CALL                     1
                       42 POP_JUMP_FORWARD_IF_FALSE    36 (to 116)
          
-         216          44 LOAD_GLOBAL              3 (NULL + find_valid_python_name)
+         219          44 LOAD_GLOBAL              3 (NULL + find_valid_python_name)
                       56 PRECALL                  0
                       60 CALL                     0
                       70 STORE_FAST               4 (valid_python_name)
          
-         217          72 LOAD_FAST                0 (cmd)
+         220          72 LOAD_FAST                0 (cmd)
                       74 LOAD_METHOD              2 (replace)
                       96 LOAD_CONST               1 ('python')
                       98 LOAD_FAST                4 (valid_python_name)
                      100 PRECALL                  2
                      104 CALL                     2
                      114 STORE_FAST               0 (cmd)
          
-         218     >>  116 LOAD_CONST               2 ('')
+         221     >>  116 LOAD_CONST               2 ('')
                      118 STORE_FAST               5 (log_msg)
          
-         219         120 LOAD_FAST                2 (msg)
+         222         120 LOAD_FAST                2 (msg)
                      122 LOAD_CONST               3 ('Execute command:')
                      124 COMPARE_OP               3 (!=)
                      130 POP_JUMP_FORWARD_IF_FALSE     5 (to 142)
          
-         220         132 LOAD_FAST                2 (msg)
+         223         132 LOAD_FAST                2 (msg)
                      134 LOAD_CONST               4 (' with command:')
                      136 BINARY_OP                0 (+)
                      140 STORE_FAST               5 (log_msg)
          
-         221     >>  142 LOAD_FAST                2 (msg)
+         224     >>  142 LOAD_FAST                2 (msg)
                      144 LOAD_CONST               5 ('no-msg')
                      146 COMPARE_OP               2 (==)
                      152 POP_JUMP_FORWARD_IF_FALSE     3 (to 160)
          
-         222         154 LOAD_CONST               2 ('')
+         225         154 LOAD_CONST               2 ('')
                      156 STORE_FAST               5 (log_msg)
                      158 JUMP_FORWARD            31 (to 222)
          
-         224     >>  160 LOAD_GLOBAL              6 (log)
+         227     >>  160 LOAD_GLOBAL              6 (log)
                      172 LOAD_METHOD              4 (debug)
                      194 LOAD_FAST                5 (log_msg)
                      196 FORMAT_VALUE             0
                      198 LOAD_CONST               6 (' ')
                      200 LOAD_FAST                0 (cmd)
                      202 FORMAT_VALUE             0
                      204 BUILD_STRING             3
                      206 PRECALL                  1
                      210 CALL                     1
                      220 POP_TOP
          
-         225     >>  222 LOAD_FAST                3 (new_line)
+         228     >>  222 LOAD_FAST                3 (new_line)
                      224 POP_JUMP_FORWARD_IF_FALSE    26 (to 278)
          
-         226         226 LOAD_GLOBAL              6 (log)
+         229         226 LOAD_GLOBAL              6 (log)
                      238 LOAD_METHOD              4 (debug)
                      260 LOAD_CONST               2 ('')
                      262 PRECALL                  1
                      266 CALL                     1
                      276 POP_TOP
          
-         228     >>  278 LOAD_FAST                1 (env)
+         231     >>  278 LOAD_FAST                1 (env)
                      280 STORE_FAST               6 (use_env)
          
-         229         282 LOAD_FAST                1 (env)
+         232         282 LOAD_FAST                1 (env)
                      284 POP_JUMP_FORWARD_IF_NOT_NONE   101 (to 488)
          
-         230         286 LOAD_GLOBAL             11 (NULL + get_api_logic_server_dir)
+         233         286 LOAD_GLOBAL             11 (NULL + get_api_logic_server_dir)
                      298 PRECALL                  0
                      302 CALL                     0
                      312 STORE_FAST               7 (project_dir)
          
-         231         314 LOAD_GLOBAL             13 (NULL + str)
+         234         314 LOAD_GLOBAL             13 (NULL + str)
                      326 LOAD_FAST                7 (project_dir)
                      328 PRECALL                  1
                      332 CALL                     1
                      342 LOAD_CONST               8 ('/venv/lib/python3.9/site_packages')
                      344 BINARY_OP                0 (+)
                      348 STORE_FAST               8 (python_path)
          
-         232         350 LOAD_GLOBAL             14 (os)
+         235         350 LOAD_GLOBAL             14 (os)
                      362 LOAD_ATTR                8 (environ)
                      372 LOAD_METHOD              9 (copy)
                      394 PRECALL                  0
                      398 CALL                     0
                      408 STORE_FAST               6 (use_env)
          
-         234         410 LOAD_GLOBAL             21 (NULL + hasattr)
+         237         410 LOAD_GLOBAL             21 (NULL + hasattr)
                      422 LOAD_FAST                6 (use_env)
                      424 LOAD_CONST               9 ('PYTHONPATH')
                      426 PRECALL                  2
                      430 CALL                     2
                      440 POP_JUMP_FORWARD_IF_FALSE    18 (to 478)
          
-         235         442 LOAD_FAST                8 (python_path)
+         238         442 LOAD_FAST                8 (python_path)
                      444 LOAD_CONST              10 (':')
                      446 BINARY_OP                0 (+)
                      450 LOAD_FAST                6 (use_env)
                      452 LOAD_CONST               9 ('PYTHONPATH')
                      454 BINARY_SUBSCR
                      464 BINARY_OP                0 (+)
                      468 LOAD_FAST                6 (use_env)
                      470 LOAD_CONST               9 ('PYTHONPATH')
                      472 STORE_SUBSCR
                      476 JUMP_FORWARD             5 (to 488)
          
-         238     >>  478 LOAD_FAST                8 (python_path)
+         241     >>  478 LOAD_FAST                8 (python_path)
                      480 LOAD_FAST                6 (use_env)
                      482 LOAD_CONST               9 ('PYTHONPATH')
                      484 STORE_SUBSCR
          
-         240     >>  488 LOAD_CONST              11 (False)
+         243     >>  488 LOAD_CONST              11 (False)
                      490 STORE_FAST               9 (use_env_debug)
          
-         241         492 LOAD_FAST                9 (use_env_debug)
+         244         492 LOAD_FAST                9 (use_env_debug)
                      494 POP_JUMP_FORWARD_IF_FALSE    24 (to 544)
          
-         242         496 LOAD_GLOBAL             23 (NULL + subprocess)
+         245         496 LOAD_GLOBAL             23 (NULL + subprocess)
                      508 LOAD_ATTR               12 (check_output)
                      518 LOAD_FAST                0 (cmd)
                      520 LOAD_CONST              12 (True)
                      522 LOAD_FAST                6 (use_env)
                      524 KW_NAMES                13
                      526 PRECALL                  3
                      530 CALL                     3
                      540 STORE_FAST              10 (result_b)
                      542 JUMP_FORWARD            22 (to 588)
          
-         244     >>  544 LOAD_GLOBAL             23 (NULL + subprocess)
+         247     >>  544 LOAD_GLOBAL             23 (NULL + subprocess)
                      556 LOAD_ATTR               12 (check_output)
                      566 LOAD_FAST                0 (cmd)
                      568 LOAD_CONST              12 (True)
                      570 KW_NAMES                14
                      572 PRECALL                  2
                      576 CALL                     2
                      586 STORE_FAST              10 (result_b)
          
-         245     >>  588 LOAD_GLOBAL             13 (NULL + str)
+         248     >>  588 LOAD_GLOBAL             13 (NULL + str)
                      600 LOAD_FAST               10 (result_b)
                      602 PRECALL                  1
                      606 CALL                     1
                      616 STORE_FAST              11 (result)
          
-         246         618 LOAD_FAST               11 (result)
+         249         618 LOAD_FAST               11 (result)
                      620 LOAD_CONST              15 (2)
                      622 LOAD_GLOBAL             27 (NULL + len)
                      634 LOAD_FAST               11 (result)
                      636 PRECALL                  1
                      640 CALL                     1
                      650 LOAD_CONST              16 (3)
                      652 BINARY_OP               10 (-)
                      656 BUILD_SLICE              2
                      658 BINARY_SUBSCR
                      668 STORE_FAST              11 (result)
          
-         247         670 LOAD_CONST              17 (20)
+         250         670 LOAD_CONST              17 (20)
                      672 LOAD_GLOBAL             27 (NULL + len)
                      684 LOAD_FAST                0 (cmd)
                      686 PRECALL                  1
                      690 CALL                     1
                      700 BINARY_OP               10 (-)
                      704 STORE_FAST              12 (tab_to)
          
-         248         706 LOAD_CONST               6 (' ')
+         251         706 LOAD_CONST               6 (' ')
                      708 LOAD_FAST               12 (tab_to)
                      710 BINARY_OP                5 (*)
                      714 STORE_FAST              13 (spaces)
          
-         249         716 LOAD_FAST                2 (msg)
+         252         716 LOAD_FAST                2 (msg)
                      718 LOAD_CONST               5 ('no-msg')
                      720 COMPARE_OP               2 (==)
                      726 POP_JUMP_FORWARD_IF_FALSE     1 (to 730)
          
-         250         728 JUMP_FORWARD            48 (to 826)
+         253         728 JUMP_FORWARD            48 (to 826)
          
-         251     >>  730 LOAD_FAST               11 (result)
+         254     >>  730 LOAD_FAST               11 (result)
                      732 LOAD_CONST               2 ('')
                      734 COMPARE_OP               3 (!=)
                      740 POP_JUMP_FORWARD_IF_FALSE    42 (to 826)
                      742 LOAD_FAST               11 (result)
                      744 LOAD_CONST              18 ('Downloaded the skeleton app, good coding!')
                      746 COMPARE_OP               3 (!=)
                      752 POP_JUMP_FORWARD_IF_FALSE    36 (to 826)
          
-         252         754 LOAD_GLOBAL              6 (log)
+         255         754 LOAD_GLOBAL              6 (log)
                      766 LOAD_METHOD              4 (debug)
                      788 LOAD_FAST                5 (log_msg)
                      790 FORMAT_VALUE             0
                      792 LOAD_CONST               6 (' ')
                      794 LOAD_FAST                0 (cmd)
                      796 FORMAT_VALUE             0
                      798 LOAD_CONST              19 (' result: ')
@@ -1693,15 +1720,15 @@
                      804 LOAD_FAST               11 (result)
                      806 FORMAT_VALUE             0
                      808 BUILD_STRING             6
                      810 PRECALL                  1
                      814 CALL                     1
                      824 POP_TOP
          
-         253     >>  826 LOAD_FAST               11 (result)
+         256     >>  826 LOAD_FAST               11 (result)
                      828 RETURN_VALUE
          consts
             ' run shell command\n\n    :param cmd: string of command to execute\n    :param env:\n    :param msg: optional message (no-msg to suppress)\n    :return:\n    '
             'python'
             ''
             'Execute command:'
             ' with command:'
@@ -1722,24 +1749,24 @@
             ' result: '
          names      ('startswith', 'find_valid_python_name', 'replace', 'log', 'debug', 'get_api_logic_server_dir', 'str', 'os', 'environ', 'copy', 'hasattr', 'subprocess', 'check_output', 'len')
          varnames   ('cmd', 'env', 'msg', 'new_line', 'valid_python_name', 'log_msg', 'use_env', 'project_dir', 'python_path', 'use_env_debug', 'result_b', 'result', 'tab_to', 'spaces')
          freevars   ()
          cellvars   ()
          filename   '/Users/val/dev/ApiLogicServer/api_logic_server_cli/create_from_model/api_logic_server_utils.py'
          name       'run_command'
-         firstlineno 207
+         firstlineno 210
          lnotab
             0x02082a011c012c0104010c010a010c0106023e0104013402040104011c
             0124013c02200124030a020401040130022c011e01340124010a010c0102
             0118014801
       (False,)
       (None, '', False)
    names      ('subprocess', 'os', 'sys', 'pathlib', 'Path', 'os.path', 'abspath', 'api_logic_server_cli.cli_args_project', 'Project', 'logging', 'getLogger', '__name__', 'log', 'str', 'resolve_home', 'get_project_directory_and_api_name', 'get_abs_db_url', 'get_api_logic_server_dir', 'bool', 'does_file_contain', 'replace_string_in_file', 'insert_lines_at', 'find_valid_python_name', 'run_command')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/val/dev/ApiLogicServer/api_logic_server_cli/create_from_model/api_logic_server_utils.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff020318010c010c010c0108022004100d06250c480c0a140c14081a
+      0x00ff020318010c010c010c0108022004100d06250c4b0c0a140c14081a
       140c16
```

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__pycache__/model_creation_services.cpython-310.pyc` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__pycache__/model_creation_services.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__pycache__/model_creation_services.cpython-311.pyc` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__pycache__/model_creation_services.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__pycache__/multi_db_utils.cpython-310.pyc` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__pycache__/multi_db_utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__pycache__/ui_admin_creator.cpython-310.pyc` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__pycache__/ui_admin_creator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__pycache__/ui_admin_creator.cpython-311.pyc` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__pycache__/ui_admin_creator.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__pycache__/uri_info.cpython-310.pyc` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__pycache__/uri_info.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__pycache__/uri_info.cpython-311.pyc` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__pycache__/uri_info.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/api_expose_api_models_creator.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/api_expose_api_models_creator.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/api_logic_server_utils.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/api_logic_server_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         rtn_api_name, \
         rtn_merge_into_prototype
 
 def get_abs_db_url(msg, project: Project):
     """
     non-relative db location - we work with this
 
-    handle db_url abbreviations (nw, nw-, todo etc)
+    handle db_url abbreviations (nw, nw-, todo, allocation, etc)
 
     but NB: we copy sqlite db to <project>/database - see create_project_with_nw_samples (below)
 
     also: compute physical nw db name (usually nw-gold) to be used for copy
 
     returns abs_db_url, nw_db_status - the real url (e.g., for nw), and whether it's really nw, and model_file_name
     """
@@ -89,14 +89,15 @@
     the file: syntax fails, though "current versions" should work:
     https://docs.sqlalchemy.org/en/14/dialects/sqlite.html#uri-connections
     """
 
     if project.db_url in [project.default_db, "", "nw", "sqlite:///nw.sqlite"]:     # nw-gold:      default sample
         rtn_abs_db_url = f'sqlite:///{str(project.api_logic_server_dir_path.joinpath("database/nw-gold.sqlite"))}'
         rtn_nw_db_status = "nw"  # api_logic_server_dir_path
+        # see also create_project_with_nw_samples for overlaying other project files
         log.debug(f'{msg} from: {rtn_abs_db_url}')  # /Users/val/dev/ApiLogicServer/api_logic_server_cli/database/nw-gold.sqlite
     elif project.db_url == "nw-":                                           # nw:           just in case
         rtn_abs_db_url = f'sqlite:///{str(project.api_logic_server_dir_path.joinpath("database/nw-gold.sqlite"))}'
         rtn_nw_db_status = "nw-"
     elif project.db_url == "nw--":                                           # nw:           unused - avoid
         rtn_abs_db_url = f'sqlite:///{str(project.api_logic_server_dir_path.joinpath("database/nw.sqlite"))}'
         rtn_nw_db_status = "nw-"
@@ -112,14 +113,16 @@
         rtn_abs_db_url = f'sqlite:///{str(project.api_logic_server_dir_path.joinpath("database/todos.sqlite"))}'
     elif  project.db_url == "new":
         rtn_abs_db_url = f'sqlite:///{str(project.api_logic_server_dir_path.joinpath("database/new.sqlite"))}'
     elif  project.db_url == "table_filters_tests":
         rtn_abs_db_url = f'sqlite:///{str(project.api_logic_server_dir_path.joinpath("database/table_filters_tests.sqlite"))}'
     elif project.db_url == "classicmodels":
         rtn_abs_db_url = f'sqlite:///{str(project.api_logic_server_dir_path.joinpath("database/classicmodels.sqlite"))}'
+    elif project.db_url == "allocation":
+        rtn_abs_db_url = f'sqlite:///{str(project.api_logic_server_dir_path.joinpath("database/allocation.sqlite"))}'
     elif project.db_url.startswith('sqlite:///'):
         url = project.db_url[10: len(project.db_url)]
         rtn_abs_db_url = abspath(url)
         rtn_abs_db_url = 'sqlite:///' + rtn_abs_db_url
     elif project.db_url.startswith('sqlsvr-sample'):  # work-around - VSCode run config arg parsing
         rtn_abs_db_url = 'mssql+pyodbc://sa:Posey3861@localhost:1433/SampleDB?driver=ODBC+Driver+18+for+SQL+Server&trusted_connection=no&Encrypt=no'
     elif project.db_url.startswith('sqlsvr-nwlogic'):  # work-around - VSCode run config arg parsing
```

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/model_creation_services.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/model_creation_services.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/multi_db_utilsZZ.txt` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/multi_db_utilsZZ.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/.DS_Store` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/asset-manifest.json` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/data/customer.json` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/data/customer.json`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/favicon.ico` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/favicon.ico`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/index.html` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/index.html`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/logo192.png` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/logo192.png`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/logo512.png` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/logo512.png`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/695.2b02568d.chunk.css` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/695.2b02568d.chunk.css`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/695.2b02568d.chunk.css.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/695.2b02568d.chunk.css.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/main.a0c288b7.css.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/main.a0c288b7.css.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1022.0747a719.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1022.0747a719.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1022.0747a719.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1022.0747a719.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1062.9e2b1e6c.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1062.9e2b1e6c.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1062.9e2b1e6c.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1062.9e2b1e6c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1069.16bec71d.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1069.16bec71d.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1069.16bec71d.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1069.16bec71d.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1074.2c3d927c.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1074.2c3d927c.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1074.2c3d927c.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1074.2c3d927c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1251.10ac0097.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1251.10ac0097.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1251.10ac0097.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1251.10ac0097.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1258.94dead34.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1258.94dead34.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1258.94dead34.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1258.94dead34.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1295.179239a3.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1295.179239a3.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1295.179239a3.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1295.179239a3.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1324.be7507c8.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1324.be7507c8.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1324.be7507c8.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1324.be7507c8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1431.d02260cd.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1431.d02260cd.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1431.d02260cd.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1431.d02260cd.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1532.41e3c0c8.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1532.41e3c0c8.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1532.41e3c0c8.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1532.41e3c0c8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1619.31b6d6e8.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1619.31b6d6e8.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1619.31b6d6e8.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1619.31b6d6e8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1690.e74e47c3.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1690.e74e47c3.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1690.e74e47c3.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1690.e74e47c3.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1989.ee922c62.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1989.ee922c62.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1989.ee922c62.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1989.ee922c62.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2154.5c399961.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2154.5c399961.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2154.5c399961.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2154.5c399961.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2402.e66e47e8.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2402.e66e47e8.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2402.e66e47e8.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2402.e66e47e8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2478.4e6b45fa.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2478.4e6b45fa.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2478.4e6b45fa.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2478.4e6b45fa.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2526.c4309069.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2526.c4309069.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2526.c4309069.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2526.c4309069.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/254.1bc22866.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/254.1bc22866.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/254.1bc22866.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/254.1bc22866.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2611.8815ae2b.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2611.8815ae2b.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2611.8815ae2b.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2611.8815ae2b.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2880.029aa44e.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2880.029aa44e.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2880.029aa44e.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2880.029aa44e.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2900.14a00390.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2900.14a00390.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2900.14a00390.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2900.14a00390.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2909.28b39275.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2909.28b39275.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2909.28b39275.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2909.28b39275.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3003.57cfe277.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3003.57cfe277.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3003.57cfe277.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3003.57cfe277.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/312.3d69e408.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/312.3d69e408.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/312.3d69e408.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/312.3d69e408.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3126.99b58416.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3126.99b58416.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3126.99b58416.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3126.99b58416.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3323.b47b9b1e.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3323.b47b9b1e.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3323.b47b9b1e.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3323.b47b9b1e.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3668.cd0becc2.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3668.cd0becc2.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3668.cd0becc2.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3668.cd0becc2.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/369.0237ca8c.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/369.0237ca8c.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/369.0237ca8c.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/369.0237ca8c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3698.750e43d6.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3698.750e43d6.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3698.750e43d6.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3698.750e43d6.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3766.d8eddcd9.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3766.d8eddcd9.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3766.d8eddcd9.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3766.d8eddcd9.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3907.7b2efd62.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3907.7b2efd62.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3907.7b2efd62.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3907.7b2efd62.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3955.f5434704.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3955.f5434704.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3955.f5434704.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3955.f5434704.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4040.613bd8c0.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4040.613bd8c0.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4040.613bd8c0.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4040.613bd8c0.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4333.61aa216a.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4333.61aa216a.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4333.61aa216a.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4333.61aa216a.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/464.522c11f6.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/464.522c11f6.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/464.522c11f6.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/464.522c11f6.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4877.7cebca37.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4877.7cebca37.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4877.7cebca37.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4877.7cebca37.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4900.19572072.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4900.19572072.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4900.19572072.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4900.19572072.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4969.ccedbf9b.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4969.ccedbf9b.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4969.ccedbf9b.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4969.ccedbf9b.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5133.71af5a54.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5133.71af5a54.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5133.71af5a54.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5133.71af5a54.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/52.22a03ee6.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/52.22a03ee6.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/52.22a03ee6.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/52.22a03ee6.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5328.77d62d48.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5328.77d62d48.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5328.77d62d48.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5328.77d62d48.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5342.e36bdc43.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5342.e36bdc43.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5342.e36bdc43.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5342.e36bdc43.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5419.3d10c516.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5419.3d10c516.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5419.3d10c516.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5419.3d10c516.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5507.c29076d8.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5507.c29076d8.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5507.c29076d8.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5507.c29076d8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5540.d957a974.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5540.d957a974.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5540.d957a974.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5540.d957a974.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5558.d0dc5575.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5558.d0dc5575.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5558.d0dc5575.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5558.d0dc5575.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5571.ad570057.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5571.ad570057.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5571.ad570057.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5571.ad570057.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5672.f0c2440f.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5672.f0c2440f.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5672.f0c2440f.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5672.f0c2440f.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/608.84469af3.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/608.84469af3.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/608.84469af3.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/608.84469af3.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6289.a7c21fba.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6289.a7c21fba.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6289.a7c21fba.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6289.a7c21fba.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6304.ce792f5f.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6304.ce792f5f.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6304.ce792f5f.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6304.ce792f5f.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6384.8f33f789.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6384.8f33f789.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6384.8f33f789.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6384.8f33f789.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6403.77f38472.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6403.77f38472.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6403.77f38472.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6403.77f38472.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/651.bf520a75.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/651.bf520a75.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/651.bf520a75.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/651.bf520a75.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6717.805e1882.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6717.805e1882.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6717.805e1882.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6717.805e1882.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js.LICENSE.txt` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6965.381dbe04.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6965.381dbe04.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6965.381dbe04.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6965.381dbe04.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7117.b2e9eb70.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7117.b2e9eb70.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7117.b2e9eb70.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7117.b2e9eb70.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7294.6813eb1f.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7294.6813eb1f.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7294.6813eb1f.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7294.6813eb1f.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7299.20100701.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7299.20100701.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7299.20100701.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7299.20100701.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7436.4e91a3a5.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7436.4e91a3a5.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7436.4e91a3a5.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7436.4e91a3a5.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7497.f56048e1.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7497.f56048e1.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7497.f56048e1.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7497.f56048e1.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7499.b216e9da.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7499.b216e9da.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7499.b216e9da.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7499.b216e9da.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7615.f5af9bae.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7615.f5af9bae.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7615.f5af9bae.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7615.f5af9bae.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7713.6d02efa2.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7713.6d02efa2.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7713.6d02efa2.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7713.6d02efa2.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/787.d5293104.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/787.d5293104.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/787.d5293104.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/787.d5293104.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7894.f8f70466.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7894.f8f70466.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7894.f8f70466.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7894.f8f70466.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7952.29e2c950.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7952.29e2c950.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7952.29e2c950.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7952.29e2c950.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8184.741e3d56.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8184.741e3d56.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8184.741e3d56.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8184.741e3d56.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8272.99aef5a5.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8272.99aef5a5.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8272.99aef5a5.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8272.99aef5a5.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8347.649393e6.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8347.649393e6.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8347.649393e6.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8347.649393e6.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/839.87662037.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/839.87662037.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/839.87662037.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/839.87662037.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8501.ea0cd3a2.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8501.ea0cd3a2.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8501.ea0cd3a2.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8501.ea0cd3a2.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8861.01a110f5.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8861.01a110f5.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8861.01a110f5.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8861.01a110f5.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/907.7b650179.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/907.7b650179.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/907.7b650179.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/907.7b650179.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9186.73a41896.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9186.73a41896.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9186.73a41896.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9186.73a41896.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9200.d0bc8746.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9200.d0bc8746.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9200.d0bc8746.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9200.d0bc8746.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9214.5198dfc3.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9214.5198dfc3.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9214.5198dfc3.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9214.5198dfc3.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9335.43329da2.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9335.43329da2.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9335.43329da2.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9335.43329da2.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9357.e2f466b8.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9357.e2f466b8.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9357.e2f466b8.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9357.e2f466b8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9361.e7bbdd03.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9361.e7bbdd03.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9361.e7bbdd03.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9361.e7bbdd03.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9381.9495a14c.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9381.9495a14c.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9381.9495a14c.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9381.9495a14c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9432.e84dc193.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9432.e84dc193.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9432.e84dc193.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9432.e84dc193.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9687.e1a38d25.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9687.e1a38d25.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9687.e1a38d25.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9687.e1a38d25.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9845.3bb55d3c.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9845.3bb55d3c.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9845.3bb55d3c.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9845.3bb55d3c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9902.bfcd7f60.chunk.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9902.bfcd7f60.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9902.bfcd7f60.chunk.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9902.bfcd7f60.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js.LICENSE.txt` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js.map` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/media/codicon.b797181c93b3755f4fa1.ttf` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/media/codicon.b797181c93b3755f4fa1.ttf`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/basic_web_app/app/__init__.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/basic_web_app/app/__init__.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/pt/LC_MESSAGES/messages.po` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/basic_web_app/app/views.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/basic_web_app/app/views.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/basic_web_app/babel/messages.pot` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/basic_web_app/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/basic_web_app/config.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/basic_web_app/config.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/create_admin.sh` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/create_admin.sh`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/fab_config.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/fab_config.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/home.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/home.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/react_admin_component.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/react_admin_component.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/ui_admin_creator.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/ui_admin_creator.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/uri_info.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/uri_info.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/database/.DS_Store` & `ApiLogicServer-8.3.6/api_logic_server_cli/database/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/database/Chinook_Sqlite.sqlite` & `ApiLogicServer-8.3.6/api_logic_server_cli/database/Chinook_Sqlite.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/database/authentication.sqlite` & `ApiLogicServer-8.3.6/api_logic_server_cli/database/authentication.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/database/classicmodels.sqlite` & `ApiLogicServer-8.3.6/api_logic_server_cli/database/classicmodels.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/database/new.sqlite` & `ApiLogicServer-8.3.6/api_logic_server_cli/database/new.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/database/nw-gold-plus.sqlite` & `ApiLogicServer-8.3.6/api_logic_server_cli/database/nw-gold-plus.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/database/nw-gold.sqlite` & `ApiLogicServer-8.3.6/api_logic_server_cli/database/nw-gold.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/database/nw.sqlite` & `ApiLogicServer-8.3.6/api_logic_server_cli/database/nw.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/database/table_filters_tests.sqlite` & `ApiLogicServer-8.3.6/api_logic_server_cli/database/table_filters_tests.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/database/todos.sqlite` & `ApiLogicServer-8.3.6/api_logic_server_cli/database/todos.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/.DS_Store` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/API-Customize.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/API-Customize.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/API.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/API.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Admin-Customization.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Admin-Customization.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Admin-Tour.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Admin-Tour.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Architecture.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Architecture.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Behave-Logic-Report.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Behave-Logic-Report.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Behave.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Behave.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Create-ApiLogicProject.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Create-ApiLogicProject.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Data-Model-Classes.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Data-Model-Classes.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Data-Model-Customization.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Data-Model-Customization.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Data-Model-Examples.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Data-Model-Examples.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Data-Model-Keys.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Data-Model-Keys.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Data-Model-Multi.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Data-Model-Multi.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Database-Connectivity.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Database-Connectivity.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Execute.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Execute.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/FAQ-Frameworks.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/FAQ-Frameworks.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/FAQ-Low-Code.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/FAQ-Low-Code.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/FAQ-RETE.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/FAQ-RETE.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/IDE-Customize.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/IDE-Customize.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/IDE-Execute.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/IDE-Execute.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Install-Eval-x.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Install-Eval-x.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Install-Eval.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Install-Eval.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Install-Express-x.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Install-Express-x.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Install-Express.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Install-Express.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Install-psycopg2.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Install-psycopg2.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Install-pyodbc.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Install-pyodbc.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Install.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Install.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Internals-CLI.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Internals-CLI.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Internals.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Internals.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Logic-Operation.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Logic-Operation.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Logic-Tutorial.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Logic-Tutorial.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Logic-Why.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Logic-Why.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Logic.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Logic.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Manage-GitHub.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Manage-GitHub.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Project-Builders.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Project-Builders.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Project-DevOps.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Project-DevOps.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Project-Env.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Project-Env.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Project-Execution.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Project-Execution.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Project-Rebuild.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Project-Rebuild.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Project-Structure.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Project-Structure.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Sample-Database.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Sample-Database.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Security-Activation.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Security-Activation.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Security-Authentication-Provider.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Security-Authentication-Provider.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Security-Authentication.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Security-Authentication.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Security-Authorization.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Security-Authorization.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Security-Overview.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Security-Overview.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Tech-CodeSpaces.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Tech-CodeSpaces.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Tech-Conference-PyCon23-Talk.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Tech-Conference-PyCon23-Talk.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Tech-Conference-PyCon23-Tutorial.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Tech-Conference-PyCon23-Tutorial.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Tech-Conference.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Tech-Conference.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Tech-Docker.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Tech-Docker.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Tech-Install-Python.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Tech-Install-Python.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Tech-Proven.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Tech-Proven.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Tech-Python-311.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Tech-Python-311.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Tech-Python.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Tech-Python.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Tech-m1.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Tech-m1.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Tech-mkdocs-material.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Tech-mkdocs-material.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Troubleshooting.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Troubleshooting.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Tutorial.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Tutorial.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Working-With-Docker.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Working-With-Docker.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Working-with-Flask-AppBuilder.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Working-with-Flask-AppBuilder.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/assets/.DS_Store` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/assets/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/assets/images/bulb-icon.svg` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/assets/images/bulb-icon.svg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/assets/images/lightbulb.svg` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/assets/images/lightbulb.svg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/index.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/index.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/docs/stylesheets/extra.css` & `ApiLogicServer-8.3.6/api_logic_server_cli/docs/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/extended_builder.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/extended_builder.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/fragments/Todo_modelsZZ.py.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/fragments/Todo_modelsZZ.py.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/fragments/configZZ.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/fragments/configZZ.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/fragments/modelsZZ.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/fragments/modelsZZ.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/fragments/nw_virtual_attrs.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/fragments/nw_virtual_attrs.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/fragments/ui_basic_web_app_runZZ.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/fragments/ui_basic_web_app_runZZ.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/logging.yml` & `ApiLogicServer-8.3.6/api_logic_server_cli/logging.yml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.DS_Store` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.devcontainer/devcontainer.json` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.idea/.DS_Store` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.idea/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.idea/runConfigurations/.DS_Store` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.idea/runConfigurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.idea/runConfigurations/ApiLogicServer.xml` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.idea/runConfigurations/ApiLogicServer.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.idea/runConfigurations/Report_Behave_Logic.xml` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.idea/runConfigurations/Report_Behave_Logic.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.idea/runConfigurations/Run_Behave.xml` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.idea/runConfigurations/Run_Behave.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.idea/runConfigurations/Windows_Run_Behave.xml` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.idea/runConfigurations/Windows_Run_Behave.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.idea/runConfigurations/run___No_Security.xml` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.idea/runConfigurations/run___No_Security.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.idea/runConfigurations/run_docker.xml` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.idea/runConfigurations/run_docker.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.vscode/launch.json` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/api/customize_api.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/api/customize_api.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/api/json_encoder.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/api/json_encoder.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/api/readme_customize_api.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/api/readme_customize_api.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/api_logic_server_run.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/api_logic_server_run.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/config.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/config.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/database/alembic/env.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/database/alembic/env.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/database/alembic/readme.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/database/alembic/readme.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/database/alembic.ini` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/database/alembic.ini`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/database/bind_databases.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/database/bind_databases.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/devops/docker/authdb_mysql.Dockerfile` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/devops/docker/authdb_mysql.Dockerfile`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/devops/docker/authdb_mysql.sql` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/devops/docker/authdb_mysql.sql`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/devops/docker/build_image.sh` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/devops/docker/build_image.sh`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/devops/git_push_new_project.sh` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/devops/git_push_new_project.sh`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/logging.yml` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/logging.yml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/logic/declare_logic.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/logic/declare_logic.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/logic/readme_declare_logic.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/logic/readme_declare_logic.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/mypy.ini` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/mypy.ini`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/python_anywhere_wsgi.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/python_anywhere_wsgi.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/readme.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/readme.md`

 * *Files 3% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 * Since they are separate files, the project can be
 [rebuilt](https://apilogicserver.github.io/Docs/Project-Rebuild/) (e.g., synchronized with a revised schema), preserving your customizations.
 
 Please see the `nw` sample for examples of typical customizations.  You can open it in GitHub (use Shift + "." to view in project mode) - [click here](https://github.com/ApiLogicServer/demo).
 
 | Directory | Usage                         | Key Customization File             | Typical Customization                                                                 |
 |:-------------- |:------------------------------|:-----------------------------------|:--------------------------------------------------------------------------------------|
-| ```api``` | JSON:API                      | ```api/customize_api.py```         | Add new end points / services                                                         |
+| ```api``` | **JSON:API**<br>*Ready to Run*                    | ```api/customize_api.py```         | Add new end points / services                                                         |
+| ```ui``` | **Multi-Page Admin App**<br>*Ready to Run*  | ```ui/admin/admin.yaml```          | Control field display - order, captions etc.                                          |
 | ```database``` | SQLAlchemy Data Model Classes | ```database/customize_models.py``` | Add derived attributes, and relationships missing in the schema                       |
-| ```logic``` | Transactional Logic           | ```logic/declare_logic.py```       | Declare multi-table derivations, constraints, and events such as send mail / messages |
-| ```ui``` | Admin App                     | ```ui/admin/admin.yaml```          | Control field display - order, captions etc.                                          |
+| ```logic``` | **Transactional Logic**<br>spreadsheet-like rules   | ```logic/declare_logic.py```       | Declare multi-table derivations, constraints, and Python events such as send mail / messages |
 | ```security``` | Authentication, Authorization   | ```security/declare_security.py```          | Control login, role-based row access         |
 | ```tests``` | Behave Test Suite              | ```tests/api_logic_server_behave/features```          | Declare and implement [Behave Tests](https://apilogicserver.github.io/Docs/Behave/)                                          |
 
 &nbsp;
 
 # Project Information
```

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/run.ps1` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/run.ps1`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/run.sh` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/run.sh`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/.DS_Store` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/.DS_Store` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/abstract_authentication_provider.cpython-310.pyc` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/abstract_authentication_provider.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/authentication_models.cpython-310.pyc` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/authentication_models.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/db_auth.cpython-310.pyc` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/db_auth.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/mem_auth.cpython-310.pyc` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/mem_auth.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/mem_auth_row.cpython-310.pyc` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/mem_auth_row.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/models.cpython-310.pyc` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/models.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/abstract_authentication_provider.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/abstract_authentication_provider.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/memory/__pycache__/auth_provider.cpython-310.pyc` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/memory/__pycache__/auth_provider.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/memory/auth_provider.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/memory/auth_provider.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/memory/auth_provider_no_swagger.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/memory/auth_provider_no_swagger.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/auth_provider.cpython-310.pyc` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/auth_provider.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/authentication_models.cpython-310.pyc` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/authentication_models.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/db_auth.cpython-310.pyc` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/db_auth.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/sql/sqlite/auth_provider.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/sql/sqlite/auth_provider.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/declare_security.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/declare_security.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/notes_temp/pip-freeze-th.txt` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/notes_temp/pip-freeze-th.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/notes_temp/pip-freeze.txt` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/notes_temp/pip-freeze.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/notes_temp/token.txt` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/notes_temp/token.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/system/__pycache__/security_manager.cpython-310.pyc` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/system/__pycache__/security_manager.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/system/authentication.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/system/authentication.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/system/authorization.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/system/authorization.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/system/custom_swagger.json` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/system/custom_swagger.json`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/templates/index.html` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/templates/index.html`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/test/api_logic_server_behave/behave_logic_report.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/test/api_logic_server_behave/behave_logic_report.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/test/api_logic_server_behave/behave_run.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/test/api_logic_server_behave/behave_run.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/steps/test_utils.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/steps/test_utils.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/Behave Logic Report Intro.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/Behave Logic Report Intro.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/Behave Logic Report Sample.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/Behave Logic Report Sample.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/test/basic/server_test.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/test/basic/server_test.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/.DS_Store` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/admin/admin_loader.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/admin/admin_loader.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/admin/home.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/admin/home.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/.DS_Store` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Employee/andrew.jpg` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Employee/andrew.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Employee/anne.jpg` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Employee/anne.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Employee/janet.jpg` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Employee/janet.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Employee/laura.jpg` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Employee/laura.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Employee/margaret.jpg` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Employee/margaret.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Employee/michael.jpg` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Employee/michael.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Employee/nancy.jpg` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Employee/nancy.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Employee/robert.jpg` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Employee/robert.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Employee/steven.jpg` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Employee/steven.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Product/beverages.gif` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Product/beverages.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Product/cereals.gif` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Product/cereals.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Product/condiments.gif` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Product/condiments.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Product/confections.gif` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Product/confections.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Product/diary.gif` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Product/diary.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Product/meat.gif` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Product/meat.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Product/produce.gif` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Product/produce.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Product/seafood.gif` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Product/seafood.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/util.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/util.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/venv_setup/py.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/venv_setup/py.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/venv_setup/readme_venv.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/venv_setup/readme_venv.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/venv_setup/requirements-no-cli.txt` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/venv_setup/requirements-no-cli.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/venv_setup/venv-linux.sh` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/venv_setup/venv-linux.sh`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/venv_setup/venv.ps1` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/venv_setup/venv.ps1`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/venv_setup/venv.sh` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/venv_setup/venv.sh`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/.DS_Store` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/api/customize_api.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/api/customize_api.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/api/multi-table-example/multi-table.json` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/api/multi-table-example/multi-table.json`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/api/multi-table-example/multi-table.txt` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/api/multi-table-example/multi-table.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/database/customize_models.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/database/customize_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     if isinstance(self, models.Employee):
         import decimal
         rtn_value = self.Salary
         rtn_value = decimal.Decimal('1.25') * rtn_value
         self._proper_salary = int(rtn_value)
         return self._proper_salary
     else:
-        print("class")
+        # print("class")
         return None
 
 @add_method(models.Employee)
 @__proper_salary__.setter
 def _proper_salary(self, value):  # type: ignore [no-redef]
     self._proper_salary = value
     print(f'_proper_salary={self._proper_salary}')
```

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/logic/declare_logic.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/logic/declare_logic.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/security/declare_security.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/security/declare_security.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/place_order.feature` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/place_order.feature`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/api.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/api.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/place_order.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/place_order.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/salary_change.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/salary_change.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/behave.log` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/behave.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Alter_Item_Qty_to_exceed_.log` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Alter_Item_Qty_to_exceed_.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Alter_Required_Date_-_adj.log` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Alter_Required_Date_-_adj.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Audit_Salary_Change.log` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Audit_Salary_Change.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Bad_Order_Custom_Service.log` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Bad_Order_Custom_Service.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Good_Order_Custom_Service.log` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Good_Order_Custom_Service.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Raise_Must_be_Meaningful.log` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Raise_Must_be_Meaningful.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Reset_Shipped_-_adjust_lo.log` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Reset_Shipped_-_adjust_lo.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Set_Shipped_-_adjust_logi.log` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Set_Shipped_-_adjust_logi.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Transaction_Processing.log` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Transaction_Processing.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/results/ADJUST_test_-_OrderDetail.log` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/results/ADJUST_test_-_OrderDetail.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/results/AUDIT_test_-_Emp_Sal.log` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/results/AUDIT_test_-_Emp_Sal.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/results/CASCADE_UPDATE_-_ShippedD.log` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/results/CASCADE_UPDATE_-_ShippedD.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/results/CUSTOM_SERVICE_Bad_Order.log` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/results/CUSTOM_SERVICE_Bad_Order.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/results/DELETE_test_-_Cust.log` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/results/DELETE_test_-_Cust.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/results/PATCH_-_low_credit.log` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/results/PATCH_-_low_credit.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/results/POST_test_-_Cust.log` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/results/POST_test_-_Cust.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/results/PRUNE_test_-_ReqdDate.log` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/results/PRUNE_test_-_ReqdDate.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/server_startup_test.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/server_startup_test.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/server_test.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/server_test.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/server_test.sh` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/server_test.sh`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/.DS_Store` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/admin/admin.yaml` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/admin/admin.yaml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/admin/home.js` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/admin/home.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/admin/multi_app_project.yaml` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/admin/multi_app_project.yaml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/.DS_Store` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Category/beverages.gif` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Category/beverages.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Category/cereals.gif` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Category/cereals.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Category/condiments.gif` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Category/condiments.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Category/confections.gif` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Category/confections.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Category/diary.gif` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Category/diary.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Category/meat.gif` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Category/meat.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Category/produce.gif` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Category/produce.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Category/seafood.gif` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Category/seafood.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Employee/buchanan.jpg` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Employee/buchanan.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Employee/callahan.jpg` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Employee/callahan.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Employee/davolio.jpg` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Employee/davolio.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Employee/dodsworth.jpg` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Employee/dodsworth.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Employee/fuller.jpg` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Employee/fuller.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Employee/king.jpg` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Employee/king.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Employee/leverling.jpg` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Employee/leverling.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Employee/peacock.jpg` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Employee/peacock.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Employee/suyama.jpg` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Employee/suyama.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw_no_cust/readme.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw_no_cust/readme.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.DS_Store` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.devcontainer/devcontainer.json` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.idea/.DS_Store` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.idea/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.idea/runConfigurations/.DS_Store` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.idea/runConfigurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.idea/runConfigurations/1__Basic_App.xml` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.idea/runConfigurations/1__Basic_App.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.idea/runConfigurations/2__ApiLogicProject.xml` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.idea/runConfigurations/2__ApiLogicProject.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.idea/runConfigurations/3__ApiLogicProject_Logic.xml` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.idea/runConfigurations/3__ApiLogicProject_Logic.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Execute_chinook.xml` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Execute_chinook.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Execute_classicmodels.xml` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Execute_classicmodels.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Execute_todo.xml` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Execute_todo.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Run_Behave.xml` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Run_Behave.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Run_Behave_Logic_Report.xml` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Run_Behave_Logic_Report.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.vscode/launch.json` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/.DS_Store` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/config.cpython-310.pyc` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/config.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/flask.cpython-310.pyc` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/flask.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/flask_basic.cpython-310.pyc` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/flask_basic.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/raw_flask.cpython-310.pyc` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/raw_flask.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/util.cpython-310.pyc` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/util.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/api/end_points.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/api/end_points.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/config.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/config.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/__pycache__/models.cpython-310.pyc` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/__pycache__/models.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/db.sqlite` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/db.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/logging.yml` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/logging.yml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/models.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/models.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/flask_basic.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/flask_basic.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/logging.yml` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/logging.yml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/readme.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/readme.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/util.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/util.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/readme.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/readme.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/sample_db.sqlite` & `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/sample_db.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/.DS_Store` & `ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/expose_existing_callable.cpython-310.pyc` & `ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/expose_existing_callable.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/sqlacodegen_wrapper.cpython-310.pyc` & `ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/sqlacodegen_wrapper.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/sqlacodegen_wrapper.cpython-311.pyc` & `ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/sqlacodegen_wrapper.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/uri_info.cpython-310.pyc` & `ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/uri_info.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/console_log.txt` & `ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/console_log.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/.travis.yml` & `ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/.travis.yml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/CHANGES.rst` & `ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/README.rst` & `ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/README.rst`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/setup.cfg` & `ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/setup.cfg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/codegen.cpython-310.pyc` & `ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/codegen.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/codegen.cpython-311.pyc` & `ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/codegen.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/codegen.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/codegen.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/main.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/main.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/tests/test_codegen.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/tests/test_codegen.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen_wrapper.py` & `ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen_wrapper.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/templates/admin.yaml` & `ApiLogicServer-8.3.6/api_logic_server_cli/templates/admin.yaml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/templates/app_fiddle.md` & `ApiLogicServer-8.3.6/api_logic_server_cli/templates/app_fiddle.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/templates/app_fiddle.txt` & `ApiLogicServer-8.3.6/api_logic_server_cli/templates/app_fiddle.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/templates/index.html` & `ApiLogicServer-8.3.6/api_logic_server_cli/templates/index.html`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/api_logic_server_cli/templates/login_endpoint.txt` & `ApiLogicServer-8.3.6/api_logic_server_cli/templates/login_endpoint.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.3/setup.py` & `ApiLogicServer-8.3.6/setup.py`

 * *Files identical despite different names*

