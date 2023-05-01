# Comparing `tmp/sqlmesh-0.6.3.dev5.tar.gz` & `tmp/sqlmesh-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlmesh-0.6.3.dev5.tar", last modified: Thu Apr 27 21:19:52 2023, max compression
+gzip compressed data, was "sqlmesh-0.6.4.tar", last modified: Mon May  1 23:49:56 2023, max compression
```

## Comparing `sqlmesh-0.6.3.dev5.tar` & `sqlmesh-0.6.4.tar`

### file list

```diff
@@ -1,736 +1,752 @@
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.686674 sqlmesh-0.6.3.dev5/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.542202 sqlmesh-0.6.3.dev5/.circleci/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1872 2023-04-17 00:43:26.000000 sqlmesh-0.6.3.dev5/.circleci/config.yml
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4414 2023-04-17 00:43:26.000000 sqlmesh-0.6.3.dev5/.circleci/continue_config.yml
--rw-r--r--   0 eakmanrq   (501) staff       (20)       66 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev5/.dockerignore
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2152 2023-04-17 00:43:26.000000 sqlmesh-0.6.3.dev5/.gitignore
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1900 2023-03-27 22:28:21.000000 sqlmesh-0.6.3.dev5/.pre-commit-config.yaml
--rw-r--r--   0 eakmanrq   (501) staff       (20)      234 2023-03-31 20:18:29.000000 sqlmesh-0.6.3.dev5/.readthedocs.yaml
--rw-r--r--   0 eakmanrq   (501) staff       (20)      135 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/Dockerfile.api
--rw-r--r--   0 eakmanrq   (501) staff       (20)      383 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/Dockerfile.app
--rw-r--r--   0 eakmanrq   (501) staff       (20)    11346 2023-03-21 00:57:17.000000 sqlmesh-0.6.3.dev5/LICENSE
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1855 2023-04-14 19:58:28.000000 sqlmesh-0.6.3.dev5/Makefile
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2143 2023-04-27 21:19:52.686777 sqlmesh-0.6.3.dev5/PKG-INFO
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1192 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/README.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1008 2023-04-27 17:19:12.000000 sqlmesh-0.6.3.dev5/docker-compose.yml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.544566 sqlmesh-0.6.3.dev5/docs/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.525031 sqlmesh-0.6.3.dev5/docs/_readthedocs/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.544809 sqlmesh-0.6.3.dev5/docs/_readthedocs/html/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-31 20:18:29.000000 sqlmesh-0.6.3.dev5/docs/_readthedocs/html/.keep
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9965 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev5/docs/comparisons.md
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.546509 sqlmesh-0.6.3.dev5/docs/concepts/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.546949 sqlmesh-0.6.3.dev5/docs/concepts/architecture/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1334 2023-03-27 03:14:49.000000 sqlmesh-0.6.3.dev5/docs/concepts/architecture/serialization.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1113 2023-03-27 03:14:49.000000 sqlmesh-0.6.3.dev5/docs/concepts/architecture/snapshots.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6689 2023-04-20 16:12:45.000000 sqlmesh-0.6.3.dev5/docs/concepts/audits.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3866 2023-03-27 03:14:49.000000 sqlmesh-0.6.3.dev5/docs/concepts/environments.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5952 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev5/docs/concepts/glossary.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)       13 2023-03-27 03:14:49.000000 sqlmesh-0.6.3.dev5/docs/concepts/hooks.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3027 2023-03-27 03:14:49.000000 sqlmesh-0.6.3.dev5/docs/concepts/macros.md
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.548078 sqlmesh-0.6.3.dev5/docs/concepts/models/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9934 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/docs/concepts/models/model_kinds.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     7859 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/docs/concepts/models/overview.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     7171 2023-03-27 03:14:56.000000 sqlmesh-0.6.3.dev5/docs/concepts/models/python_models.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4938 2023-03-27 03:14:56.000000 sqlmesh-0.6.3.dev5/docs/concepts/models/seed_models.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5356 2023-03-27 03:14:56.000000 sqlmesh-0.6.3.dev5/docs/concepts/models/sql_models.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6637 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev5/docs/concepts/overview.md
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.548250 sqlmesh-0.6.3.dev5/docs/concepts/plans/
--rw-r--r--   0 eakmanrq   (501) staff       (20)    43124 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/docs/concepts/plans/model_versioning.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8973 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev5/docs/concepts/plans.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5699 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/docs/concepts/tests.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)      607 2023-04-14 19:58:28.000000 sqlmesh-0.6.3.dev5/docs/development.md
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.549811 sqlmesh-0.6.3.dev5/docs/guides/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1943 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/docs/guides/connections.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1309 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev5/docs/guides/migrations.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)    10756 2023-04-06 22:49:28.000000 sqlmesh-0.6.3.dev5/docs/guides/models.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6133 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev5/docs/guides/multi_repo.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2142 2023-04-20 16:12:45.000000 sqlmesh-0.6.3.dev5/docs/guides/projects.md
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.551151 sqlmesh-0.6.3.dev5/docs/guides/scheduling/
--rw-r--r--   0 eakmanrq   (501) staff       (20)   740917 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/docs/guides/scheduling/airflow_successful_plan_apply.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)   379880 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/docs/guides/scheduling/airflow_successful_setup.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5648 2023-03-27 03:14:49.000000 sqlmesh-0.6.3.dev5/docs/guides/scheduling.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1854 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/docs/guides/testing.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5459 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/docs/index.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)      297 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev5/docs/installation.md
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.552873 sqlmesh-0.6.3.dev5/docs/integrations/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2905 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/docs/integrations/airflow.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     7801 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/docs/integrations/dbt.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)    24057 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/docs/integrations/engines.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)      867 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/docs/integrations/github.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)      217 2023-03-27 01:55:02.000000 sqlmesh-0.6.3.dev5/docs/integrations/overview.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)      665 2023-03-28 15:29:23.000000 sqlmesh-0.6.3.dev5/docs/prerequisites.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)    10723 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/docs/quick_start.md
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.554134 sqlmesh-0.6.3.dev5/docs/reference/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6093 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/docs/reference/cli.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)    13607 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/docs/reference/configuration.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4579 2023-04-20 16:12:45.000000 sqlmesh-0.6.3.dev5/docs/reference/notebook.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1127 2023-03-27 03:14:49.000000 sqlmesh-0.6.3.dev5/docs/reference/overview.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)       14 2023-03-27 03:14:49.000000 sqlmesh-0.6.3.dev5/docs/reference/python.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)       16 2023-03-27 03:14:49.000000 sqlmesh-0.6.3.dev5/docs/release_notes.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)      122 2023-03-31 20:18:29.000000 sqlmesh-0.6.3.dev5/docs/requirements.txt
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3249 2023-03-27 01:55:02.000000 sqlmesh-0.6.3.dev5/docs/sqlmesh.png
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.554309 sqlmesh-0.6.3.dev5/examples/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/examples/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.555438 sqlmesh-0.6.3.dev5/examples/airflow/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1713 2023-04-08 22:07:58.000000 sqlmesh-0.6.3.dev5/examples/airflow/Dockerfile.template
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2164 2023-04-14 19:58:28.000000 sqlmesh-0.6.3.dev5/examples/airflow/Makefile
--rw-r--r--   0 eakmanrq   (501) staff       (20)      942 2023-01-20 19:02:18.000000 sqlmesh-0.6.3.dev5/examples/airflow/README.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/examples/airflow/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.555604 sqlmesh-0.6.3.dev5/examples/airflow/dags/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      263 2023-03-21 21:04:44.000000 sqlmesh-0.6.3.dev5/examples/airflow/dags/sqlmesh_integration.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3515 2023-04-08 22:07:58.000000 sqlmesh-0.6.3.dev5/examples/airflow/docker_compose_decorator.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)       12 2023-01-20 19:02:18.000000 sqlmesh-0.6.3.dev5/examples/airflow/requirements.txt
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.556132 sqlmesh-0.6.3.dev5/examples/airflow/spark_conf/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      872 2023-01-20 19:02:18.000000 sqlmesh-0.6.3.dev5/examples/airflow/spark_conf/hive-site.xml
--rw-r--r--   0 eakmanrq   (501) staff       (20)      151 2023-01-20 19:02:18.000000 sqlmesh-0.6.3.dev5/examples/airflow/spark_conf/spark-defaults.conf
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.526243 sqlmesh-0.6.3.dev5/examples/multi/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.556298 sqlmesh-0.6.3.dev5/examples/multi/repo_1/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.556421 sqlmesh-0.6.3.dev5/examples/multi/repo_1/audits/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev5/examples/multi/repo_1/audits/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)      147 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/examples/multi/repo_1/config.yaml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.556603 sqlmesh-0.6.3.dev5/examples/multi/repo_1/macros/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev5/examples/multi/repo_1/macros/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev5/examples/multi/repo_1/macros/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.557047 sqlmesh-0.6.3.dev5/examples/multi/repo_1/models/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev5/examples/multi/repo_1/models/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)       63 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev5/examples/multi/repo_1/models/a.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)       53 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev5/examples/multi/repo_1/models/b.sql
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.557218 sqlmesh-0.6.3.dev5/examples/multi/repo_1/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev5/examples/multi/repo_1/tests/.gitkeep
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.557301 sqlmesh-0.6.3.dev5/examples/multi/repo_2/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.557491 sqlmesh-0.6.3.dev5/examples/multi/repo_2/audits/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev5/examples/multi/repo_2/audits/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)      147 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/examples/multi/repo_2/config.yaml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.557659 sqlmesh-0.6.3.dev5/examples/multi/repo_2/macros/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev5/examples/multi/repo_2/macros/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev5/examples/multi/repo_2/macros/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.557970 sqlmesh-0.6.3.dev5/examples/multi/repo_2/models/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev5/examples/multi/repo_2/models/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)       64 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev5/examples/multi/repo_2/models/c.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)       53 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev5/examples/multi/repo_2/models/d.sql
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.558101 sqlmesh-0.6.3.dev5/examples/multi/repo_2/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev5/examples/multi/repo_2/tests/.gitkeep
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.558674 sqlmesh-0.6.3.dev5/examples/sushi/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-20 19:02:18.000000 sqlmesh-0.6.3.dev5/examples/sushi/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.559087 sqlmesh-0.6.3.dev5/examples/sushi/audits/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      105 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/examples/sushi/audits/items.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      119 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/examples/sushi/audits/order_items.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      829 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/examples/sushi/config.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.559355 sqlmesh-0.6.3.dev5/examples/sushi/data/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-06 17:30:39.000000 sqlmesh-0.6.3.dev5/examples/sushi/data/.keep
--rw-r--r--   0 eakmanrq   (501) staff       (20)      551 2023-01-20 19:02:18.000000 sqlmesh-0.6.3.dev5/examples/sushi/helper.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.559520 sqlmesh-0.6.3.dev5/examples/sushi/hooks/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/examples/sushi/hooks/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      247 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/examples/sushi/hooks/hooks.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.566978 sqlmesh-0.6.3.dev5/examples/sushi/macros/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-20 19:02:18.000000 sqlmesh-0.6.3.dev5/examples/sushi/macros/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      702 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/examples/sushi/macros/macros.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.569144 sqlmesh-0.6.3.dev5/examples/sushi/models/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      916 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/examples/sushi/models/customer_revenue_by_day.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      204 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/examples/sushi/models/customers.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1910 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/examples/sushi/models/items.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1911 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/examples/sushi/models/order_items.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1642 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/examples/sushi/models/orders.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      346 2023-04-11 16:01:14.000000 sqlmesh-0.6.3.dev5/examples/sushi/models/top_waiters.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      465 2023-04-14 20:24:08.000000 sqlmesh-0.6.3.dev5/examples/sushi/models/waiter_as_customer_by_day.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      123 2023-02-17 23:03:10.000000 sqlmesh-0.6.3.dev5/examples/sushi/models/waiter_names.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      691 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/examples/sushi/models/waiter_revenue_by_day.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      197 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/examples/sushi/models/waiters.sql
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.569485 sqlmesh-0.6.3.dev5/examples/sushi/seeds/
--rw-r--r--   0 eakmanrq   (501) staff       (20)       88 2023-01-20 19:02:18.000000 sqlmesh-0.6.3.dev5/examples/sushi/seeds/waiter_names.csv
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.569652 sqlmesh-0.6.3.dev5/examples/sushi/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1459 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/examples/sushi/tests/test_customer_revenue_by_day.yaml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.570648 sqlmesh-0.6.3.dev5/examples/sushi_dbt/
--rw-r--r--   0 eakmanrq   (501) staff       (20)       15 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/examples/sushi_dbt/.gitignore
--rw-r--r--   0 eakmanrq   (501) staff       (20)       41 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/examples/sushi_dbt/.user.yml
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/examples/sushi_dbt/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.570896 sqlmesh-0.6.3.dev5/examples/sushi_dbt/analyses/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-20 19:02:18.000000 sqlmesh-0.6.3.dev5/examples/sushi_dbt/analyses/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)      291 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/examples/sushi_dbt/config.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      507 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/examples/sushi_dbt/dbt_project.yml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.571209 sqlmesh-0.6.3.dev5/examples/sushi_dbt/macros/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      941 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/examples/sushi_dbt/macros/incremental.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)       80 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/examples/sushi_dbt/macros/log_value.sql
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.572240 sqlmesh-0.6.3.dev5/examples/sushi_dbt/models/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1125 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/examples/sushi_dbt/models/customer_revenue_by_day.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)       80 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/examples/sushi_dbt/models/customers.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      182 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/examples/sushi_dbt/models/schema.yml
--rw-r--r--   0 eakmanrq   (501) staff       (20)      309 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/examples/sushi_dbt/models/top_waiters.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      389 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/examples/sushi_dbt/models/waiter_as_customer_by_day.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      752 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/examples/sushi_dbt/models/waiter_revenue_by_day.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      186 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/examples/sushi_dbt/models/waiters.sql
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.527422 sqlmesh-0.6.3.dev5/examples/sushi_dbt/packages/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.572386 sqlmesh-0.6.3.dev5/examples/sushi_dbt/packages/customers/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.572537 sqlmesh-0.6.3.dev5/examples/sushi_dbt/packages/customers/analyses/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/examples/sushi_dbt/packages/customers/analyses/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)      663 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/examples/sushi_dbt/packages/customers/dbt_project.yml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.572767 sqlmesh-0.6.3.dev5/examples/sushi_dbt/packages/customers/macros/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      117 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/examples/sushi_dbt/packages/customers/macros/current_engine.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)       65 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/examples/sushi_dbt/packages/customers/macros/distinct.sql
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.572923 sqlmesh-0.6.3.dev5/examples/sushi_dbt/packages/customers/models/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/examples/sushi_dbt/packages/customers/models/schema.yml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.573011 sqlmesh-0.6.3.dev5/examples/sushi_dbt/packages/customers/seeds/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/examples/sushi_dbt/packages/customers/seeds/.gitkeep
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.573099 sqlmesh-0.6.3.dev5/examples/sushi_dbt/packages/customers/snapshots/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/examples/sushi_dbt/packages/customers/snapshots/.gitkeep
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.573180 sqlmesh-0.6.3.dev5/examples/sushi_dbt/packages/customers/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/examples/sushi_dbt/packages/customers/tests/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)      783 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/examples/sushi_dbt/profiles.yml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.573812 sqlmesh-0.6.3.dev5/examples/sushi_dbt/seeds/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2327 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/examples/sushi_dbt/seeds/items.csv
--rw-r--r--   0 eakmanrq   (501) staff       (20)    10472 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/examples/sushi_dbt/seeds/order_items.csv
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9746 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/examples/sushi_dbt/seeds/orders.csv
--rw-r--r--   0 eakmanrq   (501) staff       (20)       97 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/examples/sushi_dbt/seeds/properties.yml
--rw-r--r--   0 eakmanrq   (501) staff       (20)       88 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/examples/sushi_dbt/seeds/waiter_names.csv
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.573946 sqlmesh-0.6.3.dev5/examples/sushi_dbt/snapshots/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-20 19:02:18.000000 sqlmesh-0.6.3.dev5/examples/sushi_dbt/snapshots/.gitkeep
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.574024 sqlmesh-0.6.3.dev5/examples/sushi_dbt/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-20 19:02:18.000000 sqlmesh-0.6.3.dev5/examples/sushi_dbt/tests/.gitkeep
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.574185 sqlmesh-0.6.3.dev5/examples/wursthall/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/examples/wursthall/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.528228 sqlmesh-0.6.3.dev5/examples/wursthall/audits/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.574312 sqlmesh-0.6.3.dev5/examples/wursthall/audits/db/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      141 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/examples/wursthall/audits/db/order_f.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)       66 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/examples/wursthall/config.yaml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.574518 sqlmesh-0.6.3.dev5/examples/wursthall/macros/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/examples/wursthall/macros/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      618 2023-04-06 22:49:28.000000 sqlmesh-0.6.3.dev5/examples/wursthall/macros/macros.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.574754 sqlmesh-0.6.3.dev5/examples/wursthall/models/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/examples/wursthall/models/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.575478 sqlmesh-0.6.3.dev5/examples/wursthall/models/db/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      433 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/examples/wursthall/models/db/customer_d.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      256 2023-04-27 17:28:43.000000 sqlmesh-0.6.3.dev5/examples/wursthall/models/db/item_d.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3161 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/examples/wursthall/models/db/order_f.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      542 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/examples/wursthall/models/db/order_item_f.sql
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.576137 sqlmesh-0.6.3.dev5/examples/wursthall/models/src/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/examples/wursthall/models/src/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1672 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/examples/wursthall/models/src/customer_details.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      120 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/examples/wursthall/models/src/menu_item_details.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3434 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/examples/wursthall/models/src/order_item_details.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      892 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/examples/wursthall/models/src/shared.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.528541 sqlmesh-0.6.3.dev5/examples/wursthall/seeds/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.576270 sqlmesh-0.6.3.dev5/examples/wursthall/seeds/src/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     7416 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/examples/wursthall/seeds/src/menu_item_details.csv
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.576585 sqlmesh-0.6.3.dev5/examples/wursthall/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      888 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/examples/wursthall/tests/test_customer_d.yaml
--rw-r--r--   0 eakmanrq   (501) staff       (20)      955 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/examples/wursthall/tests/test_order_item_f.yaml
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2113 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev5/mkdocs.yml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.576722 sqlmesh-0.6.3.dev5/pdoc/
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)     1153 2023-03-28 16:31:06.000000 sqlmesh-0.6.3.dev5/pdoc/cli.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.577047 sqlmesh-0.6.3.dev5/pdoc/templates/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      131 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev5/pdoc/templates/module.html.jinja2
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.577273 sqlmesh-0.6.3.dev5/posts/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.581478 sqlmesh-0.6.3.dev5/posts/virtual_data_environments/
--rw-r--r--   0 eakmanrq   (501) staff       (20)   318753 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev5/posts/virtual_data_environments/change_categorization.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)   274526 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev5/posts/virtual_data_environments/isolated_rigid_envs.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)   163619 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev5/posts/virtual_data_environments/partial_breaking.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)   298971 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev5/posts/virtual_data_environments/stateful_envs.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)   366545 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev5/posts/virtual_data_environments/virtual_envs.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)  1344487 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev5/posts/virtual_data_environments/virtual_envs_end_to_end.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)    18638 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/posts/virtual_data_environments.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)      734 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev5/pytest.ini
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1393 2023-04-27 21:19:52.687250 sqlmesh-0.6.3.dev5/setup.cfg
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3164 2023-04-27 21:05:12.000000 sqlmesh-0.6.3.dev5/setup.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.586694 sqlmesh-0.6.3.dev5/sqlmesh/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        3 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev5/sqlmesh/.airflowignore
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3950 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/sqlmesh/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      173 2023-04-27 21:19:52.000000 sqlmesh-0.6.3.dev5/sqlmesh/_version.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.588373 sqlmesh-0.6.3.dev5/sqlmesh/cli/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      898 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/sqlmesh/cli/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4314 2023-04-06 22:49:28.000000 sqlmesh-0.6.3.dev5/sqlmesh/cli/example_project.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9641 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/sqlmesh/cli/main.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1433 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev5/sqlmesh/cli/options.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.591996 sqlmesh-0.6.3.dev5/sqlmesh/core/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      586 2023-03-15 16:48:19.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/_typing.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.592573 sqlmesh-0.6.3.dev5/sqlmesh/core/audit/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      449 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/audit/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1071 2023-04-14 20:24:08.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/audit/builtin.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8136 2023-04-14 20:24:08.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/audit/definition.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.594390 sqlmesh-0.6.3.dev5/sqlmesh/core/config/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      668 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/config/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4412 2023-04-14 19:58:28.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/config/base.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1001 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/config/categorizer.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      940 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/config/common.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    21184 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/config/connection.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3351 2023-04-20 16:12:45.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/config/loader.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1655 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/config/model.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5611 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/config/root.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8421 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/config/scheduler.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    29390 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/console.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      735 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/constants.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    36130 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/context.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8904 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/context_diff.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    17626 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/dialect.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.596727 sqlmesh-0.6.3.dev5/sqlmesh/core/engine_adapter/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2626 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/engine_adapter/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      762 2023-01-17 23:57:22.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/engine_adapter/_typing.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    29488 2023-04-27 21:17:48.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/engine_adapter/base.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4191 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/engine_adapter/base_postgres.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4238 2023-04-14 22:30:56.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/engine_adapter/base_spark.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    15681 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/engine_adapter/bigquery.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      402 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/engine_adapter/databricks.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1939 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/engine_adapter/databricks_api.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1971 2023-04-14 18:08:36.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/engine_adapter/duckdb.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2149 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/engine_adapter/postgres.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6650 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/engine_adapter/redshift.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1181 2023-03-31 20:18:23.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/engine_adapter/shared.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2658 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/engine_adapter/snowflake.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4810 2023-04-27 21:18:54.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/engine_adapter/spark.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1849 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/environment.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      742 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/hooks.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    12673 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/loader.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    18920 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/macros.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.597815 sqlmesh-0.6.3.dev5/sqlmesh/core/model/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      594 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/model/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1746 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/model/cache.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1300 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/model/common.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2417 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/model/decorator.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    47699 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/model/definition.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8168 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/model/kind.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    13034 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/model/meta.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2017 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/model/seed.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2314 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/notification_target.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.598258 sqlmesh-0.6.3.dev5/sqlmesh/core/plan/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      191 2022-12-27 18:08:03.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/plan/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    22476 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/plan/definition.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8125 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/plan/evaluator.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    12623 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/renderer.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    15386 2023-04-14 20:24:08.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/scheduler.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    20418 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/schema_diff.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.598983 sqlmesh-0.6.3.dev5/sqlmesh/core/snapshot/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      527 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/snapshot/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1990 2023-03-27 01:55:02.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/snapshot/categorizer.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    33750 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/snapshot/definition.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    19247 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/snapshot/evaluator.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.599595 sqlmesh-0.6.3.dev5/sqlmesh/core/state_sync/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      692 2023-04-14 19:58:28.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/state_sync/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    13382 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/state_sync/base.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    13144 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/state_sync/common.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    20682 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/state_sync/engine_adapter.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    10834 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/test.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1412 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/sqlmesh/core/user.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.608018 sqlmesh-0.6.3.dev5/sqlmesh/dbt/
--rw-r--r--   0 eakmanrq   (501) staff       (20)       79 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/sqlmesh/dbt/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9390 2023-04-14 22:30:56.000000 sqlmesh-0.6.3.dev5/sqlmesh/dbt/adapter.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    16746 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/sqlmesh/dbt/basemodel.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    11231 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/sqlmesh/dbt/builtin.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1762 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/sqlmesh/dbt/column.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4771 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/sqlmesh/dbt/common.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5087 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/sqlmesh/dbt/context.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8044 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/sqlmesh/dbt/loader.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9806 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/sqlmesh/dbt/model.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    13257 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/sqlmesh/dbt/package.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3701 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/sqlmesh/dbt/profile.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4772 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/sqlmesh/dbt/project.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      927 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/sqlmesh/dbt/seed.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3137 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev5/sqlmesh/dbt/source.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    13503 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/sqlmesh/dbt/target.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      291 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/sqlmesh/dbt/util.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.608371 sqlmesh-0.6.3.dev5/sqlmesh/engines/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev5/sqlmesh/engines/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4437 2023-03-22 20:26:36.000000 sqlmesh-0.6.3.dev5/sqlmesh/engines/commands.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.608814 sqlmesh-0.6.3.dev5/sqlmesh/engines/spark/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev5/sqlmesh/engines/spark/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3414 2023-03-22 20:32:25.000000 sqlmesh-0.6.3.dev5/sqlmesh/engines/spark/app.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.609408 sqlmesh-0.6.3.dev5/sqlmesh/engines/spark/db_api/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev5/sqlmesh/engines/spark/db_api/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      148 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev5/sqlmesh/engines/spark/db_api/errors.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2571 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/sqlmesh/engines/spark/db_api/spark_session.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.609651 sqlmesh-0.6.3.dev5/sqlmesh/integrations/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev5/sqlmesh/integrations/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.610321 sqlmesh-0.6.3.dev5/sqlmesh/integrations/github/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev5/sqlmesh/integrations/github/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2210 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/sqlmesh/integrations/github/notification_operator_provider.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1726 2023-01-20 19:02:18.000000 sqlmesh-0.6.3.dev5/sqlmesh/integrations/github/notification_target.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1829 2023-01-18 17:26:59.000000 sqlmesh-0.6.3.dev5/sqlmesh/integrations/github/shared.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    13754 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/sqlmesh/magics.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.611184 sqlmesh-0.6.3.dev5/sqlmesh/migrations/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-14 19:58:28.000000 sqlmesh-0.6.3.dev5/sqlmesh/migrations/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1749 2023-04-14 19:58:28.000000 sqlmesh-0.6.3.dev5/sqlmesh/migrations/v0001_init.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      103 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev5/sqlmesh/migrations/v0002_remove_identify.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1183 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/sqlmesh/migrations/v0003_move_batch_size.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      534 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/sqlmesh/migrations/v0004_environmnent_add_finalized_at.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev5/sqlmesh/py.typed
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.611307 sqlmesh-0.6.3.dev5/sqlmesh/schedulers/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev5/sqlmesh/schedulers/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.613058 sqlmesh-0.6.3.dev5/sqlmesh/schedulers/airflow/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-05 17:38:29.000000 sqlmesh-0.6.3.dev5/sqlmesh/schedulers/airflow/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4020 2023-04-14 19:58:28.000000 sqlmesh-0.6.3.dev5/sqlmesh/schedulers/airflow/api.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8053 2023-04-14 19:58:28.000000 sqlmesh-0.6.3.dev5/sqlmesh/schedulers/airflow/client.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3830 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/sqlmesh/schedulers/airflow/common.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    18819 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/sqlmesh/schedulers/airflow/dag_generator.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.613693 sqlmesh-0.6.3.dev5/sqlmesh/schedulers/airflow/hooks/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-15 19:26:11.000000 sqlmesh-0.6.3.dev5/sqlmesh/schedulers/airflow/hooks/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2132 2023-03-22 20:54:22.000000 sqlmesh-0.6.3.dev5/sqlmesh/schedulers/airflow/hooks/bigquery.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      868 2023-03-22 20:54:22.000000 sqlmesh-0.6.3.dev5/sqlmesh/schedulers/airflow/hooks/redshift.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8508 2023-03-22 20:33:52.000000 sqlmesh-0.6.3.dev5/sqlmesh/schedulers/airflow/integration.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.615335 sqlmesh-0.6.3.dev5/sqlmesh/schedulers/airflow/operators/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev5/sqlmesh/schedulers/airflow/operators/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1444 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/sqlmesh/schedulers/airflow/operators/bigquery.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6307 2023-03-22 20:26:36.000000 sqlmesh-0.6.3.dev5/sqlmesh/schedulers/airflow/operators/databricks.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2549 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/sqlmesh/schedulers/airflow/operators/hwm_sensor.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      877 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/sqlmesh/schedulers/airflow/operators/notification.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1322 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev5/sqlmesh/schedulers/airflow/operators/postgres.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1211 2023-01-20 20:10:57.000000 sqlmesh-0.6.3.dev5/sqlmesh/schedulers/airflow/operators/redshift.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1340 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/sqlmesh/schedulers/airflow/operators/snowflake.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5222 2023-03-22 20:26:36.000000 sqlmesh-0.6.3.dev5/sqlmesh/schedulers/airflow/operators/spark_submit.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    11104 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/sqlmesh/schedulers/airflow/operators/targets.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4400 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/sqlmesh/schedulers/airflow/plan.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1292 2023-04-14 19:58:28.000000 sqlmesh-0.6.3.dev5/sqlmesh/schedulers/airflow/plugin.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4139 2023-04-14 19:58:28.000000 sqlmesh-0.6.3.dev5/sqlmesh/schedulers/airflow/state_sync.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5213 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev5/sqlmesh/schedulers/airflow/util.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.618182 sqlmesh-0.6.3.dev5/sqlmesh/utils/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4378 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev5/sqlmesh/utils/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3593 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/sqlmesh/utils/cache.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8053 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/sqlmesh/utils/concurrency.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     7530 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/sqlmesh/utils/connection_pool.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      410 2022-12-30 00:03:50.000000 sqlmesh-0.6.3.dev5/sqlmesh/utils/conversions.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4329 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/sqlmesh/utils/dag.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     7549 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/sqlmesh/utils/date.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1244 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/sqlmesh/utils/errors.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    16133 2023-04-27 21:05:12.000000 sqlmesh-0.6.3.dev5/sqlmesh/utils/jinja.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    15093 2023-04-06 22:49:28.000000 sqlmesh-0.6.3.dev5/sqlmesh/utils/metaprogramming.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      888 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/sqlmesh/utils/pandas.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1609 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/sqlmesh/utils/pydantic.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1534 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/sqlmesh/utils/rich.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6487 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev5/sqlmesh/utils/transactional_file.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1419 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/sqlmesh/utils/yaml.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.587574 sqlmesh-0.6.3.dev5/sqlmesh.egg-info/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2143 2023-04-27 21:19:52.000000 sqlmesh-0.6.3.dev5/sqlmesh.egg-info/PKG-INFO
--rw-r--r--   0 eakmanrq   (501) staff       (20)    21395 2023-04-27 21:19:52.000000 sqlmesh-0.6.3.dev5/sqlmesh.egg-info/SOURCES.txt
--rw-r--r--   0 eakmanrq   (501) staff       (20)        1 2023-04-27 21:19:52.000000 sqlmesh-0.6.3.dev5/sqlmesh.egg-info/dependency_links.txt
--rw-r--r--   0 eakmanrq   (501) staff       (20)      142 2023-04-27 21:19:52.000000 sqlmesh-0.6.3.dev5/sqlmesh.egg-info/entry_points.txt
--rw-r--r--   0 eakmanrq   (501) staff       (20)      844 2023-04-27 21:19:52.000000 sqlmesh-0.6.3.dev5/sqlmesh.egg-info/requires.txt
--rw-r--r--   0 eakmanrq   (501) staff       (20)       12 2023-04-27 21:19:52.000000 sqlmesh-0.6.3.dev5/sqlmesh.egg-info/top_level.txt
--rw-r--r--   0 eakmanrq   (501) staff       (20)    21020 2023-03-27 03:14:56.000000 sqlmesh-0.6.3.dev5/sqlmesh.svg
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.618528 sqlmesh-0.6.3.dev5/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev5/tests/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      285 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/tests/common_fixtures.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4037 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/tests/conftest.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.622830 sqlmesh-0.6.3.dev5/tests/core/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev5/tests/core/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.628076 sqlmesh-0.6.3.dev5/tests/core/engine_adapter/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev5/tests/core/engine_adapter/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    27881 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev5/tests/core/engine_adapter/test_base.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2114 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/tests/core/engine_adapter/test_base_postgres.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1270 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev5/tests/core/engine_adapter/test_base_spark.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     7171 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/tests/core/engine_adapter/test_bigquery.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1253 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev5/tests/core/engine_adapter/test_databricks.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2613 2023-01-17 20:15:22.000000 sqlmesh-0.6.3.dev5/tests/core/engine_adapter/test_duckdb.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1569 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev5/tests/core/engine_adapter/test_postgres.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8036 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev5/tests/core/engine_adapter/test_redshift.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3191 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev5/tests/core/engine_adapter/test_spark.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     7073 2023-04-14 20:24:08.000000 sqlmesh-0.6.3.dev5/tests/core/test_audit.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6611 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/tests/core/test_config.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      850 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/tests/core/test_connection_config.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    10197 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev5/tests/core/test_context.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2749 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/tests/core/test_dialect.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      464 2022-12-28 16:53:44.000000 sqlmesh-0.6.3.dev5/tests/core/test_environment.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    26741 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/tests/core/test_integration.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5880 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev5/tests/core/test_macros.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    25301 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/tests/core/test_model.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    15741 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/tests/core/test_plan.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3862 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/tests/core/test_plan_evaluator.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4647 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/tests/core/test_scheduler.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    32235 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev5/tests/core/test_schema_diff.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      857 2023-01-06 18:44:22.000000 sqlmesh-0.6.3.dev5/tests/core/test_seed.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    28498 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/tests/core/test_snapshot.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    10299 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/tests/core/test_snapshot_evaluator.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    23620 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/tests/core/test_state_sync.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.628693 sqlmesh-0.6.3.dev5/tests/dbt/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-16 20:33:14.000000 sqlmesh-0.6.3.dev5/tests/dbt/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      739 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/tests/dbt/conftest.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2537 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev5/tests/dbt/test_adapter.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    13195 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/tests/dbt/test_config.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    17095 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/tests/dbt/test_transformation.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.628977 sqlmesh-0.6.3.dev5/tests/engines/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev5/tests/engines/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.629381 sqlmesh-0.6.3.dev5/tests/engines/spark/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev5/tests/engines/spark/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      357 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev5/tests/engines/spark/conftest.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1503 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev5/tests/engines/spark/test_db_api.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.531641 sqlmesh-0.6.3.dev5/tests/fixtures/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.530536 sqlmesh-0.6.3.dev5/tests/fixtures/dbt/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.630285 sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.630411 sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/analyses/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/analyses/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)      291 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/config.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.530671 sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/dbt_packages/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1055 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/dbt_project.yml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.630528 sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/logs/
--rw-r--r--   0 eakmanrq   (501) staff       (20)    10264 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/logs/dbt.log.legacy
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.630835 sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/macros/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      941 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/macros/incremental.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)       80 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/macros/log_value.sql
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.631549 sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/models/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      247 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/models/schema.yml
--rw-r--r--   0 eakmanrq   (501) staff       (20)      334 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/models/top_waiters.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      389 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/models/waiter_as_customer_by_day.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      863 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/models/waiter_revenue_by_day.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      196 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/models/waiters.sql
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.530973 sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/packages/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.631680 sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/packages/customers/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.631810 sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/packages/customers/analyses/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/packages/customers/analyses/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)      663 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/packages/customers/dbt_project.yml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.632049 sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/packages/customers/macros/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      117 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/packages/customers/macros/current_engine.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)       65 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/packages/customers/macros/distinct.sql
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.632462 sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/packages/customers/models/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1155 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/packages/customers/models/customer_revenue_by_day.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      108 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/packages/customers/models/customers.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      193 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/packages/customers/models/schema.yml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.632630 sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/packages/customers/seeds/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/packages/customers/seeds/.gitkeep
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.632736 sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/packages/customers/snapshots/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/packages/customers/snapshots/.gitkeep
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.632841 sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/packages/customers/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/packages/customers/tests/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)       41 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/packages.yml
--rw-r--r--   0 eakmanrq   (501) staff       (20)      540 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/profiles.yml
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1250 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/seed_sources.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.633069 sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/seeds/
--rw-r--r--   0 eakmanrq   (501) staff       (20)       42 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/seeds/properties.yml
--rw-r--r--   0 eakmanrq   (501) staff       (20)       88 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/seeds/waiter_names.csv
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.633204 sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/snapshots/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/snapshots/.gitkeep
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.633562 sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/source_data/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2327 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/source_data/items.csv
--rw-r--r--   0 eakmanrq   (501) staff       (20)    10472 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/source_data/order_items.csv
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9746 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/source_data/orders.csv
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.633696 sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/tests/.gitkeep
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.634028 sqlmesh-0.6.3.dev5/tests/fixtures/migrations/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9823 2023-04-14 19:58:28.000000 sqlmesh-0.6.3.dev5/tests/fixtures/migrations/environments.json
--rw-r--r--   0 eakmanrq   (501) staff       (20)    25229 2023-04-14 19:58:28.000000 sqlmesh-0.6.3.dev5/tests/fixtures/migrations/snapshots.json
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.634390 sqlmesh-0.6.3.dev5/tests/integrations/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev5/tests/integrations/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.634623 sqlmesh-0.6.3.dev5/tests/integrations/github/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev5/tests/integrations/github/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.634920 sqlmesh-0.6.3.dev5/tests/integrations/github/fixtures/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      816 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev5/tests/integrations/github/fixtures/pull_request_review.json
--rw-r--r--   0 eakmanrq   (501) staff       (20)      477 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/tests/integrations/github/test_notification_target.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.635095 sqlmesh-0.6.3.dev5/tests/schedulers/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev5/tests/schedulers/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.636358 sqlmesh-0.6.3.dev5/tests/schedulers/airflow/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev5/tests/schedulers/airflow/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1414 2023-01-20 19:02:18.000000 sqlmesh-0.6.3.dev5/tests/schedulers/airflow/conftest.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.636826 sqlmesh-0.6.3.dev5/tests/schedulers/airflow/operators/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev5/tests/schedulers/airflow/operators/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4442 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/tests/schedulers/airflow/operators/test_hwm_sensor.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4392 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/tests/schedulers/airflow/operators/test_targets.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9857 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/tests/schedulers/airflow/test_client.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1345 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/tests/schedulers/airflow/test_end_to_end.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6222 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/tests/schedulers/airflow/test_integration.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5944 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/tests/schedulers/airflow/test_plan.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.639055 sqlmesh-0.6.3.dev5/tests/utils/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev5/tests/utils/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1118 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/tests/utils/test_cache.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3580 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/tests/utils/test_concurrency.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6430 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/tests/utils/test_connection_pool.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1381 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/tests/utils/test_dag.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1818 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev5/tests/utils/test_date.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      551 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev5/tests/utils/test_filesystem.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5516 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/tests/utils/test_jinja.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5790 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/tests/utils/test_metaprogramming.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2501 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/tests/utils/test_pandas.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      518 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev5/tests/utils/test_pydantic.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2911 2023-04-17 00:43:26.000000 sqlmesh-0.6.3.dev5/tests/utils/test_transactional_file.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1194 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/tests/utils/test_yaml.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.639263 sqlmesh-0.6.3.dev5/tests/web/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-20 19:02:18.000000 sqlmesh-0.6.3.dev5/tests/web/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    16232 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/tests/web/test_main.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.639391 sqlmesh-0.6.3.dev5/web/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-20 19:02:18.000000 sqlmesh-0.6.3.dev5/web/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.643815 sqlmesh-0.6.3.dev5/web/client/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1104 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/web/client/.eslintrc.js
--rw-r--r--   0 eakmanrq   (501) staff       (20)       94 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/web/client/.gitignore
--rw-r--r--   0 eakmanrq   (501) staff       (20)      129 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/web/client/.prettierignore
--rw-r--r--   0 eakmanrq   (501) staff       (20)      403 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/web/client/.prettierrc.js
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1076 2023-03-27 22:28:21.000000 sqlmesh-0.6.3.dev5/web/client/index.html
--rw-r--r--   0 eakmanrq   (501) staff       (20)    37689 2023-04-27 17:30:24.000000 sqlmesh-0.6.3.dev5/web/client/openapi.json
--rw-r--r--   0 eakmanrq   (501) staff       (20)      330 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/web/client/orval.config.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)   408504 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/web/client/package-lock.json
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2389 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/web/client/package.json
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1642 2023-04-17 00:43:26.000000 sqlmesh-0.6.3.dev5/web/client/playwright.config.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)       82 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/web/client/postcss.config.js
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.532268 sqlmesh-0.6.3.dev5/web/client/public/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.644115 sqlmesh-0.6.3.dev5/web/client/public/favicons/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2473 2023-03-27 01:55:02.000000 sqlmesh-0.6.3.dev5/web/client/public/favicons/favicon.ico
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.644886 sqlmesh-0.6.3.dev5/web/client/src/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.645674 sqlmesh-0.6.3.dev5/web/client/src/api/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1236 2023-04-20 17:40:30.000000 sqlmesh-0.6.3.dev5/web/client/src/api/channels.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5243 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/web/client/src/api/index.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3247 2023-03-22 20:27:52.000000 sqlmesh-0.6.3.dev5/web/client/src/api/instance.ts
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.532493 sqlmesh-0.6.3.dev5/web/client/src/assets/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.532586 sqlmesh-0.6.3.dev5/web/client/src/assets/fonts/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.650931 sqlmesh-0.6.3.dev5/web/client/src/assets/fonts/Circular STD/
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    74500 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev5/web/client/src/assets/fonts/Circular STD/CircularStd-Black.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    74524 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev5/web/client/src/assets/fonts/Circular STD/CircularStd-BlackItalic.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    74368 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev5/web/client/src/assets/fonts/Circular STD/CircularStd-Bold.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    73964 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev5/web/client/src/assets/fonts/Circular STD/CircularStd-BoldItalic.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    68940 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev5/web/client/src/assets/fonts/Circular STD/CircularStd-Book.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    67284 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev5/web/client/src/assets/fonts/Circular STD/CircularStd-BookItalic.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    74116 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev5/web/client/src/assets/fonts/Circular STD/CircularStd-Medium.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    73916 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev5/web/client/src/assets/fonts/Circular STD/CircularStd-MediumItalic.otf
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.656766 sqlmesh-0.6.3.dev5/web/client/src/assets/fonts/Publico/
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    55004 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev5/web/client/src/assets/fonts/Publico/Publico-Black.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    56384 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev5/web/client/src/assets/fonts/Publico/Publico-BlackItalic.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    57104 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev5/web/client/src/assets/fonts/Publico/Publico-Bold.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    62320 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev5/web/client/src/assets/fonts/Publico/Publico-BoldItalic.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    56652 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev5/web/client/src/assets/fonts/Publico/Publico-Extrabold.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    61688 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev5/web/client/src/assets/fonts/Publico/Publico-ExtraboldItalic.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    57680 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev5/web/client/src/assets/fonts/Publico/Publico-Italic.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    53148 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev5/web/client/src/assets/fonts/Publico/Publico-Light.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    57060 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev5/web/client/src/assets/fonts/Publico/Publico-LightItalic.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    56836 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev5/web/client/src/assets/fonts/Publico/Publico-Medium.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    61460 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev5/web/client/src/assets/fonts/Publico/Publico-MediumItalic.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    52820 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev5/web/client/src/assets/fonts/Publico/Publico-Roman.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    59176 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev5/web/client/src/assets/fonts/Publico/PublicoText-Bold.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    63876 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev5/web/client/src/assets/fonts/Publico/PublicoText-BoldItalic.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    60768 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev5/web/client/src/assets/fonts/Publico/PublicoText-Italic.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    81732 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev5/web/client/src/assets/fonts/Publico/PublicoText-Roman.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    60992 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev5/web/client/src/assets/fonts/Publico/PublicoText-Semibold.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    64792 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev5/web/client/src/assets/fonts/Publico/PublicoText-SemiboldItalic.otf
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.658081 sqlmesh-0.6.3.dev5/web/client/src/context/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4126 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/web/client/src/context/context.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5719 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/web/client/src/context/editor.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)      923 2023-04-14 20:24:08.000000 sqlmesh-0.6.3.dev5/web/client/src/context/fileTree.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2284 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/web/client/src/context/lineage.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2661 2023-04-14 19:58:28.000000 sqlmesh-0.6.3.dev5/web/client/src/context/plan.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1562 2023-03-22 22:04:55.000000 sqlmesh-0.6.3.dev5/web/client/src/context/theme.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.658535 sqlmesh-0.6.3.dev5/web/client/src/hooks/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      308 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/web/client/src/hooks/useActiveFocus.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)      817 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/web/client/src/hooks/useLocalStorage.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9555 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/web/client/src/index.css
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.532795 sqlmesh-0.6.3.dev5/web/client/src/library/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.534057 sqlmesh-0.6.3.dev5/web/client/src/library/components/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.658736 sqlmesh-0.6.3.dev5/web/client/src/library/components/banner/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1705 2023-04-20 17:40:30.000000 sqlmesh-0.6.3.dev5/web/client/src/library/components/banner/Banner.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.658986 sqlmesh-0.6.3.dev5/web/client/src/library/components/button/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4517 2023-03-27 01:55:02.000000 sqlmesh-0.6.3.dev5/web/client/src/library/components/button/Button.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.659236 sqlmesh-0.6.3.dev5/web/client/src/library/components/button/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3516 2023-03-27 01:55:02.000000 sqlmesh-0.6.3.dev5/web/client/src/library/components/button/tests/Button.spec.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.659439 sqlmesh-0.6.3.dev5/web/client/src/library/components/divider/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      856 2023-03-22 22:04:55.000000 sqlmesh-0.6.3.dev5/web/client/src/library/components/divider/Divider.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.659669 sqlmesh-0.6.3.dev5/web/client/src/library/components/divider/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      632 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/web/client/src/library/components/divider/tests/Divider.spec.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.661429 sqlmesh-0.6.3.dev5/web/client/src/library/components/editor/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1992 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/web/client/src/library/components/editor/Editor.css
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5699 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/web/client/src/library/components/editor/Editor.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8518 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/web/client/src/library/components/editor/EditorCode.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2718 2023-04-14 20:24:08.000000 sqlmesh-0.6.3.dev5/web/client/src/library/components/editor/EditorFooter.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1990 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/web/client/src/library/components/editor/EditorIndicator.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9819 2023-04-14 20:24:08.000000 sqlmesh-0.6.3.dev5/web/client/src/library/components/editor/EditorInspector.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)    11419 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/web/client/src/library/components/editor/EditorPreview.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3527 2023-04-27 18:23:33.000000 sqlmesh-0.6.3.dev5/web/client/src/library/components/editor/EditorTabs.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.661791 sqlmesh-0.6.3.dev5/web/client/src/library/components/editor/extensions/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5820 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/web/client/src/library/components/editor/extensions/SqlMeshDialect.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5744 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/web/client/src/library/components/editor/extensions/index.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1538 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/web/client/src/library/components/editor/help.ts
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.662509 sqlmesh-0.6.3.dev5/web/client/src/library/components/fileTree/
--rw-r--r--   0 eakmanrq   (501) staff       (20)    10852 2023-04-14 20:24:08.000000 sqlmesh-0.6.3.dev5/web/client/src/library/components/fileTree/Directory.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6045 2023-04-14 20:24:08.000000 sqlmesh-0.6.3.dev5/web/client/src/library/components/fileTree/File.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2997 2023-04-14 20:24:08.000000 sqlmesh-0.6.3.dev5/web/client/src/library/components/fileTree/FileTree.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)      562 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/web/client/src/library/components/fileTree/help.ts
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.662870 sqlmesh-0.6.3.dev5/web/client/src/library/components/graph/
--rw-r--r--   0 eakmanrq   (501) staff       (20)    15931 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/web/client/src/library/components/graph/Graph.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     7063 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/web/client/src/library/components/graph/help.ts
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.663342 sqlmesh-0.6.3.dev5/web/client/src/library/components/ide/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4342 2023-04-14 20:24:08.000000 sqlmesh-0.6.3.dev5/web/client/src/library/components/ide/ActivePlan.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4933 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/web/client/src/library/components/ide/IDE.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)    22356 2023-03-27 22:28:21.000000 sqlmesh-0.6.3.dev5/web/client/src/library/components/ide/RunPlan.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.664104 sqlmesh-0.6.3.dev5/web/client/src/library/components/input/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2087 2023-03-28 20:12:46.000000 sqlmesh-0.6.3.dev5/web/client/src/library/components/input/Input.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)      688 2023-03-22 22:04:55.000000 sqlmesh-0.6.3.dev5/web/client/src/library/components/input/InputToggle.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.664322 sqlmesh-0.6.3.dev5/web/client/src/library/components/loading/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      486 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/web/client/src/library/components/loading/Loading.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.664983 sqlmesh-0.6.3.dev5/web/client/src/library/components/logo/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2292 2023-03-22 22:04:55.000000 sqlmesh-0.6.3.dev5/web/client/src/library/components/logo/Spinner.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4637 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/web/client/src/library/components/logo/SqlMesh.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8042 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/web/client/src/library/components/logo/Tobiko.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.665604 sqlmesh-0.6.3.dev5/web/client/src/library/components/modal/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1560 2023-03-22 22:04:55.000000 sqlmesh-0.6.3.dev5/web/client/src/library/components/modal/Modal.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1953 2023-03-27 01:55:02.000000 sqlmesh-0.6.3.dev5/web/client/src/library/components/modal/ModalConfirmation.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1447 2023-03-27 01:55:02.000000 sqlmesh-0.6.3.dev5/web/client/src/library/components/modal/ModalDrawer.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.677255 sqlmesh-0.6.3.dev5/web/client/src/library/components/plan/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9269 2023-04-20 17:40:30.000000 sqlmesh-0.6.3.dev5/web/client/src/library/components/plan/Plan.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6775 2023-03-27 01:55:02.000000 sqlmesh-0.6.3.dev5/web/client/src/library/components/plan/PlanActions.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1312 2023-03-28 20:12:46.000000 sqlmesh-0.6.3.dev5/web/client/src/library/components/plan/PlanBackfillDates.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)    10448 2023-04-14 20:24:08.000000 sqlmesh-0.6.3.dev5/web/client/src/library/components/plan/PlanChangePreview.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4920 2023-04-20 17:40:30.000000 sqlmesh-0.6.3.dev5/web/client/src/library/components/plan/PlanHeader.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)    15855 2023-04-20 17:40:30.000000 sqlmesh-0.6.3.dev5/web/client/src/library/components/plan/PlanWizard.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9926 2023-03-27 22:28:21.000000 sqlmesh-0.6.3.dev5/web/client/src/library/components/plan/PlanWizardStepOptions.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)    12528 2023-04-20 17:40:30.000000 sqlmesh-0.6.3.dev5/web/client/src/library/components/plan/context.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3444 2023-03-27 01:55:02.000000 sqlmesh-0.6.3.dev5/web/client/src/library/components/plan/help.spec.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2155 2023-03-22 20:27:52.000000 sqlmesh-0.6.3.dev5/web/client/src/library/components/plan/help.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2599 2023-04-20 17:40:30.000000 sqlmesh-0.6.3.dev5/web/client/src/library/components/plan/hooks.ts
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.677390 sqlmesh-0.6.3.dev5/web/client/src/library/components/progress/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      713 2023-03-27 01:55:02.000000 sqlmesh-0.6.3.dev5/web/client/src/library/components/progress/Progress.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.677603 sqlmesh-0.6.3.dev5/web/client/src/library/components/report/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1047 2023-04-20 17:40:30.000000 sqlmesh-0.6.3.dev5/web/client/src/library/components/report/ReportTestsErrors.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.678173 sqlmesh-0.6.3.dev5/web/client/src/library/components/root/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      526 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/web/client/src/library/components/root/Footer.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1921 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/web/client/src/library/components/root/Header.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)      247 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/web/client/src/library/components/root/Main.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)      443 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/web/client/src/library/components/root/Root.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.678527 sqlmesh-0.6.3.dev5/web/client/src/library/components/splitPane/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      788 2023-03-22 22:04:55.000000 sqlmesh-0.6.3.dev5/web/client/src/library/components/splitPane/SplitPane.css
--rw-r--r--   0 eakmanrq   (501) staff       (20)      541 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/web/client/src/library/components/splitPane/SplitPane.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.678739 sqlmesh-0.6.3.dev5/web/client/src/library/components/tasksOverview/
--rw-r--r--   0 eakmanrq   (501) staff       (20)    11713 2023-04-14 20:24:08.000000 sqlmesh-0.6.3.dev5/web/client/src/library/components/tasksOverview/TasksOverview.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.678998 sqlmesh-0.6.3.dev5/web/client/src/library/components/toggle/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1453 2023-03-27 01:55:02.000000 sqlmesh-0.6.3.dev5/web/client/src/library/components/toggle/Toggle.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1197 2023-03-27 01:55:02.000000 sqlmesh-0.6.3.dev5/web/client/src/main.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.680581 sqlmesh-0.6.3.dev5/web/client/src/models/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1647 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/web/client/src/models/artifact.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3472 2023-04-06 22:49:28.000000 sqlmesh-0.6.3.dev5/web/client/src/models/directory.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4190 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/web/client/src/models/environment.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2190 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/web/client/src/models/file.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)      173 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/web/client/src/models/index.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)      766 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/web/client/src/models/initial.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)      200 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/web/client/src/routes.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.681028 sqlmesh-0.6.3.dev5/web/client/src/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)       35 2023-01-20 19:02:18.000000 sqlmesh-0.6.3.dev5/web/client/src/tests/setup.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)      541 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/web/client/src/tests/utils.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.681410 sqlmesh-0.6.3.dev5/web/client/src/types/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      467 2023-03-22 22:04:55.000000 sqlmesh-0.6.3.dev5/web/client/src/types/enum.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)      137 2023-03-22 22:04:55.000000 sqlmesh-0.6.3.dev5/web/client/src/types/index.d.ts
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.681878 sqlmesh-0.6.3.dev5/web/client/src/utils/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4102 2023-03-27 01:55:02.000000 sqlmesh-0.6.3.dev5/web/client/src/utils/index.spec.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5245 2023-04-14 20:24:08.000000 sqlmesh-0.6.3.dev5/web/client/src/utils/index.ts
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.682078 sqlmesh-0.6.3.dev5/web/client/src/workers/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      113 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/web/client/src/workers/index.ts
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.682494 sqlmesh-0.6.3.dev5/web/client/src/workers/sqlglot/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1105 2023-04-14 20:24:08.000000 sqlmesh-0.6.3.dev5/web/client/src/workers/sqlglot/sqlglot.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1578 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/web/client/src/workers/sqlglot/worker.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5879 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/web/client/tailwind.config.js
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.682705 sqlmesh-0.6.3.dev5/web/client/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      170 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/web/client/tests/initial.spec.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1141 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/web/client/tsconfig.json
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1297 2023-04-17 00:43:26.000000 sqlmesh-0.6.3.dev5/web/client/vite.config.ts
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.684531 sqlmesh-0.6.3.dev5/web/server/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-20 19:02:18.000000 sqlmesh-0.6.3.dev5/web/server/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.684709 sqlmesh-0.6.3.dev5/web/server/api/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev5/web/server/api/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 21:19:52.686464 sqlmesh-0.6.3.dev5/web/server/api/endpoints/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      784 2023-04-14 20:24:08.000000 sqlmesh-0.6.3.dev5/web/server/api/endpoints/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4564 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/web/server/api/endpoints/commands.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      819 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/web/server/api/endpoints/context.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1858 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/web/server/api/endpoints/directories.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      721 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev5/web/server/api/endpoints/environments.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      637 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/web/server/api/endpoints/events.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5383 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/web/server/api/endpoints/files.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3283 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/web/server/api/endpoints/lineage.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      962 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/web/server/api/endpoints/models.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3635 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/web/server/api/endpoints/plan.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3775 2023-04-20 17:40:30.000000 sqlmesh-0.6.3.dev5/web/server/console.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1534 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/web/server/main.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5777 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev5/web/server/models.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      260 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev5/web/server/openapi.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2421 2023-04-27 17:30:24.000000 sqlmesh-0.6.3.dev5/web/server/settings.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2114 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev5/web/server/sse.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2461 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev5/web/server/utils.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      790 2023-04-27 21:05:04.000000 sqlmesh-0.6.3.dev5/web/server/watcher.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.990806 sqlmesh-0.6.4/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.886803 sqlmesh-0.6.4/.circleci/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1872 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/.circleci/config.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4414 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/.circleci/continue_config.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       66 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/.dockerignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2152 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/.gitignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1900 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/.pre-commit-config.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      234 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/.readthedocs.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      135 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/Dockerfile.api
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      383 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/Dockerfile.app
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11346 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1855 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/Makefile
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1936 2023-05-01 23:49:56.990806 sqlmesh-0.6.4/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1192 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1008 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docker-compose.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.890804 sqlmesh-0.6.4/docs/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.866803 sqlmesh-0.6.4/docs/_readthedocs/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.890804 sqlmesh-0.6.4/docs/_readthedocs/html/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/_readthedocs/html/.keep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9965 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/comparisons.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.890804 sqlmesh-0.6.4/docs/concepts/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.890804 sqlmesh-0.6.4/docs/concepts/architecture/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1334 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/concepts/architecture/serialization.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1113 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/concepts/architecture/snapshots.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6689 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/concepts/audits.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3866 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/concepts/environments.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5952 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/concepts/glossary.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/concepts/hooks.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3027 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/concepts/macros.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.890804 sqlmesh-0.6.4/docs/concepts/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9934 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/concepts/models/model_kinds.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8189 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/concepts/models/overview.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7171 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/concepts/models/python_models.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4938 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/concepts/models/seed_models.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5356 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/concepts/models/sql_models.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6637 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/concepts/overview.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.894804 sqlmesh-0.6.4/docs/concepts/plans/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    43124 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/concepts/plans/model_versioning.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9954 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/concepts/plans.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5699 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/concepts/tests.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      607 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/development.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.894804 sqlmesh-0.6.4/docs/guides/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1943 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/guides/connections.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1309 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/guides/migrations.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10756 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/guides/models.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6133 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/guides/multi_repo.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2142 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/guides/projects.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.894804 sqlmesh-0.6.4/docs/guides/scheduling/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   740917 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/guides/scheduling/airflow_successful_plan_apply.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   379880 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/guides/scheduling/airflow_successful_setup.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5648 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/guides/scheduling.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1854 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/guides/testing.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5459 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/index.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      297 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/installation.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.894804 sqlmesh-0.6.4/docs/integrations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2905 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/integrations/airflow.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7801 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/integrations/dbt.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24057 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/integrations/engines.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      867 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/integrations/github.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      217 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/integrations/overview.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      665 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/prerequisites.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12925 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/quick_start.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.894804 sqlmesh-0.6.4/docs/reference/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6093 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/reference/cli.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13607 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/reference/configuration.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4579 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/reference/notebook.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1127 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/reference/overview.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       14 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/reference/python.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/release_notes.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      122 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/requirements.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3249 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/sqlmesh.png
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.898804 sqlmesh-0.6.4/examples/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.898804 sqlmesh-0.6.4/examples/airflow/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1713 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/airflow/Dockerfile.template
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2164 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/airflow/Makefile
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      942 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/airflow/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/airflow/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.898804 sqlmesh-0.6.4/examples/airflow/dags/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      263 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/airflow/dags/sqlmesh_integration.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3515 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/airflow/docker_compose_decorator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/airflow/requirements.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.898804 sqlmesh-0.6.4/examples/airflow/spark_conf/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      872 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/airflow/spark_conf/hive-site.xml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      151 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/airflow/spark_conf/spark-defaults.conf
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.866803 sqlmesh-0.6.4/examples/multi/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.898804 sqlmesh-0.6.4/examples/multi/repo_1/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.898804 sqlmesh-0.6.4/examples/multi/repo_1/audits/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/multi/repo_1/audits/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      147 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/multi/repo_1/config.yaml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.898804 sqlmesh-0.6.4/examples/multi/repo_1/macros/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/multi/repo_1/macros/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/multi/repo_1/macros/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.898804 sqlmesh-0.6.4/examples/multi/repo_1/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/multi/repo_1/models/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       63 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/multi/repo_1/models/a.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/multi/repo_1/models/b.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.898804 sqlmesh-0.6.4/examples/multi/repo_1/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/multi/repo_1/tests/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.898804 sqlmesh-0.6.4/examples/multi/repo_2/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.898804 sqlmesh-0.6.4/examples/multi/repo_2/audits/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/multi/repo_2/audits/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      147 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/multi/repo_2/config.yaml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.898804 sqlmesh-0.6.4/examples/multi/repo_2/macros/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/multi/repo_2/macros/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/multi/repo_2/macros/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.898804 sqlmesh-0.6.4/examples/multi/repo_2/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/multi/repo_2/models/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       64 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/multi/repo_2/models/c.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/multi/repo_2/models/d.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.898804 sqlmesh-0.6.4/examples/multi/repo_2/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/multi/repo_2/tests/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.902804 sqlmesh-0.6.4/examples/sushi/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.902804 sqlmesh-0.6.4/examples/sushi/audits/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      105 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi/audits/items.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      119 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi/audits/order_items.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      829 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi/config.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.902804 sqlmesh-0.6.4/examples/sushi/data/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi/data/.keep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      551 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi/helper.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.902804 sqlmesh-0.6.4/examples/sushi/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi/hooks/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      247 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi/hooks/hooks.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.902804 sqlmesh-0.6.4/examples/sushi/macros/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi/macros/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      702 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi/macros/macros.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.902804 sqlmesh-0.6.4/examples/sushi/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      934 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi/models/customer_revenue_by_day.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      223 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi/models/customers.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1911 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi/models/items.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1912 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi/models/order_items.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1643 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi/models/orders.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      346 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi/models/top_waiters.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      465 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi/models/waiter_as_customer_by_day.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      123 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi/models/waiter_names.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      691 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi/models/waiter_revenue_by_day.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      197 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi/models/waiters.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.902804 sqlmesh-0.6.4/examples/sushi/seeds/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       88 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi/seeds/waiter_names.csv
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.902804 sqlmesh-0.6.4/examples/sushi/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1459 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi/tests/test_customer_revenue_by_day.yaml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.906804 sqlmesh-0.6.4/examples/sushi_dbt/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       15 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/.gitignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       41 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/.user.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.906804 sqlmesh-0.6.4/examples/sushi_dbt/analyses/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/analyses/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      291 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      507 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/dbt_project.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.906804 sqlmesh-0.6.4/examples/sushi_dbt/macros/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      941 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/macros/incremental.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/macros/log_value.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.906804 sqlmesh-0.6.4/examples/sushi_dbt/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1125 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/models/customer_revenue_by_day.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/models/customers.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      182 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/models/schema.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      309 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/models/top_waiters.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      389 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/models/waiter_as_customer_by_day.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      752 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/models/waiter_revenue_by_day.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      186 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/models/waiters.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.870803 sqlmesh-0.6.4/examples/sushi_dbt/packages/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.906804 sqlmesh-0.6.4/examples/sushi_dbt/packages/customers/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.906804 sqlmesh-0.6.4/examples/sushi_dbt/packages/customers/analyses/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/packages/customers/analyses/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      663 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/packages/customers/dbt_project.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.906804 sqlmesh-0.6.4/examples/sushi_dbt/packages/customers/macros/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      117 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/packages/customers/macros/current_engine.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       65 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/packages/customers/macros/distinct.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.906804 sqlmesh-0.6.4/examples/sushi_dbt/packages/customers/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/packages/customers/models/schema.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.906804 sqlmesh-0.6.4/examples/sushi_dbt/packages/customers/seeds/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/packages/customers/seeds/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.906804 sqlmesh-0.6.4/examples/sushi_dbt/packages/customers/snapshots/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/packages/customers/snapshots/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.906804 sqlmesh-0.6.4/examples/sushi_dbt/packages/customers/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/packages/customers/tests/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1092 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/profiles.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.906804 sqlmesh-0.6.4/examples/sushi_dbt/seeds/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2327 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/seeds/items.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10472 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/seeds/order_items.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9746 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/seeds/orders.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       97 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/seeds/properties.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       88 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/seeds/waiter_names.csv
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.906804 sqlmesh-0.6.4/examples/sushi_dbt/snapshots/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/snapshots/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.906804 sqlmesh-0.6.4/examples/sushi_dbt/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/tests/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.910804 sqlmesh-0.6.4/examples/wursthall/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/wursthall/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.870803 sqlmesh-0.6.4/examples/wursthall/audits/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.910804 sqlmesh-0.6.4/examples/wursthall/audits/db/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      141 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/wursthall/audits/db/order_f.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       66 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/wursthall/config.yaml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.910804 sqlmesh-0.6.4/examples/wursthall/macros/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/wursthall/macros/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      618 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/wursthall/macros/macros.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.910804 sqlmesh-0.6.4/examples/wursthall/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/wursthall/models/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.910804 sqlmesh-0.6.4/examples/wursthall/models/db/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      433 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/wursthall/models/db/customer_d.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      256 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/wursthall/models/db/item_d.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3158 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/wursthall/models/db/order_f.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      542 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/wursthall/models/db/order_item_f.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.910804 sqlmesh-0.6.4/examples/wursthall/models/src/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/wursthall/models/src/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1652 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/wursthall/models/src/customer_details.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      120 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/wursthall/models/src/menu_item_details.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3414 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/wursthall/models/src/order_item_details.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      892 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/wursthall/models/src/shared.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.870803 sqlmesh-0.6.4/examples/wursthall/seeds/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.910804 sqlmesh-0.6.4/examples/wursthall/seeds/src/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7416 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/wursthall/seeds/src/menu_item_details.csv
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.910804 sqlmesh-0.6.4/examples/wursthall/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      888 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/wursthall/tests/test_customer_d.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      955 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/wursthall/tests/test_order_item_f.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2113 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/mkdocs.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.910804 sqlmesh-0.6.4/pdoc/
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     1153 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/pdoc/cli.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.910804 sqlmesh-0.6.4/pdoc/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      131 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/pdoc/templates/module.html.jinja2
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.910804 sqlmesh-0.6.4/posts/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.914804 sqlmesh-0.6.4/posts/virtual_data_environments/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   318753 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/posts/virtual_data_environments/change_categorization.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   274526 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/posts/virtual_data_environments/isolated_rigid_envs.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   163619 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/posts/virtual_data_environments/partial_breaking.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   298971 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/posts/virtual_data_environments/stateful_envs.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   366545 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/posts/virtual_data_environments/virtual_envs.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)  1344487 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/posts/virtual_data_environments/virtual_envs_end_to_end.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18638 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/posts/virtual_data_environments.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      734 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/pytest.ini
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1393 2023-05-01 23:49:56.990806 sqlmesh-0.6.4/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3164 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.918805 sqlmesh-0.6.4/sqlmesh/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        3 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/.airflowignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3950 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      160 2023-05-01 23:49:56.000000 sqlmesh-0.6.4/sqlmesh/_version.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.918805 sqlmesh-0.6.4/sqlmesh/cli/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      898 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/cli/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4742 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/cli/example_project.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9930 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/cli/main.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1433 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/cli/options.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.922804 sqlmesh-0.6.4/sqlmesh/core/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      586 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/_typing.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.922804 sqlmesh-0.6.4/sqlmesh/core/audit/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      449 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/audit/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1071 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/audit/builtin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8136 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/audit/definition.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.926805 sqlmesh-0.6.4/sqlmesh/core/config/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      668 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/config/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4412 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/config/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1001 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/config/categorizer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      940 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/config/common.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21184 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/config/connection.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3351 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/config/loader.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1655 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/config/model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5611 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/config/root.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8421 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/config/scheduler.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    31743 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/console.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      826 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    36329 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/context.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8904 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/context_diff.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17484 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/dialect.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.926805 sqlmesh-0.6.4/sqlmesh/core/engine_adapter/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2626 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/engine_adapter/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      762 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/engine_adapter/_typing.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    29549 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/engine_adapter/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4191 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/engine_adapter/base_postgres.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4238 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/engine_adapter/base_spark.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15681 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/engine_adapter/bigquery.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      402 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/engine_adapter/databricks.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1939 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/engine_adapter/databricks_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1971 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/engine_adapter/duckdb.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2149 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/engine_adapter/postgres.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6673 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/engine_adapter/redshift.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1181 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/engine_adapter/shared.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2658 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/engine_adapter/snowflake.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4879 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/engine_adapter/spark.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1849 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/environment.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      742 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/hooks.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12673 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/loader.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19726 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/macros.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.930805 sqlmesh-0.6.4/sqlmesh/core/model/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      594 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/model/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1746 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/model/cache.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1300 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/model/common.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2417 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/model/decorator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    47510 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/model/definition.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8168 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/model/kind.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13069 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/model/meta.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2017 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/model/seed.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2314 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/notification_target.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.930805 sqlmesh-0.6.4/sqlmesh/core/plan/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      191 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/plan/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23956 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/plan/definition.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8565 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/plan/evaluator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12623 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/renderer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15386 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/scheduler.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20418 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/schema_diff.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.930805 sqlmesh-0.6.4/sqlmesh/core/snapshot/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      527 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/snapshot/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1990 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/snapshot/categorizer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    34694 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/snapshot/definition.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19245 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/snapshot/evaluator.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.930805 sqlmesh-0.6.4/sqlmesh/core/state_sync/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      692 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/state_sync/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13382 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/state_sync/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14349 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/state_sync/common.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20765 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/state_sync/engine_adapter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10834 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1412 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/user.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.934805 sqlmesh-0.6.4/sqlmesh/dbt/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       79 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/dbt/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9390 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/dbt/adapter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17485 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/dbt/basemodel.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11231 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/dbt/builtin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1762 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/dbt/column.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4978 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/dbt/common.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5087 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/dbt/context.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8044 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/dbt/loader.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9851 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/dbt/model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13257 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/dbt/package.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3701 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/dbt/profile.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4772 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/dbt/project.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      927 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/dbt/seed.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3137 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/dbt/source.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13618 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/dbt/target.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      291 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/dbt/util.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.934805 sqlmesh-0.6.4/sqlmesh/engines/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/engines/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4437 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/engines/commands.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.934805 sqlmesh-0.6.4/sqlmesh/engines/spark/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/engines/spark/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3414 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/engines/spark/app.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.934805 sqlmesh-0.6.4/sqlmesh/engines/spark/db_api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/engines/spark/db_api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      148 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/engines/spark/db_api/errors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2571 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/engines/spark/db_api/spark_session.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.934805 sqlmesh-0.6.4/sqlmesh/integrations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/integrations/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.934805 sqlmesh-0.6.4/sqlmesh/integrations/github/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/integrations/github/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2210 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/integrations/github/notification_operator_provider.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1726 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/integrations/github/notification_target.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1829 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/integrations/github/shared.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13960 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/magics.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.938805 sqlmesh-0.6.4/sqlmesh/migrations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/migrations/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1749 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/migrations/v0001_init.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      103 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/migrations/v0002_remove_identify.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1183 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/migrations/v0003_move_batch_size.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      534 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/migrations/v0004_environmnent_add_finalized_at.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/py.typed
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.938805 sqlmesh-0.6.4/sqlmesh/schedulers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/schedulers/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.938805 sqlmesh-0.6.4/sqlmesh/schedulers/airflow/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/schedulers/airflow/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4020 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/schedulers/airflow/api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8128 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/schedulers/airflow/client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3888 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/schedulers/airflow/common.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19132 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/schedulers/airflow/dag_generator.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.938805 sqlmesh-0.6.4/sqlmesh/schedulers/airflow/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/schedulers/airflow/hooks/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2132 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/schedulers/airflow/hooks/bigquery.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      868 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/schedulers/airflow/hooks/redshift.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8508 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/schedulers/airflow/integration.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.942805 sqlmesh-0.6.4/sqlmesh/schedulers/airflow/operators/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/schedulers/airflow/operators/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1444 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/schedulers/airflow/operators/bigquery.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6307 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/schedulers/airflow/operators/databricks.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2549 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/schedulers/airflow/operators/hwm_sensor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      877 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/schedulers/airflow/operators/notification.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1322 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/schedulers/airflow/operators/postgres.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1211 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/schedulers/airflow/operators/redshift.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1340 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/schedulers/airflow/operators/snowflake.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5222 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/schedulers/airflow/operators/spark_submit.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11104 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/schedulers/airflow/operators/targets.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4660 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/schedulers/airflow/plan.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1292 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/schedulers/airflow/plugin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4139 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/schedulers/airflow/state_sync.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5213 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/schedulers/airflow/util.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.942805 sqlmesh-0.6.4/sqlmesh/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4386 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3593 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/utils/cache.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8053 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/utils/concurrency.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7530 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/utils/connection_pool.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      410 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/utils/conversions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4329 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/utils/dag.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7549 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/utils/date.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1244 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/utils/errors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16133 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/utils/jinja.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15093 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/utils/metaprogramming.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      888 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/utils/pandas.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1609 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/utils/pydantic.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1534 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/utils/rich.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6487 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/utils/transactional_file.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1419 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/utils/yaml.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.918805 sqlmesh-0.6.4/sqlmesh.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1936 2023-05-01 23:49:56.000000 sqlmesh-0.6.4/sqlmesh.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21986 2023-05-01 23:49:56.000000 sqlmesh-0.6.4/sqlmesh.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-01 23:49:56.000000 sqlmesh-0.6.4/sqlmesh.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      141 2023-05-01 23:49:56.000000 sqlmesh-0.6.4/sqlmesh.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      844 2023-05-01 23:49:56.000000 sqlmesh-0.6.4/sqlmesh.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2023-05-01 23:49:56.000000 sqlmesh-0.6.4/sqlmesh.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21020 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh.svg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.942805 sqlmesh-0.6.4/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      285 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/common_fixtures.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4037 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/conftest.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.946805 sqlmesh-0.6.4/tests/core/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.946805 sqlmesh-0.6.4/tests/core/engine_adapter/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/engine_adapter/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    28133 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/engine_adapter/test_base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2114 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/engine_adapter/test_base_postgres.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1270 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/engine_adapter/test_base_spark.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7171 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/engine_adapter/test_bigquery.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1253 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/engine_adapter/test_databricks.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2613 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/engine_adapter/test_duckdb.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1569 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/engine_adapter/test_postgres.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8036 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/engine_adapter/test_redshift.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3191 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/engine_adapter/test_spark.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7073 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/test_audit.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6611 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/test_config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      850 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/test_connection_config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10197 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/test_context.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2749 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/test_dialect.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      464 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/test_environment.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    26773 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/test_integration.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6500 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/test_macros.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25378 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/test_model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17081 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/test_plan.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3890 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/test_plan_evaluator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4647 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/test_scheduler.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    32235 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/test_schema_diff.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      857 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/test_seed.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    29629 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/test_snapshot.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10299 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/test_snapshot_evaluator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24610 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/test_state_sync.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.950805 sqlmesh-0.6.4/tests/dbt/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/dbt/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      739 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/dbt/conftest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2537 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/dbt/test_adapter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13195 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/dbt/test_config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17095 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/dbt/test_transformation.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.950805 sqlmesh-0.6.4/tests/engines/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/engines/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.950805 sqlmesh-0.6.4/tests/engines/spark/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/engines/spark/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      357 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/engines/spark/conftest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1503 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/engines/spark/test_db_api.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.878803 sqlmesh-0.6.4/tests/fixtures/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.874803 sqlmesh-0.6.4/tests/fixtures/dbt/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.950805 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.950805 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/analyses/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/analyses/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      291 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/config.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.878803 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/dbt_packages/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1055 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/dbt_project.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.950805 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/logs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10264 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/logs/dbt.log.legacy
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.950805 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/macros/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      941 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/macros/incremental.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/macros/log_value.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.950805 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      247 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/models/schema.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      334 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/models/top_waiters.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      389 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/models/waiter_as_customer_by_day.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      863 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/models/waiter_revenue_by_day.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      196 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/models/waiters.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.878803 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/packages/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.950805 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/packages/customers/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.950805 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/packages/customers/analyses/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/packages/customers/analyses/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      663 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/packages/customers/dbt_project.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.950805 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/packages/customers/macros/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      117 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/packages/customers/macros/current_engine.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       65 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/packages/customers/macros/distinct.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.954805 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/packages/customers/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1155 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/packages/customers/models/customer_revenue_by_day.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      108 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/packages/customers/models/customers.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      193 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/packages/customers/models/schema.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.954805 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/packages/customers/seeds/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/packages/customers/seeds/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.954805 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/packages/customers/snapshots/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/packages/customers/snapshots/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.954805 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/packages/customers/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/packages/customers/tests/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       41 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/packages.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      540 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/profiles.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1250 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/seed_sources.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.954805 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/seeds/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       42 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/seeds/properties.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       88 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/seeds/waiter_names.csv
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.954805 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/snapshots/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/snapshots/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.954805 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/source_data/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2327 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/source_data/items.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10472 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/source_data/order_items.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9746 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/source_data/orders.csv
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.954805 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/tests/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.954805 sqlmesh-0.6.4/tests/fixtures/migrations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9823 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/migrations/environments.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25229 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/migrations/snapshots.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.954805 sqlmesh-0.6.4/tests/integrations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/integrations/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.954805 sqlmesh-0.6.4/tests/integrations/github/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/integrations/github/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.954805 sqlmesh-0.6.4/tests/integrations/github/fixtures/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      816 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/integrations/github/fixtures/pull_request_review.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      477 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/integrations/github/test_notification_target.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.954805 sqlmesh-0.6.4/tests/schedulers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/schedulers/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.954805 sqlmesh-0.6.4/tests/schedulers/airflow/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/schedulers/airflow/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1414 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/schedulers/airflow/conftest.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.958806 sqlmesh-0.6.4/tests/schedulers/airflow/operators/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/schedulers/airflow/operators/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4442 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/schedulers/airflow/operators/test_hwm_sensor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4392 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/schedulers/airflow/operators/test_targets.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9920 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/schedulers/airflow/test_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1345 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/schedulers/airflow/test_end_to_end.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6222 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/schedulers/airflow/test_integration.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6054 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/schedulers/airflow/test_plan.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.958806 sqlmesh-0.6.4/tests/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1118 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/utils/test_cache.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3580 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/utils/test_concurrency.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6430 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/utils/test_connection_pool.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1381 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/utils/test_dag.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1818 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/utils/test_date.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      551 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/utils/test_filesystem.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5516 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/utils/test_jinja.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5790 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/utils/test_metaprogramming.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2501 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/utils/test_pandas.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      518 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/utils/test_pydantic.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2911 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/utils/test_transactional_file.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1194 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/utils/test_yaml.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.958806 sqlmesh-0.6.4/tests/web/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/web/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16232 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/web/test_main.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.958806 sqlmesh-0.6.4/web/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.962806 sqlmesh-0.6.4/web/client/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1104 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/.eslintrc.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       94 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/.gitignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      129 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/.prettierignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      403 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/.prettierrc.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.962806 sqlmesh-0.6.4/web/client/dist/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.966806 sqlmesh-0.6.4/web/client/dist/assets/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    74500 2023-05-01 23:49:40.000000 sqlmesh-0.6.4/web/client/dist/assets/CircularStd-Black-52659624.otf
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    74368 2023-05-01 23:49:40.000000 sqlmesh-0.6.4/web/client/dist/assets/CircularStd-Bold-0e6c076d.otf
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    74116 2023-05-01 23:49:40.000000 sqlmesh-0.6.4/web/client/dist/assets/CircularStd-Medium-2f373e53.otf
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24788 2023-05-01 23:49:40.000000 sqlmesh-0.6.4/web/client/dist/assets/Plan-683a0552.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    55004 2023-05-01 23:49:40.000000 sqlmesh-0.6.4/web/client/dist/assets/Publico-Black-e6bd2ea2.otf
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    57104 2023-05-01 23:49:40.000000 sqlmesh-0.6.4/web/client/dist/assets/Publico-Bold-c79acd56.otf
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    56836 2023-05-01 23:49:40.000000 sqlmesh-0.6.4/web/client/dist/assets/Publico-Medium-01b4a891.otf
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    43132 2023-05-01 23:49:40.000000 sqlmesh-0.6.4/web/client/dist/assets/index-b61dbb6f.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)  2636063 2023-05-01 23:49:40.000000 sqlmesh-0.6.4/web/client/dist/assets/index-f2c4b7c5.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2419 2023-05-01 23:49:40.000000 sqlmesh-0.6.4/web/client/dist/assets/worker-e891d118.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.966806 sqlmesh-0.6.4/web/client/dist/favicons/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2473 2023-05-01 23:49:37.000000 sqlmesh-0.6.4/web/client/dist/favicons/favicon.ico
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1150 2023-05-01 23:49:40.000000 sqlmesh-0.6.4/web/client/dist/index.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1076 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/index.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    37689 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/openapi.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      330 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/orval.config.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   408504 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/package-lock.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2389 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/package.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1642 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/playwright.config.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       82 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/postcss.config.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.882803 sqlmesh-0.6.4/web/client/public/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.966806 sqlmesh-0.6.4/web/client/public/favicons/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2473 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/public/favicons/favicon.ico
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.966806 sqlmesh-0.6.4/web/client/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.966806 sqlmesh-0.6.4/web/client/src/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1236 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/api/channels.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5243 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/api/index.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3247 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/api/instance.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.882803 sqlmesh-0.6.4/web/client/src/assets/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.882803 sqlmesh-0.6.4/web/client/src/assets/fonts/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.970806 sqlmesh-0.6.4/web/client/src/assets/fonts/Circular STD/
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    74500 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/assets/fonts/Circular STD/CircularStd-Black.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    74524 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/assets/fonts/Circular STD/CircularStd-BlackItalic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    74368 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/assets/fonts/Circular STD/CircularStd-Bold.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    73964 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/assets/fonts/Circular STD/CircularStd-BoldItalic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    68940 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/assets/fonts/Circular STD/CircularStd-Book.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    67284 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/assets/fonts/Circular STD/CircularStd-BookItalic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    74116 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/assets/fonts/Circular STD/CircularStd-Medium.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    73916 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/assets/fonts/Circular STD/CircularStd-MediumItalic.otf
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.974806 sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    55004 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/Publico-Black.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    56384 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/Publico-BlackItalic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    57104 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/Publico-Bold.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    62320 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/Publico-BoldItalic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    56652 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/Publico-Extrabold.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    61688 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/Publico-ExtraboldItalic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    57680 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/Publico-Italic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    53148 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/Publico-Light.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    57060 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/Publico-LightItalic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    56836 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/Publico-Medium.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    61460 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/Publico-MediumItalic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    52820 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/Publico-Roman.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    59176 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/PublicoText-Bold.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    63876 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/PublicoText-BoldItalic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    60768 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/PublicoText-Italic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    81732 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/PublicoText-Roman.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    60992 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/PublicoText-Semibold.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    64792 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/PublicoText-SemiboldItalic.otf
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.974806 sqlmesh-0.6.4/web/client/src/context/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4126 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/context/context.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6470 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/context/editor.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      923 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/context/fileTree.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2187 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/context/lineage.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2661 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/context/plan.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1562 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/context/theme.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.974806 sqlmesh-0.6.4/web/client/src/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      308 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/hooks/useActiveFocus.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      817 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/hooks/useLocalStorage.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9555 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/index.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.882803 sqlmesh-0.6.4/web/client/src/library/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.886803 sqlmesh-0.6.4/web/client/src/library/components/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.974806 sqlmesh-0.6.4/web/client/src/library/components/banner/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1705 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/banner/Banner.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.974806 sqlmesh-0.6.4/web/client/src/library/components/button/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4517 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/button/Button.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.974806 sqlmesh-0.6.4/web/client/src/library/components/button/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3516 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/button/tests/Button.spec.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.974806 sqlmesh-0.6.4/web/client/src/library/components/divider/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      856 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/divider/Divider.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.974806 sqlmesh-0.6.4/web/client/src/library/components/divider/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      632 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/divider/tests/Divider.spec.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.978806 sqlmesh-0.6.4/web/client/src/library/components/editor/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1992 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/editor/Editor.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5764 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/editor/Editor.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8518 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/editor/EditorCode.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2718 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/editor/EditorFooter.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1990 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/editor/EditorIndicator.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9819 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/editor/EditorInspector.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11905 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/editor/EditorPreview.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3527 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/editor/EditorTabs.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.978806 sqlmesh-0.6.4/web/client/src/library/components/editor/extensions/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5820 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/editor/extensions/SqlMeshDialect.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5744 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/editor/extensions/index.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1538 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/editor/help.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.978806 sqlmesh-0.6.4/web/client/src/library/components/fileTree/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10852 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/fileTree/Directory.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6045 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/fileTree/File.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2997 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/fileTree/FileTree.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      562 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/fileTree/help.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.978806 sqlmesh-0.6.4/web/client/src/library/components/graph/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      159 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/graph/Graph.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14454 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/graph/Graph.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7679 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/graph/help.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.978806 sqlmesh-0.6.4/web/client/src/library/components/ide/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4342 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/ide/ActivePlan.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4933 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/ide/IDE.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22356 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/ide/RunPlan.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.978806 sqlmesh-0.6.4/web/client/src/library/components/input/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2087 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/input/Input.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      688 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/input/InputToggle.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.978806 sqlmesh-0.6.4/web/client/src/library/components/loading/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      486 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/loading/Loading.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.978806 sqlmesh-0.6.4/web/client/src/library/components/logo/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2292 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/logo/Spinner.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4637 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/logo/SqlMesh.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8042 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/logo/Tobiko.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.978806 sqlmesh-0.6.4/web/client/src/library/components/modal/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1560 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/modal/Modal.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1953 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/modal/ModalConfirmation.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1447 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/modal/ModalDrawer.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.982806 sqlmesh-0.6.4/web/client/src/library/components/plan/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9269 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/plan/Plan.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6775 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/plan/PlanActions.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1312 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/plan/PlanBackfillDates.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10448 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/plan/PlanChangePreview.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4920 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/plan/PlanHeader.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15855 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/plan/PlanWizard.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9926 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/plan/PlanWizardStepOptions.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12528 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/plan/context.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3444 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/plan/help.spec.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2155 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/plan/help.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2599 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/plan/hooks.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.982806 sqlmesh-0.6.4/web/client/src/library/components/progress/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      713 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/progress/Progress.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.982806 sqlmesh-0.6.4/web/client/src/library/components/report/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1047 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/report/ReportTestsErrors.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.982806 sqlmesh-0.6.4/web/client/src/library/components/root/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      526 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/root/Footer.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1921 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/root/Header.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      247 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/root/Main.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      443 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/root/Root.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.982806 sqlmesh-0.6.4/web/client/src/library/components/splitPane/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      788 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/splitPane/SplitPane.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      541 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/splitPane/SplitPane.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.982806 sqlmesh-0.6.4/web/client/src/library/components/tasksOverview/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11713 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/tasksOverview/TasksOverview.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.982806 sqlmesh-0.6.4/web/client/src/library/components/toggle/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1453 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/toggle/Toggle.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1197 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/main.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.982806 sqlmesh-0.6.4/web/client/src/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1647 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/models/artifact.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3472 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/models/directory.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4190 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/models/environment.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2190 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/models/file.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      173 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/models/index.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      766 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/models/initial.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      200 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/routes.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.986806 sqlmesh-0.6.4/web/client/src/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       35 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/tests/setup.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      541 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/tests/utils.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.986806 sqlmesh-0.6.4/web/client/src/types/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      467 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/types/enum.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      137 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/types/index.d.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.986806 sqlmesh-0.6.4/web/client/src/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4102 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/utils/index.spec.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5413 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/utils/index.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.986806 sqlmesh-0.6.4/web/client/src/workers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      113 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/workers/index.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.986806 sqlmesh-0.6.4/web/client/src/workers/sqlglot/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1105 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/workers/sqlglot/sqlglot.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1578 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/workers/sqlglot/worker.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5879 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/tailwind.config.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.986806 sqlmesh-0.6.4/web/client/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      170 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/tests/initial.spec.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1141 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/tsconfig.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1297 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/vite.config.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.986806 sqlmesh-0.6.4/web/server/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/server/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.986806 sqlmesh-0.6.4/web/server/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/server/api/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.990806 sqlmesh-0.6.4/web/server/api/endpoints/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      784 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/server/api/endpoints/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4564 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/server/api/endpoints/commands.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      819 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/server/api/endpoints/context.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1858 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/server/api/endpoints/directories.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      721 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/server/api/endpoints/environments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      637 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/server/api/endpoints/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5383 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/server/api/endpoints/files.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3283 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/server/api/endpoints/lineage.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      962 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/server/api/endpoints/models.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3635 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/server/api/endpoints/plan.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3775 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/server/console.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1534 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/server/main.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5777 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/server/models.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      260 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/server/openapi.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2421 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/server/settings.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2114 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/server/sse.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2461 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/server/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      790 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/server/watcher.py
```

### Comparing `sqlmesh-0.6.3.dev5/.circleci/config.yml` & `sqlmesh-0.6.4/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/.circleci/continue_config.yml` & `sqlmesh-0.6.4/.circleci/continue_config.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/.gitignore` & `sqlmesh-0.6.4/.gitignore`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/.pre-commit-config.yaml` & `sqlmesh-0.6.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/LICENSE` & `sqlmesh-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/Makefile` & `sqlmesh-0.6.4/Makefile`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 core-it-test:
 	pytest -m "core_integration"
 
 it-test: core-it-test airflow-it-test-with-env
 
 it-test-docker: core-it-test airflow-it-test-docker-with-env
 
