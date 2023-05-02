# Comparing `tmp/clickhouse-sqlalchemy-0.2.3.tar.gz` & `tmp/clickhouse-sqlalchemy-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clickhouse-sqlalchemy-0.2.3.tar", last modified: Thu Nov 24 20:41:30 2022, max compression
+gzip compressed data, was "clickhouse-sqlalchemy-0.2.4.tar", last modified: Tue May  2 17:42:00 2023, max compression
```

## Comparing `clickhouse-sqlalchemy-0.2.3.tar` & `clickhouse-sqlalchemy-0.2.4.tar`

### file list

```diff
@@ -1,69 +1,73 @@
-drwxrwxr-x   0 klebedev  (1000) klebedev  (1000)        0 2022-11-24 20:41:30.257965 clickhouse-sqlalchemy-0.2.3/
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1143 2017-06-15 17:55:32.000000 clickhouse-sqlalchemy-0.2.3/LICENSE
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     4952 2022-11-24 20:41:30.257965 clickhouse-sqlalchemy-0.2.3/PKG-INFO
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     2664 2022-06-09 14:31:39.000000 clickhouse-sqlalchemy-0.2.3/README.rst
-drwxrwxr-x   0 klebedev  (1000) klebedev  (1000)        0 2022-11-24 20:41:30.233965 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      315 2022-11-24 20:41:08.000000 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/__init__.py
-drwxrwxr-x   0 klebedev  (1000) klebedev  (1000)        0 2022-11-24 20:41:30.237966 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/alembic/
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)        0 2022-02-13 17:42:00.000000 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/alembic/__init__.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     6128 2022-03-15 14:52:55.000000 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/alembic/comparators.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     2529 2022-07-05 17:20:31.000000 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/alembic/dialect.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     5153 2022-02-13 17:42:00.000000 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/alembic/operations.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     3184 2022-02-13 17:42:00.000000 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/alembic/renderers.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     2113 2022-02-13 17:42:00.000000 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/alembic/toimpl.py
-drwxrwxr-x   0 klebedev  (1000) klebedev  (1000)        0 2022-11-24 20:41:30.237966 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/drivers/
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)       93 2018-06-20 17:33:49.000000 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/drivers/__init__.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)    14425 2022-11-17 15:03:12.000000 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/drivers/base.py
-drwxrwxr-x   0 klebedev  (1000) klebedev  (1000)        0 2022-11-24 20:41:30.241966 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/drivers/compilers/
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)        0 2022-06-09 14:31:39.000000 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/drivers/compilers/__init__.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     9087 2022-11-06 16:45:48.000000 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/drivers/compilers/ddlcompiler.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)    14948 2022-11-06 12:48:46.000000 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/drivers/compilers/sqlcompiler.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     3825 2022-11-17 15:03:12.000000 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/drivers/compilers/typecompiler.py
-drwxrwxr-x   0 klebedev  (1000) klebedev  (1000)        0 2022-11-24 20:41:30.245966 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/drivers/http/
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)        0 2018-06-20 17:33:49.000000 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/drivers/http/__init__.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1556 2022-07-05 17:20:24.000000 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/drivers/http/base.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     5958 2022-07-05 17:20:24.000000 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/drivers/http/connector.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     2300 2022-06-09 14:31:39.000000 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/drivers/http/escaper.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)       49 2018-06-20 17:33:49.000000 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/drivers/http/exceptions.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     5130 2022-07-05 17:20:24.000000 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/drivers/http/transport.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      318 2022-07-05 17:20:24.000000 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/drivers/http/utils.py
-drwxrwxr-x   0 klebedev  (1000) klebedev  (1000)        0 2022-11-24 20:41:30.249966 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/drivers/native/
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)        0 2018-06-20 17:33:49.000000 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/drivers/native/__init__.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1846 2022-07-25 19:53:46.000000 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/drivers/native/base.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     6924 2022-08-24 07:07:27.000000 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/drivers/native/connector.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1820 2022-06-10 17:10:58.000000 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/drivers/reflection.py
-drwxrwxr-x   0 klebedev  (1000) klebedev  (1000)        0 2022-11-24 20:41:30.253965 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/engines/
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1010 2021-12-08 19:51:43.000000 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/engines/__init__.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1845 2022-06-13 10:21:51.000000 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/engines/base.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     7364 2022-06-10 16:46:21.000000 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/engines/mergetree.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     3935 2021-12-08 19:51:43.000000 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/engines/misc.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     5956 2022-05-07 21:40:43.000000 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/engines/replicated.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1210 2021-10-16 12:46:53.000000 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/engines/util.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      225 2022-06-09 14:31:39.000000 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/exceptions.py
-drwxrwxr-x   0 klebedev  (1000) klebedev  (1000)        0 2022-11-24 20:41:30.253965 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/ext/
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)        0 2018-06-20 17:33:49.000000 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/ext/__init__.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1606 2022-06-09 14:31:39.000000 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/ext/clauses.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1514 2022-06-09 14:31:39.000000 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/ext/declarative.py
-drwxrwxr-x   0 klebedev  (1000) klebedev  (1000)        0 2022-11-24 20:41:30.253965 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/orm/
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)       66 2018-06-20 17:33:49.000000 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/orm/__init__.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     3505 2022-11-06 12:48:46.000000 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/orm/query.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      171 2018-06-20 17:33:49.000000 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/orm/session.py
-drwxrwxr-x   0 klebedev  (1000) klebedev  (1000)        0 2022-11-24 20:41:30.257965 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/sql/
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      146 2022-02-13 17:42:00.000000 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/sql/__init__.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     2321 2022-06-13 10:21:51.000000 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/sql/ddl.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     4061 2022-10-22 20:03:56.000000 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/sql/schema.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1851 2022-11-06 12:48:46.000000 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/sql/selectable.py
-drwxrwxr-x   0 klebedev  (1000) klebedev  (1000)        0 2022-11-24 20:41:30.257965 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/types/
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1393 2022-11-17 15:03:12.000000 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/types/__init__.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     3653 2022-11-17 15:18:23.000000 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/types/common.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     5003 2022-06-13 10:21:51.000000 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/types/ip.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     2029 2022-07-05 18:50:08.000000 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/types/nested.py
-drwxrwxr-x   0 klebedev  (1000) klebedev  (1000)        0 2022-11-24 20:41:30.233965 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy.egg-info/
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     4952 2022-11-24 20:41:29.000000 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy.egg-info/PKG-INFO
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     2211 2022-11-24 20:41:29.000000 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy.egg-info/SOURCES.txt
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)        1 2022-11-24 20:41:29.000000 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy.egg-info/dependency_links.txt
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      267 2022-11-24 20:41:29.000000 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy.egg-info/entry_points.txt
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)       55 2022-11-24 20:41:29.000000 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy.egg-info/requires.txt
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)       22 2022-11-24 20:41:29.000000 clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy.egg-info/top_level.txt
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      189 2022-11-24 20:41:30.261965 clickhouse-sqlalchemy-0.2.3/setup.cfg
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     2911 2022-06-13 15:27:07.000000 clickhouse-sqlalchemy-0.2.3/setup.py
+drwxrwxr-x   0 klebedev  (1000) klebedev  (1000)        0 2023-05-02 17:42:00.748756 clickhouse-sqlalchemy-0.2.4/
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1143 2017-06-15 17:55:32.000000 clickhouse-sqlalchemy-0.2.4/LICENSE
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     5034 2023-05-02 17:42:00.748756 clickhouse-sqlalchemy-0.2.4/PKG-INFO
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     2738 2023-05-02 17:16:59.000000 clickhouse-sqlalchemy-0.2.4/README.rst
+drwxrwxr-x   0 klebedev  (1000) klebedev  (1000)        0 2023-05-02 17:42:00.732756 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      315 2023-05-02 17:41:23.000000 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/__init__.py
+drwxrwxr-x   0 klebedev  (1000) klebedev  (1000)        0 2023-05-02 17:42:00.736756 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/alembic/
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)        0 2023-05-02 17:16:59.000000 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/alembic/__init__.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     6555 2023-05-02 17:18:55.000000 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/alembic/comparators.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     2764 2023-05-02 17:18:55.000000 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/alembic/dialect.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     5153 2023-05-02 17:16:59.000000 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/alembic/operations.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     3184 2023-05-02 17:16:59.000000 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/alembic/renderers.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     2113 2023-05-02 17:16:59.000000 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/alembic/toimpl.py
+drwxrwxr-x   0 klebedev  (1000) klebedev  (1000)        0 2023-05-02 17:42:00.740756 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/drivers/
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)       93 2018-06-20 17:33:49.000000 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/drivers/__init__.py
+drwxrwxr-x   0 klebedev  (1000) klebedev  (1000)        0 2023-05-02 17:42:00.740756 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/drivers/asynch/
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)        0 2023-05-02 17:16:59.000000 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/drivers/asynch/__init__.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1220 2023-05-02 17:16:59.000000 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/drivers/asynch/base.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     5253 2023-05-02 17:16:59.000000 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/drivers/asynch/connector.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)    14425 2023-05-02 17:16:59.000000 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/drivers/base.py
+drwxrwxr-x   0 klebedev  (1000) klebedev  (1000)        0 2023-05-02 17:42:00.740756 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/drivers/compilers/
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)        0 2023-05-02 17:16:59.000000 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/drivers/compilers/__init__.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     9087 2023-05-02 17:16:59.000000 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/drivers/compilers/ddlcompiler.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)    16035 2023-05-02 17:18:55.000000 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/drivers/compilers/sqlcompiler.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     3921 2023-05-02 17:16:59.000000 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/drivers/compilers/typecompiler.py
+drwxrwxr-x   0 klebedev  (1000) klebedev  (1000)        0 2023-05-02 17:42:00.740756 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/drivers/http/
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)        0 2018-06-20 17:33:49.000000 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/drivers/http/__init__.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1556 2023-05-02 17:16:59.000000 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/drivers/http/base.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     5958 2022-07-05 17:20:24.000000 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/drivers/http/connector.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     2300 2023-05-02 17:16:59.000000 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/drivers/http/escaper.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)       49 2018-06-20 17:33:49.000000 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/drivers/http/exceptions.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     5130 2023-05-02 17:16:59.000000 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/drivers/http/transport.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      318 2022-07-05 17:20:24.000000 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/drivers/http/utils.py
+drwxrwxr-x   0 klebedev  (1000) klebedev  (1000)        0 2023-05-02 17:42:00.744756 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/drivers/native/
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)        0 2018-06-20 17:33:49.000000 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/drivers/native/__init__.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     2042 2023-05-02 17:16:59.000000 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/drivers/native/base.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     6924 2022-08-24 07:07:27.000000 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/drivers/native/connector.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1820 2023-05-02 17:16:59.000000 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/drivers/reflection.py
+drwxrwxr-x   0 klebedev  (1000) klebedev  (1000)        0 2023-05-02 17:42:00.744756 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/engines/
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1010 2021-12-08 19:51:43.000000 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/engines/__init__.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1845 2023-05-02 17:16:59.000000 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/engines/base.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     7364 2023-05-02 17:16:59.000000 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/engines/mergetree.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     3935 2021-12-08 19:51:43.000000 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/engines/misc.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     5956 2023-05-02 17:16:59.000000 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/engines/replicated.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1210 2021-10-16 12:46:53.000000 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/engines/util.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      225 2023-05-02 17:16:59.000000 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/exceptions.py
+drwxrwxr-x   0 klebedev  (1000) klebedev  (1000)        0 2023-05-02 17:42:00.744756 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/ext/
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)        0 2018-06-20 17:33:49.000000 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/ext/__init__.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1606 2023-05-02 17:16:59.000000 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/ext/clauses.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1514 2023-05-02 17:16:59.000000 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/ext/declarative.py
+drwxrwxr-x   0 klebedev  (1000) klebedev  (1000)        0 2023-05-02 17:42:00.744756 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/orm/
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)       66 2018-06-20 17:33:49.000000 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/orm/__init__.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     3489 2023-05-02 17:16:59.000000 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/orm/query.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      349 2023-05-02 17:16:59.000000 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/orm/session.py
+drwxrwxr-x   0 klebedev  (1000) klebedev  (1000)        0 2023-05-02 17:42:00.748756 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/sql/
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      146 2023-05-02 17:16:59.000000 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/sql/__init__.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     2650 2023-05-02 17:18:55.000000 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/sql/ddl.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     4061 2023-05-02 17:16:59.000000 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/sql/schema.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1851 2023-05-02 17:16:59.000000 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/sql/selectable.py
+drwxrwxr-x   0 klebedev  (1000) klebedev  (1000)        0 2023-05-02 17:42:00.748756 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/types/
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1393 2023-05-02 17:16:59.000000 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/types/__init__.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     3755 2023-05-02 17:16:59.000000 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/types/common.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     5003 2023-05-02 17:16:59.000000 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/types/ip.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     2029 2022-07-05 18:50:08.000000 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/types/nested.py
+drwxrwxr-x   0 klebedev  (1000) klebedev  (1000)        0 2023-05-02 17:42:00.736756 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy.egg-info/
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     5034 2023-05-02 17:42:00.000000 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy.egg-info/PKG-INFO
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     2355 2023-05-02 17:42:00.000000 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy.egg-info/SOURCES.txt
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)        1 2023-05-02 17:42:00.000000 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy.egg-info/dependency_links.txt
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      354 2023-05-02 17:42:00.000000 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy.egg-info/entry_points.txt
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)       88 2023-05-02 17:42:00.000000 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy.egg-info/requires.txt
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)       22 2023-05-02 17:42:00.000000 clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy.egg-info/top_level.txt
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      226 2023-05-02 17:42:00.752756 clickhouse-sqlalchemy-0.2.4/setup.cfg
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     3029 2023-05-02 17:16:59.000000 clickhouse-sqlalchemy-0.2.4/setup.py
```

### Comparing `clickhouse-sqlalchemy-0.2.3/LICENSE` & `clickhouse-sqlalchemy-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `clickhouse-sqlalchemy-0.2.3/PKG-INFO` & `clickhouse-sqlalchemy-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: clickhouse-sqlalchemy
-Version: 0.2.3
+Version: 0.2.4
 Summary: Simple ClickHouse SQLAlchemy Dialect
 Home-page: https://github.com/xzkostyan/clickhouse-sqlalchemy
 Author: Konstantin Lebedev
 Author-email: kostyan.lebedev@gmail.com
 License: MIT
 Project-URL: Documentation, https://clickhouse-sqlalchemy.readthedocs.io
 Project-URL: Changes, https://github.com/xzkostyan/clickhouse-sqlalchemy/blob/master/CHANGELOG.md
@@ -40,15 +40,16 @@
         
         
         Usage
         =====
         
         Supported interfaces:
         
-        - **native** [recommended] (TCP) via `clickhouse-driver <https://github.com/mymarilyn/clickhouse-driver>`_
+        - **native** [recommended] (TCP) via `clickhouse-driver <https://github.com/mymarilyn/clickhouse-driver>`
+        - **async native** (TCP) via `asynch <https://github.com/long2ice/asynch>`
         - **http** via requests
         
         Define table
         
             .. code-block:: python
         
                 from sqlalchemy import create_engine, Column, MetaData
@@ -125,8 +126,8 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Requires-Python: >=3.6, <4
+Requires-Python: >=3.7, <4
```

### Comparing `clickhouse-sqlalchemy-0.2.3/README.rst` & `clickhouse-sqlalchemy-0.2.4/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -30,15 +30,16 @@
 
 
 Usage
 =====
 
 Supported interfaces:
 
-- **native** [recommended] (TCP) via `clickhouse-driver <https://github.com/mymarilyn/clickhouse-driver>`_
+- **native** [recommended] (TCP) via `clickhouse-driver <https://github.com/mymarilyn/clickhouse-driver>`
+- **async native** (TCP) via `asynch <https://github.com/long2ice/asynch>`
 - **http** via requests
 
 Define table
 
     .. code-block:: python
 
         from sqlalchemy import create_engine, Column, MetaData
```

### Comparing `clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/alembic/comparators.py` & `clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/alembic/comparators.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,15 +17,23 @@
     query = create_table_query
     # Naive inner name detection
     brace = query.index('(')
     inner_name = query[query.index(' TO ', 0, brace) + 4:brace - 1].strip(' `')
     return inner_name.split('.')[1] if '.' in inner_name else inner_name
 
 
-@comparators.dispatch_for('schema')
+# Direct call .dispatch_for('schema', 'clickhouse') override an Alembic
+# default ('schema', 'default') comparator. To avoid it (as we have own
+# implementation only for a materialized views ) register default "schema"
+# comparators as "clickhouse" comparators too.
+for default_comparator in comparators._registry[('schema', 'default')]:
+    comparators.dispatch_for('schema', 'clickhouse')(default_comparator)
+
+
+@comparators.dispatch_for('schema', 'clickhouse')
 def compare_mat_view(autogen_context, upgrade_ops, schemas):
     connection = autogen_context.connection
     dialect = autogen_context.dialect
     metadata = autogen_context.metadata
 
     database_engine = dialect._execute(
         connection,
```

### Comparing `clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/alembic/dialect.py` & `clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/alembic/dialect.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,16 +21,24 @@
 
 
 class ClickHouseDialectImpl(impl.DefaultImpl):
     __dialect__ = 'clickhouse'
     transactional_ddl = False
 
     def drop_table(self, table):
+        table.dispatch.before_drop(
+            table, self.connection, checkfirst=False, _ddl_runner=self
+        )
+
         self._exec(DropTable(table))
 
+        table.dispatch.after_drop(
+            table, self.connection, checkfirst=False, _ddl_runner=self
+        )
+
 
 def patch_alembic_version(context, **kwargs):
     migration_context = context._proxy._migration_context
     version = migration_context._version
 
     dt = Column('dt', types.DateTime, server_default=func.now())
     version_num = Column('version_num', types.String, primary_key=True)
```

### Comparing `clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/alembic/operations.py` & `clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/alembic/operations.py`

 * *Files identical despite different names*

### Comparing `clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/alembic/renderers.py` & `clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/alembic/renderers.py`

 * *Files identical despite different names*

### Comparing `clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/alembic/toimpl.py` & `clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/alembic/toimpl.py`

 * *Files identical despite different names*

### Comparing `clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/drivers/base.py` & `clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/drivers/base.py`

 * *Files identical despite different names*

### Comparing `clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/drivers/compilers/ddlcompiler.py` & `clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/drivers/compilers/ddlcompiler.py`

 * *Files identical despite different names*

### Comparing `clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/drivers/compilers/sqlcompiler.py` & `clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/drivers/compilers/sqlcompiler.py`

 * *Files 6% similar despite different names*

```diff
@@ -282,22 +282,22 @@
                         )
                         for f in froms
                     ]
                 )
         else:
             text += self.default_from()
 