-test: unit-test it-test doc-test
+test: unit-test doc-test it-test
 
 package:
 	pip3 install wheel && python3 setup.py sdist bdist_wheel
 
 publish: package
 	pip3 install twine && python3 -m twine upload dist/*
```

### Comparing `sqlmesh-0.6.3.dev5/PKG-INFO` & `sqlmesh-0.6.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,14 @@
 Metadata-Version: 2.1
 Name: sqlmesh
-Version: 0.6.3.dev5
-Summary: UNKNOWN
+Version: 0.6.4
 Home-page: https://github.com/TobikoData/sqlmesh
 Author: TobikoData Inc.
 Author-email: engineering@tobikodata.com
 License: Apache License 2.0
-Description: ![SQLMesh logo](sqlmesh.svg)
-        
-        SQLMesh is a DataOps framework that brings the benefits of DevOps to data teams. It enables data scientists, analysts, and engineers to efficiently run and deploy data transformations written in SQL or Python.
-        
-        For more information, check out the [website](https://sqlmesh.com) and [documentation](https://sqlmesh.readthedocs.io/en/stable/).
-        
-        ## Geting Started
-        Install SQLMesh through [pypi](https://pypi.org/project/sqlmesh/) by running:
-        
-        ```pip install sqlmesh```
-        
-        Follow the [tutorial](https://sqlmesh.readthedocs.io/en/stable/quick_start/) to learn how to use SQLMesh.
-        
-        ## Join our community
-        We'd love to join you on your data journey. Connect with us in the following ways:
-        
-        * Join the [Tobiko Slack community](https://tobikodata.com/slack) to ask questions, or just to say hi!
-        * File an issue on our [GitHub](https://github.com/TobikoData/sqlmesh/issues/new).
-        * Send us an email at [hello@tobikodata.com](hello@tobikodata.com) with your questions or feedback.
-        
-        ## Contribution
-        Contributions in the form of issues or pull requests are greatly appreciated. [Read more](https://sqlmesh.readthedocs.io/en/stable/development/) about how to develop for SQLMesh.
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: SQL
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
@@ -41,7 +16,31 @@
 Provides-Extra: databricks
 Provides-Extra: dev
 Provides-Extra: dbt
 Provides-Extra: postgres
 Provides-Extra: redshift
 Provides-Extra: snowflake
 Provides-Extra: web
+License-File: LICENSE
+
+![SQLMesh logo](sqlmesh.svg)
+
+SQLMesh is a DataOps framework that brings the benefits of DevOps to data teams. It enables data scientists, analysts, and engineers to efficiently run and deploy data transformations written in SQL or Python.
+
+For more information, check out the [website](https://sqlmesh.com) and [documentation](https://sqlmesh.readthedocs.io/en/stable/).
+
+## Geting Started
+Install SQLMesh through [pypi](https://pypi.org/project/sqlmesh/) by running:
+
+```pip install sqlmesh```
+
+Follow the [tutorial](https://sqlmesh.readthedocs.io/en/stable/quick_start/) to learn how to use SQLMesh.
+
+## Join our community
+We'd love to join you on your data journey. Connect with us in the following ways:
+
+* Join the [Tobiko Slack community](https://tobikodata.com/slack) to ask questions, or just to say hi!
+* File an issue on our [GitHub](https://github.com/TobikoData/sqlmesh/issues/new).
+* Send us an email at [hello@tobikodata.com](hello@tobikodata.com) with your questions or feedback.
+
+## Contribution
+Contributions in the form of issues or pull requests are greatly appreciated. [Read more](https://sqlmesh.readthedocs.io/en/stable/development/) about how to develop for SQLMesh.
```

### Comparing `sqlmesh-0.6.3.dev5/README.md` & `sqlmesh-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/docker-compose.yml` & `sqlmesh-0.6.4/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/docs/comparisons.md` & `sqlmesh-0.6.4/docs/comparisons.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/docs/concepts/architecture/serialization.md` & `sqlmesh-0.6.4/docs/concepts/architecture/serialization.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/docs/concepts/architecture/snapshots.md` & `sqlmesh-0.6.4/docs/concepts/architecture/snapshots.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/docs/concepts/audits.md` & `sqlmesh-0.6.4/docs/concepts/audits.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/docs/concepts/environments.md` & `sqlmesh-0.6.4/docs/concepts/environments.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/docs/concepts/glossary.md` & `sqlmesh-0.6.4/docs/concepts/glossary.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/docs/concepts/macros.md` & `sqlmesh-0.6.4/docs/concepts/macros.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/docs/concepts/models/model_kinds.md` & `sqlmesh-0.6.4/docs/concepts/models/model_kinds.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/docs/concepts/models/overview.md` & `sqlmesh-0.6.4/docs/concepts/models/overview.md`

 * *Files 3% similar despite different names*

```diff
@@ -63,52 +63,57 @@
   SUM(x) as x, -- explicitly x
 ```
 
 ## Properties
 The `MODEL` DDL statement takes various properties, which are used for both metadata and controlling behavior.
 
 ### name
-`name` specifies the name of the model. This name represents the production view name that the model outputs, so it generally takes the form of `"schema"."view_name"`. The name of a model must be unique in a SQLMesh project.
-
-When models are used in non-production environments, SQLMesh automatically prefixes the names. For example, consider a model named `"sushi"."customers"`. In production its view is named `"sushi"."customers"`, and in dev its view is named `"dev__sushi"."customers"`.
-
+- `name` specifies the name of the model. This name represents the production view name that the model outputs, so it generally takes the form of `"schema"."view_name"`. The name of a model must be unique in a SQLMesh project.<br /><br />
+When models are used in non-production environments, SQLMesh automatically prefixes the names. For example, consider a model named `"sushi"."customers"`. In production its view is named `"sushi"."customers"`, and in dev its view is named `"dev__sushi"."customers"`.<br /><br />
 Name is ***required*** and must be ***unique***.
 
 ### kind
-- Kind specifies what [kind](model_kinds.md) a model is. A model's kind determines how it is computed and stored. The default kind is `VIEW`, which means a view is created and your query is run each time that view is accessed.
+- Kind specifies what [kind](model_kinds.md) a model is. A model's kind determines how it is computed and stored. The default kind is `VIEW`, which means a view is created and your query is run each time that view is accessed. See [below](#incremental-model-properties) for properties that apply to incremental model kinds.
 
 ### dialect
 - Dialect defines the SQL dialect of the file. By default, this uses the dialect of the SQLMesh `sqlmesh.core.config`.
 
 ### owner
 - Owner specifies who the main point of contact is for the model. It is an important field for organizations that have many data collaborators.
 
 ### stamp
-An optional arbitrary string sequence used to create new model versions without making changes to any of the functional components of the definition.
+- An optional arbitrary string sequence used to create new model versions without making changes to any of the functional components of the definition.
 
 ### start
 - Start is used to determine the earliest time needed to process the model. It can be an absolute date/time (`2022-01-01`), or a relative one (`1 year ago`).
 
 ### cron
 - Cron is used to schedule your model to process or refresh at a certain interval. It uses [croniter](https://github.com/kiorky/croniter) under the hood, so expressions such as `@daily` can be used. A model's `IntervalUnit` is determined implicity by the cron expression.
 
-### batch_size
-- Batch size is used to optimize backfilling incremental data. It determines the maximum number of intervals to run in a single job. For example, if a model specifies a cron of `@hourly` and a batch_size of `12`, when backfilling 3 days of data, the scheduler will spawn 6 jobs. (3 days * 24 hours/day = 72 hour intervals to fill. 72 intervals / 12 intervals per job = 6 jobs.)
-
-### lookback
-- Lookback is used for [incremental](model_kinds.md#incremental_by_time_range) models to capture late arriving data. This must be a positive integer and refers to the number of units that late arriving data is expected.
-
 ### storage_format
 - Storage format is a property for engines such as Spark or Hive that support storage formats such as  `parquet` and `orc`.
 
+### partitioned_by
+- Partitioned by is an optional property for engines such as Spark or Hive that support partitioning. Use this to add additional columns to the time column partition key.
+
+### tags
+- Tags are one or more labels used to organize your models.
+
+## Incremental Model Properties
+
+For models that are incremental, the following parameters can be specified in the `kind`'s definition.
+
 ### time_column
 - Time column is a required property for incremental models. It is used to determine which records to overwrite when doing an incremental insert. Engines that support partitioning such as Spark and Hive also use it as the partition key. Additional partition key columns can be specified with the `partitioned_by` property (see below). Time column can have an optional format string. The format should be in the dialect of the model.
 
-### partitioned_by
-- Partitioned by is an optional property for engines such as Spark or Hive that support partitioning. Use this to add additional columns to the time column partition key.
+### lookback
+- Lookback is used for [incremental](model_kinds.md#incremental_by_time_range) models to capture late arriving data. This must be a positive integer and refers to the number of units that late arriving data is expected.
+
+### batch_size
+- Batch size is used to optimize backfilling incremental data. It determines the maximum number of intervals to run in a single job. For example, if a model specifies a cron of `@hourly` and a batch_size of `12`, when backfilling 3 days of data, the scheduler will spawn 6 jobs. (3 days * 24 hours/day = 72 hour intervals to fill. 72 intervals / 12 intervals per job = 6 jobs.)
 
 ## Macros
 Macros can be used for passing in paramaterized arguments such as dates, as well as for making SQL less repetitive. By default, SQLMesh provides several predefined macro variables that can be used. Macros are used by prefixing with the `@` symbol. For more information, refer to [macros](../macros.md).
 
 ## Statements
 Models can have additional statements that run before the main query. This can be useful for loading things such as [UDFs](../glossary.md#user-defined-function-udf).
```

### Comparing `sqlmesh-0.6.3.dev5/docs/concepts/models/python_models.md` & `sqlmesh-0.6.4/docs/concepts/models/python_models.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/docs/concepts/models/seed_models.md` & `sqlmesh-0.6.4/docs/concepts/models/seed_models.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/docs/concepts/models/sql_models.md` & `sqlmesh-0.6.4/docs/concepts/models/sql_models.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/docs/concepts/overview.md` & `sqlmesh-0.6.4/docs/concepts/overview.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/docs/concepts/plans/model_versioning.png` & `sqlmesh-0.6.4/docs/concepts/plans/model_versioning.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/docs/concepts/plans.md` & `sqlmesh-0.6.4/docs/concepts/plans.md`

 * *Files 10% similar despite different names*

```diff
@@ -42,15 +42,25 @@
 *Each model variant gets its own physical table while environments only contain references to these tables.*
 
 This unique approach to understanding and applying changes is what enables SQLMesh's Virtual Environments. This technology allows SQLMesh to ensure complete isolation between environments while allowing it to share physical data assets between environments when appropriate and safe to do so. Additionally, since each model change is captured in a separate physical table, reverting to a previous version becomes a simple and quick operation (refer to [Virtual Update](#virtual-update)) as long as its physical table hasn't been garbage collected by the janitor process. SQLMesh makes it easy to be correct, and really hard to accidentally and irreversibly break things.
 
 ### Backfilling
 Despite all the benefits, the approach described above is not without trade-offs. When a new model version is just created, a physical table assigned to it is empty. Therefore, SQLMesh needs to re-apply the logic of the new model version to the entire date range of this model in order to populate the new version's physical table. This process is called backfilling.
 
-Despite the fact that backfilling happens incrementally, there is an extra cost associated with this operation due to additional runtime involved. If the runtime cost is a concern, a [forward-only plan](#forward-only-plans) can be used instead.
+At the moment, we are using the term backfilling broadly to describe any situation in which a model is updated. That includes these operations: 
+
+* When a VIEW model is created
+* When a FULL model is built 
+* When an INCREMENTAL model is built for the first time
+* When an INCREMENTAL model has recent data appended to it
+* When an INCREMENTAL model has older data inserted (i.e., resolving a data gap or prepending historical data)
+
+We will be iterating on terminology to better capture the nuances of each type in future versions. 
+
+Note for incremental models: despite the fact that backfilling can happen incrementally (see `batch_size` parameter on models), there is an extra cost associated with this operation due to additional runtime involved. If the runtime cost is a concern, a [forward-only plan](#forward-only-plans) can be used instead.
 
 ### Virtual Update
 Another benefit of the aforementioned approach is that data for a new model version can be fully pre-built while still in a development environment. This means that all changes and their downstream dependencies can be fully previewed before they get promoted to the production environment. Therefore, the process of promoting a change to production is reduced to reference swapping. If during plan creation no data gaps have been detected and only references to new model versions need to be updated, then such update is referred to as a Virtual Update. Virtual Updates impose no additional runtime overhead or cost.
 
 ## Forward-only plans
 Sometimes the runtime cost associated with rebuilding an entire physical table is too high and outweighs the benefits a separate table provides. This is when a forward-only plan comes in handy.
 
@@ -63,14 +73,21 @@
  Note that all changes made as part of a forward-only plan automatically get a **forward-only** category assigned to them. These types of changes can't be mixed together with breaking and non-breaking changes (refer to [change categories](#change-categories)) as part of the same plan.
 
 To create a forward-only plan, the `--forward-only` option has to be added to the `plan` command:
 ```bash
 sqlmesh plan --forward-only
 ```
 
+### Effective date
+Changes that are part of the forward-only plan can also be applied retroactively to the production environment by specifying the effective date:
+```bash
+sqlmesh plan --forward-only --effective-from 2023-01-01
+```
+This way SQLMesh will know to recompute data intervals starting from the specified date once forward-only changes are deployed to production.
+
 ## Restatement plans
 There are cases when models need to be re-evaluated for a given time range, even though changes may not have been made to those model definitions. This could be due to an upstream issue with a dataset defined outside the SQLMesh platform, or when a [forward-only plan](#forward-only-plans) change needs to be applied retroactively to a bounded interval of historical data.
 
 For this reason, the `plan` command supports the `--restate-model` option, which allows users to specify one or more names of a model to be reprocessed. Each name can also refer to an external table defined outside SQLMesh.
 
 Application of such a plan will trigger a cascading backfill for all specified models (excluding external tables), as well as all models downstream from them. The plan's date range in this case determines data intervals that will be affected. For example:
```

### Comparing `sqlmesh-0.6.3.dev5/docs/concepts/tests.md` & `sqlmesh-0.6.4/docs/concepts/tests.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/docs/development.md` & `sqlmesh-0.6.4/docs/development.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/docs/guides/connections.md` & `sqlmesh-0.6.4/docs/guides/connections.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/docs/guides/migrations.md` & `sqlmesh-0.6.4/docs/guides/migrations.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/docs/guides/models.md` & `sqlmesh-0.6.4/docs/guides/models.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/docs/guides/multi_repo.md` & `sqlmesh-0.6.4/docs/guides/multi_repo.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/docs/guides/projects.md` & `sqlmesh-0.6.4/docs/guides/projects.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/docs/guides/scheduling/airflow_successful_plan_apply.png` & `sqlmesh-0.6.4/docs/guides/scheduling/airflow_successful_plan_apply.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/docs/guides/scheduling/airflow_successful_setup.png` & `sqlmesh-0.6.4/docs/guides/scheduling/airflow_successful_setup.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/docs/guides/scheduling.md` & `sqlmesh-0.6.4/docs/guides/scheduling.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/docs/guides/testing.md` & `sqlmesh-0.6.4/docs/guides/testing.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/docs/index.md` & `sqlmesh-0.6.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/docs/integrations/airflow.md` & `sqlmesh-0.6.4/docs/integrations/airflow.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/docs/integrations/dbt.md` & `sqlmesh-0.6.4/docs/integrations/dbt.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/docs/integrations/engines.md` & `sqlmesh-0.6.4/docs/integrations/engines.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/docs/integrations/github.md` & `sqlmesh-0.6.4/docs/integrations/github.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/docs/prerequisites.md` & `sqlmesh-0.6.4/docs/prerequisites.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/docs/quick_start.md` & `sqlmesh-0.6.4/docs/quick_start.md`

 * *Files 13% similar despite different names*

```diff
@@ -23,43 +23,66 @@
 
 This will create the directories and files that you can use to organize your SQLMesh project code:
 
 - config.yaml
     - The file for project configuration. Refer to [configuration](reference/configuration.md).
 - ./models
     - SQL and Python models. Refer to [models](concepts/models/overview.md).
+- ./seeds
+    - Seed files. Refer to [seeds](concepts/models/seed_models.md).
 - ./audits
     - Shared audit files. Refer to [auditing](concepts/audits.md).
 - ./tests
     - Unit test files. Refer to [testing](concepts/tests.md).
 - ./macros
     - Macro files. Refer to [macros](concepts/macros.md).
 
 ## 2. Plan and apply environments
 ### 2.1 Create a prod environment
-This example project structure is a two-model pipeline, where `sqlmesh_example.example_full_model` depends on `sqlmesh_example.example_incremental_model`.
+This example project structure is a three-model pipeline with a CSV acting as a source data file: 
+
+```
+┌─────────────┐
+│seed_data.csv│
+└────────────┬┘
+             │
+            ┌▼─────────────┐
+            │seed_model.sql│
+            └─────────────┬┘
+                          │
+                         ┌▼────────────────────┐
+                         │incremental_model.sql│
+                         └────────────────────┬┘
+                                              │
+                                             ┌▼─────────────┐
+                                             │full_model.sql│
+                                             └──────────────┘
+```
 
 To materialize this pipeline into DuckDB, run `sqlmesh plan` to get started with the plan/apply flow. The prompt will ask you what date to backfill; you can leave those blank for now (hit `Enter`) to backfill all of history. Finally, it will ask you whether or not you want backfill the plan. Enter `y`:
 
 ```bash
 (.env) [user@computer sqlmesh-example]$ sqlmesh plan
 ======================================================================
 Successfully Ran 1 tests against duckdb
 ----------------------------------------------------------------------
 New environment `prod` will be created from `prod`
 Summary of differences against `prod`:
 └── Added Models:
-    ├── sqlmesh_example.example_incremental_model
-    └── sqlmesh_example.example_full_model
+    ├── sqlmesh_example.seed_model
+    ├── sqlmesh_example.incremental_model
+    └── sqlmesh_example.full_model
 Models needing backfill (missing dates):
-├── sqlmesh_example.example_incremental_model: (2020-01-01, 2023-03-22)
-└── sqlmesh_example.example_full_model: (2023-03-22, 2023-03-22)
+├── sqlmesh_example.seed_model: (2020-01-01, 2023-03-22)
+├── sqlmesh_example.incremental_model: (2020-01-01, 2023-03-22)
+└── sqlmesh_example.full_model: (2023-03-22, 2023-03-22)
 Apply - Backfill Tables [y/n]: y
-sqlmesh_example.example_incremental_model ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 100.0% • 1/1 • 0:00:00
-       sqlmesh_example.example_full_model ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 100.0% • 1/1 • 0:00:00
+       sqlmesh_example.seed_model ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 100.0% • 1/1 • 0:00:00
+sqlmesh_example.incremental_model ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 100.0% • 1/1 • 0:00:00
+       sqlmesh_example.full_model ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 100.0% • 1/1 • 0:00:00
 
 All model batches have been executed successfully
 
 Virtually Updating 'prod' ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 100.0% • 0:00:00
 
 The target environment has been updated successfully
 ```
@@ -84,102 +107,101 @@
 
 
 Virtual Update executed successfully
 ```
 
 ## 3. Make your first update
 ### 3.1 Edit the configuration
-Let's add a new column. Open the `models/example_incremental_model.sql` file and add `#!sql 'z' AS new_column` under `item_id` as follows:
+Let's add a new column. Open the `models/incremental_model.sql` file and add `#!sql 'z' AS new_column` under `item_id` as follows:
 
 ```bash
-diff --git a/models/example_incremental_model.sql b/models/example_incremental_model.sql
+diff --git a/models/incremental_model.sql b/models/incremental_model.sql
 index e1407e6..8154da2 100644
---- a/models/example_incremental_model.sql
-+++ b/models/example_incremental_model.sql
+--- a/models/incremental_model.sql
++++ b/models/incremental_model.sql
 @@ -10,6 +10,7 @@ MODEL (
  SELECT
      id,
      item_id,
 +    'z' AS new_column,
      ds,
  FROM
-     (VALUES
+     sqlmesh_example.seed_model
 ```
 
 ## 4. Plan and apply updates
 Once this change is made, we can preview it using the `sqlmesh plan` command to understand the impact it had.
 
 Run `sqlmesh plan dev` and hit `Enter` to leave the backfill start and end dates empty:
 
 ```bash
 (.env) [user@computer sqlmesh-example]$ sqlmesh plan dev
 ======================================================================
 Successfully Ran 1 tests against duckdb
 ----------------------------------------------------------------------
 Summary of differences against `dev`:
 ├── Directly Modified:
-│   └── sqlmesh_example.example_incremental_model
+│   └── sqlmesh_example.incremental_model
 └── Indirectly Modified:
-    └── sqlmesh_example.example_full_model
----
-
-+++
-
-@@ -1,6 +1,7 @@
-
- SELECT
-   id,
-   item_id,
-+  'z' AS new_column,
-   ds
- FROM (VALUES
-   (1, 1, '2020-01-01'),
-Directly Modified: sqlmesh_example.example_incremental_model (Non-breaking)
+    └── sqlmesh_example.full_model
+---                                                                                                             
+                                                                                                                
++++                                                                                                             
+                                                                                                                
+@@ -1,6 +1,7 @@                                                                                                 
+                                                                                                                
+ SELECT                                                                                                         
+   id,                                                                                                          
+   item_id,                                                                                                     
++  'z' AS new_column,                                                                                           
+   ds                                                                                                           
+ FROM sqlmesh_example.seed_model                                                                                
+ WHERE                                                                                                          
+Directly Modified: sqlmesh_example.incremental_model (Non-breaking)
 └── Indirectly Modified Children:
-    └── sqlmesh_example.example_full_model
+    └── sqlmesh_example.full_model
 Models needing backfill (missing dates):
-└── sqlmesh_example.example_incremental_model: (2020-01-01, 2023-03-22)
-Enter the backfill start date (eg. '1 year', '2020-01-01') or blank for the beginning of history:
-Enter the backfill end date (eg. '1 month ago', '2020-01-01') or blank to backfill up until now:
+└── sqlmesh_example__dev.incremental_model: (2020-01-01, 2023-04-27)
+Enter the backfill start date (eg. '1 year', '2020-01-01') or blank for the beginning of history: 
+Enter the backfill end date (eg. '1 month ago', '2020-01-01') or blank to backfill up until now: 
 Apply - Backfill Tables [y/n]: y
 
-sqlmesh_example__dev.example_incremental_model ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 100.0% • 1/1 • 0:00:00
+sqlmesh_example__dev.incremental_model ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 100.0% • 1/1 • 0:00:00
 
 All model batches have been executed successfully
 
 Virtually Updating 'dev' ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 100.0% • 0:00:00
 
 The target environment has been updated successfully
 ```
 
-Notice that SQLMesh has detected that you've added `new_column`. It also shows you that the downstream model `sqlmesh_example.example_full_model` was indirectly modified. SQLMesh semantically understood that your change was additive (added an unused column) and so it was automatically classified as a non-breaking change.
+Notice that SQLMesh has detected that you've added `new_column`. It also shows you that the downstream model `sqlmesh_example.full_model` was indirectly modified. SQLMesh semantically understood that your change was additive (added an unused column) and so it was automatically classified as a non-breaking change.
 
-SQLMesh now applies the change to `sqlmesh_example.example_incremental_model` and backfills the model. SQLMesh did not need to backfill `sqlmesh_example.example_full_model`, since it was `non-breaking`.
+SQLMesh now applies the change to `sqlmesh_example.incremental_model` and backfills the model. SQLMesh did not need to backfill `sqlmesh_example.full_model`, since it was `non-breaking`.
 
 ### 4.1 Validate updates in dev
-You can now view this change by running `sqlmesh fetchdf "select * from sqlmesh_example__dev.example_incremental_model"`:
+You can now view this change by running `sqlmesh fetchdf "select * from sqlmesh_example__dev.incremental_model"`:
 
 ```bash
-(.env) [user@computer sqlmesh-example]$ sqlmesh fetchdf "select * from sqlmesh_example__dev.example_incremental_model"
+(.env) [user@computer sqlmesh-example]$ sqlmesh fetchdf "select * from sqlmesh_example__dev.incremental_model"
 
-   id  item_id  new_column          ds
-0   1        1           1  2020-01-01
-1   1        2           1  2020-01-01
-2   2        1           1  2020-01-01
-3   3        3           1  2020-01-03
-4   4        1           1  2020-01-04
-5   5        1           1  2020-01-05
-6   6        1           1  2020-01-06
-7   7        1           1  2020-01-07
+   id  item_id new_column         ds
+0   1        2          z 2020-01-01
+1   2        1          z 2020-01-01
+2   3        3          z 2020-01-03
+3   4        1          z 2020-01-04
+4   5        1          z 2020-01-05
+5   6        1          z 2020-01-06
+6   7        1          z 2020-01-07
 ```
 
-You can see that `new_column` was added to your dataset. The production table was not modified; you can validate this by querying the table using `sqlmesh fetchdf "select * from sqlmesh_example.example_incremental_model"`:
+You can see that `new_column` was added to your dataset. The production table was not modified; you can validate this by querying the table using `sqlmesh fetchdf "select * from sqlmesh_example.incremental_model"`:
 
 ```bash
-(.env) [user@computer sqlmesh-example]$ sqlmesh fetchdf "select * from sqlmesh_example.example_incremental_model"
+(.env) [user@computer sqlmesh-example]$ sqlmesh fetchdf "select * from sqlmesh_example.incremental_model"
 
    id  item_id          ds
 0   1        1  2020-01-01
 1   1        2  2020-01-01
 2   2        1  2020-01-01
 3   3        3  2020-01-03
 4   4        1  2020-01-04
@@ -196,59 +218,58 @@
 ```bash
 (.env) [toby@muc sqlmesh-example]$ sqlmesh plan
 ======================================================================
 Successfully Ran 1 tests against duckdb
 ----------------------------------------------------------------------
 Summary of differences against `prod`:
 ├── Directly Modified:
-│   └── sqlmesh_example.example_incremental_model
+│   └── sqlmesh_example.incremental_model
 └── Indirectly Modified:
-    └── sqlmesh_example.example_full_model
+    └── sqlmesh_example.full_model
 ---
 
 +++
 
 @@ -1,6 +1,7 @@
 
  SELECT
    id,
    item_id,
 +  'z' AS new_column,
    ds
  FROM (VALUES
    (1, 1, '2020-01-01'),
-Directly Modified: sqlmesh_example.example_incremental_model (Non-breaking)
+Directly Modified: sqlmesh_example.incremental_model (Non-breaking)
 └── Indirectly Modified Children:
-    └── sqlmesh_example.example_full_model
+    └── sqlmesh_example.full_model
 Apply - Virtual Update [y/n]: y
 Virtually Updating 'prod' ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 100.0% • 0:00:00
 
 The target environment has been updated successfully
 
 
 Virtual Update executed successfully
 ```
 
 Notice that a backfill was not necessary and only a Virtual Update occurred.
 
 ### 4.3. Validate updates in prod
-Double-check that the data did indeed update in prod by running `sqlmesh fetchdf "select * from sqlmesh_example.example_incremental_model"`:
+Double-check that the data did indeed update in prod by running `sqlmesh fetchdf "select * from sqlmesh_example.incremental_model"`:
 
 ```bash
-(.env) [user@computer sqlmesh-example]$ sqlmesh fetchdf "select * from sqlmesh_example.example_incremental_model"
+(.env) [user@computer sqlmesh-example]$ sqlmesh fetchdf "select * from sqlmesh_example.incremental_model"
 
-   id  item_id  new_column          ds
-0   1        1           1  2020-01-01
-1   1        2           1  2020-01-01
-2   2        1           1  2020-01-01
-3   3        3           1  2020-01-03
-4   4        1           1  2020-01-04
-5   5        1           1  2020-01-05
-6   6        1           1  2020-01-06
-7   7        1           1  2020-01-07
+   id  item_id new_column         ds
+0   1        2          z 2020-01-01
+1   2        1          z 2020-01-01
+2   3        3          z 2020-01-03
+3   4        1          z 2020-01-04
+4   5        1          z 2020-01-05
+5   6        1          z 2020-01-06
+6   7        1          z 2020-01-07
 ```
 
 ## 5. Next steps
 
 Congratulations, you've now conquered the basics of using SQLMesh!
 
 * [Learn more about SQLMesh concepts](concepts/overview.md)
```

### Comparing `sqlmesh-0.6.3.dev5/docs/reference/cli.md` & `sqlmesh-0.6.4/docs/reference/cli.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/docs/reference/configuration.md` & `sqlmesh-0.6.4/docs/reference/configuration.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/docs/reference/notebook.md` & `sqlmesh-0.6.4/docs/reference/notebook.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/docs/reference/overview.md` & `sqlmesh-0.6.4/docs/reference/overview.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/docs/sqlmesh.png` & `sqlmesh-0.6.4/docs/sqlmesh.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/examples/airflow/Dockerfile.template` & `sqlmesh-0.6.4/examples/airflow/Dockerfile.template`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/examples/airflow/Makefile` & `sqlmesh-0.6.4/examples/airflow/Makefile`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/examples/airflow/README.md` & `sqlmesh-0.6.4/examples/airflow/README.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/examples/airflow/docker_compose_decorator.py` & `sqlmesh-0.6.4/examples/airflow/docker_compose_decorator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/examples/airflow/spark_conf/hive-site.xml` & `sqlmesh-0.6.4/examples/airflow/spark_conf/hive-site.xml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/examples/sushi/config.py` & `sqlmesh-0.6.4/examples/sushi/config.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/examples/sushi/helper.py` & `sqlmesh-0.6.4/examples/sushi/helper.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/examples/sushi/macros/macros.py` & `sqlmesh-0.6.4/examples/sushi/macros/macros.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/examples/sushi/models/customer_revenue_by_day.sql` & `sqlmesh-0.6.4/examples/sushi/models/customer_revenue_by_day.sql`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
   kind incremental_by_time_range (
     time_column (ds, 'YYYY-MM-dd'),
     batch_size 10,
   ),
   owner jen,
   cron '@daily',
   dialect hive,
+  tags expensive,
 );
 
 WITH order_total AS (
   SELECT
     oi.order_id AS order_id,
     SUM(oi.quantity * i.price) AS total,
     oi.ds AS ds
```

### Comparing `sqlmesh-0.6.3.dev5/examples/sushi/models/items.py` & `sqlmesh-0.6.4/examples/sushi/models/items.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import random
 import typing as t
 from datetime import datetime
 
 import numpy as np
 import pandas as pd
+from helper import iter_dates  # type: ignore
 from sqlglot.expressions import to_column
 
-from examples.sushi.helper import iter_dates
 from sqlmesh import ExecutionContext, model
 from sqlmesh.core.model import IncrementalByTimeRangeKind
 from sqlmesh.utils.date import to_ds
 
 ITEMS = [
     "Ahi",
     "Aji",
```

### Comparing `sqlmesh-0.6.3.dev5/examples/sushi/models/order_items.py` & `sqlmesh-0.6.4/examples/sushi/models/order_items.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import random
 import typing as t
 from datetime import datetime
 
 import numpy as np
 import pandas as pd
+from helper import iter_dates  # type: ignore
 from sqlglot.expressions import to_column
 
-from examples.sushi.helper import iter_dates
 from sqlmesh import ExecutionContext, model
 from sqlmesh.core.model import IncrementalByTimeRangeKind
 from sqlmesh.utils.date import to_ds
 
 ITEMS = "sushi.items"
```

### Comparing `sqlmesh-0.6.3.dev5/examples/sushi/models/orders.py` & `sqlmesh-0.6.4/examples/sushi/models/orders.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import random
 import typing as t
 from datetime import datetime, timedelta
 
 import pandas as pd
+from helper import iter_dates  # type: ignore
 
-from examples.sushi.helper import iter_dates
 from sqlmesh import ExecutionContext, model
 from sqlmesh.core.model import IncrementalByTimeRangeKind
 from sqlmesh.utils.date import to_ds
 
 CUSTOMERS = list(range(0, 100))
 WAITERS = list(range(0, 10))
```

### Comparing `sqlmesh-0.6.3.dev5/examples/sushi/models/waiter_revenue_by_day.sql` & `sqlmesh-0.6.4/examples/sushi/models/waiter_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/examples/sushi/tests/test_customer_revenue_by_day.yaml` & `sqlmesh-0.6.4/examples/sushi/tests/test_customer_revenue_by_day.yaml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/examples/sushi_dbt/macros/incremental.sql` & `sqlmesh-0.6.4/examples/sushi_dbt/macros/incremental.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/examples/sushi_dbt/models/customer_revenue_by_day.sql` & `sqlmesh-0.6.4/examples/sushi_dbt/models/customer_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/examples/sushi_dbt/models/waiter_revenue_by_day.sql` & `sqlmesh-0.6.4/examples/sushi_dbt/models/waiter_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/examples/sushi_dbt/packages/customers/dbt_project.yml` & `sqlmesh-0.6.4/examples/sushi_dbt/packages/customers/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/examples/sushi_dbt/profiles.yml` & `sqlmesh-0.6.4/examples/sushi_dbt/profiles.yml`

 * *Files 13% similar despite different names*

```diff
@@ -21,8 +21,17 @@
       type: bigquery
       method: service-account
       project: "{{ env_var('BQ_PROJECT') }}"
       dataset: "{{ env_var('BQ_SCHEMA') }}"
       threads: 1
       keyfile: "{{ env_var('BQ_KEYFILE') }}"
       location: "{{ env_var('BQ_LOCATION') }}"
+    redshift:
+      host: "{{ env_var('REDSHIFT_HOST') }}"
+      user: "{{ env_var('REDSHIFT_USER') }}"
+      password: "{{ env_var('REDSHIFT_PASSWORD') }}"
+      port: "{{ env_var('REDSHIFT_PORT') }}"
+      dbname: "{{ env_var('REDSHIFT_DBNAME') }}"
+      schema: sushi
+      threads: 1
+      type: redshift
   target: in_memory
```

### Comparing `sqlmesh-0.6.3.dev5/examples/sushi_dbt/seeds/items.csv` & `sqlmesh-0.6.4/examples/sushi_dbt/seeds/items.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/examples/sushi_dbt/seeds/order_items.csv` & `sqlmesh-0.6.4/examples/sushi_dbt/seeds/order_items.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/examples/sushi_dbt/seeds/orders.csv` & `sqlmesh-0.6.4/examples/sushi_dbt/seeds/orders.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/examples/wursthall/macros/macros.py` & `sqlmesh-0.6.4/examples/wursthall/macros/macros.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/examples/wursthall/models/db/order_f.py` & `sqlmesh-0.6.4/examples/wursthall/models/db/order_f.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import random
 import typing as t
 from datetime import datetime
 
 import numpy as np
 import pandas as pd
+from models.src.shared import DATA_START_DATE_STR, set_seed  # type: ignore
 
-from examples.wursthall.models.src.shared import DATA_START_DATE_STR, set_seed
 from sqlmesh import ExecutionContext, model
 from sqlmesh.core.model import IncrementalByTimeRangeKind, TimeColumn
 from sqlmesh.utils.date import to_ds
 
 COLUMN_TO_TYPE = {
     "order_id": "text",
     "customer_id": "text",
```

### Comparing `sqlmesh-0.6.3.dev5/examples/wursthall/models/db/order_item_f.sql` & `sqlmesh-0.6.4/examples/wursthall/models/db/order_item_f.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/examples/wursthall/models/src/customer_details.py` & `sqlmesh-0.6.4/examples/wursthall/models/src/customer_details.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 import random
 import typing as t
 from dataclasses import dataclass
 from datetime import datetime, timedelta
 
 import pandas as pd
 from faker import Faker
+from models.src.shared import DATA_START_DATE_STR, iter_dates, set_seed  # type: ignore
 
-from examples.wursthall.models.src.shared import (
-    DATA_START_DATE_STR,
-    iter_dates,
-    set_seed,
-)
 from sqlmesh import model
 from sqlmesh.core.model import IncrementalByTimeRangeKind, TimeColumn
 
 
 @dataclass(frozen=True)
 class CustomerDetails:
     id: str
```

### Comparing `sqlmesh-0.6.3.dev5/examples/wursthall/models/src/order_item_details.py` & `sqlmesh-0.6.4/examples/wursthall/models/src/order_item_details.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,20 +2,16 @@
 import typing as t
 from dataclasses import dataclass
 from datetime import datetime
 
 import numpy as np
 import pandas as pd
 from faker import Faker
+from models.src.shared import DATA_START_DATE_STR, iter_dates, set_seed  # type: ignore
 
-from examples.wursthall.models.src.shared import (
-    DATA_START_DATE_STR,
-    iter_dates,
-    set_seed,
-)
 from sqlmesh import ExecutionContext, model
 from sqlmesh.core.model import IncrementalByTimeRangeKind, TimeColumn
 from sqlmesh.utils.date import to_ds
 
 
 @dataclass(frozen=True)
 class OrderItemDetails:
```

### Comparing `sqlmesh-0.6.3.dev5/examples/wursthall/models/src/shared.py` & `sqlmesh-0.6.4/examples/wursthall/models/src/shared.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/examples/wursthall/seeds/src/menu_item_details.csv` & `sqlmesh-0.6.4/examples/wursthall/seeds/src/menu_item_details.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/examples/wursthall/tests/test_customer_d.yaml` & `sqlmesh-0.6.4/examples/wursthall/tests/test_customer_d.yaml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/examples/wursthall/tests/test_order_item_f.yaml` & `sqlmesh-0.6.4/examples/wursthall/tests/test_order_item_f.yaml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/mkdocs.yml` & `sqlmesh-0.6.4/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/pdoc/cli.py` & `sqlmesh-0.6.4/pdoc/cli.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/posts/virtual_data_environments/change_categorization.png` & `sqlmesh-0.6.4/posts/virtual_data_environments/change_categorization.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/posts/virtual_data_environments/isolated_rigid_envs.png` & `sqlmesh-0.6.4/posts/virtual_data_environments/isolated_rigid_envs.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/posts/virtual_data_environments/partial_breaking.png` & `sqlmesh-0.6.4/posts/virtual_data_environments/partial_breaking.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/posts/virtual_data_environments/stateful_envs.png` & `sqlmesh-0.6.4/posts/virtual_data_environments/stateful_envs.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/posts/virtual_data_environments/virtual_envs.png` & `sqlmesh-0.6.4/posts/virtual_data_environments/virtual_envs.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/posts/virtual_data_environments/virtual_envs_end_to_end.png` & `sqlmesh-0.6.4/posts/virtual_data_environments/virtual_envs_end_to_end.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/posts/virtual_data_environments.md` & `sqlmesh-0.6.4/posts/virtual_data_environments.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/pytest.ini` & `sqlmesh-0.6.4/pytest.ini`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/setup.cfg` & `sqlmesh-0.6.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/setup.py` & `sqlmesh-0.6.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         "hyperscript",
         "jinja2",
         "pandas",
         "pydantic>=1.9.1,<2.0.0",
         "requests",
         "rich",
         "ruamel.yaml",
-        "sqlglot~=11.5.7",
+        "sqlglot~=11.6.3",
         "fsspec",
     ],
     extras_require={
         "bigquery": [
             "google-cloud-bigquery[pandas]",
             "google-cloud-bigquery-storage",
         ],
```

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/__init__.py` & `sqlmesh-0.6.4/sqlmesh/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/cli/__init__.py` & `sqlmesh-0.6.4/sqlmesh/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/cli/example_project.py` & `sqlmesh-0.6.4/sqlmesh/cli/example_project.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,17 +24,17 @@
 
 from sqlmesh.dbt.loader import sqlmesh_config
 
 config = sqlmesh_config(Path(__file__).parent)
 """
 
 EXAMPLE_SCHEMA_NAME = "sqlmesh_example"
-EXAMPLE_FULL_MODEL_NAME = f"{EXAMPLE_SCHEMA_NAME}.example_full_model"
-EXAMPLE_INCREMENTAL_MODEL_NAME = f"{EXAMPLE_SCHEMA_NAME}.example_incremental_model"
-
+EXAMPLE_FULL_MODEL_NAME = f"{EXAMPLE_SCHEMA_NAME}.full_model"
+EXAMPLE_INCREMENTAL_MODEL_NAME = f"{EXAMPLE_SCHEMA_NAME}.incremental_model"
+EXAMPLE_SEED_MODEL_NAME = f"{EXAMPLE_SCHEMA_NAME}.seed_model"
 
 EXAMPLE_FULL_MODEL_DEF = f"""MODEL (
   name {EXAMPLE_FULL_MODEL_NAME},
   kind FULL,
   cron '@daily',
   audits [assert_positive_order_ids],
 );
@@ -57,38 +57,51 @@
 );
 
 SELECT
     id,
     item_id,
     ds,
 FROM
-    (VALUES
-        (1, 1, '2020-01-01'),
-        (1, 2, '2020-01-01'),
-        (2, 1, '2020-01-01'),
-        (3, 3, '2020-01-03'),
-        (4, 1, '2020-01-04'),
-        (5, 1, '2020-01-05'),
-        (6, 1, '2020-01-06'),
-        (7, 1, '2020-01-07')
-    ) AS t (id, item_id, ds)
+    {EXAMPLE_SEED_MODEL_NAME}
 WHERE
     ds between @start_ds and @end_ds
 """
 
+EXAMPLE_SEED_MODEL_DEF = f"""MODEL (
+    name {EXAMPLE_SEED_MODEL_NAME},
+    kind SEED (
+        path '../seeds/seed_data.csv'
+    ),
+    columns (
+        id INTEGER,
+        item_id INTEGER,
+        ds DATE
+    )
+);
+"""
+
 EXAMPLE_AUDIT = f"""AUDIT (
   name assert_positive_order_ids,
 );
 
 SELECT *
 FROM @this_model
 WHERE
   item_id < 0
 """
 
+EXAMPLE_SEED_DATA = f"""id,item_id,ds
+1, 2, 2020-01-01
+2, 1, 2020-01-01
+3, 3, 2020-01-03
+4, 1, 2020-01-04
+5, 1, 2020-01-05
+6, 1, 2020-01-06
+7, 1, 2020-01-07
+"""
 
 EXAMPLE_TEST = f"""test_example_full_model:
   model: {EXAMPLE_FULL_MODEL_NAME}
   inputs:
     {EXAMPLE_INCREMENTAL_MODEL_NAME}:
         rows:
         - id: 1
@@ -128,27 +141,29 @@
 ) -> None:
     root_path = Path(path)
     config_extension = "py" if template == ProjectTemplate.DBT else "yaml"
     config_path = root_path / f"config.{config_extension}"
     audits_path = root_path / "audits"
     macros_path = root_path / "macros"
     models_path = root_path / "models"
+    seeds_path = root_path / "seeds"
     tests_path = root_path / "tests"
 
     if config_path.exists():
         raise click.ClickException(f"Found an existing config in '{config_path}'")
 
     _create_config(config_path, template)
     if template == ProjectTemplate.DBT:
         return
 
-    _create_folders([audits_path, macros_path, models_path, tests_path])
+    _create_folders([audits_path, macros_path, models_path, seeds_path, tests_path])
     _create_macros(macros_path)
     _create_audits(audits_path)
     _create_models(models_path)
+    _create_seeds(seeds_path)
     _create_tests(tests_path)
 
 
 def _create_folders(target_folders: t.Sequence[Path]) -> None:
     for folder_path in target_folders:
         folder_path.mkdir(exist_ok=True)
         (folder_path / ".gitkeep").touch()
@@ -162,25 +177,30 @@
 
 
 def _create_macros(macros_path: Path) -> None:
     (macros_path / "__init__.py").touch()
 
 
 def _create_audits(audits_path: Path) -> None:
-    _write_file(audits_path / "example_full_model.sql", EXAMPLE_AUDIT)
+    _write_file(audits_path / "assert_positive_order_ids.sql", EXAMPLE_AUDIT)
 
 
 def _create_models(models_path: Path) -> None:
     for model_name, model_def in [
         (EXAMPLE_FULL_MODEL_NAME, EXAMPLE_FULL_MODEL_DEF),
         (EXAMPLE_INCREMENTAL_MODEL_NAME, EXAMPLE_INCREMENTAL_MODEL_DEF),
+        (EXAMPLE_SEED_MODEL_NAME, EXAMPLE_SEED_MODEL_DEF),
     ]:
         _write_file(models_path / f"{model_name.split('.')[-1]}.sql", model_def)
 
 
+def _create_seeds(seeds_path: Path) -> None:
+    _write_file(seeds_path / "seed_data.csv", EXAMPLE_SEED_DATA)
+
+
 def _create_tests(tests_path: Path) -> None:
-    _write_file(tests_path / "test_example_full_model.yaml", EXAMPLE_TEST)
+    _write_file(tests_path / "test_full_model.yaml", EXAMPLE_TEST)
 
 
 def _write_file(path: Path, payload: str) -> None:
     with open(path, "w", encoding="utf-8") as fd:
         fd.write(payload)
```

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/cli/main.py` & `sqlmesh-0.6.4/sqlmesh/cli/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -209,14 +209,20 @@
 )
 @click.option(
     "--forward-only",
     is_flag=True,
     help="Create a plan for forward-only changes.",
 )
 @click.option(
+    "--effective-from",
+    type=str,
+    required=False,
+    help="The effective date from which to apply forward-only changes on production.",
+)
+@click.option(
     "--no-prompts",
     is_flag=True,
     help="Disable interactive prompts for the backfill time range. Please note that if this flag is set and there are uncategorized changes, plan creation will fail.",
 )
 @click.option(
     "--auto-apply",
     is_flag=True,
@@ -256,15 +262,17 @@
 @error_handler
 def dag(ctx: click.Context, file: str) -> None:
     """
     Renders the dag using graphviz.
 
     This command requires a manual install of both the python and system graphviz package.
     """
-    ctx.obj.render_dag(file)
+    rendered_dag_path = ctx.obj.render_dag(file)
+    if rendered_dag_path:
+        ctx.obj.console.log_success(f"Generated the dag to {rendered_dag_path}")
 
 
 @cli.command("test")
 @opt.match_pattern
 @opt.verbose
 @click.argument("tests", nargs=-1)
 @click.pass_obj
```

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/cli/options.py` & `sqlmesh-0.6.4/sqlmesh/cli/options.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/_typing.py` & `sqlmesh-0.6.4/sqlmesh/core/_typing.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/audit/builtin.py` & `sqlmesh-0.6.4/sqlmesh/core/audit/builtin.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/audit/definition.py` & `sqlmesh-0.6.4/sqlmesh/core/audit/definition.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/config/__init__.py` & `sqlmesh-0.6.4/sqlmesh/core/config/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/config/base.py` & `sqlmesh-0.6.4/sqlmesh/core/config/base.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/config/categorizer.py` & `sqlmesh-0.6.4/sqlmesh/core/config/categorizer.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/config/common.py` & `sqlmesh-0.6.4/sqlmesh/core/config/common.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/config/connection.py` & `sqlmesh-0.6.4/sqlmesh/core/config/connection.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/config/loader.py` & `sqlmesh-0.6.4/sqlmesh/core/config/loader.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/config/model.py` & `sqlmesh-0.6.4/sqlmesh/core/config/model.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/config/root.py` & `sqlmesh-0.6.4/sqlmesh/core/config/root.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/config/scheduler.py` & `sqlmesh-0.6.4/sqlmesh/core/config/scheduler.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/console.py` & `sqlmesh-0.6.4/sqlmesh/core/console.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from rich.status import Status
 from rich.syntax import Syntax
 from rich.tree import Tree
 
 from sqlmesh.core.snapshot import Snapshot, SnapshotChangeCategory
 from sqlmesh.core.test import ModelTest
 from sqlmesh.utils import rich as srich
-from sqlmesh.utils.date import to_date
+from sqlmesh.utils.date import to_date, yesterday_ds
 
 if t.TYPE_CHECKING:
     import ipywidgets as widgets
 
     from sqlmesh.core.context_diff import ContextDiff
     from sqlmesh.core.plan import Plan
 
@@ -288,14 +288,17 @@
         self._prompt_categorize(plan, auto_apply)
         self._show_options_after_categorization(plan, auto_apply)
 
         if auto_apply:
             plan.apply()
 
     def _show_options_after_categorization(self, plan: Plan, auto_apply: bool) -> None:
+        if plan.forward_only and plan.new_snapshots:
+            self._prompt_effective_from(plan, auto_apply)
+
         if plan.requires_backfill:
             self._show_missing_dates(plan)
             self._prompt_backfill(plan, auto_apply)
         elif plan.context_diff.has_changes and not auto_apply:
             self._prompt_promote(plan)
 
     def _prompt_categorize(self, plan: Plan, auto_apply: bool) -> None:
@@ -344,30 +347,51 @@
             snapshot = plan.context_diff.snapshots[missing.snapshot_name]
             view_name = snapshot.qualified_view_name.for_environment(plan.environment_name)
             backfill.add(
                 f"{view_name}: {missing.format_missing_range(snapshot.model.interval_unit())}"
             )
         self._print(backfill)
 
+    def _prompt_effective_from(self, plan: Plan, auto_apply: bool) -> None:
+        if not plan.effective_from:
+            effective_from = self._prompt(
+                "Enter the effective date (eg. '1 year', '2020-01-01') to apply forward-only changes retroactively or blank to only apply them going forward once changes are deployed to prod"
+            )
+            if effective_from:
+                plan.effective_from = effective_from
+
+        if plan.is_dev and plan.effective_from:
+            plan.set_start(plan.effective_from)
+
     def _prompt_backfill(self, plan: Plan, auto_apply: bool) -> None:
         is_forward_only_dev = plan.is_dev and plan.forward_only
         backfill_or_preview = "preview" if is_forward_only_dev else "backfill"
 
         if plan.is_start_and_end_allowed:
             if not plan.override_start:
-                blank_meaning = (
-                    "to preview starting from yesterday"
-                    if is_forward_only_dev
-                    else "for the beginning of history"
-                )
+                if is_forward_only_dev:
+                    if plan.effective_from:
+                        blank_meaning = (
+                            f"to preview starting from the effective date ('{plan.effective_from}')"
+                        )
+                        default_start = plan.effective_from
+                    else:
+                        blank_meaning = "to preview starting from yesterday"
+                        default_start = yesterday_ds()
+                else:
+                    blank_meaning = "to backfill from the beginning of history"
+                    default_start = None
+
                 start = self._prompt(
                     f"Enter the {backfill_or_preview} start date (eg. '1 year', '2020-01-01') or blank {blank_meaning}",
                 )
                 if start:
                     plan.start = start
+                elif default_start:
+                    plan.start = default_start
 
             if not plan.override_end:
                 end = self._prompt(
                     f"Enter the {backfill_or_preview} end date (eg. '1 month ago', '2020-01-01') or blank to {backfill_or_preview} up until now",
                 )
                 if end:
                     plan.end = end
@@ -529,14 +553,56 @@
         output = widgets.Output()
         self._add_to_dynamic_options(output)
 
         button.plan = plan
         button.on_click(self._apply)
         button.output = output
 
+    def _prompt_effective_from(self, plan: Plan, auto_apply: bool) -> None:
+        import ipywidgets as widgets
+
+        prompt = widgets.VBox()
+
+        def effective_from_change_callback(change: t.Dict[str, datetime.datetime]) -> None:
+            plan.effective_from = change["new"]
+            self._show_options_after_categorization(plan, auto_apply)
+
+        def going_forward_change_callback(change: t.Dict[str, bool]) -> None:
+            checked = change["new"]
+            plan.effective_from = None if checked else yesterday_ds()
+            self._show_options_after_categorization(plan, auto_apply=auto_apply)
+
+        date_picker = widgets.DatePicker(
+            disabled=plan.effective_from is None,
+            value=to_date(plan.effective_from or yesterday_ds()),
+            layout={"width": "auto"},
+        )
+        date_picker.observe(effective_from_change_callback, "value")
+
+        going_forward_checkbox = widgets.Checkbox(
+            value=plan.effective_from is None,
+            description="Apply Going Forward Once Deployed To Prod",
+            disabled=False,
+            indent=False,
+        )
+        going_forward_checkbox.observe(going_forward_change_callback, "value")
+
+        add_to_layout_widget(
+            prompt,
+            widgets.HBox(
+                [
+                    widgets.Label("Effective From Date:", layout={"width": "8rem"}),
+                    date_picker,
+                    going_forward_checkbox,
+                ]
+            ),
+        )
+
+        self._add_to_dynamic_options(prompt)
+
     def _prompt_backfill(self, plan: Plan, auto_apply: bool) -> None:
         import ipywidgets as widgets
 
         prompt = widgets.VBox()
 
         backfill_or_preview = "Preview" if plan.is_dev and plan.forward_only else "Backfill"
 
@@ -548,25 +614,14 @@
                 value=value,
                 layout={"width": "auto"},
             )
 
             picker.observe(on_change, "value")
             return picker
 
-        def _checkbox(description: str, value: bool, on_change: t.Callable) -> widgets.Checkbox:
-            checkbox = widgets.Checkbox(
-                value=value,
-                description=description,
-                disabled=False,
-                indent=False,
-            )
-
-            checkbox.observe(on_change, "value")
-            return checkbox
-
         def start_change_callback(change: t.Dict[str, datetime.datetime]) -> None:
             plan.start = change["new"]
             self._show_options_after_categorization(plan, auto_apply)
 
         def end_change_callback(change: t.Dict[str, datetime.datetime]) -> None:
             plan.end = change["new"]
             self._show_options_after_categorization(plan, auto_apply)
```

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/context.py` & `sqlmesh-0.6.4/sqlmesh/core/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -580,14 +580,15 @@
         restate_models: t.Optional[t.Iterable[str]] = None,
         no_gaps: bool = False,
         skip_backfill: bool = False,
         forward_only: bool = False,
         no_prompts: bool = False,
         auto_apply: bool = False,
         no_auto_categorization: t.Optional[bool] = None,
+        effective_from: t.Optional[TimeLike] = None,
     ) -> Plan:
         """Interactively create a migration plan.
 
         This method compares the current context with an environment. It then presents
         the differences and asks whether to backfill each modified model.
 
         Args:
@@ -612,14 +613,15 @@
             no_prompts: Whether to disable interactive prompts for the backfill time range. Please note that
                 if this flag is set to true and there are uncategorized changes the plan creation will
                 fail. Default: False.
             auto_apply: Whether to automatically apply the new plan after creation. Default: False.
             no_auto_categorization: Indicates whether to disable automatic categorization of model
                 changes (breaking / non-breaking). If not provided, then the corresponding configuration
                 option determines the behavior.
+            effective_from: The effective date from which to apply forward-only changes on production.
 
         Returns:
             The populated Plan object.
         """
         environment = environment or c.PROD
         environment = Environment.normalize_name(environment)
 
@@ -641,14 +643,15 @@
             no_gaps=no_gaps,
             skip_backfill=skip_backfill,
             is_dev=environment != c.PROD,
             forward_only=forward_only,
             environment_ttl=self.environment_ttl,
             categorizer_config=self.auto_categorize_changes,
             auto_categorization_enabled=not no_auto_categorization,
+            effective_from=effective_from,
         )
 
         if not no_prompts:
             self.console.plan(plan, auto_apply)
         elif auto_apply:
             self.apply(plan)
```

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/context_diff.py` & `sqlmesh-0.6.4/sqlmesh/core/context_diff.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/dialect.py` & `sqlmesh-0.6.4/sqlmesh/core/dialect.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import typing as t
 from difflib import unified_diff
 
 import pandas as pd
 from jinja2.meta import find_undeclared_variables
 from sqlglot import Dialect, Generator, Parser, TokenType, exp
 
+from sqlmesh.core.constants import MAX_MODEL_DEFINITION_SIZE
 from sqlmesh.utils.jinja import ENVIRONMENT
 
 
 class Model(exp.Expression):
     arg_types = {"expressions": True}
 
 
@@ -392,15 +393,15 @@
     Args:
         sql: The sql based definition.
         default_dialect: The dialect to use if the model does not specify one.
 
     Returns:
         A list of the expressions, [Model, *Statements, Query | Jinja]
     """
-    match = DIALECT_PATTERN.search(sql)
+    match = DIALECT_PATTERN.search(sql[:MAX_MODEL_DEFINITION_SIZE])
     dialect = Dialect.get_or_raise(match.group(2) if match else default_dialect)()
 
     tokens = dialect.tokenizer.tokenize(sql)
     chunks: t.List[t.Tuple[t.List, bool]] = [([], False)]
     total = len(tokens)
 
     for i, token in enumerate(tokens):
@@ -413,24 +414,19 @@
                 and token.token_type == TokenType.L_BRACE
                 and tokens[i + 1].token_type == TokenType.L_BRACE
             ):
                 chunks[-1] = (chunks[-1][0], True)
             chunks[-1][0].append(token)
 
     expressions: t.List[exp.Expression] = []
-    sql_lines = None
 
     for chunk, is_jinja in chunks:
         if is_jinja:
             start, *_, end = chunk
-            sql_lines = sql_lines or sql.split("\n")
-            lines = sql_lines[start.line - 1 : end.line]
-            lines[0] = lines[0][start.col - 1 :]
-            lines[-1] = lines[-1][: end.col + len(end.text) - 1]
-            segment = "\n".join(lines)
+            segment = sql[start.start : end.end + 1]
             variables = [
                 exp.Literal.string(var)
                 for var in find_undeclared_variables(ENVIRONMENT.parse(segment))
             ]
             expressions.append(Jinja(this=exp.Literal.string(segment), expressions=variables))
         else:
             for expression in dialect.parser().parse(chunk, sql):
```

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/engine_adapter/__init__.py` & `sqlmesh-0.6.4/sqlmesh/core/engine_adapter/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/engine_adapter/_typing.py` & `sqlmesh-0.6.4/sqlmesh/core/engine_adapter/_typing.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/engine_adapter/base.py` & `sqlmesh-0.6.4/sqlmesh/core/engine_adapter/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -639,17 +639,18 @@
             )
         )
 
     def merge(
         self,
         target_table: TableName,
         source_table: QueryOrDF,
-        column_names: t.Sequence[str],
+        columns_to_types: t.Dict[str, exp.DataType],
         unique_key: t.Sequence[str],
     ) -> None:
+        column_names = columns_to_types.keys()
         on = exp.and_(
             *(
                 exp.EQ(
                     this=exp.column(part, TARGET_ALIAS),
                     expression=exp.column(part, SOURCE_ALIAS),
                 )
                 for part in unique_key
```

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/engine_adapter/base_postgres.py` & `sqlmesh-0.6.4/sqlmesh/core/engine_adapter/base_postgres.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/engine_adapter/base_spark.py` & `sqlmesh-0.6.4/sqlmesh/core/engine_adapter/base_spark.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/engine_adapter/bigquery.py` & `sqlmesh-0.6.4/sqlmesh/core/engine_adapter/bigquery.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/engine_adapter/databricks_api.py` & `sqlmesh-0.6.4/sqlmesh/core/engine_adapter/databricks_api.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/engine_adapter/duckdb.py` & `sqlmesh-0.6.4/sqlmesh/core/engine_adapter/duckdb.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/engine_adapter/postgres.py` & `sqlmesh-0.6.4/sqlmesh/core/engine_adapter/postgres.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/engine_adapter/redshift.py` & `sqlmesh-0.6.4/sqlmesh/core/engine_adapter/redshift.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     from sqlmesh.core._typing import TableName
     from sqlmesh.core.engine_adapter._typing import QueryOrDF
 
 
 class RedshiftEngineAdapter(BasePostgresEngineAdapter):
     DIALECT = "redshift"
     DEFAULT_BATCH_SIZE = 1000
+    ESCAPE_JSON = True
 
     @property
     def cursor(self) -> t.Any:
         connection = self._connection_pool.get()
         # The SQLMesh implementation relies on autocommit being set to True
         connection.autocommit = True
         cursor = self._connection_pool.get_cursor()
```

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/engine_adapter/shared.py` & `sqlmesh-0.6.4/sqlmesh/core/engine_adapter/shared.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/engine_adapter/snowflake.py` & `sqlmesh-0.6.4/sqlmesh/core/engine_adapter/snowflake.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/engine_adapter/spark.py` & `sqlmesh-0.6.4/sqlmesh/core/engine_adapter/spark.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,26 +59,27 @@
         else:
             super().insert_append(table_name, query_or_df, columns_to_types, contains_json)
 
     def merge(
         self,
         target_table: TableName,
         source_table: QueryOrDF,
-        column_names: t.Sequence[str],
+        columns_to_types: t.Dict[str, exp.DataType],
         unique_key: t.Sequence[str],
     ) -> None:
+        column_names = columns_to_types.keys()
         if isinstance(source_table, PySparkDataFrame):
             temp_view_name = self._get_temp_table(target_table, table_only=True).sql(
                 dialect=self.dialect
             )
             source_table.createOrReplaceTempView(temp_view_name)
             query = exp.select(*column_names).from_(temp_view_name)
-            super().merge(target_table, query, column_names, unique_key)
+            super().merge(target_table, query, columns_to_types, unique_key)
         else:
-            super().merge(target_table, source_table, column_names, unique_key)
+            super().merge(target_table, source_table, columns_to_types, unique_key)
 
     def _insert_append_pandas_df(
         self,
         table_name: TableName,
         df: pd.DataFrame,
         columns_to_types: t.Optional[t.Dict[str, exp.DataType]] = None,
     ) -> None:
```

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/environment.py` & `sqlmesh-0.6.4/sqlmesh/core/environment.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/hooks.py` & `sqlmesh-0.6.4/sqlmesh/core/hooks.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/loader.py` & `sqlmesh-0.6.4/sqlmesh/core/loader.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/macros.py` & `sqlmesh-0.6.4/sqlmesh/core/macros.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,22 +184,26 @@
         if result is None:
             return None
 
         if isinstance(result, list):
             return [exp.convert(item) for item in result if item is not None]
         return exp.convert(result)
 
-    def eval_expression(self, node: exp.Expression) -> t.Any:
+    def eval_expression(self, node: t.Any) -> t.Any:
         """Converts a SQLGlot expression into executable Python code and evals it.
 
+        If the node is not an expression, it will simply be returned.
+
         Args:
             node: expression
         Returns:
             The return value of the evaled Python Code.
         """
+        if not isinstance(node, exp.Expression):
+            return node
         code = node.sql()
         try:
             code = self.generator.generate(node)
             return eval(code, self.env, self.locals)
         except Exception as e:
             print_exception(e, self.python_env)
             raise MacroEvalError(
@@ -329,14 +333,39 @@
         A list of items that is the result of func
     """
     *items, func = args
     items, func = _norm_var_arg_lambda(evaluator, func, *items)  # type: ignore
     return [item for item in map(func, ensure_collection(items)) if item is not None]
 
 
+@macro("IF")
+def if_(
+    evaluator: MacroEvaluator,
+    condition: t.Any,
+    true: t.Any,
+    false: t.Any = None,
+) -> t.Any:
+    """Evaluates a given condition and returns the second argument if true or else the third argument.
+
+    If false is not passed in, the default return value will be None.
+
+    Example:
+        >>> from sqlglot import parse_one
+        >>> from sqlmesh.core.macros import MacroEvaluator
+        >>> MacroEvaluator().transform(parse_one("@IF('a' = 1, a, b)")).sql()
+        'b'
+
+        >>> MacroEvaluator().transform(parse_one("@IF('a' = 1, a)"))
+    """
+
+    if evaluator.eval_expression(condition):
+        return true
+    return false
+
+
 @macro("REDUCE")
 def reduce_(evaluator: MacroEvaluator, *args: t.Any) -> t.Any:
     """Iterates through items applying provided function that takes two arguments
     cumulatively to the items of iterable items, from left to right, so as to reduce
     the iterable to a single item.
 
     Example:
```

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/model/__init__.py` & `sqlmesh-0.6.4/sqlmesh/core/model/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/model/cache.py` & `sqlmesh-0.6.4/sqlmesh/core/model/cache.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/model/common.py` & `sqlmesh-0.6.4/sqlmesh/core/model/common.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/model/decorator.py` & `sqlmesh-0.6.4/sqlmesh/core/model/decorator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/model/definition.py` & `sqlmesh-0.6.4/sqlmesh/core/model/definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -825,25 +825,17 @@
                 df_or_iter = [df_or_iter]
 
             for df in df_or_iter:
                 if self.kind.is_incremental_by_time_range:
                     assert self.time_column
 
                     if PySparkDataFrame is not None and isinstance(df, PySparkDataFrame):
-                        import pyspark
-
                         df = df.where(
-                            pyspark.sql.functions.col(self.time_column.column).between(
-                                pyspark.sql.functions.lit(
-                                    self.convert_to_time_column(start).sql("spark")
-                                ),
-                                pyspark.sql.functions.lit(
-                                    self.convert_to_time_column(end).sql("spark")
-                                ),
-                            )
+                            f"{self.time_column.column} BETWEEN {self.convert_to_time_column(start).sql('spark')} "
+                            f"AND {self.convert_to_time_column(end).sql('spark')}"
                         )
                     else:
                         assert self.time_column.format, "Time column format is required."
                         df = filter_df_by_timelike(
                             df, self.time_column.column, self.time_column.format, start, end
                         )
                 yield df
@@ -1304,8 +1296,11 @@
     "depends_on_": lambda value: exp.Tuple(expressions=value),
     "pre": _list_of_calls_to_exp,
     "post": _list_of_calls_to_exp,
     "audits": _list_of_calls_to_exp,
     "columns_to_types_": lambda value: exp.Schema(
         expressions=[exp.ColumnDef(this=exp.to_column(c), kind=t) for c, t in value.items()]
     ),
+    "tags": lambda value: (
+        exp.to_identifier(value[0]) if len(value) == 1 else exp.Tuple(expressions=value)
+    ),
 }
```

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/model/kind.py` & `sqlmesh-0.6.4/sqlmesh/core/model/kind.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/model/meta.py` & `sqlmesh-0.6.4/sqlmesh/core/model/meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     partitioned_by_: t.List[str] = Field(default=[], alias="partitioned_by")
     pre: t.List[HookCall] = []
     post: t.List[HookCall] = []
     depends_on_: t.Optional[t.Set[str]] = Field(default=None, alias="depends_on")
     columns_to_types_: t.Optional[t.Dict[str, exp.DataType]] = Field(default=None, alias="columns")
     column_descriptions_: t.Optional[t.Dict[str, str]]
     audits: t.List[AuditReference] = []
+    tags: t.List[str] = []
 
     _croniter: t.Optional[croniter] = None
     _interval_unit: t.Optional[IntervalUnit] = None
 
     _model_kind_validator = model_kind_validator
 
     @validator("audits", pre=True)
@@ -163,15 +164,15 @@
                             },
                         )
                     )
             return transformed
 
         return v
 
-    @validator("partitioned_by_", pre=True)
+    @validator("partitioned_by_", "tags", pre=True)
     def _value_or_tuple_validator(cls, v: t.Any) -> t.Any:
         if isinstance(v, (exp.Tuple, exp.Array)):
             return [e.name for e in v.expressions]
         if isinstance(v, exp.Expression):
             return [v.name]
         return v
```

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/model/seed.py` & `sqlmesh-0.6.4/sqlmesh/core/model/seed.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/notification_target.py` & `sqlmesh-0.6.4/sqlmesh/core/notification_target.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/plan/definition.py` & `sqlmesh-0.6.4/sqlmesh/core/plan/definition.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,14 +56,15 @@
             snapshots for same models.
         skip_backfill: Whether to skip the backfill step.
         is_dev: Whether this plan is for development purposes.
         forward_only: Whether the purpose of the plan is to make forward only changes.
         environment_ttl: The period of time that a development environment should exist before being deleted.
         categorizer_config: Auto categorization settings.
         auto_categorization_enabled: Whether to apply auto categorization.
+        effective_from: The effective date from which to apply forward-only changes on production.
     """
 
     def __init__(
         self,
         context_diff: ContextDiff,
         state_reader: StateReader,
         start: t.Optional[TimeLike] = None,
@@ -74,26 +75,28 @@
         no_gaps: bool = False,
         skip_backfill: bool = False,
         is_dev: bool = False,
         forward_only: bool = False,
         environment_ttl: t.Optional[str] = None,
         categorizer_config: t.Optional[CategorizerConfig] = None,
         auto_categorization_enabled: bool = True,
+        effective_from: t.Optional[TimeLike] = None,
     ):
         self.context_diff = context_diff
         self.override_start = start is not None
         self.override_end = end is not None
         self.plan_id: str = random_id()
         self.no_gaps = no_gaps
         self.skip_backfill = skip_backfill
         self.is_dev = is_dev
         self.forward_only = forward_only
         self.environment_ttl = environment_ttl
         self.categorizer_config = categorizer_config or CategorizerConfig()
         self.auto_categorization_enabled = auto_categorization_enabled
+        self._effective_from: t.Optional[TimeLike] = None
         self._start = start if start or not (is_dev and forward_only) else yesterday_ds()
         self._end = end if end or not is_dev else now()
         self._latest = latest or now()
         self._apply = apply
         self._dag: DAG[str] = DAG()
 
         for name, snapshot in self.context_diff.snapshots.items():
@@ -129,14 +132,17 @@
         self.indirectly_modified = directly_indirectly_modified[1]
 
         self._categorize_snapshots()
 
         self._categorized: t.Optional[t.List[Snapshot]] = None
         self._uncategorized: t.Optional[t.List[Snapshot]] = None
 
+        if effective_from:
+            self._set_effective_from(effective_from)
+
     @property
     def categorized(self) -> t.List[Snapshot]:
         """Returns the already categorized snapshots."""
         if self._categorized is None:
             self._categorized = [s for s in self.directly_modified if s.version]
         return self._categorized
 
@@ -316,14 +322,48 @@
                         break
 
         # Invalidate caches.
         self._categorized = None
         self._uncategorized = None
 
     @property
+    def effective_from(self) -> t.Optional[TimeLike]:
+        """The effective date for all new snapshots in the plan.
+
+        Note: this is only applicable for forward-only plans.
+
+        Returns:
+            The effective date.
+        """
+        return self._effective_from
+
+    @effective_from.setter
+    def effective_from(self, effective_from: t.Optional[TimeLike]) -> None:
+        """Sets the effective date for all new snapshots in the plan.
+
+        Note: this is only applicable for forward-only plans.
+
+        Args:
+            effective_from: The effective date to set.
+        """
+        self._set_effective_from(effective_from)
+
+    def _set_effective_from(self, effective_from: t.Optional[TimeLike]) -> None:
+        if not self.forward_only:
+            raise PlanError("Effective date can only be set for a forward-only plan.")
+        if effective_from and to_datetime(effective_from) > now():
+            raise PlanError("Effective date cannot be in the future.")
+
+        self.__missing_intervals = None
+        self._effective_from = effective_from
+
+        for snapshot in self.new_snapshots:
+            snapshot.effective_from = effective_from
+
+    @property
     def _missing_intervals(self) -> t.Dict[str, Intervals]:
         if self.__missing_intervals is None:
             previous_ids = [
                 SnapshotId(
                     name=snapshot.name,
                     identifier=snapshot.previous_version.fingerprint.to_identifier(),
                 )
```

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/plan/evaluator.py` & `sqlmesh-0.6.4/sqlmesh/core/plan/evaluator.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,40 +55,49 @@
     ):
         self.state_sync = state_sync
         self.snapshot_evaluator = snapshot_evaluator
         self.backfill_concurrent_tasks = backfill_concurrent_tasks
         self.console = console or get_console()
 
     def evaluate(self, plan: Plan) -> None:
-        self._push(plan)
+        tasks = (
+            [self._push, self._restate, self._backfill, self._promote]
+            if not plan.forward_only or plan.is_dev
+            else [self._push, self._restate, self._promote, self._backfill]
+        )
 
-        if plan.restatements:
-            self._restate(plan)
+        for task in tasks:
+            task(plan)
 
-        if plan.requires_backfill:
-            snapshots = plan.snapshots
-            scheduler = Scheduler(
-                snapshots,
-                self.snapshot_evaluator,
-                self.state_sync,
-                max_workers=self.backfill_concurrent_tasks,
-                console=self.console,
-            )
-            is_run_successful = scheduler.run(plan.environment_name, plan.start, plan.end)
-            if not is_run_successful:
-                raise SQLMeshError("Plan application failed.")
+        if not plan.requires_backfill:
+            self.console.log_success("Virtual Update executed successfully")
 
-        self._promote(plan)
+    def _backfill(self, plan: Plan) -> None:
+        """Backfill missing intervals for snapshots that are part of the given plan.
 
+        Args:
+            plan: The plan to source snapshots from.
+        """
         if not plan.requires_backfill:
-            self.console.log_success("Virtual Update executed successfully")
+            return
+
+        snapshots = plan.snapshots
+        scheduler = Scheduler(
+            snapshots,
+            self.snapshot_evaluator,
+            self.state_sync,
+            max_workers=self.backfill_concurrent_tasks,
+            console=self.console,
+        )
+        is_run_successful = scheduler.run(plan.environment_name, plan.start, plan.end)
+        if not is_run_successful:
+            raise SQLMeshError("Plan application failed.")
 
     def _push(self, plan: Plan) -> None:
-        """
-        Push the snapshots to the state sync.
+        """Push the snapshots to the state sync.
 
         As a part of plan pushing, snapshot tables are created.
 
         Args:
             plan: The plan to source snapshots from.
         """
         parent_snapshot_ids = {
@@ -139,14 +148,17 @@
             )
             self.state_sync.finalize(environment)
             completed = True
         finally:
             self.console.stop_promotion_progress(success=completed)
 
     def _restate(self, plan: Plan) -> None:
+        if not plan.restatements:
+            return
+
         all_snapshots = (
             [s for s in plan.snapshots if s.name in plan.restatements]
             if plan.is_dev
             else self.state_sync.get_snapshots_by_models(*plan.restatements)
         )
         self.state_sync.remove_interval(
             [],
@@ -194,14 +206,15 @@
             skip_backfill=plan.skip_backfill,
             restatements=plan.restatements,
             notification_targets=self.notification_targets,
             backfill_concurrent_tasks=self.backfill_concurrent_tasks,
             ddl_concurrent_tasks=self.ddl_concurrent_tasks,
             users=self.users,
             is_dev=plan.is_dev,
+            forward_only=plan.forward_only,
         )
 
         if self.blocking:
             plan_application_dag_id = airflow_common.plan_application_dag_id(
                 environment.name, plan_request_id
             )
```

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/renderer.py` & `sqlmesh-0.6.4/sqlmesh/core/renderer.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/scheduler.py` & `sqlmesh-0.6.4/sqlmesh/core/scheduler.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/schema_diff.py` & `sqlmesh-0.6.4/sqlmesh/core/schema_diff.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/snapshot/__init__.py` & `sqlmesh-0.6.4/sqlmesh/core/snapshot/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/snapshot/categorizer.py` & `sqlmesh-0.6.4/sqlmesh/core/snapshot/categorizer.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/snapshot/definition.py` & `sqlmesh-0.6.4/sqlmesh/core/snapshot/definition.py`

 * *Files 5% similar despite different names*

```diff
@@ -291,14 +291,16 @@
         previous: The snapshot data version that this snapshot was based on. If this snapshot is new, then previous will be None.
         version: User specified version for a snapshot that is used for physical storage.
             By default, the version is the fingerprint, but not all changes to models require a backfill.
             If a user passes a previous version, that will be used instead and no backfill will be required.
         change_category: User specified change category indicating which models require backfill from model changes made in this snapshot.
         unpaused_ts: The timestamp which indicates when this snapshot was unpaused. Unpaused means that
             this snapshot is evaluated on a recurring basis. None indicates that this snapshot is paused.
+        effective_from: The timestamp which indicates when this snapshot should be considered effective.
+            Applicable for forward-only snapshots only.
     """
 
     name: str
     fingerprint: SnapshotFingerprint
     physical_schema: str
     model: Model
     parents: t.Tuple[SnapshotId, ...]
@@ -311,14 +313,15 @@
     ttl: str
     previous_versions: t.Tuple[SnapshotDataVersion, ...] = ()
     indirect_versions: t.Dict[str, t.Tuple[SnapshotDataVersion, ...]] = {}
     version: t.Optional[str] = None
     temp_version: t.Optional[str] = None
     change_category: t.Optional[SnapshotChangeCategory] = None
     unpaused_ts: t.Optional[int] = None
+    effective_from: t.Optional[TimeLike] = None
 
     @validator("ttl")
     @classmethod
     def _time_delta_must_be_positive(cls, v: str) -> str:
         current_time = now()
         if to_datetime(v, current_time) < current_time:
             raise ValueError(
@@ -495,16 +498,24 @@
 
     def merge_intervals(self, other: Snapshot) -> None:
         """Inherits intervals from the target snapshot.
 
         Args:
             other: The target snapshot to inherit intervals from.
         """
+        effective_from_ts = self.normalized_effective_from_ts or 0
+        apply_effective_from = effective_from_ts > 0 and self.fingerprint != other.fingerprint
+
         for start, end in other.intervals:
-            self.add_interval(start, end)
+            # If the effective_from is set, then intervals that come after it must come from
+            # the current snapshost.
+            if apply_effective_from and start < effective_from_ts:
+                end = min(end, effective_from_ts)
+            if not apply_effective_from or end <= effective_from_ts:
+                self.add_interval(start, end)
 
     def missing_intervals(
         self, start: TimeLike, end: TimeLike, latest: t.Optional[TimeLike] = None
     ) -> Intervals:
         """Find all missing intervals between [start, end].
 
         Although the inputs are inclusive, the returned stored intervals are
@@ -693,14 +704,22 @@
     def is_materialized(self) -> bool:
         return self.model.kind.is_materialized
 
     @property
     def is_paused(self) -> bool:
         return self.unpaused_ts is None
 
+    @property
+    def normalized_effective_from_ts(self) -> t.Optional[int]:
+        return (
+            to_timestamp(self.model.cron_floor(self.effective_from))
+            if self.effective_from
+            else None
+        )
+
     def _ensure_categorized(self) -> None:
         if not self.change_category:
             raise SQLMeshError(f"Snapshot {self.snapshot_id} has not been categorized yet.")
         if not self.version:
             raise SQLMeshError(f"Snapshot {self.snapshot_id} has not been versioned yet.")
 
 
@@ -833,14 +852,15 @@
     metadata = [
         model.dialect,
         model.owner,
         model.description,
         str(model.start) if model.start else None,
         str(model.retention) if model.retention else None,
         str(model.batch_size) if model.batch_size is not None else None,
+        *model.tags,
     ]
 
     for audit_name, audit_args in sorted(model.audits, key=lambda a: a[0]):
         metadata.append(audit_name)
 
         if audit_name in BUILT_IN_AUDITS:
             for arg_name, arg_value in audit_args.items():
```

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/snapshot/evaluator.py` & `sqlmesh-0.6.4/sqlmesh/core/snapshot/evaluator.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,15 @@
                         time_column=model.time_column,
                         columns_to_types=columns_to_types,
                     )
                 elif snapshot.is_incremental_by_unique_key_kind:
                     self.adapter.merge(
                         table_name,
                         query_or_df,
-                        column_names=list(columns_to_types),
+                        columns_to_types=columns_to_types,
                         unique_key=model.unique_key,
                     )
                 else:
                     raise SQLMeshError(f"Unexpected SnapshotKind: {snapshot.model.kind}")
 
         for sql_statement in model.sql_statements:
             self.adapter.execute(sql_statement)
```

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/state_sync/__init__.py` & `sqlmesh-0.6.4/sqlmesh/core/state_sync/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/state_sync/base.py` & `sqlmesh-0.6.4/sqlmesh/core/state_sync/base.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/state_sync/common.py` & `sqlmesh-0.6.4/sqlmesh/core/state_sync/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -218,26 +218,52 @@
             snapshot.remove_interval(start, end)
             self._update_snapshot(snapshot)
 
     @transactional()
     def unpause_snapshots(
         self, snapshots: t.Iterable[SnapshotInfoLike], unpaused_dt: TimeLike
     ) -> None:
+        current_ts = now()
+
         target_snapshot_ids = {s.snapshot_id for s in snapshots}
         snapshots = self._get_snapshots_with_same_version(snapshots, lock_for_update=True)
+        target_snapshots_by_version = {
+            (s.name, s.version): s for s in snapshots if s.snapshot_id in target_snapshot_ids
+        }
+
         for snapshot in snapshots:
             is_target_snapshot = snapshot.snapshot_id in target_snapshot_ids
             if is_target_snapshot and not snapshot.unpaused_ts:
-                logger.info(f"Unpausing snapshot %s", snapshot.snapshot_id)
+                logger.info("Unpausing snapshot %s", snapshot.snapshot_id)
                 snapshot.set_unpaused_ts(unpaused_dt)
                 self._update_snapshot(snapshot)
-            elif not is_target_snapshot and snapshot.unpaused_ts:
-                logger.info(f"Pausing snapshot %s", snapshot.snapshot_id)
-                snapshot.set_unpaused_ts(None)
-                self._update_snapshot(snapshot)
+            elif not is_target_snapshot:
+                snapshot_updated = False
+
+                if snapshot.unpaused_ts:
+                    logger.info("Pausing snapshot %s", snapshot.snapshot_id)
+                    snapshot.set_unpaused_ts(None)
+                    snapshot_updated = True
+
+                target_snapshot = target_snapshots_by_version[(snapshot.name, snapshot.version)]
+                if target_snapshot.normalized_effective_from_ts:
+                    # Making sure that there are no overlapping intervals.
+                    effective_from_ts = target_snapshot.normalized_effective_from_ts
+                    if snapshot.intervals and snapshot.intervals[-1][1] > effective_from_ts:
+                        logger.info(
+                            "Removing all intervals after '%s' for snapshot %s, superseded by snapshot %s",
+                            target_snapshot.effective_from,
+                            snapshot.snapshot_id,
+                            target_snapshot.snapshot_id,
+                        )
+                        snapshot.remove_interval(effective_from_ts, current_ts)
+                        snapshot_updated = True
+
+                if snapshot_updated:
+                    self._update_snapshot(snapshot)
 
     def _ensure_no_gaps(
         self, target_snapshots: t.Iterable[Snapshot], target_environment: Environment
     ) -> None:
         from sqlmesh.core.scheduler import start_date
 
         target_snapshots_by_name = {s.name: s for s in target_snapshots}
```

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/state_sync/engine_adapter.py` & `sqlmesh-0.6.4/sqlmesh/core/state_sync/engine_adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -355,21 +355,25 @@
         if lock_for_update:
             query = query.lock(copy=False)
 
         snapshot_rows = self.engine_adapter.fetchall(query, ignore_unsupported_errors=True)
         return [Snapshot(**json.loads(row[0])) for row in snapshot_rows]
 
     def _get_versions(self, lock_for_update: bool = False) -> Versions:
+        no_version = Versions(schema_version=0, sqlglot_version="0.0.0")
+
         if not self.engine_adapter.table_exists(self.versions_table):
-            return Versions(schema_version=0, sqlglot_version="0.0.0")
+            return no_version
 
         query = exp.select("*").from_(self.versions_table)
         if lock_for_update:
             query.lock(copy=False)
         row = self.engine_adapter.fetchone(query)
+        if not row:
+            return no_version
         return Versions(schema_version=row[0], sqlglot_version=row[1])
 
     def _get_environment(
         self, environment: str, lock_for_update: bool = False
     ) -> t.Optional[Environment]:
         """Fetches the environment if it exists.
```

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/test.py` & `sqlmesh-0.6.4/sqlmesh/core/test.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/core/user.py` & `sqlmesh-0.6.4/sqlmesh/core/user.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/dbt/adapter.py` & `sqlmesh-0.6.4/sqlmesh/dbt/adapter.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/dbt/basemodel.py` & `sqlmesh-0.6.4/sqlmesh/dbt/basemodel.py`

 * *Files 3% similar despite different names*

```diff
@@ -98,14 +98,15 @@
         owner: The owner of the model.
         stamp: An optional arbitrary string sequence used to create new model versions without making
             changes to any of the functional components of the definition.
         storage_format: The storage format used to store the physical table, only applicable in certain engines.
             (eg. 'parquet')
         path: The file path of the model
         target_schema: The schema for the profile target
+        dependencies: The macro, source, var, and ref dependencies used to execute the model and its hooks
         database: Database the model is stored in
         schema: Custom schema name added to the model schema name
         alias: Relation identifier for this model instead of the filename
         pre-hook: List of SQL statements to run before the model is built
         post-hook: List of SQL statements to run after the model is built
         full_refresh: Forces the model to always do a full refresh or never do a full refresh
         grants: Set or revoke permissions to the database object for this model
@@ -218,14 +219,18 @@
         )
 
     @property
     def model_materialization(self) -> Materialization:
         return Materialization.TABLE
 
     @property
+    def model_dialect(self) -> t.Optional[str]:
+        return None
+
+    @property
     def relation_info(self) -> AttributeDict[str, t.Any]:
         if self.model_materialization == Materialization.VIEW:
             relation_type = RelationType.View
         elif self.model_materialization == Materialization.EPHEMERAL:
             relation_type = RelationType.CTE
         else:
             relation_type = RelationType.Table
@@ -239,20 +244,24 @@
                 "quote_policy": AttributeDict(self.quoting.dict()),
             }
         )
 
     def attribute_dict(self) -> AttributeDict[str, t.Any]:
         return AttributeDict(self.dict())
 
+    def model_function(self) -> AttributeDict[str, t.Any]:
+        return AttributeDict({"config": self.attribute_dict()})
+
     def sqlmesh_model_kwargs(self, model_context: DbtContext) -> t.Dict[str, t.Any]:
         """Get common sqlmesh model parameters"""
         jinja_macros = model_context.jinja_macros.trim(self.dependencies.macros)
         jinja_macros.global_objs.update(
             {
                 "this": self.relation_info,
+                "model": self.model_function(),
                 "schema": self.table_schema,
                 "config": self.attribute_dict(),
                 **model_context.jinja_globals,  # type: ignore
             }
         )
 
         optional_kwargs: t.Dict[str, t.Any] = {}
@@ -263,16 +272,28 @@
 
         return {
             "columns": column_types_to_sqlmesh(self.columns) or None,
             "column_descriptions_": column_descriptions_to_sqlmesh(self.columns) or None,
             "depends_on": {model_context.refs[ref] for ref in self.dependencies.refs},
             "jinja_macros": jinja_macros,
             "path": self.path,
-            "pre": [exp for hook in self.pre_hook for exp in d.parse(hook.sql)],
-            "post": [exp for hook in self.post_hook for exp in d.parse(hook.sql)],
+            "pre": [
+                exp
+                for hook in self.pre_hook
+                for exp in d.parse(
+                    hook.sql, default_dialect=self.model_dialect or model_context.dialect
+                )
+            ],
+            "post": [
+                exp
+                for hook in self.post_hook
+                for exp in d.parse(
+                    hook.sql, default_dialect=self.model_dialect or model_context.dialect
+                )
+            ],
             **optional_kwargs,
         }
 
     def render_config(self: BMC, context: DbtContext) -> BMC:
         rendered = super().render_config(context)
         rendered = ModelSqlRenderer(context, rendered).enriched_config
 
@@ -343,14 +364,15 @@
                 **context.jinja_globals,
                 **date_dict(c.EPOCH, c.EPOCH, c.EPOCH),
                 "config": lambda *args, **kwargs: "",
                 "ref": self._ref,
                 "var": self._var,
                 "source": self._source,
                 "this": self.config.relation_info,
+                "model": self.config.model_function(),
                 "schema": self.config.table_schema,
             },
             engine_adapter=None,
         )
 
         # Set the adapter separately since it requires jinja globals to passed into it.
         self._jinja_globals["adapter"] = ModelSqlRenderer.TrackingAdapter(
```

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/dbt/builtin.py` & `sqlmesh-0.6.4/sqlmesh/dbt/builtin.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/dbt/column.py` & `sqlmesh-0.6.4/sqlmesh/dbt/column.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/dbt/common.py` & `sqlmesh-0.6.4/sqlmesh/dbt/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from __future__ import annotations
 
 import typing as t
 from pathlib import Path
 
 from pydantic import Field, validator
+from ruamel.yaml.constructor import DuplicateKeyError
 from sqlglot.helper import ensure_list
 
 from sqlmesh.core.config.base import BaseConfig, UpdateStrategy
 from sqlmesh.utils.conversions import ensure_bool, try_str_to_bool
+from sqlmesh.utils.errors import ConfigError
 from sqlmesh.utils.yaml import load
 
 if t.TYPE_CHECKING:
     from sqlmesh.dbt.context import DbtContext
 
 
 T = t.TypeVar("T", bound="GeneralConfig")
@@ -30,15 +32,18 @@
     "statement",
     "store_result",
     "target",
 }
 
 
 def load_yaml(source: str | Path) -> t.OrderedDict:
-    return load(source, render_jinja=False, allow_duplicate_keys=True)
+    try:
+        return load(source, render_jinja=False)
+    except DuplicateKeyError as ex:
+        raise ConfigError(f"{source}: {ex}" if isinstance(source, Path) else f"{ex}")
 
 
 def parse_meta(v: t.Dict[str, t.Any]) -> t.Dict[str, t.Any]:
     for key, value in v.items():
         if isinstance(value, str):
             v[key] = try_str_to_bool(value)
```

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/dbt/context.py` & `sqlmesh-0.6.4/sqlmesh/dbt/context.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/dbt/loader.py` & `sqlmesh-0.6.4/sqlmesh/dbt/loader.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/dbt/model.py` & `sqlmesh-0.6.4/sqlmesh/dbt/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,16 +206,17 @@
                 if self._sql_embedded_config
                 else extracted
             )
             self._sql_no_config = SqlStr(self._sql_no_config.replace(extracted, "").strip())
 
     def to_sqlmesh(self, context: DbtContext) -> Model:
         """Converts the dbt model into a SQLMesh model."""
+        dialect = self.model_dialect or context.dialect
         model_context = self._context_for_dependencies(context, self.dependencies)
-        expressions = d.parse(self.sql_no_config)
+        expressions = d.parse(self.sql_no_config, default_dialect=dialect)
         if not expressions:
             raise ConfigError(f"Model '{self.table_name}' must have a query.")
 
         optional_kwargs: t.Dict[str, t.Any] = {}
         if self.partitioned_by:
             optional_kwargs["partitioned_by"] = self.partitioned_by
         for field in ["cron"]:
@@ -225,14 +226,14 @@
 
         if not context.target:
             raise ConfigError(f"Target required to load '{self.model_name}' into SQLMesh.")
 
         return create_sql_model(
             self.model_name,
             expressions[-1],
-            dialect=self.model_dialect or model_context.dialect,
+            dialect=dialect,
             kind=self.model_kind(context.target),
             start=self.start,
             statements=expressions[0:-1],
             **optional_kwargs,
             **self.sqlmesh_model_kwargs(model_context),
         )
```

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/dbt/package.py` & `sqlmesh-0.6.4/sqlmesh/dbt/package.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/dbt/profile.py` & `sqlmesh-0.6.4/sqlmesh/dbt/profile.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/dbt/project.py` & `sqlmesh-0.6.4/sqlmesh/dbt/project.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/dbt/seed.py` & `sqlmesh-0.6.4/sqlmesh/dbt/seed.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/dbt/source.py` & `sqlmesh-0.6.4/sqlmesh/dbt/source.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/dbt/target.py` & `sqlmesh-0.6.4/sqlmesh/dbt/target.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import abc
 import sys
 import typing as t
 
-from pydantic import Field, root_validator
+from pydantic import Field, root_validator, validator
 
 from sqlmesh.core.config.connection import (
     BigQueryConnectionConfig,
     BigQueryConnectionMethod,
     BigQueryPriority,
     ConnectionConfig,
     DatabricksSQLConnectionConfig,
@@ -206,14 +206,18 @@
         cls, values: t.Dict[str, t.Union[t.Tuple[str, ...], t.Optional[str], t.Dict[str, t.Any]]]
     ) -> t.Dict[str, t.Union[t.Tuple[str, ...], t.Optional[str], t.Dict[str, t.Any]]]:
         values["database"] = values.get("database") or values.get("dbname")
         if not values["database"]:
             raise ConfigError("Either database or dbname must be set")
         return values
 
+    @validator("port")
+    def _validate_port(cls, v: t.Union[int, str]) -> int:
+        return int(v)
+
     def default_incremental_strategy(self, kind: IncrementalKind) -> str:
         return "delete+insert" if kind is IncrementalByUniqueKeyKind else "append"
 
     def to_sqlmesh(self) -> ConnectionConfig:
         return PostgresConnectionConfig(
             host=self.host,
             user=self.user,
```

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/engines/commands.py` & `sqlmesh-0.6.4/sqlmesh/engines/commands.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/engines/spark/app.py` & `sqlmesh-0.6.4/sqlmesh/engines/spark/app.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/engines/spark/db_api/spark_session.py` & `sqlmesh-0.6.4/sqlmesh/engines/spark/db_api/spark_session.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/integrations/github/notification_operator_provider.py` & `sqlmesh-0.6.4/sqlmesh/integrations/github/notification_operator_provider.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/integrations/github/notification_target.py` & `sqlmesh-0.6.4/sqlmesh/integrations/github/notification_target.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/integrations/github/shared.py` & `sqlmesh-0.6.4/sqlmesh/integrations/github/shared.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/magics.py` & `sqlmesh-0.6.4/sqlmesh/magics.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,14 +210,19 @@
     )
     @argument(
         "--forward-only",
         action="store_true",
         help="Create a plan for forward-only changes.",
     )
     @argument(
+        "--effective-from",
+        type=str,
+        help="The effective date from which to apply forward-only changes on production.",
+    )
+    @argument(
         "--no-prompts",
         action="store_true",
         help="Disables interactive prompts for the backfill time range. Please note that if this flag is set and there are uncategorized changes, plan creation will fail.",
     )
     @argument(
         "--auto-apply",
         action="store_true",
@@ -249,14 +254,15 @@
             restate_models=args.restate_model,
             no_gaps=args.no_gaps,
             skip_backfill=args.skip_backfill,
             forward_only=args.forward_only,
             no_prompts=args.no_prompts,
             auto_apply=args.auto_apply,
             no_auto_categorization=args.no_auto_categorization,
+            effective_from=args.effective_from,
         )
         self._context.console = console
 
     @magic_arguments()
     @argument(
         "environment",
         nargs="?",
```

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/migrations/v0001_init.py` & `sqlmesh-0.6.4/sqlmesh/migrations/v0001_init.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/migrations/v0003_move_batch_size.py` & `sqlmesh-0.6.4/sqlmesh/migrations/v0003_move_batch_size.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/migrations/v0004_environmnent_add_finalized_at.py` & `sqlmesh-0.6.4/sqlmesh/migrations/v0004_environmnent_add_finalized_at.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/schedulers/airflow/api.py` & `sqlmesh-0.6.4/sqlmesh/schedulers/airflow/api.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/schedulers/airflow/client.py` & `sqlmesh-0.6.4/sqlmesh/schedulers/airflow/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,27 +51,29 @@
         skip_backfill: bool = False,
         restatements: t.Optional[t.Iterable[str]] = None,
         notification_targets: t.Optional[t.List[NotificationTarget]] = None,
         backfill_concurrent_tasks: int = 1,
         ddl_concurrent_tasks: int = 1,
         users: t.Optional[t.List[User]] = None,
         is_dev: bool = False,
+        forward_only: bool = False,
     ) -> None:
         request = common.PlanApplicationRequest(
             new_snapshots=list(new_snapshots),
             environment=environment,
             no_gaps=no_gaps,
             skip_backfill=skip_backfill,
             request_id=request_id,
             restatements=set(restatements or []),
             notification_targets=notification_targets or [],
             backfill_concurrent_tasks=backfill_concurrent_tasks,
             ddl_concurrent_tasks=ddl_concurrent_tasks,
             users=users or [],
             is_dev=is_dev,
+            forward_only=forward_only,
         )
 
         response = self._session.post(
             urljoin(self._airflow_url, PLANS_PATH),
             data=request.json(),
         )
         self._raise_for_status(response)
```

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/schedulers/airflow/common.py` & `sqlmesh-0.6.4/sqlmesh/schedulers/airflow/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     skip_backfill: bool
     restatements: t.Set[str]
     notification_targets: t.List[NotificationTarget]
     backfill_concurrent_tasks: int
     ddl_concurrent_tasks: int
     users: t.List[User]
     is_dev: bool
+    forward_only: bool
 
 
 class BackfillIntervalsPerSnapshot(PydanticModel):
     snapshot_id: SnapshotId
     intervals: t.List[Interval]
 
 
@@ -70,14 +71,15 @@
     plan_id: str
     previous_plan_id: t.Optional[str]
     notification_targets: t.List[NotificationTarget]
     backfill_concurrent_tasks: int
     ddl_concurrent_tasks: int
     users: t.List[User]
     is_dev: bool
+    forward_only: t.Optional[bool]
     environment_expiration_ts: t.Optional[int]
 
 
 class EnvironmentsResponse(PydanticModel):
     environments: t.List[Environment]
```

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/schedulers/airflow/dag_generator.py` & `sqlmesh-0.6.4/sqlmesh/schedulers/airflow/dag_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,28 +162,34 @@
 
             (
                 promote_start_task,
                 promote_end_task,
             ) = self._create_promotion_demotion_tasks(plan_dag_spec)
 
             start_task >> create_start_task
-            create_end_task >> backfill_start_task
-            backfill_end_task >> promote_start_task
+            if not plan_dag_spec.forward_only or plan_dag_spec.is_dev:
+                create_end_task >> backfill_start_task
+                backfill_end_task >> promote_start_task
+                latest_end_task = promote_end_task
+            else:
+                create_end_task >> promote_start_task
+                promote_end_task >> backfill_start_task
+                latest_end_task = backfill_end_task
 
             self._add_notification_target_tasks(
-                plan_dag_spec, start_task, end_task, promote_end_task
+                plan_dag_spec, start_task, end_task, latest_end_task
             )
             return dag
 
     def _add_notification_target_tasks(
         self,
         request: common.PlanDagSpec,
         start_task: BaseOperator,
         end_task: BaseOperator,
-        promote_end_task: BaseOperator,
+        previous_end_task: BaseOperator,
     ) -> None:
         has_success_or_failed_notification = False
         for notification_target in request.notification_targets:
             notification_operator_provider = NOTIFICATION_TARGET_TO_OPERATOR_PROVIDER.get(
                 type(notification_target)
             )
             if not notification_operator_provider:
@@ -197,22 +203,22 @@
             plan_failed_notification_task = notification_operator_provider.operator(
                 notification_target, PlanStatus.FAILED, request
             )
             if plan_start_notification_task:
                 start_task >> plan_start_notification_task
             if plan_success_notification_task:
                 has_success_or_failed_notification = True
-                promote_end_task >> plan_success_notification_task
+                previous_end_task >> plan_success_notification_task
                 plan_success_notification_task >> end_task
             if plan_failed_notification_task:
                 has_success_or_failed_notification = True
-                promote_end_task >> plan_failed_notification_task
+                previous_end_task >> plan_failed_notification_task
                 plan_failed_notification_task >> end_task
         if not has_success_or_failed_notification:
-            promote_end_task >> end_task
+            previous_end_task >> end_task
 
     def _create_creation_tasks(
         self, new_snapshots: t.List[Snapshot], ddl_concurrent_tasks: int
     ) -> t.Tuple[BaseOperator, BaseOperator]:
         start_task = EmptyOperator(task_id="snapshot_creation_start")
         end_task = EmptyOperator(task_id="snapshot_creation_end")
```

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/schedulers/airflow/hooks/bigquery.py` & `sqlmesh-0.6.4/sqlmesh/schedulers/airflow/hooks/bigquery.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/schedulers/airflow/hooks/redshift.py` & `sqlmesh-0.6.4/sqlmesh/schedulers/airflow/hooks/redshift.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/schedulers/airflow/integration.py` & `sqlmesh-0.6.4/sqlmesh/schedulers/airflow/integration.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/schedulers/airflow/operators/bigquery.py` & `sqlmesh-0.6.4/sqlmesh/schedulers/airflow/operators/bigquery.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/schedulers/airflow/operators/databricks.py` & `sqlmesh-0.6.4/sqlmesh/schedulers/airflow/operators/databricks.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/schedulers/airflow/operators/hwm_sensor.py` & `sqlmesh-0.6.4/sqlmesh/schedulers/airflow/operators/hwm_sensor.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/schedulers/airflow/operators/notification.py` & `sqlmesh-0.6.4/sqlmesh/schedulers/airflow/operators/notification.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/schedulers/airflow/operators/postgres.py` & `sqlmesh-0.6.4/sqlmesh/schedulers/airflow/operators/postgres.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/schedulers/airflow/operators/redshift.py` & `sqlmesh-0.6.4/sqlmesh/schedulers/airflow/operators/redshift.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/schedulers/airflow/operators/snowflake.py` & `sqlmesh-0.6.4/sqlmesh/schedulers/airflow/operators/snowflake.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/schedulers/airflow/operators/spark_submit.py` & `sqlmesh-0.6.4/sqlmesh/schedulers/airflow/operators/spark_submit.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/schedulers/airflow/operators/targets.py` & `sqlmesh-0.6.4/sqlmesh/schedulers/airflow/operators/targets.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/schedulers/airflow/plan.py` & `sqlmesh-0.6.4/sqlmesh/schedulers/airflow/plan.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,21 +47,26 @@
                 previous_snapshot_ids = all_snapshots_by_version[(s.name, s.version)] - {
                     s.snapshot_id
                 }
                 for sid in previous_snapshot_ids:
                     snapshots_for_intervals.pop(sid)
 
     if request.restatements:
+        snapshots_for_restatement = (
+            snapshots_for_intervals.values()
+            if not request.is_dev
+            else [snapshots_for_intervals[s.snapshot_id] for s in request.environment.snapshots]
+        )
         state_sync.remove_interval(
             [],
             start=request.environment.start_at,
             end=end,
             all_snapshots=(
                 snapshot
-                for snapshot in snapshots_for_intervals.values()
+                for snapshot in snapshots_for_restatement
                 if snapshot.name in request.restatements
                 and snapshot.snapshot_id not in new_snapshots
             ),
         )
 
     if not request.skip_backfill:
         backfill_batches = scheduler.compute_interval_params(
@@ -96,14 +101,15 @@
         plan_id=request.environment.plan_id,
         previous_plan_id=request.environment.previous_plan_id,
         notification_targets=request.notification_targets,
         backfill_concurrent_tasks=request.backfill_concurrent_tasks,
         ddl_concurrent_tasks=request.ddl_concurrent_tasks,
         users=request.users,
         is_dev=request.is_dev,
+        forward_only=request.forward_only,
         environment_expiration_ts=request.environment.expiration_ts,
     )
 
 
 def _get_demoted_snapshots(
     new_environment: Environment, state_sync: StateSync
 ) -> t.List[SnapshotTableInfo]:
```

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/schedulers/airflow/plugin.py` & `sqlmesh-0.6.4/sqlmesh/schedulers/airflow/plugin.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/schedulers/airflow/state_sync.py` & `sqlmesh-0.6.4/sqlmesh/schedulers/airflow/state_sync.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/schedulers/airflow/util.py` & `sqlmesh-0.6.4/sqlmesh/schedulers/airflow/util.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/utils/__init__.py` & `sqlmesh-0.6.4/sqlmesh/utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     def __init__(self, name: str = "") -> None:
         self.name = name
 
     def __call__(
         self, func: t.Callable[..., DECORATOR_RETURN_TYPE]
     ) -> t.Callable[..., DECORATOR_RETURN_TYPE]:
         self.func = func
-        self.registry()[(self.name or func.__name__)] = self
+        self.registry()[(self.name or func.__name__).lower()] = self
 
         @wraps(func)
         def wrapper(*args: t.Any, **kwargs: t.Any) -> DECORATOR_RETURN_TYPE:
             return func(*args, **kwargs)
 
         return wrapper
```

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/utils/cache.py` & `sqlmesh-0.6.4/sqlmesh/utils/cache.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/utils/concurrency.py` & `sqlmesh-0.6.4/sqlmesh/utils/concurrency.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/utils/connection_pool.py` & `sqlmesh-0.6.4/sqlmesh/utils/connection_pool.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/utils/dag.py` & `sqlmesh-0.6.4/sqlmesh/utils/dag.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/utils/date.py` & `sqlmesh-0.6.4/sqlmesh/utils/date.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/utils/errors.py` & `sqlmesh-0.6.4/sqlmesh/utils/errors.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/utils/jinja.py` & `sqlmesh-0.6.4/sqlmesh/utils/jinja.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/utils/metaprogramming.py` & `sqlmesh-0.6.4/sqlmesh/utils/metaprogramming.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/utils/pandas.py` & `sqlmesh-0.6.4/sqlmesh/utils/pandas.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/utils/pydantic.py` & `sqlmesh-0.6.4/sqlmesh/utils/pydantic.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/utils/rich.py` & `sqlmesh-0.6.4/sqlmesh/utils/rich.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/utils/transactional_file.py` & `sqlmesh-0.6.4/sqlmesh/utils/transactional_file.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh/utils/yaml.py` & `sqlmesh-0.6.4/sqlmesh/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh.egg-info/PKG-INFO` & `sqlmesh-0.6.4/sqlmesh.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,14 @@
 Metadata-Version: 2.1
 Name: sqlmesh
-Version: 0.6.3.dev5
-Summary: UNKNOWN
+Version: 0.6.4
 Home-page: https://github.com/TobikoData/sqlmesh
 Author: TobikoData Inc.
 Author-email: engineering@tobikodata.com
 License: Apache License 2.0
-Description: ![SQLMesh logo](sqlmesh.svg)
-        
-        SQLMesh is a DataOps framework that brings the benefits of DevOps to data teams. It enables data scientists, analysts, and engineers to efficiently run and deploy data transformations written in SQL or Python.
-        
-        For more information, check out the [website](https://sqlmesh.com) and [documentation](https://sqlmesh.readthedocs.io/en/stable/).
-        
-        ## Geting Started
-        Install SQLMesh through [pypi](https://pypi.org/project/sqlmesh/) by running:
-        
-        ```pip install sqlmesh```
-        
-        Follow the [tutorial](https://sqlmesh.readthedocs.io/en/stable/quick_start/) to learn how to use SQLMesh.
-        
-        ## Join our community
-        We'd love to join you on your data journey. Connect with us in the following ways:
-        
-        * Join the [Tobiko Slack community](https://tobikodata.com/slack) to ask questions, or just to say hi!
-        * File an issue on our [GitHub](https://github.com/TobikoData/sqlmesh/issues/new).
-        * Send us an email at [hello@tobikodata.com](hello@tobikodata.com) with your questions or feedback.
-        
-        ## Contribution
-        Contributions in the form of issues or pull requests are greatly appreciated. [Read more](https://sqlmesh.readthedocs.io/en/stable/development/) about how to develop for SQLMesh.
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: SQL
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
@@ -41,7 +16,31 @@
 Provides-Extra: databricks
 Provides-Extra: dev
 Provides-Extra: dbt
 Provides-Extra: postgres
 Provides-Extra: redshift
 Provides-Extra: snowflake
 Provides-Extra: web
+License-File: LICENSE
+
+![SQLMesh logo](sqlmesh.svg)
+
+SQLMesh is a DataOps framework that brings the benefits of DevOps to data teams. It enables data scientists, analysts, and engineers to efficiently run and deploy data transformations written in SQL or Python.
+
+For more information, check out the [website](https://sqlmesh.com) and [documentation](https://sqlmesh.readthedocs.io/en/stable/).
+
+## Geting Started
+Install SQLMesh through [pypi](https://pypi.org/project/sqlmesh/) by running:
+
+```pip install sqlmesh```
+
+Follow the [tutorial](https://sqlmesh.readthedocs.io/en/stable/quick_start/) to learn how to use SQLMesh.
+
+## Join our community
+We'd love to join you on your data journey. Connect with us in the following ways:
+
+* Join the [Tobiko Slack community](https://tobikodata.com/slack) to ask questions, or just to say hi!
+* File an issue on our [GitHub](https://github.com/TobikoData/sqlmesh/issues/new).
+* Send us an email at [hello@tobikodata.com](hello@tobikodata.com) with your questions or feedback.
+
+## Contribution
+Contributions in the form of issues or pull requests are greatly appreciated. [Read more](https://sqlmesh.readthedocs.io/en/stable/development/) about how to develop for SQLMesh.
```

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh.egg-info/SOURCES.txt` & `sqlmesh-0.6.4/sqlmesh.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -430,14 +430,26 @@
 web/client/package-lock.json
 web/client/package.json
 web/client/playwright.config.ts
 web/client/postcss.config.js
 web/client/tailwind.config.js
 web/client/tsconfig.json
 web/client/vite.config.ts
+web/client/dist/index.html
+web/client/dist/assets/CircularStd-Black-52659624.otf
+web/client/dist/assets/CircularStd-Bold-0e6c076d.otf
+web/client/dist/assets/CircularStd-Medium-2f373e53.otf
+web/client/dist/assets/Plan-683a0552.js
+web/client/dist/assets/Publico-Black-e6bd2ea2.otf
+web/client/dist/assets/Publico-Bold-c79acd56.otf
+web/client/dist/assets/Publico-Medium-01b4a891.otf
+web/client/dist/assets/index-b61dbb6f.css
+web/client/dist/assets/index-f2c4b7c5.js
+web/client/dist/assets/worker-e891d118.js
+web/client/dist/favicons/favicon.ico
 web/client/public/favicons/favicon.ico
 web/client/src/index.css
 web/client/src/main.tsx
 web/client/src/routes.tsx
 web/client/src/api/channels.ts
 web/client/src/api/index.ts
 web/client/src/api/instance.ts
@@ -491,14 +503,15 @@
 web/client/src/library/components/editor/help.ts
 web/client/src/library/components/editor/extensions/SqlMeshDialect.ts
 web/client/src/library/components/editor/extensions/index.ts
 web/client/src/library/components/fileTree/Directory.tsx
 web/client/src/library/components/fileTree/File.tsx
 web/client/src/library/components/fileTree/FileTree.tsx
 web/client/src/library/components/fileTree/help.ts
+web/client/src/library/components/graph/Graph.css
 web/client/src/library/components/graph/Graph.tsx
 web/client/src/library/components/graph/help.ts
 web/client/src/library/components/ide/ActivePlan.tsx
 web/client/src/library/components/ide/IDE.tsx
 web/client/src/library/components/ide/RunPlan.tsx
 web/client/src/library/components/input/Input.tsx
 web/client/src/library/components/input/InputToggle.tsx
```

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh.egg-info/requires.txt` & `sqlmesh-0.6.4/sqlmesh.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 hyperscript
 jinja2
 pandas
 pydantic<2.0.0,>=1.9.1
 requests
 rich
 ruamel.yaml
-sqlglot~=11.5.7
+sqlglot~=11.6.3
 fsspec
 
 [bigquery]
 google-cloud-bigquery[pandas]
 google-cloud-bigquery-storage
 
 [databricks]
```

### Comparing `sqlmesh-0.6.3.dev5/sqlmesh.svg` & `sqlmesh-0.6.4/sqlmesh.svg`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/tests/conftest.py` & `sqlmesh-0.6.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/tests/core/engine_adapter/test_base.py` & `sqlmesh-0.6.4/tests/core/engine_adapter/test_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -578,28 +578,36 @@
     cursor_mock = mocker.Mock()
     connection_mock.cursor.return_value = cursor_mock
 
     adapter = EngineAdapter(lambda: connection_mock, "")  # type: ignore
     adapter.merge(
         target_table="target",
         source_table="SELECT id, ts, val FROM source",
-        column_names=["id", "ts", "val"],
+        columns_to_types={
+            "id": exp.DataType.Type.INT,
+            "ts": exp.DataType.Type.TIMESTAMP,
+            "val": exp.DataType.Type.INT,
+        },
         unique_key=["id"],
     )
     cursor_mock.execute.assert_called_once_with(
         "MERGE INTO target AS __MERGE_TARGET__ USING (SELECT id, ts, val FROM source) AS __MERGE_SOURCE__ ON __MERGE_TARGET__.id = __MERGE_SOURCE__.id "
         "WHEN MATCHED THEN UPDATE SET __MERGE_TARGET__.id = __MERGE_SOURCE__.id, __MERGE_TARGET__.ts = __MERGE_SOURCE__.ts, __MERGE_TARGET__.val = __MERGE_SOURCE__.val "
         "WHEN NOT MATCHED THEN INSERT (id, ts, val) VALUES (__MERGE_SOURCE__.id, __MERGE_SOURCE__.ts, __MERGE_SOURCE__.val)"
     )
 
     cursor_mock.reset_mock()
     adapter.merge(
         target_table="target",
         source_table="SELECT id, ts, val FROM source",
-        column_names=["id", "ts", "val"],
+        columns_to_types={
+            "id": exp.DataType.Type.INT,
+            "ts": exp.DataType.Type.TIMESTAMP,
+            "val": exp.DataType.Type.INT,
+        },
         unique_key=["id", "ts"],
     )
     cursor_mock.execute.assert_called_once_with(
         "MERGE INTO target AS __MERGE_TARGET__ USING (SELECT id, ts, val FROM source) AS __MERGE_SOURCE__ ON __MERGE_TARGET__.id = __MERGE_SOURCE__.id AND __MERGE_TARGET__.ts = __MERGE_SOURCE__.ts "
         "WHEN MATCHED THEN UPDATE SET __MERGE_TARGET__.id = __MERGE_SOURCE__.id, __MERGE_TARGET__.ts = __MERGE_SOURCE__.ts, __MERGE_TARGET__.val = __MERGE_SOURCE__.val "
         "WHEN NOT MATCHED THEN INSERT (id, ts, val) VALUES (__MERGE_SOURCE__.id, __MERGE_SOURCE__.ts, __MERGE_SOURCE__.val)"
     )
```

### Comparing `sqlmesh-0.6.3.dev5/tests/core/engine_adapter/test_base_postgres.py` & `sqlmesh-0.6.4/tests/core/engine_adapter/test_base_postgres.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/tests/core/engine_adapter/test_base_spark.py` & `sqlmesh-0.6.4/tests/core/engine_adapter/test_base_spark.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/tests/core/engine_adapter/test_bigquery.py` & `sqlmesh-0.6.4/tests/core/engine_adapter/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/tests/core/engine_adapter/test_databricks.py` & `sqlmesh-0.6.4/tests/core/engine_adapter/test_databricks.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/tests/core/engine_adapter/test_duckdb.py` & `sqlmesh-0.6.4/tests/core/engine_adapter/test_duckdb.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/tests/core/engine_adapter/test_postgres.py` & `sqlmesh-0.6.4/tests/core/engine_adapter/test_postgres.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/tests/core/engine_adapter/test_redshift.py` & `sqlmesh-0.6.4/tests/core/engine_adapter/test_redshift.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/tests/core/engine_adapter/test_spark.py` & `sqlmesh-0.6.4/tests/core/engine_adapter/test_spark.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/tests/core/test_audit.py` & `sqlmesh-0.6.4/tests/core/test_audit.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/tests/core/test_config.py` & `sqlmesh-0.6.4/tests/core/test_config.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/tests/core/test_connection_config.py` & `sqlmesh-0.6.4/tests/core/test_connection_config.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/tests/core/test_context.py` & `sqlmesh-0.6.4/tests/core/test_context.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/tests/core/test_dialect.py` & `sqlmesh-0.6.4/tests/core/test_dialect.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/tests/core/test_integration.py` & `sqlmesh-0.6.4/tests/core/test_integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -624,15 +624,15 @@
     assert sushi_context.snapshots["sushi.waiter_as_customer_by_day"].version == version
 
 
 @pytest.mark.integration
 @pytest.mark.core_integration
 def test_multi(mocker):
     context = Context(paths=["examples/multi/repo_1", "examples/multi/repo_2"], config="memory")
-    context.state_sync.reset()
+    context._new_state_sync().reset()
     plan = context.plan()
     assert len(plan.new_snapshots) == 4
     context.apply(plan)
 
     context = Context(paths=["examples/multi/repo_1"], engine_adapter=context.engine_adapter)
     model = context.models["bronze.a"]
     model.query.select("'c' AS c", copy=False)
@@ -663,14 +663,15 @@
 ):
     plan_validators = plan_validators or []
     apply_validators = apply_validators or []
 
     plan = context.plan(
         environment,
         forward_only=choice == SnapshotChangeCategory.FORWARD_ONLY,
+        no_prompts=True,
     )
     plan.set_start(start(context))
 
     if choice:
         plan_choice(plan, choice)
     for validator in plan_validators:
         validator(context, plan)
```

### Comparing `sqlmesh-0.6.3.dev5/tests/core/test_macros.py` & `sqlmesh-0.6.4/tests/core/test_macros.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,22 +8,31 @@
 @macro()
 def filter_country(
     evaluator: MacroEvaluator, expression: exp.Condition, country: str
 ) -> exp.Condition:
     return exp.and_(expression, f"country = '{country}'")
 
 
+@macro("UPPER")
+def upper_case(evaluator: MacroEvaluator, expression: exp.Condition, country: str) -> exp.Condition:
+    return exp.true()
+
+
 @pytest.fixture
 def macro_evaluator() -> MacroEvaluator:
     return MacroEvaluator(
         "hive",
         {"test": Executable(name="test", payload=f"def test(_):\n    return 'test'")},
     )
 
 
+def test_case():
+    assert macro.get_registry()["upper"]
+
+
 def test_macro_var(macro_evaluator):
     expression = parse_one("@x")
     for k, v in [
         (1, "1"),
         ("1", "'1'"),
         (None, "NULL"),
         (True, "TRUE"),
@@ -155,12 +164,32 @@
             {"do_order": True},
         ),
         (
             """select * from city @ORDER_BY(@do_order) population, name DESC""",
             "SELECT * FROM city",
             {"do_order": False},
         ),
+        (
+            """select @if(TRUE, 1, 0)""",
+            "SELECT 1",
+            {},
+        ),
+        (
+            """select @if(FALSE, 1, 0)""",
+            "SELECT 0",
+            {},
+        ),
+        (
+            """select @if(1 > 0, 1, 0)""",
+            "SELECT 1",
+            {},
+        ),
+        (
+            """select @if('a' = 'b', c), d""",
+            "SELECT d",
+            {},
+        ),
     ],
 )
 def test_macro_functions(macro_evaluator, assert_exp_eq, sql, expected, args):
     macro_evaluator.locals = args or {}
     assert_exp_eq(macro_evaluator.transform(parse_one(sql)), expected)
```

### Comparing `sqlmesh-0.6.3.dev5/tests/core/test_model.py` & `sqlmesh-0.6.4/tests/core/test_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,14 +33,15 @@
             dialect spark,
             owner owner_name,
             storage_format iceberg,
             partitioned_by d,
             kind INCREMENTAL_BY_TIME_RANGE(
                 time_column a,
             ),
+            tags [tag_foo, tag_bar],
         );
 
         @DEF(x, 1);
         CACHE TABLE x AS SELECT 1;
         ADD JAR 's3://my_jar.jar';
 
         SELECT
@@ -97,14 +98,15 @@
         db.other_table t1
         LEFT JOIN
         db.table t2
         ON
             t1.a = t2.a
     """,
     )
+    assert model.tags == ["tag_foo", "tag_bar"]
 
 
 @pytest.mark.parametrize(
     "query, error",
     [
         ("y::int, x::int AS y", "duplicate"),
     ],
@@ -149,15 +151,15 @@
             kind FULL,
         );
 
         SELECT a, a UNION SELECT c, c
         """
     )
 
-    with pytest.raises(ConfigError, match=r"Found duplicate outer select name 'a'") as ex:
+    with pytest.raises(ConfigError, match=r"Found duplicate outer select name 'a'"):
         load_model(expressions)
 
 
 def test_partitioned_by():
     expressions = parse(
         """
         MODEL (
@@ -886,15 +888,15 @@
 
     model2 = load_model(
         d.parse(
             """
         MODEL (name db.model2, kind full);
 
         SELECT * FROM db.model1 AS model1
-		"""
+        """
         ),
     )
 
     model3 = load_model(
         d.parse(
             """
             MODEL(name db.model3, kind full);
@@ -906,15 +908,15 @@
 
     context.upsert_model(model1)
     context.upsert_model(model2)
     context.upsert_model(model3)
 
     assert_exp_eq(
         context.render("db.model2"),
-        f"""
+        """
         SELECT
           model1.id AS id,
           model1.item_id AS item_id,
           model1.ds AS ds
         FROM (
           SELECT
             CAST(t.id AS INT) AS id,
@@ -930,15 +932,15 @@
             (6, 1, '2020-01-06'),
             (7, 1, '2020-01-07')) AS t(id, item_id, ds)
         ) AS model1
         """,
     )
     assert_exp_eq(
         context.render("db.model3"),
-        f"""
+        """
         SELECT
           model2.id AS id,
           model2.item_id AS item_id,
           model2.ds AS ds
         FROM (
           SELECT
             model1.id AS id,
@@ -978,15 +980,15 @@
               alias varchar
             ),
             batch_size 100,
         );
     """
     )
 
-    with pytest.raises(ConfigError) as ex:
+    with pytest.raises(ConfigError):
         load_model(expressions, path=Path("./examples/sushi/models/test_model.sql"))
 
 
 def test_model_cache(tmp_path: Path, mocker: MockerFixture):
     cache = ModelCache(tmp_path)
 
     expressions = parse(
```

### Comparing `sqlmesh-0.6.3.dev5/tests/core/test_plan.py` & `sqlmesh-0.6.4/tests/core/test_plan.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from sqlmesh.core.model.seed import Seed
 from sqlmesh.core.plan import Plan
 from sqlmesh.core.snapshot import (
     SnapshotChangeCategory,
     SnapshotDataVersion,
     SnapshotFingerprint,
 )
-from sqlmesh.utils.date import to_date, to_datetime, to_timestamp
+from sqlmesh.utils.date import now, to_date, to_datetime, to_timestamp
 from sqlmesh.utils.errors import PlanError
 
 
 def test_forward_only_plan_sets_version(make_snapshot, mocker: MockerFixture):
     snapshot_a = make_snapshot(SqlModel(name="a", query=parse_one("select 1, ds")))
     snapshot_a.categorize_as(SnapshotChangeCategory.BREAKING)
 
@@ -419,7 +419,47 @@
     state_reader_mock = mocker.Mock()
 
     with pytest.raises(
         PlanError,
         match=r"Removed models {'a'} are referenced in model 'b'.*",
     ):
         Plan(context_diff_mock, state_reader_mock)
+
+
+def test_effective_from(make_snapshot, mocker: MockerFixture):
+    snapshot = make_snapshot(SqlModel(name="a", query=parse_one("select 1, ds FROM a")))
+    snapshot.categorize_as(SnapshotChangeCategory.FORWARD_ONLY)
+
+    context_diff_mock = mocker.Mock()
+    context_diff_mock.snapshots = {"a": snapshot}
+    context_diff_mock.added = set()
+    context_diff_mock.removed = set()
+    context_diff_mock.modified_snapshots = {}
+    context_diff_mock.new_snapshots = {snapshot.snapshot_id: snapshot}
+
+    state_reader_mock = mocker.Mock()
+
+    with pytest.raises(
+        PlanError,
+        match="Effective date can only be set for a forward-only plan.",
+    ):
+        plan = Plan(context_diff_mock, state_reader_mock)
+        plan.effective_from = "2023-01-01"
+
+    plan = Plan(context_diff_mock, state_reader_mock, forward_only=True)
+
+    with pytest.raises(
+        PlanError,
+        match="Effective date cannot be in the future.",
+    ):
+        plan.effective_from = now() + timedelta(days=1)
+
+    assert plan.effective_from is None
+    assert snapshot.effective_from is None
+
+    plan.effective_from = "2023-01-01"
+    assert plan.effective_from == "2023-01-01"
+    assert snapshot.effective_from == "2023-01-01"
+
+    plan.effective_from = None
+    assert plan.effective_from is None
+    assert snapshot.effective_from is None
```

### Comparing `sqlmesh-0.6.3.dev5/tests/core/test_plan_evaluator.py` & `sqlmesh-0.6.4/tests/core/test_plan_evaluator.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,14 +85,15 @@
         notification_targets=[],
         restatements=set(),
         backfill_concurrent_tasks=1,
         ddl_concurrent_tasks=1,
         skip_backfill=False,
         users=[],
         is_dev=True,
+        forward_only=False,
     )
 
     airflow_client_mock.wait_for_dag_run_completion.assert_called_once()
     airflow_client_mock.wait_for_first_dag_run.assert_called_once()
 
 
 def test_airflow_evaluator_plan_application_dag_fails(sushi_plan: Plan, mocker: MockerFixture):
```

### Comparing `sqlmesh-0.6.3.dev5/tests/core/test_scheduler.py` & `sqlmesh-0.6.4/tests/core/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/tests/core/test_schema_diff.py` & `sqlmesh-0.6.4/tests/core/test_schema_diff.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/tests/core/test_seed.py` & `sqlmesh-0.6.4/tests/core/test_seed.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/tests/core/test_snapshot.py` & `sqlmesh-0.6.4/tests/core/test_snapshot.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+from copy import deepcopy
 from pathlib import Path
 
 import pytest
 from _pytest.monkeypatch import MonkeyPatch
 from pytest_mock.plugin import MockerFixture
 from sqlglot import exp, parse, parse_one, to_column
 
@@ -97,14 +98,15 @@
             "query": "SELECT @EACH(ARRAY(1, 2), x -> x), ds FROM parent.tbl",
             "jinja_macros": {
                 "global_objs": {},
                 "packages": {},
                 "root_macros": {},
             },
             "source_type": "sql",
+            "tags": [],
         },
         "audits": [],
         "name": "name",
         "parents": [{"name": "parent.tbl", "identifier": snapshot.parents[0].identifier}],
         "previous_versions": [],
         "project": "",
         "indirect_versions": {},
@@ -838,7 +840,33 @@
         categorize_change(
             new=make_snapshot(create_seed_model(model_name, model_kind)),
             old=original_snapshot,
             config=config,
         )
         is None
     )
+
+
+def test_effective_from(snapshot: Snapshot):
+    previous_snapshot = deepcopy(snapshot)
+    previous_snapshot.add_interval("2023-01-01", "2023-01-05")
+    previous_snapshot.add_interval("2023-01-07", "2023-01-09")
+
+    new_snapshot_same_fingerprint = deepcopy(snapshot)
+    new_snapshot_same_fingerprint.effective_from = "2023-01-04"
+    new_snapshot_same_fingerprint.merge_intervals(previous_snapshot)
+
+    assert new_snapshot_same_fingerprint.intervals == [
+        (to_timestamp("2023-01-01"), to_timestamp("2023-01-06")),
+        (to_timestamp("2023-01-07"), to_timestamp("2023-01-10")),
+    ]
+
+    new_snapshot_different_fingerprint = deepcopy(snapshot)
+    new_snapshot_different_fingerprint.fingerprint = SnapshotFingerprint(
+        data_hash="1", metadata_hash="1", parent_data_hash="1"
+    )
+    new_snapshot_different_fingerprint.effective_from = "2023-01-04"
+    new_snapshot_different_fingerprint.merge_intervals(previous_snapshot)
+
+    assert new_snapshot_different_fingerprint.intervals == [
+        (to_timestamp("2023-01-01"), to_timestamp("2023-01-04")),
+    ]
```

### Comparing `sqlmesh-0.6.3.dev5/tests/core/test_snapshot_evaluator.py` & `sqlmesh-0.6.4/tests/core/test_snapshot_evaluator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/tests/core/test_state_sync.py` & `sqlmesh-0.6.4/tests/core/test_state_sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -588,14 +588,43 @@
     state_sync.unpause_snapshots([new_snapshot], unpaused_dt)
 
     actual_snapshots = state_sync.get_snapshots([snapshot, new_snapshot])
     assert not actual_snapshots[snapshot.snapshot_id].unpaused_ts
     assert actual_snapshots[new_snapshot.snapshot_id].unpaused_ts == to_timestamp(unpaused_dt)
 
 
+def test_unpause_snapshots_remove_intervals(
+    state_sync: EngineAdapterStateSync, make_snapshot: t.Callable
+):
+    snapshot = make_snapshot(
+        SqlModel(
+            name="test_snapshot",
+            query=parse_one("select 1, ds"),
+            cron="@daily",
+        ),
+        version="a",
+    )
+    snapshot.add_interval("2023-01-01", "2023-01-05")
+    state_sync.push_snapshots([snapshot])
+
+    new_snapshot = make_snapshot(
+        SqlModel(name="test_snapshot", query=parse_one("select 2, ds"), cron="@daily"),
+        version="a",
+    )
+    new_snapshot.effective_from = "2023-01-03"
+    state_sync.push_snapshots([new_snapshot])
+    state_sync.unpause_snapshots([new_snapshot], "2023-01-06")
+
+    actual_snapshots = state_sync.get_snapshots([snapshot, new_snapshot])
+    assert not actual_snapshots[new_snapshot.snapshot_id].intervals
+    assert actual_snapshots[snapshot.snapshot_id].intervals == [
+        (to_timestamp("2023-01-01"), to_timestamp("2023-01-03")),
+    ]
+
+
 def test_get_version(state_sync: EngineAdapterStateSync) -> None:
     # fresh install should not raise
     assert state_sync.get_versions() == Versions(
         schema_version=SCHEMA_VERSION, sqlglot_version=SQLGLOT_VERSION
     )
 
     # Start with a clean slate.
```

### Comparing `sqlmesh-0.6.3.dev5/tests/dbt/conftest.py` & `sqlmesh-0.6.4/tests/dbt/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/tests/dbt/test_adapter.py` & `sqlmesh-0.6.4/tests/dbt/test_adapter.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/tests/dbt/test_config.py` & `sqlmesh-0.6.4/tests/dbt/test_config.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/tests/dbt/test_transformation.py` & `sqlmesh-0.6.4/tests/dbt/test_transformation.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/tests/engines/spark/test_db_api.py` & `sqlmesh-0.6.4/tests/engines/spark/test_db_api.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/dbt_project.yml` & `sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/logs/dbt.log.legacy` & `sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/logs/dbt.log.legacy`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/macros/incremental.sql` & `sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/macros/incremental.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/models/waiter_revenue_by_day.sql` & `sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/models/waiter_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/packages/customers/dbt_project.yml` & `sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/packages/customers/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/packages/customers/models/customer_revenue_by_day.sql` & `sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/packages/customers/models/customer_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/profiles.yml` & `sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/profiles.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/seed_sources.py` & `sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/seed_sources.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/source_data/items.csv` & `sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/source_data/items.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/source_data/order_items.csv` & `sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/source_data/order_items.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/tests/fixtures/dbt/sushi_test/source_data/orders.csv` & `sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/source_data/orders.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/tests/fixtures/migrations/environments.json` & `sqlmesh-0.6.4/tests/fixtures/migrations/environments.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/tests/fixtures/migrations/snapshots.json` & `sqlmesh-0.6.4/tests/fixtures/migrations/snapshots.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/tests/integrations/github/fixtures/pull_request_review.json` & `sqlmesh-0.6.4/tests/integrations/github/fixtures/pull_request_review.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/tests/schedulers/airflow/conftest.py` & `sqlmesh-0.6.4/tests/schedulers/airflow/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/tests/schedulers/airflow/operators/test_hwm_sensor.py` & `sqlmesh-0.6.4/tests/schedulers/airflow/operators/test_hwm_sensor.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/tests/schedulers/airflow/operators/test_targets.py` & `sqlmesh-0.6.4/tests/schedulers/airflow/operators/test_targets.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/tests/schedulers/airflow/test_client.py` & `sqlmesh-0.6.4/tests/schedulers/airflow/test_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,14 +87,15 @@
                     "storage_format": "parquet",
                     "jinja_macros": {
                         "global_objs": {},
                         "packages": {},
                         "root_macros": {},
                     },
                     "source_type": "sql",
+                    "tags": [],
                 },
                 "audits": [],
                 "name": "test_model",
                 "parents": [],
                 "previous_versions": [],
                 "project": "",
                 "physical_schema": "physical_schema",
@@ -128,14 +129,15 @@
         "notification_targets": [],
         "request_id": request_id,
         "restatements": [],
         "backfill_concurrent_tasks": 1,
         "ddl_concurrent_tasks": 1,
         "users": [],
         "is_dev": False,
+        "forward_only": False,
     }
 
 
 def snapshot_url(snapshot_ids, key="ids") -> str:
     return urlencode({key: _list_to_json(snapshot_ids)})
```

### Comparing `sqlmesh-0.6.3.dev5/tests/schedulers/airflow/test_end_to_end.py` & `sqlmesh-0.6.4/tests/schedulers/airflow/test_end_to_end.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/tests/schedulers/airflow/test_integration.py` & `sqlmesh-0.6.4/tests/schedulers/airflow/test_integration.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/tests/schedulers/airflow/test_plan.py` & `sqlmesh-0.6.4/tests/schedulers/airflow/test_plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,15 @@
         skip_backfill=False,
         restatements={"raw.items"},
         notification_targets=[],
         backfill_concurrent_tasks=1,
         ddl_concurrent_tasks=1,
         users=[],
         is_dev=False,
+        forward_only=True,
     )
 
     deleted_snapshot = SnapshotTableInfo(
         name="test_schema.deleted_model",
         fingerprint=SnapshotFingerprint(data_hash="1", metadata_hash="1"),
         version="test_version",
         physical_schema="test_physical_schema",
@@ -98,14 +99,15 @@
         plan_id="test_plan_id",
         previous_plan_id=None,
         notification_targets=[],
         backfill_concurrent_tasks=1,
         ddl_concurrent_tasks=1,
         users=[],
         is_dev=False,
+        forward_only=True,
     )
 
     state_sync_mock.get_snapshots.assert_called_once()
     state_sync_mock.get_environment.assert_called_once()
 
 
 @pytest.mark.airflow
@@ -129,14 +131,15 @@
         skip_backfill=False,
         restatements=set(),
         notification_targets=[],
         backfill_concurrent_tasks=1,
         ddl_concurrent_tasks=1,
         users=[],
         is_dev=False,
+        forward_only=False,
     )
 
     dag_run_mock = mocker.Mock()
     dag_run_mock.conf = plan_request.dict()
 
     state_sync_mock = mocker.Mock()
     state_sync_mock.get_snapshots.return_value = {snapshot.snapshot_id: snapshot}
@@ -177,14 +180,15 @@
         skip_backfill=False,
         restatements={"raw.items"},
         notification_targets=[],
         backfill_concurrent_tasks=1,
         ddl_concurrent_tasks=1,
         users=[],
         is_dev=False,
+        forward_only=False,
     )
 
     state_sync_mock = mocker.Mock()
     state_sync_mock.get_snapshots.return_value = {
         snapshot.snapshot_id: snapshot,
         unrelated_snapshot.snapshot_id: unrelated_snapshot,
     }
```

### Comparing `sqlmesh-0.6.3.dev5/tests/utils/test_cache.py` & `sqlmesh-0.6.4/tests/utils/test_cache.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/tests/utils/test_concurrency.py` & `sqlmesh-0.6.4/tests/utils/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/tests/utils/test_connection_pool.py` & `sqlmesh-0.6.4/tests/utils/test_connection_pool.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/tests/utils/test_dag.py` & `sqlmesh-0.6.4/tests/utils/test_dag.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/tests/utils/test_date.py` & `sqlmesh-0.6.4/tests/utils/test_date.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/tests/utils/test_filesystem.py` & `sqlmesh-0.6.4/tests/utils/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/tests/utils/test_jinja.py` & `sqlmesh-0.6.4/tests/utils/test_jinja.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/tests/utils/test_metaprogramming.py` & `sqlmesh-0.6.4/tests/utils/test_metaprogramming.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/tests/utils/test_pandas.py` & `sqlmesh-0.6.4/tests/utils/test_pandas.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/tests/utils/test_pydantic.py` & `sqlmesh-0.6.4/tests/utils/test_pydantic.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/tests/utils/test_transactional_file.py` & `sqlmesh-0.6.4/tests/utils/test_transactional_file.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/tests/utils/test_yaml.py` & `sqlmesh-0.6.4/tests/utils/test_yaml.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/tests/web/test_main.py` & `sqlmesh-0.6.4/tests/web/test_main.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/.eslintrc.js` & `sqlmesh-0.6.4/web/client/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/index.html` & `sqlmesh-0.6.4/web/client/index.html`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/openapi.json` & `sqlmesh-0.6.4/web/client/openapi.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/package-lock.json` & `sqlmesh-0.6.4/web/client/package-lock.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/package.json` & `sqlmesh-0.6.4/web/client/package.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/playwright.config.ts` & `sqlmesh-0.6.4/web/client/playwright.config.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/public/favicons/favicon.ico` & `sqlmesh-0.6.4/web/client/dist/favicons/favicon.ico`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/api/channels.ts` & `sqlmesh-0.6.4/web/client/src/api/channels.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/api/index.ts` & `sqlmesh-0.6.4/web/client/src/api/index.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/api/instance.ts` & `sqlmesh-0.6.4/web/client/src/api/instance.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/assets/fonts/Circular STD/CircularStd-Black.otf` & `sqlmesh-0.6.4/web/client/dist/assets/CircularStd-Black-52659624.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/assets/fonts/Circular STD/CircularStd-BlackItalic.otf` & `sqlmesh-0.6.4/web/client/src/assets/fonts/Circular STD/CircularStd-BlackItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/assets/fonts/Circular STD/CircularStd-Bold.otf` & `sqlmesh-0.6.4/web/client/dist/assets/CircularStd-Bold-0e6c076d.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/assets/fonts/Circular STD/CircularStd-BoldItalic.otf` & `sqlmesh-0.6.4/web/client/src/assets/fonts/Circular STD/CircularStd-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/assets/fonts/Circular STD/CircularStd-Book.otf` & `sqlmesh-0.6.4/web/client/src/assets/fonts/Circular STD/CircularStd-Book.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/assets/fonts/Circular STD/CircularStd-BookItalic.otf` & `sqlmesh-0.6.4/web/client/src/assets/fonts/Circular STD/CircularStd-BookItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/assets/fonts/Circular STD/CircularStd-Medium.otf` & `sqlmesh-0.6.4/web/client/dist/assets/CircularStd-Medium-2f373e53.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/assets/fonts/Circular STD/CircularStd-MediumItalic.otf` & `sqlmesh-0.6.4/web/client/src/assets/fonts/Circular STD/CircularStd-MediumItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/assets/fonts/Publico/Publico-Black.otf` & `sqlmesh-0.6.4/web/client/dist/assets/Publico-Black-e6bd2ea2.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/assets/fonts/Publico/Publico-BlackItalic.otf` & `sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/Publico-BlackItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/assets/fonts/Publico/Publico-Bold.otf` & `sqlmesh-0.6.4/web/client/dist/assets/Publico-Bold-c79acd56.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/assets/fonts/Publico/Publico-BoldItalic.otf` & `sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/Publico-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/assets/fonts/Publico/Publico-Extrabold.otf` & `sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/Publico-Extrabold.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/assets/fonts/Publico/Publico-ExtraboldItalic.otf` & `sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/Publico-ExtraboldItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/assets/fonts/Publico/Publico-Italic.otf` & `sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/Publico-Italic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/assets/fonts/Publico/Publico-Light.otf` & `sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/Publico-Light.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/assets/fonts/Publico/Publico-LightItalic.otf` & `sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/Publico-LightItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/assets/fonts/Publico/Publico-Medium.otf` & `sqlmesh-0.6.4/web/client/dist/assets/Publico-Medium-01b4a891.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/assets/fonts/Publico/Publico-MediumItalic.otf` & `sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/Publico-MediumItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/assets/fonts/Publico/Publico-Roman.otf` & `sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/Publico-Roman.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/assets/fonts/Publico/PublicoText-Bold.otf` & `sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/PublicoText-Bold.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/assets/fonts/Publico/PublicoText-BoldItalic.otf` & `sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/PublicoText-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/assets/fonts/Publico/PublicoText-Italic.otf` & `sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/PublicoText-Italic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/assets/fonts/Publico/PublicoText-Roman.otf` & `sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/PublicoText-Roman.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/assets/fonts/Publico/PublicoText-Semibold.otf` & `sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/PublicoText-Semibold.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/assets/fonts/Publico/PublicoText-SemiboldItalic.otf` & `sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/PublicoText-SemiboldItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/context/context.ts` & `sqlmesh-0.6.4/web/client/src/context/context.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/context/editor.ts` & `sqlmesh-0.6.4/web/client/src/context/editor.ts`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,12 @@
-import { type ColumnLineageApiLineageModelNameColumnNameGet200 } from '@api/client'
-import { isObjectEmpty } from '@utils/index'
+import {
+  type Model,
+  type ColumnLineageApiLineageModelNameColumnNameGet200,
+} from '@api/client'
+import { uid, isObjectEmpty } from '@utils/index'
 import { create } from 'zustand'
 import useLocalStorage from '~/hooks/useLocalStorage'
 import { ModelFile } from '~/models'
 import { sqlglotWorker } from '~/workers'
 
 export interface Dialect {
   dialect_title: string
@@ -38,27 +41,29 @@
   createTab: (file?: ModelFile) => EditorTab
   setDialects: (dialects: Dialect[]) => void
   refreshTab: () => void
   setPreviewQuery: (previewQuery?: string) => void
   setPreviewTable: (previewTable?: any[]) => void
   setPreviewConsole: (previewConsole?: string) => void
   setPreviewLineage: (
+    models: Map<string, Model>,
     previewLineage?: Record<string, Lineage>,
     columns?: ColumnLineageApiLineageModelNameColumnNameGet200,
   ) => void
 }
 
 interface EditorPreview<TTable = any> {
   queryPreview?: string
   table?: TTable[]
   terminal?: string
   lineage?: Record<string, Lineage>
 }
 
 export interface EditorTab {
+  id: string
   file: ModelFile
   isValid: boolean
   isSaved: boolean
   dialect?: string
   dialectOptions?: {
     keywords: string
     types: string
@@ -149,27 +154,28 @@
   },
   setPreviewTable(previewTable) {
     set(() => ({ previewTable }))
   },
   setPreviewConsole(previewConsole) {
     set(() => ({ previewConsole }))
   },
-  setPreviewLineage(lineage, columns) {
+  setPreviewLineage(models, lineage, columns) {
     const previewLineage = structuredClone(lineage)
 
     if (columns != null && previewLineage != null) {
-      mergeLineageWithColumns(previewLineage, columns)
+      mergeLineageWithColumns(models, previewLineage, columns)
     }
 
     set(() => ({ previewLineage }))
   },
 }))
 
 function createTab(file: ModelFile = createLocalFile()): EditorTab {
   return {
+    id: uid(),
     file,
     isValid: true,
     isSaved: true,
   }
 }
 
 function createLocalFile(): ModelFile {
@@ -181,15 +187,17 @@
   })
 }
 
 function getStoredTabsIds(): ID[] {
   return getStoredTabs()?.ids ?? []
 }
 
+// TODO: use better merge
 function mergeLineageWithColumns(
+  models: Map<string, Model>,
   lineage: Record<string, Lineage>,
   columns: ColumnLineageApiLineageModelNameColumnNameGet200,
 ): Record<string, Lineage> {
   for (const model in columns) {
     const lineageModel = lineage[model]
     const columnsModel = columns[model]
 
@@ -227,9 +235,38 @@
             new Set(lineageModelColumnModel.concat(columnsModelColumnModel)),
           )
         }
       }
     }
   }
 
+  for (const modelName in lineage) {
+    const model = models.get(modelName)
+    const modelLineage = lineage[modelName]
+
+    if (model == null || modelLineage == null) {
+      delete lineage[modelName]
+
+      continue
+    }
+
+    if (modelLineage.columns == null) continue
+
+    if (model.columns == null) {
+      delete modelLineage.columns
+
+      continue
+    }
+
+    for (const columnName in modelLineage.columns) {
+      const found = model.columns.find(c => c.name === columnName)
+
+      if (found == null) {
+        delete modelLineage.columns[columnName]
+
+        continue
+      }
+    }
+  }
+
   return lineage
 }
```

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/context/fileTree.ts` & `sqlmesh-0.6.4/web/client/src/context/fileTree.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/context/lineage.tsx` & `sqlmesh-0.6.4/web/client/src/context/lineage.tsx`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,14 @@
   nodes: Node[]
   edges: Edge[]
   setNodes: (nodes: Node[]) => void
   setEdges: (edges: Edge[]) => void
   onNodesChange: OnNodesChange
   onEdgesChange: OnEdgesChange
   onConnect: OnConnect
-  clearNodesAndEdges: () => void
 }
 
 export const useStoreReactFlow = create<ReactFlowStore>((set, get) => ({
   nodes: [],
   edges: [],
   setNodes(nodes) {
     set({ nodes })
@@ -56,17 +55,14 @@
     })
   },
   onConnect: (connection: Connection) => {
     set({
       edges: addEdge(connection, get().edges),
     })
   },
-  clearNodesAndEdges() {
-    set({ nodes: [], edges: [] })
-  },
 }))
 
 export const useStoreLineage = create<LineageStore>((set, get) => ({
   columns: undefined,
   activeEdges: new Map(),
   addActiveEdges(edges) {
     const { activeEdges } = get()
```

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/context/plan.ts` & `sqlmesh-0.6.4/web/client/src/context/plan.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/context/theme.tsx` & `sqlmesh-0.6.4/web/client/src/context/theme.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/hooks/useLocalStorage.ts` & `sqlmesh-0.6.4/web/client/src/hooks/useLocalStorage.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/index.css` & `sqlmesh-0.6.4/web/client/src/index.css`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/library/components/banner/Banner.tsx` & `sqlmesh-0.6.4/web/client/src/library/components/banner/Banner.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/library/components/button/Button.tsx` & `sqlmesh-0.6.4/web/client/src/library/components/button/Button.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/library/components/button/tests/Button.spec.tsx` & `sqlmesh-0.6.4/web/client/src/library/components/button/tests/Button.spec.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/library/components/divider/Divider.tsx` & `sqlmesh-0.6.4/web/client/src/library/components/divider/Divider.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/library/components/divider/tests/Divider.spec.tsx` & `sqlmesh-0.6.4/web/client/src/library/components/divider/tests/Divider.spec.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/library/components/editor/Editor.css` & `sqlmesh-0.6.4/web/client/src/library/components/editor/Editor.css`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/library/components/editor/Editor.tsx` & `sqlmesh-0.6.4/web/client/src/library/components/editor/Editor.tsx`

 * *Files 22% similar despite different names*

```diff
@@ -6,37 +6,34 @@
 import CodeEditor from './EditorCode'
 import EditorFooter from './EditorFooter'
 import EditorTabs from './EditorTabs'
 import EditorInspector from './EditorInspector'
 import './Editor.css'
 import EditorPreview from './EditorPreview'
 import { useStoreEditor } from '~/context/editor'
-import { useStoreLineage, useStoreReactFlow } from '@context/lineage'
-
+import { useStoreLineage } from '@context/lineage'
 import clsx from 'clsx'
+import Loading from '@components/loading/Loading'
+import Spinner from '@components/logo/Spinner'
 
 export default function Editor(): JSX.Element {
   const files = useStoreFileTree(s => s.files)
   const selectedFile = useStoreFileTree(s => s.selectedFile)
 
   const tab = useStoreEditor(s => s.tab)
   const storedTabsIds = useStoreEditor(s => s.storedTabsIds)
   const engine = useStoreEditor(s => s.engine)
   const previewTable = useStoreEditor(s => s.previewTable)
   const previewConsole = useStoreEditor(s => s.previewConsole)
   const selectTab = useStoreEditor(s => s.selectTab)
   const createTab = useStoreEditor(s => s.createTab)
   const addTab = useStoreEditor(s => s.addTab)
   const setDialects = useStoreEditor(s => s.setDialects)
-  const setPreviewQuery = useStoreEditor(s => s.setPreviewQuery)
-  const setPreviewConsole = useStoreEditor(s => s.setPreviewConsole)
-  const setPreviewTable = useStoreEditor(s => s.setPreviewTable)
 
   const clearActiveEdges = useStoreLineage(s => s.clearActiveEdges)
-  const clearNodesAndEdges = useStoreReactFlow(s => s.clearNodesAndEdges)
 
   const [isReadyEngine, setIsreadyEngine] = useState(false)
   const [direction, setDirection] = useState<'vertical' | 'horizontal'>(
     'vertical',
   )
 
   const handleEngineWorkerMessage = useCallback((e: MessageEvent): void => {
@@ -85,19 +82,15 @@
         addTab(createTab(file))
       }
     })
   }, [files])
 
   useEffect(() => {
     clearActiveEdges()
-    clearNodesAndEdges()
-    setPreviewQuery(undefined)
-    setPreviewTable(undefined)
-    setPreviewConsole(undefined)
-  }, [tab])
+  }, [tab?.file.fingerprint, tab?.id])
 
   useEffect(() => {
     if (selectedFile == null || tab?.file === selectedFile) return
 
     selectTab(createTab(selectedFile))
   }, [selectedFile])
 
@@ -105,42 +98,49 @@
     setDirection(direction =>
       direction === 'vertical' ? 'horizontal' : 'vertical',
     )
   }
 
   return (
     <div className="w-full h-full flex flex-col overflow-hidden">
-      <EditorTabs />
-      <Divider />
-      {tab == null ? (
+      {isFalse(isReadyEngine) ? (
         <div className="flex justify-center items-center w-full h-full">
-          <div className="p-4 text-center text-theme-darker dark:text-theme-lighter">
-            <h2 className="text-3xl">Select File or Add New SQL Tab</h2>
-          </div>
+          <Loading className="inline-block ">
+            <Spinner className="w-5 h-5 border border-neutral-10 mr-4" />
+            <h3 className="text-xl">Starting Editor...</h3>
+          </Loading>
         </div>
       ) : (
-        <SplitPane
-          key={direction}
-          className={clsx(
-            'w-full h-full overflow-hidden',
-            direction === 'vertical' ? 'flex flex-col' : 'flex',
-          )}
-          sizes={sizesCodeEditorAndPreview}
-          direction={direction}
-          minSize={0}
-          snapOffset={0}
-        >
-          <div
-            className={clsx(
-              'flex flex-col overflow-hidden',
-              direction === 'vertical' ? 'w-full ' : 'h-full',
-            )}
-          >
-            {isReadyEngine && (
-              <>
+        <>
+          <EditorTabs />
+          <Divider />
+          {tab == null ? (
+            <div className="flex justify-center items-center w-full h-full">
+              <div className="p-4 text-center text-theme-darker dark:text-theme-lighter">
+                <h2 className="text-3xl">Select File or Add New SQL Tab</h2>
+              </div>
+            </div>
+          ) : (
+            <SplitPane
+              key={direction}
+              className={clsx(
+                'w-full h-full overflow-hidden',
+                direction === 'vertical' ? 'flex flex-col' : 'flex',
+              )}
+              sizes={sizesCodeEditorAndPreview}
+              direction={direction}
+              minSize={0}
+              snapOffset={0}
+            >
+              <div
+                className={clsx(
+                  'flex flex-col overflow-hidden',
+                  direction === 'vertical' ? 'w-full ' : 'h-full',
+                )}
+              >
                 <div className="flex flex-col h-full overflow-hidden">
                   <SplitPane
                     className="flex h-full"
                     sizes={sizesCodeEditorAndInspector}
                     minSize={0}
                     snapOffset={0}
                   >
@@ -152,28 +152,25 @@
                     </div>
                   </SplitPane>
                 </div>
                 <Divider />
                 <div className="px-2 flex justify-between items-center min-h-[2rem]">
                   <EditorFooter tab={tab} />
                 </div>
-              </>
-            )}
-          </div>
-          <div
-            className={clsx(
-              direction === 'vertical' ? 'flex flex-col' : 'flex',
-            )}
-          >
-            {tab != null && (
-              <EditorPreview
-                key={tab.file.id}
-                tab={tab}
-                toggleDirection={toggleDirection}
-              />
-            )}
-          </div>
-        </SplitPane>
+              </div>
+              <div
+                className={clsx(
+                  direction === 'vertical' ? 'flex flex-col' : 'flex',
+                )}
+              >
+                <EditorPreview
+                  tab={tab}
+                  toggleDirection={toggleDirection}
+                />
+              </div>
+            </SplitPane>
+          )}
+        </>
       )}
     </div>
   )
 }
```

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/library/components/editor/EditorCode.tsx` & `sqlmesh-0.6.4/web/client/src/library/components/editor/EditorCode.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/library/components/editor/EditorFooter.tsx` & `sqlmesh-0.6.4/web/client/src/library/components/editor/EditorFooter.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/library/components/editor/EditorIndicator.tsx` & `sqlmesh-0.6.4/web/client/src/library/components/editor/EditorIndicator.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/library/components/editor/EditorInspector.tsx` & `sqlmesh-0.6.4/web/client/src/library/components/editor/EditorInspector.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/library/components/editor/EditorPreview.tsx` & `sqlmesh-0.6.4/web/client/src/library/components/editor/EditorPreview.tsx`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,17 @@
   toggleDirection: () => void
 }): JSX.Element {
   const models = useStoreContext(s => s.models)
 
   const previewQuery = useStoreEditor(s => s.previewQuery)
   const previewConsole = useStoreEditor(s => s.previewConsole)
   const previewTable = useStoreEditor(s => s.previewTable)
+  const setPreviewQuery = useStoreEditor(s => s.setPreviewQuery)
+  const setPreviewConsole = useStoreEditor(s => s.setPreviewConsole)
+  const setPreviewTable = useStoreEditor(s => s.setPreviewTable)
 
   const [activeTabIndex, setActiveTabIndex] = useState(-1)
   const [modelName, setModelName] = useState<string | undefined>()
 
   const tabs = useMemo(() => {
     if (tab.file.isLocal)
       return [
@@ -53,15 +56,15 @@
         EnumEditorPreviewTabs.Table,
         EnumEditorPreviewTabs.Query,
         EnumEditorPreviewTabs.Console,
         EnumEditorPreviewTabs.Lineage,
       ]
 
     return [EnumEditorPreviewTabs.Console]
-  }, [tab])
+  }, [tab.id, tab.file.fingerprint])
 
   const [headers, data] = useMemo(
     () =>
       previewTable == null
         ? [[], []]
         : [previewTable[0] ?? [], previewTable[1] ?? []],
     [previewTable],
@@ -82,14 +85,20 @@
         Boolean(previewQuery),
         Boolean(previewConsole),
       ].findIndex(isTrue),
     [previewTable, previewQuery, previewConsole],
   )
 
   useEffect(() => {
+    setPreviewQuery(undefined)
+    setPreviewTable(undefined)
+    setPreviewConsole(undefined)
+  }, [tab.id])
+
+  useEffect(() => {
     setActiveTabIndex(tab.file.isSQLMeshModel ? 3 : -1)
   }, [previewTable, previewQuery, previewConsole, tab])
 
   useEffect(() => {
     setModelName(models.get(tab.file.path)?.name)
   }, [models, tab.file])
 
@@ -286,31 +295,36 @@
   tab,
 }: {
   model: string
   tab: EditorTab
 }): JSX.Element {
   const { data: lineage, refetch: getModelLineage } = useApiModelLineage(model)
 
+  const models = useStoreContext(s => s.models)
+
   const previewLineage = useStoreEditor(s => s.previewLineage)
   const setPreviewLineage = useStoreEditor(s => s.setPreviewLineage)
 
   const debouncedGetModelLineage = useCallback(
     debounceAsync(getModelLineage, 1000, true),
     [model, tab.file.path, tab.file.fingerprint],
   )
 
+  const highlightedNodes = useMemo(() => [model], [model])
+
   useEffect(() => {
     void debouncedGetModelLineage()
   }, [debouncedGetModelLineage])
 
   useEffect(() => {
     if (lineage == null) {
-      setPreviewLineage(undefined)
+      setPreviewLineage(models)
     } else {
       setPreviewLineage(
+        models,
         Object.keys(lineage).reduce((acc: Record<string, Lineage>, key) => {
           acc[key] = {
             models: lineage[key] ?? [],
             columns: previewLineage?.[key]?.columns ?? undefined,
           }
 
           return acc
@@ -322,11 +336,11 @@
   return previewLineage == null ? (
     <div className="w-full h-full flex items-center justify-center bg-primary-10">
       <Loading hasSpinner>Loading Lineage...</Loading>
     </div>
   ) : (
     <Graph
       lineage={previewLineage}
-      highlightedNodes={[model]}
+      highlightedNodes={highlightedNodes}
     />
   )
 }
```

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/library/components/editor/EditorTabs.tsx` & `sqlmesh-0.6.4/web/client/src/library/components/editor/EditorTabs.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/library/components/editor/extensions/SqlMeshDialect.ts` & `sqlmesh-0.6.4/web/client/src/library/components/editor/extensions/SqlMeshDialect.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/library/components/editor/extensions/index.ts` & `sqlmesh-0.6.4/web/client/src/library/components/editor/extensions/index.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/library/components/editor/help.ts` & `sqlmesh-0.6.4/web/client/src/library/components/editor/help.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/library/components/fileTree/Directory.tsx` & `sqlmesh-0.6.4/web/client/src/library/components/fileTree/Directory.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/library/components/fileTree/File.tsx` & `sqlmesh-0.6.4/web/client/src/library/components/fileTree/File.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/library/components/fileTree/FileTree.tsx` & `sqlmesh-0.6.4/web/client/src/library/components/fileTree/FileTree.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/library/components/fileTree/help.ts` & `sqlmesh-0.6.4/web/client/src/library/components/fileTree/help.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/library/components/graph/Graph.tsx` & `sqlmesh-0.6.4/web/client/src/library/components/graph/Graph.tsx`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import React, {
+  memo,
   type MouseEvent,
   useEffect,
   useMemo,
   useState,
   useCallback,
-  Fragment,
 } from 'react'
 import ReactFlow, {
   Controls,
   Background,
   Panel,
   Handle,
   Position,
@@ -23,29 +23,26 @@
   createGraphLayout,
   toNodeOrEdgeId,
   type GraphNodeData,
 } from './help'
 import { debounceAsync, isArrayNotEmpty, isFalse, isTrue } from '../../../utils'
 import { EnumSize, EnumVariant } from '~/types/enum'
 import { useStoreContext } from '@context/context'
-import {
-  ArrowRightCircleIcon,
-  InformationCircleIcon,
-} from '@heroicons/react/24/solid'
+import { ArrowRightCircleIcon } from '@heroicons/react/24/solid'
 import { useStoreLineage, useStoreReactFlow } from '@context/lineage'
 import clsx from 'clsx'
 import { type Column } from '@api/client'
 import { useStoreFileTree } from '@context/fileTree'
 import { useApiColumnLineage } from '@api/index'
-import { Popover, Transition } from '@headlessui/react'
 import { useStoreEditor, type Lineage } from '@context/editor'
 import Loading from '@components/loading/Loading'
 import Spinner from '@components/logo/Spinner'
+import './Graph.css'
 
-export default function Flow({
+const Flow = memo(function Flow({
   lineage,
   closeGraph,
   highlightedNodes = [],
 }: {
   lineage: Record<string, Lineage>
   closeGraph?: () => void
   highlightedNodes?: string[]
@@ -60,60 +57,49 @@
   const onEdgesChange = useStoreReactFlow(s => s.onEdgesChange)
   const onConnect = useStoreReactFlow(s => s.onConnect)
 
   const setColumns = useStoreLineage(s => s.setColumns)
   const activeEdges = useStoreLineage(s => s.activeEdges)
   const hasActiveEdge = useStoreLineage(s => s.hasActiveEdge)
 
+  const [key, setKey] = useState('default')
+
   const nodeTypes = useMemo(() => ({ model: ModelNode }), [ModelNode])
-  const nodesAndEdges = useMemo(
-    () =>
-      getNodesAndEdges({
-        lineage,
-        highlightedNodes,
-        models,
-        nodes,
-        edges,
-      }),
-    [lineage, highlightedNodes, models],
-  )
 
   useEffect(() => {
-    let active = true
+    const nodesAndEdges = getNodesAndEdges({
+      lineage,
+      highlightedNodes,
+      models,
+      nodes,
+      edges,
+    })
 
     void load()
 
-    return () => {
-      active = false
-    }
-
     async function load(): Promise<void> {
-      const layout = await createGraphLayout({
-        nodes: nodesAndEdges.nodes,
-        edges: nodesAndEdges.edges,
-        nodesMap: nodesAndEdges.nodesMap,
-      })
-
-      if (isFalse(active)) return
+      const layout = await createGraphLayout(nodesAndEdges)
 
       setNodes(layout.nodes)
-      setEdges(layout.edges)
+      setEdges(toggleEdge(layout.edges))
       setColumns(nodesAndEdges.columns)
+      setKey(nodesAndEdges.key)
     }
-  }, [nodesAndEdges])
+  }, [lineage, highlightedNodes, models])
 
   useEffect(() => {
-    setEdges(toggleEdge(nodesAndEdges.edges))
+    setEdges(toggleEdge(edges))
   }, [activeEdges])
 
   useEffect(() => {
-    setNodes(nodesAndEdges.nodes)
-    setEdges(nodesAndEdges.edges)
-    setColumns(nodesAndEdges.columns)
-  }, [lineage, highlightedNodes, models])
+    nodes.forEach(node => {
+      node.position.x = 0
+      node.position.y = 0
+    })
+  }, [highlightedNodes])
 
   function toggleEdge(edges: Edge[] = []): Edge[] {
     return edges.map(edge => {
       if (edge.sourceHandle != null && edge.targetHandle != null) {
         edge.hidden =
           isFalse(hasActiveEdge(edge.sourceHandle)) &&
           isFalse(hasActiveEdge(edge.targetHandle))
@@ -124,20 +110,22 @@
       return edge
     })
   }
 
   return (
     <div className="px-2 py-1 w-full h-full">
       <ReactFlow
+        key={key}
         nodes={nodes}
         edges={edges}
         nodeTypes={nodeTypes}
         onConnect={onConnect}
         onNodesChange={onNodesChange}
         onEdgesChange={onEdgesChange}
+        nodeOrigin={[0.5, 0.5]}
         fitView
       >
         {closeGraph != null && (
           <Panel
             position="top-right"
             className="flex"
           >
@@ -160,15 +148,17 @@
           variant={BackgroundVariant.Dots}
           gap={16}
           size={2}
         />
       </ReactFlow>
     </div>
   )
-}
+})
+
+export default Flow
 
 function ModelNode({
   id,
   data,
   sourcePosition,
   targetPosition,
 }: NodeProps & { data: GraphNodeData }): JSX.Element {
@@ -282,15 +272,15 @@
             <span>{data.label}</span>
           </span>
         </ModelNodeHandles>
       </div>
       {file != null && (
         <div
           className={clsx(
-            'w-full py-2 bg-theme-lighter opacity-90 cursor-default',
+            'w-full py-2 bg-theme-lighter cursor-default',
             columns.length <= COLUMS_LIMIT_DEFAULT && 'rounded-b-lg',
           )}
         >
           {columnsVisible.map(column => (
             <ModelColumn
               key={column.name}
               id={id}
@@ -352,136 +342,113 @@
   disabled?: boolean
   toggleEdgeById: (
     type: 'add' | 'remove',
     edgeIds: [string, string],
     connections?: { ins: string[]; outs: string[] },
   ) => void
 }): JSX.Element {
-  const { refetch: getColumnLineage, isFetching } = useApiColumnLineage(
-    id,
-    column.name,
-  )
+  const {
+    refetch: getColumnLineage,
+    isFetching,
+    isError,
+  } = useApiColumnLineage(id, column.name)
 
   const debouncedGetColumnLineage = useCallback(
     debounceAsync(getColumnLineage, 1000, true),
     [getColumnLineage],
   )
 
+  const models = useStoreContext(s => s.models)
   const activeEdges = useStoreLineage(s => s.activeEdges)
   const hasActiveEdge = useStoreLineage(s => s.hasActiveEdge)
   const columns = useStoreLineage(s => s.columns)
 
   const columnId = toNodeOrEdgeId(id, column.name)
   const sourceId = toNodeOrEdgeId('source', columnId)
   const targetId = toNodeOrEdgeId('target', columnId)
 
   const previewLineage = useStoreEditor(s => s.previewLineage)
   const setPreviewLineage = useStoreEditor(s => s.setPreviewLineage)
 
-  const [isShowing, setIsShowing] = useState(false)
   const [isActive, setIsActive] = useState(
     hasActiveEdge(sourceId) || hasActiveEdge(targetId),
   )
-  const [shouldUpdate, setShouldUpdate] = useState(false)
 
   useEffect(() => {
     setIsActive(hasActiveEdge(sourceId) || hasActiveEdge(targetId))
   }, [activeEdges])
 
-  useEffect(() => {
-    if (shouldUpdate) {
-      toggleEdgeById('add', [sourceId, targetId], columns?.[columnId])
-      setShouldUpdate(false)
-    }
-  }, [columns, shouldUpdate])
-
-  const lineage = previewLineage?.[id]?.columns?.[column.name]
   const hasTarget = isArrayNotEmpty(columns?.[columnId]?.outs)
   const hasSource = isArrayNotEmpty(columns?.[columnId]?.ins)
 
   return (
     <div
       key={column.name}
       className={clsx(
         isActive && 'bg-secondary-10 dark:bg-primary-900',
-        disabled && 'opacity-50 cursor-not-allowed',
         className,
       )}
       onClick={() => {
         if (disabled) return
 
         if (isFalse(isActive)) {
           void debouncedGetColumnLineage().then(({ data: columnLineage }) => {
-            if (columnLineage?.[id]?.[column.name] != null) {
-              setPreviewLineage(previewLineage, columnLineage)
-              setShouldUpdate(true)
+            const upstreamModels = columnLineage?.[id]?.[column.name]?.models
+            if (upstreamModels != null) {
+              const columns = Object.entries(upstreamModels)
+                .map(([id, columns]) =>
+                  columns.map(column => toNodeOrEdgeId(id, column)),
+                )
+                .flat()
+
+              toggleEdgeById('add', [sourceId, targetId], {
+                ins: columns,
+                outs: [],
+              })
+              setPreviewLineage(models, previewLineage, columnLineage)
             }
           })
         } else {
           toggleEdgeById('remove', [sourceId, targetId], columns?.[columnId])
         }
       }}
     >
       <ModelNodeHandles
         id={columnId}
         targetPosition={targetPosition}
         sourcePosition={sourcePosition}
         hasTarget={hasTarget}
         hasSource={hasSource}
-        className={clsx(disabled && 'pointer-events-none')}
+        disabled={disabled}
       >
-        <div className="flex w-full justify-between">
-          <div className={clsx('mr-3 flex')}>
+        <div className="flex w-full items-center">
+          <div className="flex items-center">
             {isFetching && (
-              <Loading className="inline-block mr-3 w-4 h-4">
-                <Spinner className="w-4 h-4 mr-2" />
+              <Loading className="inline-block mr-2">
+                <Spinner className="w-3 h-3 border border-neutral-10" />
               </Loading>
             )}
-            {lineage?.source != null && isFalse(disabled) && (
-              <Popover
-                onMouseEnter={() => {
-                  setIsShowing(true)
-                }}
-                onMouseLeave={() => {
-                  setIsShowing(false)
-                }}
-                className="relative flex"
-              >
-                {() => (
-                  <>
-                    <InformationCircleIcon className="text-secondary-500 dark:text-primary-500 inline-block mr-3 w-4 h-4" />
-                    <Transition
-                      show={isShowing}
-                      as={Fragment}
-                      enter="transition ease-out duration-200"
-                      enterFrom="opacity-0 translate-y-1"
-                      enterTo="opacity-100 translate-y-0"
-                      leave="transition ease-in duration-150"
-                      leaveFrom="opacity-100 translate-y-0"
-                      leaveTo="opacity-0 translate-y-1"
-                    >
-                      <Popover.Panel className="absolute bottom-2 z-10 transform">
-                        <div
-                          className="overflow-auto scrollbar scrollbar--vertical scrollbar--horizontal max-h-[25vh] max-w-[50vw] rounded-lg bg-theme p-4 border-4 border-primary-20"
-                          dangerouslySetInnerHTML={{
-                            __html: `<pre class='inline-block w-full h-full'>${
-                              lineage.source ?? ''
-                            }</pre>`,
-                          }}
-                        ></div>
-                      </Popover.Panel>
-                    </Transition>
-                  </>
-                )}
-              </Popover>
-            )}
-            {column.name}
           </div>
-          <div className="text-neutral-400 dark:text-neutral-300">
-            {column.type}
+          <div
+            className={clsx(
+              'w-full mr-3 flex justify-between',
+              disabled && 'opacity-50 cursor-not-allowed',
+            )}
+          >
+            <span
+              className={clsx(
+                'mr-3',
+                isError ? 'text-danger-500' : 'text-neutral-400',
+              )}
+            >
+              {column.name}
+            </span>
+            <div className="text-neutral-400 dark:text-neutral-300">
+              {column.type}
+            </div>
           </div>
         </div>
       </ModelNodeHandles>
     </div>
   )
 }
 
@@ -490,29 +457,33 @@
   sourcePosition,
   targetPosition,
   children,
   className,
   isLeading = false,
   hasTarget = true,
   hasSource = true,
+  disabled = false,
 }: {
   id: string
   sourcePosition?: Position
   targetPosition?: Position
   children: React.ReactNode
   isLeading?: boolean
   className?: string
   hasTarget?: boolean
   hasSource?: boolean
+  disabled?: boolean
 }): JSX.Element {
   return (
     <div
       className={clsx(
         'flex w-full !relative px-3 py-1 items-center',
-        isFalse(isLeading) && 'hover:bg-secondary-10 dark:hover:bg-primary-10',
+        isFalse(isLeading) &&
+          isFalse(disabled) &&
+          'hover:bg-secondary-10 dark:hover:bg-primary-10',
         className,
       )}
     >
       {targetPosition === Position.Right && (
         <Handle
           type="target"
           id={toNodeOrEdgeId('target', id)}
```

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/library/components/graph/help.ts` & `sqlmesh-0.6.4/web/client/src/library/components/graph/help.ts`

 * *Files 5% similar despite different names*

```diff
@@ -7,19 +7,14 @@
 export interface GraphNodeData {
   label: string
   isHighlighted?: boolean
   isInteractive?: boolean
   [key: string]: any
 }
 
-const elk = new ELK()
-
-const NODE_WIDTH = 64
-const NODE_HEIGHT = 32
-
 export function getNodesAndEdges({
   lineage,
   highlightedNodes,
   models,
   nodes = [],
   edges = [],
 }: {
@@ -29,14 +24,15 @@
   nodes?: Node[]
   edges?: Edge[]
 }): {
   nodesMap: Record<string, Node>
   edges: Edge[]
   nodes: Node[]
   columns: Record<string, { ins: string[]; outs: string[] }>
+  key: string
 } {
   const currentEdges = edges.reduce(
     (acc: Record<string, Edge>, edge) =>
       Object.assign(acc, { [edge.id]: edge }),
     {},
   )
   const targets = new Set(
@@ -51,22 +47,26 @@
     highlightedNodes,
     models,
     targets,
     nodes,
   )
   const outputEdges: Edge[] = []
   const columns: Record<string, { ins: string[]; outs: string[] }> = {}
+  const ids = Object.keys(nodesMap)
 
   for (const modelSource of modelNames) {
     const modelLineage = lineage[modelSource]
 
     if (modelLineage == null) continue
 
     modelLineage.models.forEach(modelTarget => {
-      outputEdges.push(createGraphEdge(modelSource, modelTarget))
+      const edge = createGraphEdge(modelSource, modelTarget)
+
+      ids.push(edge.id)
+      outputEdges.push(edge)
     })
 
     if (modelLineage.columns == null || isObjectEmpty(modelLineage.columns))
       continue
 
     for (const columnSource in modelLineage.columns) {
       const sourceId = toNodeOrEdgeId(modelSource, columnSource)
@@ -112,53 +112,56 @@
           const edgeId = toNodeOrEdgeId(
             modelSource,
             modelTarget,
             sourceHandle,
             targetHandle,
           )
           const currentEdge = currentEdges[edgeId]
-
-          outputEdges.push(
+          const edge =
             currentEdge ??
-              createGraphEdge(
-                modelSource,
-                modelTarget,
-                sourceHandle,
-                targetHandle,
-                false,
-                {
-                  target: modelTarget,
-                  source: modelSource,
-                  columnSource,
-                  columnTarget,
-                },
-              ),
-          )
+            createGraphEdge(
+              modelSource,
+              modelTarget,
+              sourceHandle,
+              targetHandle,
+              false,
+              {
+                target: modelTarget,
+                source: modelSource,
+                columnSource,
+                columnTarget,
+              },
+            )
+
+          ids.push(edge.id)
+          outputEdges.push(edge)
         }
       }
     }
   }
 
   return {
     edges: outputEdges,
     nodes: Object.values(nodesMap),
     nodesMap,
     columns,
+    key: ids.join('-'),
   }
 }
 
 export async function createGraphLayout({
   nodes = [],
   edges = [],
   nodesMap,
 }: {
   nodes: Node[]
   edges: Edge[]
   nodesMap: Record<string, Node>
 }): Promise<{ nodes: Node[]; edges: Edge[] }> {
+  const elk = new ELK()
   const layout = await elk.layout({
     id: 'root',
     layoutOptions: { algorithm: 'layered' },
     children: nodes.map(node => ({
       id: node.id,
       width: node.data.width,
       height: node.data.height,
@@ -180,29 +183,46 @@
   modelNames: string[],
   lineage: Record<string, Lineage>,
   highlightedNodes: string[],
   models: Map<string, Model>,
   targets: Set<string>,
   nodes: Node[],
 ): Record<string, Node> {
+  const NODE_BALANCE_SPACE = 64
+  const COLUMN_LINE_HEIGHT = 24
+  const CHAR_WIDTH = 8
+
   const current = nodes.reduce(
     (acc: Record<string, Node>, node) =>
       Object.assign(acc, { [node.id]: node }),
     {},
   )
 
   return modelNames.reduce((acc: Record<string, Node>, label: string) => {
-    const node =
-      current[label] ??
-      createGraphNode({
-        label,
-        width: NODE_WIDTH + label.length * 8,
-        height: NODE_HEIGHT + 32 * (models.get(label)?.columns?.length ?? 0),
-      })
+    const node = current[label] ?? createGraphNode({ label })
+
+    const maxWidth =
+      models.get(label)?.columns?.length == null
+        ? 0
+        : Math.max(
+            ...(models
+              .get(label)
+              ?.columns?.map(
+                column =>
+                  (column.name.length + column.type.length) * CHAR_WIDTH +
+                  NODE_BALANCE_SPACE,
+              ) ?? []),
+            label.length * CHAR_WIDTH,
+          )
+    const maxHeight =
+      COLUMN_LINE_HEIGHT * (models.get(label)?.columns?.length ?? 0) +
+      NODE_BALANCE_SPACE
 
+    node.data.width = NODE_BALANCE_SPACE + maxWidth
+    node.data.height = NODE_BALANCE_SPACE + maxHeight
     node.data.isHighlighted = highlightedNodes.includes(label)
     node.data.isInteractive =
       isArrayNotEmpty(highlightedNodes) &&
       isFalse(highlightedNodes.includes(label))
 
     if (isArrayNotEmpty(lineage[node.id]?.models)) {
       node.sourcePosition = Position.Left
@@ -226,19 +246,19 @@
 
   elkNodes.forEach(node => {
     const output = nodesMap[node.id]
 
     if (output == null) return
 
     if (output.position.x === 0 && node.x != null) {
-      output.position.x = -node.x * 2
+      output.position.x = -node.x
     }
 
     if (output.position.y === 0 && node.y != null) {
-      output.position.y = -node.y * 1.5
+      output.position.y = -node.y
     }
 
     nodes.push(output)
   })
 
   return nodes
 }
@@ -256,17 +276,15 @@
     position,
     hidden,
     data,
     connectable: false,
     selectable: false,
     deletable: false,
     focusable: false,
-    style: {
-      zIndex: 'auto',
-    },
+    zIndex: -1,
   }
 }
 
 function createGraphEdge<TData = any>(
   source: string,
   target: string,
   sourceHandle?: string,
```

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/library/components/ide/ActivePlan.tsx` & `sqlmesh-0.6.4/web/client/src/library/components/ide/ActivePlan.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/library/components/ide/IDE.tsx` & `sqlmesh-0.6.4/web/client/src/library/components/ide/IDE.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/library/components/ide/RunPlan.tsx` & `sqlmesh-0.6.4/web/client/src/library/components/ide/RunPlan.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/library/components/input/Input.tsx` & `sqlmesh-0.6.4/web/client/src/library/components/input/Input.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/library/components/input/InputToggle.tsx` & `sqlmesh-0.6.4/web/client/src/library/components/input/InputToggle.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/library/components/logo/Spinner.tsx` & `sqlmesh-0.6.4/web/client/src/library/components/logo/Spinner.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/library/components/logo/SqlMesh.tsx` & `sqlmesh-0.6.4/web/client/src/library/components/logo/SqlMesh.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/library/components/logo/Tobiko.tsx` & `sqlmesh-0.6.4/web/client/src/library/components/logo/Tobiko.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/library/components/modal/Modal.tsx` & `sqlmesh-0.6.4/web/client/src/library/components/modal/Modal.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/library/components/modal/ModalConfirmation.tsx` & `sqlmesh-0.6.4/web/client/src/library/components/modal/ModalConfirmation.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/library/components/modal/ModalDrawer.tsx` & `sqlmesh-0.6.4/web/client/src/library/components/modal/ModalDrawer.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/library/components/plan/Plan.tsx` & `sqlmesh-0.6.4/web/client/src/library/components/plan/Plan.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/library/components/plan/PlanActions.tsx` & `sqlmesh-0.6.4/web/client/src/library/components/plan/PlanActions.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/library/components/plan/PlanBackfillDates.tsx` & `sqlmesh-0.6.4/web/client/src/library/components/plan/PlanBackfillDates.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/library/components/plan/PlanChangePreview.tsx` & `sqlmesh-0.6.4/web/client/src/library/components/plan/PlanChangePreview.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/library/components/plan/PlanHeader.tsx` & `sqlmesh-0.6.4/web/client/src/library/components/plan/PlanHeader.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/library/components/plan/PlanWizard.tsx` & `sqlmesh-0.6.4/web/client/src/library/components/plan/PlanWizard.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/library/components/plan/PlanWizardStepOptions.tsx` & `sqlmesh-0.6.4/web/client/src/library/components/plan/PlanWizardStepOptions.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/library/components/plan/context.tsx` & `sqlmesh-0.6.4/web/client/src/library/components/plan/context.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/library/components/plan/help.spec.ts` & `sqlmesh-0.6.4/web/client/src/library/components/plan/help.spec.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/library/components/plan/help.ts` & `sqlmesh-0.6.4/web/client/src/library/components/plan/help.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/library/components/plan/hooks.ts` & `sqlmesh-0.6.4/web/client/src/library/components/plan/hooks.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/library/components/progress/Progress.tsx` & `sqlmesh-0.6.4/web/client/src/library/components/progress/Progress.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/library/components/report/ReportTestsErrors.tsx` & `sqlmesh-0.6.4/web/client/src/library/components/report/ReportTestsErrors.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/library/components/root/Footer.tsx` & `sqlmesh-0.6.4/web/client/src/library/components/root/Footer.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/library/components/root/Header.tsx` & `sqlmesh-0.6.4/web/client/src/library/components/root/Header.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/library/components/splitPane/SplitPane.css` & `sqlmesh-0.6.4/web/client/src/library/components/splitPane/SplitPane.css`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/library/components/splitPane/SplitPane.tsx` & `sqlmesh-0.6.4/web/client/src/library/components/splitPane/SplitPane.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/library/components/tasksOverview/TasksOverview.tsx` & `sqlmesh-0.6.4/web/client/src/library/components/tasksOverview/TasksOverview.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/library/components/toggle/Toggle.tsx` & `sqlmesh-0.6.4/web/client/src/library/components/toggle/Toggle.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/main.tsx` & `sqlmesh-0.6.4/web/client/src/main.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/models/artifact.ts` & `sqlmesh-0.6.4/web/client/src/models/artifact.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/models/directory.ts` & `sqlmesh-0.6.4/web/client/src/models/directory.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/models/environment.ts` & `sqlmesh-0.6.4/web/client/src/models/environment.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/models/file.ts` & `sqlmesh-0.6.4/web/client/src/models/file.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/models/initial.ts` & `sqlmesh-0.6.4/web/client/src/models/initial.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/tests/utils.tsx` & `sqlmesh-0.6.4/web/client/src/tests/utils.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/utils/index.spec.ts` & `sqlmesh-0.6.4/web/client/src/utils/index.spec.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/utils/index.ts` & `sqlmesh-0.6.4/web/client/src/utils/index.ts`

 * *Files 2% similar despite different names*

```diff
@@ -202,7 +202,14 @@
     clearTimeout(timeoutIdTrailing)
     timeoutIdLeading = undefined
     timeoutIdTrailing = undefined
   }
 
   return callback
 }
+
+export function uid(): string {
+  const time = new Date().getTime().toString(36)
+  const random = Math.random().toString(36).substring(2, 8)
+
+  return time + random
+}
```

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/workers/sqlglot/sqlglot.py` & `sqlmesh-0.6.4/web/client/src/workers/sqlglot/sqlglot.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/src/workers/sqlglot/worker.ts` & `sqlmesh-0.6.4/web/client/src/workers/sqlglot/worker.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/tailwind.config.js` & `sqlmesh-0.6.4/web/client/tailwind.config.js`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/tsconfig.json` & `sqlmesh-0.6.4/web/client/tsconfig.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/client/vite.config.ts` & `sqlmesh-0.6.4/web/client/vite.config.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/server/api/endpoints/__init__.py` & `sqlmesh-0.6.4/web/server/api/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/server/api/endpoints/commands.py` & `sqlmesh-0.6.4/web/server/api/endpoints/commands.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/server/api/endpoints/context.py` & `sqlmesh-0.6.4/web/server/api/endpoints/context.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/server/api/endpoints/directories.py` & `sqlmesh-0.6.4/web/server/api/endpoints/directories.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/server/api/endpoints/environments.py` & `sqlmesh-0.6.4/web/server/api/endpoints/environments.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/server/api/endpoints/events.py` & `sqlmesh-0.6.4/web/server/api/endpoints/events.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/server/api/endpoints/files.py` & `sqlmesh-0.6.4/web/server/api/endpoints/files.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/server/api/endpoints/lineage.py` & `sqlmesh-0.6.4/web/server/api/endpoints/lineage.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/server/api/endpoints/models.py` & `sqlmesh-0.6.4/web/server/api/endpoints/models.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/server/api/endpoints/plan.py` & `sqlmesh-0.6.4/web/server/api/endpoints/plan.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/server/console.py` & `sqlmesh-0.6.4/web/server/console.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/server/main.py` & `sqlmesh-0.6.4/web/server/main.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/server/models.py` & `sqlmesh-0.6.4/web/server/models.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/server/settings.py` & `sqlmesh-0.6.4/web/server/settings.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/server/sse.py` & `sqlmesh-0.6.4/web/server/sse.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/server/utils.py` & `sqlmesh-0.6.4/web/server/utils.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev5/web/server/watcher.py` & `sqlmesh-0.6.4/web/server/watcher.py`

 * *Files identical despite different names*