-        if getattr(select, '_array_join', None) is not None:
-            text += select._array_join._compiler_dispatch(self, **kwargs)
-
         sample_clause = getattr(select, '_sample_clause', None)
 
         if sample_clause is not None:
             text += self.sample_clause(select, **kwargs)
 
+        if getattr(select, '_array_join', None) is not None:
+            text += select._array_join._compiler_dispatch(self, **kwargs)
+
         final_clause = getattr(select, '_final_clause', None)
 
         if final_clause is not None:
             text += self.final_clause()
 
         if select._where_criteria:
             t = self._generate_delimited_and_list(
@@ -462,7 +462,38 @@
                     ) for x in value) +
                 ']'
             )
         else:
             return super(ClickHouseSQLCompiler, self).render_literal_value(
                 value, type_
             )
+
+    def _get_regexp_args(self, binary, kw):
+        string = self.process(binary.left, **kw)
+        pattern = self.process(binary.right, **kw)
+        return string, pattern
+
+    def visit_regexp_match_op_binary(self, binary, operator, **kw):
+        string, pattern = self._get_regexp_args(binary, kw)
+        return "MATCH(%s, %s)" % (string, pattern)
+
+    def visit_not_regexp_match_op_binary(self, binary, operator, **kw):
+        return "NOT %s" % self.visit_regexp_match_op_binary(
+            binary,
+            operator,
+            **kw
+        )
+
+    def visit_ilike_case_insensitive_operand(self, element, **kw):
+        return element.element._compiler_dispatch(self, **kw)
+
+    def visit_ilike_op_binary(self, binary, operator, **kw):
+        return "%s ILIKE %s" % (
+            self.process(binary.left, **kw),
+            self.process(binary.right, **kw)
+        )
+
+    def visit_not_ilike_op_binary(self, binary, operator, **kw):
+        return "%s NOT ILIKE %s" % (
+            self.process(binary.left, **kw),
+            self.process(binary.right, **kw)
+        )
```

### Comparing `clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/drivers/compilers/typecompiler.py` & `clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/drivers/compilers/typecompiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,19 +57,22 @@
     def visit_uint256(self, type_, **kw):
         return 'UInt256'
 
     def visit_date(self, type_, **kw):
         return 'Date'
 
     def visit_datetime(self, type_, **kw):
-        return 'DateTime'
+        if type_.timezone:
+            return "DateTime('%s')" % type_.timezone
+        else:
+            return 'DateTime'
 
     def visit_datetime64(self, type_, **kw):
         if type_.timezone:
-            return 'DateTime64(%s, \'%s\')' % (type_.precision, type_.timezone)
+            return "DateTime64(%s, '%s')" % (type_.precision, type_.timezone)
         else:
             return 'DateTime64(%s)' % type_.precision
 
     def visit_float32(self, type_, **kw):
         return 'Float32'
 
     def visit_float64(self, type_, **kw):
```

### Comparing `clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/drivers/http/base.py` & `clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/drivers/http/base.py`

 * *Files identical despite different names*

### Comparing `clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/drivers/http/connector.py` & `clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/drivers/http/connector.py`

 * *Files identical despite different names*

### Comparing `clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/drivers/http/escaper.py` & `clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/drivers/http/escaper.py`

 * *Files identical despite different names*

### Comparing `clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/drivers/http/transport.py` & `clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/drivers/http/transport.py`

 * *Files identical despite different names*

### Comparing `clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/drivers/native/base.py` & `clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/drivers/native/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from urllib.parse import quote
+
 from sqlalchemy.util import asbool
 
 from . import connector
 from ..base import (
     ClickHouseDialect, ClickHouseExecutionContextBase, ClickHouseSQLCompiler,
 )
 
@@ -45,14 +47,20 @@
     @classmethod
     def dbapi(cls):
         return connector
 
     def create_connect_args(self, url):
         url = url.set(drivername='clickhouse')
 
+        if url.username:
+            url = url.set(username=quote(url.username))
+
+        if url.password:
+            url = url.set(password=quote(url.password))
+
         self.engine_reflection = asbool(
             url.query.get('engine_reflection', 'true')
         )
 
         return (str(url), ), {}
 
     def _execute(self, connection, sql, scalar=False, **kwargs):
```

### Comparing `clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/drivers/native/connector.py` & `clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/drivers/native/connector.py`

 * *Files identical despite different names*

### Comparing `clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/drivers/reflection.py` & `clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/drivers/reflection.py`

 * *Files identical despite different names*

### Comparing `clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/engines/__init__.py` & `clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/engines/base.py` & `clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/engines/base.py`

 * *Files identical despite different names*

### Comparing `clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/engines/mergetree.py` & `clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/engines/mergetree.py`

 * *Files identical despite different names*

### Comparing `clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/engines/misc.py` & `clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/engines/misc.py`

 * *Files identical despite different names*

### Comparing `clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/engines/replicated.py` & `clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/engines/replicated.py`

 * *Files identical despite different names*

### Comparing `clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/engines/util.py` & `clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/engines/util.py`

 * *Files identical despite different names*

### Comparing `clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/ext/clauses.py` & `clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/ext/clauses.py`

 * *Files identical despite different names*

### Comparing `clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/ext/declarative.py` & `clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/ext/declarative.py`

 * *Files identical despite different names*

### Comparing `clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/orm/query.py` & `clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/orm/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,17 +101,19 @@
     def join(self, *props, **kwargs):
         spec = {
             'type': kwargs.pop('type', None),
             'strictness': kwargs.pop('strictness', None),
             'distribution': kwargs.pop('distribution', None)
         }
         rv = super(Query, self).join(*props, **kwargs)
-        for x in rv._legacy_setup_joins:
-            x_spec = dict(spec)
-            # use 'full' key to pass extra flags
-            x_spec['full'] = x[-1]['full']
-            x[-1]['full'] = x_spec
+
+        x = rv._legacy_setup_joins[-1]
+        x_spec = dict(spec)
+        # use 'full' key to pass extra flags
+        x_spec['full'] = x[-1]['full']
+        x[-1]['full'] = x_spec
+
         return rv
 
     def outerjoin(self, *props, **kwargs):
         kwargs['type'] = kwargs.get('type') or 'LEFT OUTER'
         return self.join(*props, **kwargs)
```

### Comparing `clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/sql/ddl.py` & `clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/sql/ddl.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,16 +21,30 @@
 
 class SchemaDropper(SchemaDropperBase):
     def __init__(self, dialect, connection, if_exists=False, **kwargs):
         self.if_exists = if_exists
         super(SchemaDropper, self).__init__(dialect, connection, **kwargs)
 
     def visit_table(self, table, **kwargs):
+        table.dispatch.before_drop(
+            table,
+            self.connection,
+            checkfirst=self.checkfirst,
+            _ddl_runner=self,
+        )
+
         self.connection.execute(DropTable(table, if_exists=self.if_exists))
 
+        table.dispatch.after_drop(
+            table,
+            self.connection,
+            checkfirst=self.checkfirst,
+            _ddl_runner=self,
+        )
+
     def visit_materialized_view(self, table, **kwargs):
         self.connection.execute(DropView(table, if_exists=self.if_exists))
 
 
 class CreateMaterializedView(_CreateDropBase):
     """Represent a CREATE MATERIALIZED VIEW statement."""
```

### Comparing `clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/sql/schema.py` & `clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/sql/schema.py`

 * *Files identical despite different names*

### Comparing `clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/sql/selectable.py` & `clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/sql/selectable.py`

 * *Files identical despite different names*

### Comparing `clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/types/__init__.py` & `clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/types/__init__.py`

 * *Files identical despite different names*

### Comparing `clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/types/common.py` & `clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/types/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -124,25 +124,28 @@
     __visit_name__ = 'float64'
 
 
 class Date(types.Date, ClickHouseTypeEngine):
     __visit_name__ = 'date'
 
 
-class DateTime(types.Date, ClickHouseTypeEngine):
+class DateTime(types.DateTime, ClickHouseTypeEngine):
     __visit_name__ = 'datetime'
 
+    def __init__(self, timezone=None):
+        super(DateTime, self).__init__()
+        self.timezone = timezone
+
 
 class DateTime64(DateTime, ClickHouseTypeEngine):
     __visit_name__ = 'datetime64'
 
     def __init__(self, precision=3, timezone=None):
         self.precision = precision
-        self.timezone = timezone
-        super(DateTime64, self).__init__()
+        super(DateTime64, self).__init__(timezone=timezone)
 
 
 class Enum(types.Enum, ClickHouseTypeEngine):
     __visit_name__ = 'enum'
 
     def __init__(self, *enums, **kw):
         if not enums:
```

### Comparing `clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/types/ip.py` & `clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/types/ip.py`

 * *Files identical despite different names*

### Comparing `clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy/types/nested.py` & `clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy/types/nested.py`

 * *Files identical despite different names*

### Comparing `clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy.egg-info/PKG-INFO` & `clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: clickhouse-sqlalchemy
-Version: 0.2.3
+Version: 0.2.4
 Summary: Simple ClickHouse SQLAlchemy Dialect
 Home-page: https://github.com/xzkostyan/clickhouse-sqlalchemy
 Author: Konstantin Lebedev
 Author-email: kostyan.lebedev@gmail.com
 License: MIT
 Project-URL: Documentation, https://clickhouse-sqlalchemy.readthedocs.io
 Project-URL: Changes, https://github.com/xzkostyan/clickhouse-sqlalchemy/blob/master/CHANGELOG.md
@@ -40,15 +40,16 @@
         
         
         Usage
         =====
         
         Supported interfaces:
         
-        - **native** [recommended] (TCP) via `clickhouse-driver <https://github.com/mymarilyn/clickhouse-driver>`_
+        - **native** [recommended] (TCP) via `clickhouse-driver <https://github.com/mymarilyn/clickhouse-driver>`
+        - **async native** (TCP) via `asynch <https://github.com/long2ice/asynch>`
         - **http** via requests
         
         Define table
         
             .. code-block:: python
         
                 from sqlalchemy import create_engine, Column, MetaData
@@ -125,8 +126,8 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Requires-Python: >=3.6, <4
+Requires-Python: >=3.7, <4
```

### Comparing `clickhouse-sqlalchemy-0.2.3/clickhouse_sqlalchemy.egg-info/SOURCES.txt` & `clickhouse-sqlalchemy-0.2.4/clickhouse_sqlalchemy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,17 @@
 clickhouse_sqlalchemy/alembic/dialect.py
 clickhouse_sqlalchemy/alembic/operations.py
 clickhouse_sqlalchemy/alembic/renderers.py
 clickhouse_sqlalchemy/alembic/toimpl.py
 clickhouse_sqlalchemy/drivers/__init__.py
 clickhouse_sqlalchemy/drivers/base.py
 clickhouse_sqlalchemy/drivers/reflection.py
+clickhouse_sqlalchemy/drivers/asynch/__init__.py
+clickhouse_sqlalchemy/drivers/asynch/base.py
+clickhouse_sqlalchemy/drivers/asynch/connector.py
 clickhouse_sqlalchemy/drivers/compilers/__init__.py
 clickhouse_sqlalchemy/drivers/compilers/ddlcompiler.py
 clickhouse_sqlalchemy/drivers/compilers/sqlcompiler.py
 clickhouse_sqlalchemy/drivers/compilers/typecompiler.py
 clickhouse_sqlalchemy/drivers/http/__init__.py
 clickhouse_sqlalchemy/drivers/http/base.py
 clickhouse_sqlalchemy/drivers/http/connector.py
```

### Comparing `clickhouse-sqlalchemy-0.2.3/setup.py` & `clickhouse-sqlalchemy-0.2.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,15 +27,16 @@
 
 dialects = [
     'clickhouse{}=clickhouse_sqlalchemy.drivers.{}'.format(driver, d_path)
 
     for driver, d_path in [
         ('', 'http.base:ClickHouseDialect_http'),
         ('.http', 'http.base:ClickHouseDialect_http'),
-        ('.native', 'native.base:ClickHouseDialect_native')
+        ('.native', 'native.base:ClickHouseDialect_native'),
+        ('.asynch', 'asynch.base:ClickHouseDialect_asynch'),
     ]
 ]
 
 github_url = 'https://github.com/xzkostyan/clickhouse-sqlalchemy'
 
 setup(
     name='clickhouse-sqlalchemy',
@@ -87,19 +88,21 @@
     keywords='ClickHouse db database cloud analytics',
 
     project_urls={
         'Documentation': 'https://clickhouse-sqlalchemy.readthedocs.io',
         'Changes': github_url + '/blob/master/CHANGELOG.md'
     },
     packages=find_packages('.', exclude=["tests*"]),
-    python_requires='>=3.6, <4',
+    python_requires='>=3.7, <4',
     install_requires=[
-        'sqlalchemy>=1.4,<1.5',
+        'sqlalchemy>=1.4.24,<1.5',
+        'greenlet>=2.0.1',
         'requests',
-        'clickhouse-driver>=0.1.2'
+        'clickhouse-driver>=0.1.2',
+        'asynch>=0.2.2',
     ],
     # Registering `clickhouse` as dialect.
     entry_points={
         'sqlalchemy.dialects': dialects
     },
     test_suite='pytest'
 )
```

