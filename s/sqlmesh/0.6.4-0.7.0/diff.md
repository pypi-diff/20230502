# Comparing `tmp/sqlmesh-0.6.4.tar.gz` & `tmp/sqlmesh-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlmesh-0.6.4.tar", last modified: Mon May  1 23:49:56 2023, max compression
+gzip compressed data, was "sqlmesh-0.7.0.tar", last modified: Tue May  2 18:24:02 2023, max compression
```

## Comparing `sqlmesh-0.6.4.tar` & `sqlmesh-0.7.0.tar`

### file list

```diff
@@ -1,752 +1,753 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.990806 sqlmesh-0.6.4/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.886803 sqlmesh-0.6.4/.circleci/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1872 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/.circleci/config.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4414 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/.circleci/continue_config.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       66 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/.dockerignore
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2152 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/.gitignore
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1900 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/.pre-commit-config.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      234 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/.readthedocs.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      135 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/Dockerfile.api
--rw-r--r--   0 circleci  (1001) circleci  (1002)      383 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/Dockerfile.app
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11346 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1855 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/Makefile
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1936 2023-05-01 23:49:56.990806 sqlmesh-0.6.4/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1192 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1008 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docker-compose.yml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.890804 sqlmesh-0.6.4/docs/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.866803 sqlmesh-0.6.4/docs/_readthedocs/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.890804 sqlmesh-0.6.4/docs/_readthedocs/html/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/_readthedocs/html/.keep
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9965 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/comparisons.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.890804 sqlmesh-0.6.4/docs/concepts/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.890804 sqlmesh-0.6.4/docs/concepts/architecture/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1334 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/concepts/architecture/serialization.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1113 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/concepts/architecture/snapshots.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6689 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/concepts/audits.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3866 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/concepts/environments.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5952 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/concepts/glossary.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/concepts/hooks.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3027 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/concepts/macros.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.890804 sqlmesh-0.6.4/docs/concepts/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9934 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/concepts/models/model_kinds.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8189 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/concepts/models/overview.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7171 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/concepts/models/python_models.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4938 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/concepts/models/seed_models.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5356 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/concepts/models/sql_models.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6637 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/concepts/overview.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.894804 sqlmesh-0.6.4/docs/concepts/plans/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    43124 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/concepts/plans/model_versioning.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9954 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/concepts/plans.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5699 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/concepts/tests.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      607 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/development.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.894804 sqlmesh-0.6.4/docs/guides/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1943 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/guides/connections.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1309 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/guides/migrations.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10756 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/guides/models.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6133 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/guides/multi_repo.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2142 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/guides/projects.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.894804 sqlmesh-0.6.4/docs/guides/scheduling/
--rw-r--r--   0 circleci  (1001) circleci  (1002)   740917 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/guides/scheduling/airflow_successful_plan_apply.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)   379880 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/guides/scheduling/airflow_successful_setup.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5648 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/guides/scheduling.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1854 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/guides/testing.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5459 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/index.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      297 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/installation.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.894804 sqlmesh-0.6.4/docs/integrations/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2905 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/integrations/airflow.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7801 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/integrations/dbt.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24057 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/integrations/engines.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      867 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/integrations/github.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      217 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/integrations/overview.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      665 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/prerequisites.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12925 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/quick_start.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.894804 sqlmesh-0.6.4/docs/reference/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6093 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/reference/cli.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13607 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/reference/configuration.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4579 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/reference/notebook.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1127 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/reference/overview.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)       14 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/reference/python.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/release_notes.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      122 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/requirements.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3249 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/docs/sqlmesh.png
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.898804 sqlmesh-0.6.4/examples/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.898804 sqlmesh-0.6.4/examples/airflow/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1713 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/airflow/Dockerfile.template
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2164 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/airflow/Makefile
--rw-r--r--   0 circleci  (1001) circleci  (1002)      942 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/airflow/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/airflow/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.898804 sqlmesh-0.6.4/examples/airflow/dags/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      263 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/airflow/dags/sqlmesh_integration.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3515 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/airflow/docker_compose_decorator.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/airflow/requirements.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.898804 sqlmesh-0.6.4/examples/airflow/spark_conf/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      872 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/airflow/spark_conf/hive-site.xml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      151 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/airflow/spark_conf/spark-defaults.conf
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.866803 sqlmesh-0.6.4/examples/multi/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.898804 sqlmesh-0.6.4/examples/multi/repo_1/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.898804 sqlmesh-0.6.4/examples/multi/repo_1/audits/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/multi/repo_1/audits/.gitkeep
--rw-r--r--   0 circleci  (1001) circleci  (1002)      147 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/multi/repo_1/config.yaml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.898804 sqlmesh-0.6.4/examples/multi/repo_1/macros/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/multi/repo_1/macros/.gitkeep
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/multi/repo_1/macros/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.898804 sqlmesh-0.6.4/examples/multi/repo_1/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/multi/repo_1/models/.gitkeep
--rw-r--r--   0 circleci  (1001) circleci  (1002)       63 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/multi/repo_1/models/a.sql
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/multi/repo_1/models/b.sql
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.898804 sqlmesh-0.6.4/examples/multi/repo_1/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/multi/repo_1/tests/.gitkeep
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.898804 sqlmesh-0.6.4/examples/multi/repo_2/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.898804 sqlmesh-0.6.4/examples/multi/repo_2/audits/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/multi/repo_2/audits/.gitkeep
--rw-r--r--   0 circleci  (1001) circleci  (1002)      147 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/multi/repo_2/config.yaml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.898804 sqlmesh-0.6.4/examples/multi/repo_2/macros/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/multi/repo_2/macros/.gitkeep
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/multi/repo_2/macros/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.898804 sqlmesh-0.6.4/examples/multi/repo_2/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/multi/repo_2/models/.gitkeep
--rw-r--r--   0 circleci  (1001) circleci  (1002)       64 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/multi/repo_2/models/c.sql
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/multi/repo_2/models/d.sql
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.898804 sqlmesh-0.6.4/examples/multi/repo_2/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/multi/repo_2/tests/.gitkeep
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.902804 sqlmesh-0.6.4/examples/sushi/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.902804 sqlmesh-0.6.4/examples/sushi/audits/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      105 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi/audits/items.sql
--rw-r--r--   0 circleci  (1001) circleci  (1002)      119 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi/audits/order_items.sql
--rw-r--r--   0 circleci  (1001) circleci  (1002)      829 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi/config.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.902804 sqlmesh-0.6.4/examples/sushi/data/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi/data/.keep
--rw-r--r--   0 circleci  (1001) circleci  (1002)      551 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi/helper.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.902804 sqlmesh-0.6.4/examples/sushi/hooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi/hooks/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      247 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi/hooks/hooks.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.902804 sqlmesh-0.6.4/examples/sushi/macros/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi/macros/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      702 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi/macros/macros.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.902804 sqlmesh-0.6.4/examples/sushi/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      934 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi/models/customer_revenue_by_day.sql
--rw-r--r--   0 circleci  (1001) circleci  (1002)      223 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi/models/customers.sql
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1911 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi/models/items.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1912 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi/models/order_items.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1643 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi/models/orders.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      346 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi/models/top_waiters.sql
--rw-r--r--   0 circleci  (1001) circleci  (1002)      465 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi/models/waiter_as_customer_by_day.sql
--rw-r--r--   0 circleci  (1001) circleci  (1002)      123 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi/models/waiter_names.sql
--rw-r--r--   0 circleci  (1001) circleci  (1002)      691 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi/models/waiter_revenue_by_day.sql
--rw-r--r--   0 circleci  (1001) circleci  (1002)      197 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi/models/waiters.sql
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.902804 sqlmesh-0.6.4/examples/sushi/seeds/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       88 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi/seeds/waiter_names.csv
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.902804 sqlmesh-0.6.4/examples/sushi/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1459 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi/tests/test_customer_revenue_by_day.yaml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.906804 sqlmesh-0.6.4/examples/sushi_dbt/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       15 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/.gitignore
--rw-r--r--   0 circleci  (1001) circleci  (1002)       41 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/.user.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.906804 sqlmesh-0.6.4/examples/sushi_dbt/analyses/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/analyses/.gitkeep
--rw-r--r--   0 circleci  (1001) circleci  (1002)      291 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/config.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      507 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/dbt_project.yml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.906804 sqlmesh-0.6.4/examples/sushi_dbt/macros/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      941 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/macros/incremental.sql
--rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/macros/log_value.sql
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.906804 sqlmesh-0.6.4/examples/sushi_dbt/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1125 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/models/customer_revenue_by_day.sql
--rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/models/customers.sql
--rw-r--r--   0 circleci  (1001) circleci  (1002)      182 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/models/schema.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      309 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/models/top_waiters.sql
--rw-r--r--   0 circleci  (1001) circleci  (1002)      389 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/models/waiter_as_customer_by_day.sql
--rw-r--r--   0 circleci  (1001) circleci  (1002)      752 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/models/waiter_revenue_by_day.sql
--rw-r--r--   0 circleci  (1001) circleci  (1002)      186 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/models/waiters.sql
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.870803 sqlmesh-0.6.4/examples/sushi_dbt/packages/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.906804 sqlmesh-0.6.4/examples/sushi_dbt/packages/customers/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.906804 sqlmesh-0.6.4/examples/sushi_dbt/packages/customers/analyses/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/packages/customers/analyses/.gitkeep
--rw-r--r--   0 circleci  (1001) circleci  (1002)      663 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/packages/customers/dbt_project.yml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.906804 sqlmesh-0.6.4/examples/sushi_dbt/packages/customers/macros/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      117 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/packages/customers/macros/current_engine.sql
--rw-r--r--   0 circleci  (1001) circleci  (1002)       65 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/packages/customers/macros/distinct.sql
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.906804 sqlmesh-0.6.4/examples/sushi_dbt/packages/customers/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/packages/customers/models/schema.yml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.906804 sqlmesh-0.6.4/examples/sushi_dbt/packages/customers/seeds/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/packages/customers/seeds/.gitkeep
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.906804 sqlmesh-0.6.4/examples/sushi_dbt/packages/customers/snapshots/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/packages/customers/snapshots/.gitkeep
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.906804 sqlmesh-0.6.4/examples/sushi_dbt/packages/customers/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/packages/customers/tests/.gitkeep
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1092 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/profiles.yml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.906804 sqlmesh-0.6.4/examples/sushi_dbt/seeds/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2327 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/seeds/items.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10472 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/seeds/order_items.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9746 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/seeds/orders.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)       97 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/seeds/properties.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       88 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/seeds/waiter_names.csv
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.906804 sqlmesh-0.6.4/examples/sushi_dbt/snapshots/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/snapshots/.gitkeep
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.906804 sqlmesh-0.6.4/examples/sushi_dbt/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/sushi_dbt/tests/.gitkeep
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.910804 sqlmesh-0.6.4/examples/wursthall/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/wursthall/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.870803 sqlmesh-0.6.4/examples/wursthall/audits/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.910804 sqlmesh-0.6.4/examples/wursthall/audits/db/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      141 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/wursthall/audits/db/order_f.sql
--rw-r--r--   0 circleci  (1001) circleci  (1002)       66 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/wursthall/config.yaml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.910804 sqlmesh-0.6.4/examples/wursthall/macros/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/wursthall/macros/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      618 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/wursthall/macros/macros.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.910804 sqlmesh-0.6.4/examples/wursthall/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/wursthall/models/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.910804 sqlmesh-0.6.4/examples/wursthall/models/db/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      433 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/wursthall/models/db/customer_d.sql
--rw-r--r--   0 circleci  (1001) circleci  (1002)      256 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/wursthall/models/db/item_d.sql
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3158 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/wursthall/models/db/order_f.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      542 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/wursthall/models/db/order_item_f.sql
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.910804 sqlmesh-0.6.4/examples/wursthall/models/src/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/wursthall/models/src/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1652 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/wursthall/models/src/customer_details.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      120 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/wursthall/models/src/menu_item_details.sql
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3414 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/wursthall/models/src/order_item_details.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      892 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/wursthall/models/src/shared.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.870803 sqlmesh-0.6.4/examples/wursthall/seeds/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.910804 sqlmesh-0.6.4/examples/wursthall/seeds/src/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7416 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/wursthall/seeds/src/menu_item_details.csv
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.910804 sqlmesh-0.6.4/examples/wursthall/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      888 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/wursthall/tests/test_customer_d.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      955 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/examples/wursthall/tests/test_order_item_f.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2113 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/mkdocs.yml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.910804 sqlmesh-0.6.4/pdoc/
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     1153 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/pdoc/cli.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.910804 sqlmesh-0.6.4/pdoc/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      131 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/pdoc/templates/module.html.jinja2
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.910804 sqlmesh-0.6.4/posts/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.914804 sqlmesh-0.6.4/posts/virtual_data_environments/
--rw-r--r--   0 circleci  (1001) circleci  (1002)   318753 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/posts/virtual_data_environments/change_categorization.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)   274526 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/posts/virtual_data_environments/isolated_rigid_envs.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)   163619 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/posts/virtual_data_environments/partial_breaking.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)   298971 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/posts/virtual_data_environments/stateful_envs.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)   366545 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/posts/virtual_data_environments/virtual_envs.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)  1344487 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/posts/virtual_data_environments/virtual_envs_end_to_end.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18638 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/posts/virtual_data_environments.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      734 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/pytest.ini
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1393 2023-05-01 23:49:56.990806 sqlmesh-0.6.4/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3164 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.918805 sqlmesh-0.6.4/sqlmesh/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        3 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/.airflowignore
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3950 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      160 2023-05-01 23:49:56.000000 sqlmesh-0.6.4/sqlmesh/_version.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.918805 sqlmesh-0.6.4/sqlmesh/cli/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      898 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/cli/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4742 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/cli/example_project.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9930 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/cli/main.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1433 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/cli/options.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.922804 sqlmesh-0.6.4/sqlmesh/core/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      586 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/_typing.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.922804 sqlmesh-0.6.4/sqlmesh/core/audit/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      449 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/audit/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1071 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/audit/builtin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8136 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/audit/definition.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.926805 sqlmesh-0.6.4/sqlmesh/core/config/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      668 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/config/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4412 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/config/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1001 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/config/categorizer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      940 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/config/common.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21184 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/config/connection.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3351 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/config/loader.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1655 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/config/model.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5611 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/config/root.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8421 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/config/scheduler.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    31743 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/console.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      826 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    36329 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/context.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8904 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/context_diff.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17484 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/dialect.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.926805 sqlmesh-0.6.4/sqlmesh/core/engine_adapter/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2626 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/engine_adapter/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      762 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/engine_adapter/_typing.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    29549 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/engine_adapter/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4191 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/engine_adapter/base_postgres.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4238 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/engine_adapter/base_spark.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15681 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/engine_adapter/bigquery.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      402 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/engine_adapter/databricks.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1939 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/engine_adapter/databricks_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1971 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/engine_adapter/duckdb.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2149 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/engine_adapter/postgres.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6673 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/engine_adapter/redshift.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1181 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/engine_adapter/shared.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2658 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/engine_adapter/snowflake.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4879 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/engine_adapter/spark.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1849 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/environment.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      742 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/hooks.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12673 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/loader.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19726 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/macros.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.930805 sqlmesh-0.6.4/sqlmesh/core/model/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      594 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/model/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1746 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/model/cache.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1300 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/model/common.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2417 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/model/decorator.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    47510 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/model/definition.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8168 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/model/kind.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13069 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/model/meta.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2017 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/model/seed.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2314 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/notification_target.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.930805 sqlmesh-0.6.4/sqlmesh/core/plan/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      191 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/plan/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23956 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/plan/definition.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8565 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/plan/evaluator.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12623 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/renderer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15386 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/scheduler.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20418 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/schema_diff.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.930805 sqlmesh-0.6.4/sqlmesh/core/snapshot/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      527 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/snapshot/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1990 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/snapshot/categorizer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    34694 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/snapshot/definition.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19245 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/snapshot/evaluator.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.930805 sqlmesh-0.6.4/sqlmesh/core/state_sync/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      692 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/state_sync/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13382 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/state_sync/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14349 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/state_sync/common.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20765 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/state_sync/engine_adapter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10834 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1412 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/core/user.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.934805 sqlmesh-0.6.4/sqlmesh/dbt/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       79 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/dbt/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9390 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/dbt/adapter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17485 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/dbt/basemodel.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11231 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/dbt/builtin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1762 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/dbt/column.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4978 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/dbt/common.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5087 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/dbt/context.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8044 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/dbt/loader.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9851 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/dbt/model.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13257 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/dbt/package.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3701 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/dbt/profile.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4772 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/dbt/project.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      927 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/dbt/seed.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3137 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/dbt/source.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13618 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/dbt/target.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      291 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/dbt/util.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.934805 sqlmesh-0.6.4/sqlmesh/engines/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/engines/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4437 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/engines/commands.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.934805 sqlmesh-0.6.4/sqlmesh/engines/spark/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/engines/spark/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3414 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/engines/spark/app.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.934805 sqlmesh-0.6.4/sqlmesh/engines/spark/db_api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/engines/spark/db_api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      148 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/engines/spark/db_api/errors.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2571 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/engines/spark/db_api/spark_session.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.934805 sqlmesh-0.6.4/sqlmesh/integrations/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/integrations/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.934805 sqlmesh-0.6.4/sqlmesh/integrations/github/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/integrations/github/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2210 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/integrations/github/notification_operator_provider.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1726 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/integrations/github/notification_target.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1829 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/integrations/github/shared.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13960 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/magics.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.938805 sqlmesh-0.6.4/sqlmesh/migrations/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/migrations/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1749 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/migrations/v0001_init.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      103 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/migrations/v0002_remove_identify.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1183 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/migrations/v0003_move_batch_size.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      534 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/migrations/v0004_environmnent_add_finalized_at.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/py.typed
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.938805 sqlmesh-0.6.4/sqlmesh/schedulers/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/schedulers/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.938805 sqlmesh-0.6.4/sqlmesh/schedulers/airflow/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/schedulers/airflow/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4020 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/schedulers/airflow/api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8128 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/schedulers/airflow/client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3888 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/schedulers/airflow/common.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19132 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/schedulers/airflow/dag_generator.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.938805 sqlmesh-0.6.4/sqlmesh/schedulers/airflow/hooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/schedulers/airflow/hooks/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2132 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/schedulers/airflow/hooks/bigquery.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      868 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/schedulers/airflow/hooks/redshift.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8508 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/schedulers/airflow/integration.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.942805 sqlmesh-0.6.4/sqlmesh/schedulers/airflow/operators/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/schedulers/airflow/operators/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1444 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/schedulers/airflow/operators/bigquery.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6307 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/schedulers/airflow/operators/databricks.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2549 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/schedulers/airflow/operators/hwm_sensor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      877 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/schedulers/airflow/operators/notification.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1322 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/schedulers/airflow/operators/postgres.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1211 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/schedulers/airflow/operators/redshift.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1340 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/schedulers/airflow/operators/snowflake.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5222 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/schedulers/airflow/operators/spark_submit.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11104 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/schedulers/airflow/operators/targets.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4660 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/schedulers/airflow/plan.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1292 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/schedulers/airflow/plugin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4139 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/schedulers/airflow/state_sync.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5213 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/schedulers/airflow/util.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.942805 sqlmesh-0.6.4/sqlmesh/utils/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4386 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/utils/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3593 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/utils/cache.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8053 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/utils/concurrency.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7530 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/utils/connection_pool.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      410 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/utils/conversions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4329 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/utils/dag.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7549 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/utils/date.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1244 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/utils/errors.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16133 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/utils/jinja.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15093 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/utils/metaprogramming.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      888 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/utils/pandas.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1609 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/utils/pydantic.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1534 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/utils/rich.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6487 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/utils/transactional_file.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1419 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh/utils/yaml.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.918805 sqlmesh-0.6.4/sqlmesh.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1936 2023-05-01 23:49:56.000000 sqlmesh-0.6.4/sqlmesh.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21986 2023-05-01 23:49:56.000000 sqlmesh-0.6.4/sqlmesh.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-01 23:49:56.000000 sqlmesh-0.6.4/sqlmesh.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      141 2023-05-01 23:49:56.000000 sqlmesh-0.6.4/sqlmesh.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      844 2023-05-01 23:49:56.000000 sqlmesh-0.6.4/sqlmesh.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2023-05-01 23:49:56.000000 sqlmesh-0.6.4/sqlmesh.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21020 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/sqlmesh.svg
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.942805 sqlmesh-0.6.4/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      285 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/common_fixtures.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4037 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/conftest.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.946805 sqlmesh-0.6.4/tests/core/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.946805 sqlmesh-0.6.4/tests/core/engine_adapter/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/engine_adapter/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    28133 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/engine_adapter/test_base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2114 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/engine_adapter/test_base_postgres.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1270 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/engine_adapter/test_base_spark.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7171 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/engine_adapter/test_bigquery.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1253 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/engine_adapter/test_databricks.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2613 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/engine_adapter/test_duckdb.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1569 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/engine_adapter/test_postgres.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8036 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/engine_adapter/test_redshift.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3191 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/engine_adapter/test_spark.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7073 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/test_audit.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6611 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/test_config.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      850 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/test_connection_config.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10197 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/test_context.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2749 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/test_dialect.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      464 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/test_environment.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    26773 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/test_integration.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6500 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/test_macros.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    25378 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/test_model.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17081 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/test_plan.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3890 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/test_plan_evaluator.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4647 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/test_scheduler.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    32235 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/test_schema_diff.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      857 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/test_seed.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    29629 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/test_snapshot.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10299 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/test_snapshot_evaluator.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24610 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/core/test_state_sync.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.950805 sqlmesh-0.6.4/tests/dbt/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/dbt/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      739 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/dbt/conftest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2537 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/dbt/test_adapter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13195 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/dbt/test_config.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17095 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/dbt/test_transformation.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.950805 sqlmesh-0.6.4/tests/engines/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/engines/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.950805 sqlmesh-0.6.4/tests/engines/spark/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/engines/spark/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      357 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/engines/spark/conftest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1503 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/engines/spark/test_db_api.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.878803 sqlmesh-0.6.4/tests/fixtures/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.874803 sqlmesh-0.6.4/tests/fixtures/dbt/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.950805 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.950805 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/analyses/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/analyses/.gitkeep
--rw-r--r--   0 circleci  (1001) circleci  (1002)      291 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/config.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.878803 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/dbt_packages/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1055 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/dbt_project.yml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.950805 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/logs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10264 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/logs/dbt.log.legacy
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.950805 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/macros/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      941 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/macros/incremental.sql
--rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/macros/log_value.sql
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.950805 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      247 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/models/schema.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      334 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/models/top_waiters.sql
--rw-r--r--   0 circleci  (1001) circleci  (1002)      389 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/models/waiter_as_customer_by_day.sql
--rw-r--r--   0 circleci  (1001) circleci  (1002)      863 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/models/waiter_revenue_by_day.sql
--rw-r--r--   0 circleci  (1001) circleci  (1002)      196 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/models/waiters.sql
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.878803 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/packages/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.950805 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/packages/customers/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.950805 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/packages/customers/analyses/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/packages/customers/analyses/.gitkeep
--rw-r--r--   0 circleci  (1001) circleci  (1002)      663 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/packages/customers/dbt_project.yml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.950805 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/packages/customers/macros/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      117 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/packages/customers/macros/current_engine.sql
--rw-r--r--   0 circleci  (1001) circleci  (1002)       65 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/packages/customers/macros/distinct.sql
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.954805 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/packages/customers/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1155 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/packages/customers/models/customer_revenue_by_day.sql
--rw-r--r--   0 circleci  (1001) circleci  (1002)      108 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/packages/customers/models/customers.sql
--rw-r--r--   0 circleci  (1001) circleci  (1002)      193 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/packages/customers/models/schema.yml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.954805 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/packages/customers/seeds/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/packages/customers/seeds/.gitkeep
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.954805 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/packages/customers/snapshots/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/packages/customers/snapshots/.gitkeep
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.954805 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/packages/customers/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/packages/customers/tests/.gitkeep
--rw-r--r--   0 circleci  (1001) circleci  (1002)       41 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/packages.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      540 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/profiles.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1250 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/seed_sources.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.954805 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/seeds/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       42 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/seeds/properties.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       88 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/seeds/waiter_names.csv
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.954805 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/snapshots/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/snapshots/.gitkeep
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.954805 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/source_data/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2327 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/source_data/items.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10472 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/source_data/order_items.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9746 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/source_data/orders.csv
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.954805 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/tests/.gitkeep
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.954805 sqlmesh-0.6.4/tests/fixtures/migrations/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9823 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/migrations/environments.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)    25229 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/fixtures/migrations/snapshots.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.954805 sqlmesh-0.6.4/tests/integrations/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/integrations/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.954805 sqlmesh-0.6.4/tests/integrations/github/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/integrations/github/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.954805 sqlmesh-0.6.4/tests/integrations/github/fixtures/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      816 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/integrations/github/fixtures/pull_request_review.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      477 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/integrations/github/test_notification_target.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.954805 sqlmesh-0.6.4/tests/schedulers/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/schedulers/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.954805 sqlmesh-0.6.4/tests/schedulers/airflow/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/schedulers/airflow/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1414 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/schedulers/airflow/conftest.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.958806 sqlmesh-0.6.4/tests/schedulers/airflow/operators/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/schedulers/airflow/operators/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4442 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/schedulers/airflow/operators/test_hwm_sensor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4392 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/schedulers/airflow/operators/test_targets.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9920 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/schedulers/airflow/test_client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1345 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/schedulers/airflow/test_end_to_end.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6222 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/schedulers/airflow/test_integration.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6054 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/schedulers/airflow/test_plan.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.958806 sqlmesh-0.6.4/tests/utils/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/utils/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1118 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/utils/test_cache.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3580 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/utils/test_concurrency.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6430 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/utils/test_connection_pool.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1381 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/utils/test_dag.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1818 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/utils/test_date.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      551 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/utils/test_filesystem.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5516 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/utils/test_jinja.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5790 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/utils/test_metaprogramming.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2501 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/utils/test_pandas.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      518 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/utils/test_pydantic.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2911 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/utils/test_transactional_file.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1194 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/utils/test_yaml.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.958806 sqlmesh-0.6.4/tests/web/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/web/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16232 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/tests/web/test_main.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.958806 sqlmesh-0.6.4/web/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.962806 sqlmesh-0.6.4/web/client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1104 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/.eslintrc.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)       94 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/.gitignore
--rw-r--r--   0 circleci  (1001) circleci  (1002)      129 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/.prettierignore
--rw-r--r--   0 circleci  (1001) circleci  (1002)      403 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/.prettierrc.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.962806 sqlmesh-0.6.4/web/client/dist/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.966806 sqlmesh-0.6.4/web/client/dist/assets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    74500 2023-05-01 23:49:40.000000 sqlmesh-0.6.4/web/client/dist/assets/CircularStd-Black-52659624.otf
--rw-r--r--   0 circleci  (1001) circleci  (1002)    74368 2023-05-01 23:49:40.000000 sqlmesh-0.6.4/web/client/dist/assets/CircularStd-Bold-0e6c076d.otf
--rw-r--r--   0 circleci  (1001) circleci  (1002)    74116 2023-05-01 23:49:40.000000 sqlmesh-0.6.4/web/client/dist/assets/CircularStd-Medium-2f373e53.otf
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24788 2023-05-01 23:49:40.000000 sqlmesh-0.6.4/web/client/dist/assets/Plan-683a0552.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    55004 2023-05-01 23:49:40.000000 sqlmesh-0.6.4/web/client/dist/assets/Publico-Black-e6bd2ea2.otf
--rw-r--r--   0 circleci  (1001) circleci  (1002)    57104 2023-05-01 23:49:40.000000 sqlmesh-0.6.4/web/client/dist/assets/Publico-Bold-c79acd56.otf
--rw-r--r--   0 circleci  (1001) circleci  (1002)    56836 2023-05-01 23:49:40.000000 sqlmesh-0.6.4/web/client/dist/assets/Publico-Medium-01b4a891.otf
--rw-r--r--   0 circleci  (1001) circleci  (1002)    43132 2023-05-01 23:49:40.000000 sqlmesh-0.6.4/web/client/dist/assets/index-b61dbb6f.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)  2636063 2023-05-01 23:49:40.000000 sqlmesh-0.6.4/web/client/dist/assets/index-f2c4b7c5.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2419 2023-05-01 23:49:40.000000 sqlmesh-0.6.4/web/client/dist/assets/worker-e891d118.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.966806 sqlmesh-0.6.4/web/client/dist/favicons/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2473 2023-05-01 23:49:37.000000 sqlmesh-0.6.4/web/client/dist/favicons/favicon.ico
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1150 2023-05-01 23:49:40.000000 sqlmesh-0.6.4/web/client/dist/index.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1076 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/index.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)    37689 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/openapi.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      330 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/orval.config.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)   408504 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/package-lock.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2389 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1642 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/playwright.config.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)       82 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/postcss.config.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.882803 sqlmesh-0.6.4/web/client/public/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.966806 sqlmesh-0.6.4/web/client/public/favicons/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2473 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/public/favicons/favicon.ico
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.966806 sqlmesh-0.6.4/web/client/src/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.966806 sqlmesh-0.6.4/web/client/src/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1236 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/api/channels.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5243 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/api/index.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3247 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/api/instance.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.882803 sqlmesh-0.6.4/web/client/src/assets/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.882803 sqlmesh-0.6.4/web/client/src/assets/fonts/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.970806 sqlmesh-0.6.4/web/client/src/assets/fonts/Circular STD/
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)    74500 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/assets/fonts/Circular STD/CircularStd-Black.otf
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)    74524 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/assets/fonts/Circular STD/CircularStd-BlackItalic.otf
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)    74368 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/assets/fonts/Circular STD/CircularStd-Bold.otf
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)    73964 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/assets/fonts/Circular STD/CircularStd-BoldItalic.otf
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)    68940 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/assets/fonts/Circular STD/CircularStd-Book.otf
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)    67284 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/assets/fonts/Circular STD/CircularStd-BookItalic.otf
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)    74116 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/assets/fonts/Circular STD/CircularStd-Medium.otf
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)    73916 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/assets/fonts/Circular STD/CircularStd-MediumItalic.otf
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.974806 sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)    55004 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/Publico-Black.otf
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)    56384 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/Publico-BlackItalic.otf
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)    57104 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/Publico-Bold.otf
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)    62320 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/Publico-BoldItalic.otf
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)    56652 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/Publico-Extrabold.otf
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)    61688 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/Publico-ExtraboldItalic.otf
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)    57680 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/Publico-Italic.otf
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)    53148 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/Publico-Light.otf
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)    57060 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/Publico-LightItalic.otf
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)    56836 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/Publico-Medium.otf
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)    61460 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/Publico-MediumItalic.otf
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)    52820 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/Publico-Roman.otf
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)    59176 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/PublicoText-Bold.otf
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)    63876 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/PublicoText-BoldItalic.otf
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)    60768 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/PublicoText-Italic.otf
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)    81732 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/PublicoText-Roman.otf
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)    60992 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/PublicoText-Semibold.otf
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)    64792 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/PublicoText-SemiboldItalic.otf
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.974806 sqlmesh-0.6.4/web/client/src/context/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4126 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/context/context.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6470 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/context/editor.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      923 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/context/fileTree.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2187 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/context/lineage.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2661 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/context/plan.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1562 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/context/theme.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.974806 sqlmesh-0.6.4/web/client/src/hooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      308 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/hooks/useActiveFocus.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      817 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/hooks/useLocalStorage.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9555 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/index.css
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.882803 sqlmesh-0.6.4/web/client/src/library/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.886803 sqlmesh-0.6.4/web/client/src/library/components/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.974806 sqlmesh-0.6.4/web/client/src/library/components/banner/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1705 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/banner/Banner.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.974806 sqlmesh-0.6.4/web/client/src/library/components/button/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4517 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/button/Button.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.974806 sqlmesh-0.6.4/web/client/src/library/components/button/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3516 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/button/tests/Button.spec.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.974806 sqlmesh-0.6.4/web/client/src/library/components/divider/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      856 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/divider/Divider.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.974806 sqlmesh-0.6.4/web/client/src/library/components/divider/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      632 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/divider/tests/Divider.spec.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.978806 sqlmesh-0.6.4/web/client/src/library/components/editor/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1992 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/editor/Editor.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5764 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/editor/Editor.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8518 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/editor/EditorCode.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2718 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/editor/EditorFooter.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1990 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/editor/EditorIndicator.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9819 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/editor/EditorInspector.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11905 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/editor/EditorPreview.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3527 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/editor/EditorTabs.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.978806 sqlmesh-0.6.4/web/client/src/library/components/editor/extensions/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5820 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/editor/extensions/SqlMeshDialect.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5744 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/editor/extensions/index.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1538 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/editor/help.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.978806 sqlmesh-0.6.4/web/client/src/library/components/fileTree/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10852 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/fileTree/Directory.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6045 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/fileTree/File.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2997 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/fileTree/FileTree.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      562 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/fileTree/help.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.978806 sqlmesh-0.6.4/web/client/src/library/components/graph/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      159 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/graph/Graph.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14454 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/graph/Graph.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7679 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/graph/help.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.978806 sqlmesh-0.6.4/web/client/src/library/components/ide/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4342 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/ide/ActivePlan.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4933 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/ide/IDE.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22356 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/ide/RunPlan.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.978806 sqlmesh-0.6.4/web/client/src/library/components/input/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2087 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/input/Input.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      688 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/input/InputToggle.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.978806 sqlmesh-0.6.4/web/client/src/library/components/loading/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      486 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/loading/Loading.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.978806 sqlmesh-0.6.4/web/client/src/library/components/logo/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2292 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/logo/Spinner.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4637 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/logo/SqlMesh.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8042 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/logo/Tobiko.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.978806 sqlmesh-0.6.4/web/client/src/library/components/modal/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1560 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/modal/Modal.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1953 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/modal/ModalConfirmation.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1447 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/modal/ModalDrawer.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.982806 sqlmesh-0.6.4/web/client/src/library/components/plan/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9269 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/plan/Plan.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6775 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/plan/PlanActions.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1312 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/plan/PlanBackfillDates.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10448 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/plan/PlanChangePreview.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4920 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/plan/PlanHeader.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15855 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/plan/PlanWizard.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9926 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/plan/PlanWizardStepOptions.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12528 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/plan/context.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3444 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/plan/help.spec.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2155 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/plan/help.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2599 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/plan/hooks.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.982806 sqlmesh-0.6.4/web/client/src/library/components/progress/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      713 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/progress/Progress.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.982806 sqlmesh-0.6.4/web/client/src/library/components/report/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1047 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/report/ReportTestsErrors.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.982806 sqlmesh-0.6.4/web/client/src/library/components/root/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      526 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/root/Footer.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1921 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/root/Header.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      247 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/root/Main.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      443 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/root/Root.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.982806 sqlmesh-0.6.4/web/client/src/library/components/splitPane/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      788 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/splitPane/SplitPane.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)      541 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/splitPane/SplitPane.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.982806 sqlmesh-0.6.4/web/client/src/library/components/tasksOverview/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11713 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/tasksOverview/TasksOverview.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.982806 sqlmesh-0.6.4/web/client/src/library/components/toggle/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1453 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/library/components/toggle/Toggle.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1197 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/main.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.982806 sqlmesh-0.6.4/web/client/src/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1647 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/models/artifact.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3472 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/models/directory.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4190 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/models/environment.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2190 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/models/file.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      173 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/models/index.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      766 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/models/initial.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      200 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/routes.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.986806 sqlmesh-0.6.4/web/client/src/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       35 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/tests/setup.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      541 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/tests/utils.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.986806 sqlmesh-0.6.4/web/client/src/types/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      467 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/types/enum.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      137 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/types/index.d.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.986806 sqlmesh-0.6.4/web/client/src/utils/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4102 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/utils/index.spec.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5413 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/utils/index.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.986806 sqlmesh-0.6.4/web/client/src/workers/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      113 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/workers/index.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.986806 sqlmesh-0.6.4/web/client/src/workers/sqlglot/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1105 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/workers/sqlglot/sqlglot.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1578 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/src/workers/sqlglot/worker.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5879 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/tailwind.config.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.986806 sqlmesh-0.6.4/web/client/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      170 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/tests/initial.spec.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1141 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/tsconfig.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1297 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/client/vite.config.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.986806 sqlmesh-0.6.4/web/server/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/server/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.986806 sqlmesh-0.6.4/web/server/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/server/api/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-01 23:49:56.990806 sqlmesh-0.6.4/web/server/api/endpoints/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      784 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/server/api/endpoints/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4564 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/server/api/endpoints/commands.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      819 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/server/api/endpoints/context.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1858 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/server/api/endpoints/directories.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      721 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/server/api/endpoints/environments.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      637 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/server/api/endpoints/events.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5383 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/server/api/endpoints/files.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3283 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/server/api/endpoints/lineage.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      962 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/server/api/endpoints/models.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3635 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/server/api/endpoints/plan.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3775 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/server/console.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1534 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/server/main.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5777 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/server/models.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      260 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/server/openapi.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2421 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/server/settings.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2114 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/server/sse.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2461 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/server/utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      790 2023-05-01 23:49:51.000000 sqlmesh-0.6.4/web/server/watcher.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.209089 sqlmesh-0.7.0/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.073086 sqlmesh-0.7.0/.circleci/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1872 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/.circleci/config.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4414 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/.circleci/continue_config.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       66 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/.dockerignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2152 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/.gitignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1900 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      234 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/.readthedocs.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      135 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/Dockerfile.api
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      383 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/Dockerfile.app
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11346 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1855 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/Makefile
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1956 2023-05-02 18:24:02.209089 sqlmesh-0.7.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1192 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1008 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docker-compose.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.073086 sqlmesh-0.7.0/docs/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.049085 sqlmesh-0.7.0/docs/_readthedocs/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.073086 sqlmesh-0.7.0/docs/_readthedocs/html/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/_readthedocs/html/.keep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9965 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/comparisons.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.077086 sqlmesh-0.7.0/docs/concepts/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.077086 sqlmesh-0.7.0/docs/concepts/architecture/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1334 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/concepts/architecture/serialization.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1113 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/concepts/architecture/snapshots.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6689 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/concepts/audits.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3866 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/concepts/environments.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5952 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/concepts/glossary.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/concepts/hooks.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3086 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/concepts/macros.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.077086 sqlmesh-0.7.0/docs/concepts/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9934 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/concepts/models/model_kinds.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8189 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/concepts/models/overview.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7171 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/concepts/models/python_models.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4938 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/concepts/models/seed_models.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5356 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/concepts/models/sql_models.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6637 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/concepts/overview.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.077086 sqlmesh-0.7.0/docs/concepts/plans/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    43124 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/concepts/plans/model_versioning.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9954 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/concepts/plans.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5699 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/concepts/tests.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      607 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/development.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.077086 sqlmesh-0.7.0/docs/guides/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1943 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/guides/connections.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1309 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/guides/migrations.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10756 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/guides/models.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6133 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/guides/multi_repo.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2142 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/guides/projects.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.081086 sqlmesh-0.7.0/docs/guides/scheduling/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   740917 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/guides/scheduling/airflow_successful_plan_apply.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   379880 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/guides/scheduling/airflow_successful_setup.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5648 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/guides/scheduling.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1854 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/guides/testing.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5459 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/index.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      297 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/installation.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.081086 sqlmesh-0.7.0/docs/integrations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2905 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/integrations/airflow.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7801 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/integrations/dbt.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24057 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/integrations/engines.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      867 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/integrations/github.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      217 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/integrations/overview.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      665 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/prerequisites.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12925 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/quick_start.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.081086 sqlmesh-0.7.0/docs/reference/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6093 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/reference/cli.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13607 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/reference/configuration.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4579 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/reference/notebook.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1127 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/reference/overview.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       14 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/reference/python.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/release_notes.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      122 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/requirements.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3249 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/sqlmesh.png
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.081086 sqlmesh-0.7.0/examples/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.085086 sqlmesh-0.7.0/examples/airflow/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1713 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/airflow/Dockerfile.template
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2164 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/airflow/Makefile
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      942 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/airflow/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/airflow/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.085086 sqlmesh-0.7.0/examples/airflow/dags/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      263 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/airflow/dags/sqlmesh_integration.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3515 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/airflow/docker_compose_decorator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/airflow/requirements.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.085086 sqlmesh-0.7.0/examples/airflow/spark_conf/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      872 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/airflow/spark_conf/hive-site.xml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      151 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/airflow/spark_conf/spark-defaults.conf
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.049085 sqlmesh-0.7.0/examples/multi/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.085086 sqlmesh-0.7.0/examples/multi/repo_1/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.085086 sqlmesh-0.7.0/examples/multi/repo_1/audits/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/multi/repo_1/audits/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      147 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/multi/repo_1/config.yaml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.085086 sqlmesh-0.7.0/examples/multi/repo_1/macros/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/multi/repo_1/macros/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/multi/repo_1/macros/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.085086 sqlmesh-0.7.0/examples/multi/repo_1/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/multi/repo_1/models/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       63 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/multi/repo_1/models/a.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/multi/repo_1/models/b.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.085086 sqlmesh-0.7.0/examples/multi/repo_1/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/multi/repo_1/tests/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.085086 sqlmesh-0.7.0/examples/multi/repo_2/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.085086 sqlmesh-0.7.0/examples/multi/repo_2/audits/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/multi/repo_2/audits/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      147 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/multi/repo_2/config.yaml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.085086 sqlmesh-0.7.0/examples/multi/repo_2/macros/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/multi/repo_2/macros/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/multi/repo_2/macros/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.085086 sqlmesh-0.7.0/examples/multi/repo_2/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/multi/repo_2/models/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       64 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/multi/repo_2/models/c.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/multi/repo_2/models/d.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.089086 sqlmesh-0.7.0/examples/multi/repo_2/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/multi/repo_2/tests/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.089086 sqlmesh-0.7.0/examples/sushi/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.089086 sqlmesh-0.7.0/examples/sushi/audits/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      105 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi/audits/items.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      119 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi/audits/order_items.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      829 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi/config.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.089086 sqlmesh-0.7.0/examples/sushi/data/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi/data/.keep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      551 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi/helper.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.089086 sqlmesh-0.7.0/examples/sushi/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi/hooks/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      247 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi/hooks/hooks.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.089086 sqlmesh-0.7.0/examples/sushi/macros/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi/macros/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      702 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi/macros/macros.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.093086 sqlmesh-0.7.0/examples/sushi/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      934 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi/models/customer_revenue_by_day.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      223 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi/models/customers.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1911 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi/models/items.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1912 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi/models/order_items.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1643 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi/models/orders.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      346 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi/models/top_waiters.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      465 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi/models/waiter_as_customer_by_day.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      123 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi/models/waiter_names.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      691 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi/models/waiter_revenue_by_day.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      197 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi/models/waiters.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.093086 sqlmesh-0.7.0/examples/sushi/seeds/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       88 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi/seeds/waiter_names.csv
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.093086 sqlmesh-0.7.0/examples/sushi/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1459 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi/tests/test_customer_revenue_by_day.yaml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.093086 sqlmesh-0.7.0/examples/sushi_dbt/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       15 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/.gitignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       41 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/.user.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.093086 sqlmesh-0.7.0/examples/sushi_dbt/analyses/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/analyses/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      291 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      507 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/dbt_project.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.093086 sqlmesh-0.7.0/examples/sushi_dbt/macros/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      941 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/macros/incremental.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/macros/log_value.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.097086 sqlmesh-0.7.0/examples/sushi_dbt/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1125 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/models/customer_revenue_by_day.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/models/customers.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      182 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/models/schema.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      309 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/models/top_waiters.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      389 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/models/waiter_as_customer_by_day.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      752 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/models/waiter_revenue_by_day.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      186 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/models/waiters.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.053085 sqlmesh-0.7.0/examples/sushi_dbt/packages/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.097086 sqlmesh-0.7.0/examples/sushi_dbt/packages/customers/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.097086 sqlmesh-0.7.0/examples/sushi_dbt/packages/customers/analyses/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/packages/customers/analyses/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      663 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/packages/customers/dbt_project.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.097086 sqlmesh-0.7.0/examples/sushi_dbt/packages/customers/macros/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      117 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/packages/customers/macros/current_engine.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       65 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/packages/customers/macros/distinct.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.097086 sqlmesh-0.7.0/examples/sushi_dbt/packages/customers/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/packages/customers/models/schema.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.097086 sqlmesh-0.7.0/examples/sushi_dbt/packages/customers/seeds/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/packages/customers/seeds/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.097086 sqlmesh-0.7.0/examples/sushi_dbt/packages/customers/snapshots/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/packages/customers/snapshots/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.097086 sqlmesh-0.7.0/examples/sushi_dbt/packages/customers/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/packages/customers/tests/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1092 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/profiles.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.097086 sqlmesh-0.7.0/examples/sushi_dbt/seeds/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2327 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/seeds/items.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10472 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/seeds/order_items.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9746 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/seeds/orders.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       97 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/seeds/properties.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       88 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/seeds/waiter_names.csv
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.097086 sqlmesh-0.7.0/examples/sushi_dbt/snapshots/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/snapshots/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.097086 sqlmesh-0.7.0/examples/sushi_dbt/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/tests/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.101086 sqlmesh-0.7.0/examples/wursthall/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/wursthall/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.053085 sqlmesh-0.7.0/examples/wursthall/audits/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.101086 sqlmesh-0.7.0/examples/wursthall/audits/db/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      141 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/wursthall/audits/db/order_f.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       66 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/wursthall/config.yaml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.101086 sqlmesh-0.7.0/examples/wursthall/macros/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/wursthall/macros/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      618 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/wursthall/macros/macros.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.101086 sqlmesh-0.7.0/examples/wursthall/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/wursthall/models/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.101086 sqlmesh-0.7.0/examples/wursthall/models/db/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      433 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/wursthall/models/db/customer_d.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      256 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/wursthall/models/db/item_d.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3158 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/wursthall/models/db/order_f.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      542 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/wursthall/models/db/order_item_f.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.101086 sqlmesh-0.7.0/examples/wursthall/models/src/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/wursthall/models/src/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1652 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/wursthall/models/src/customer_details.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      120 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/wursthall/models/src/menu_item_details.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3414 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/wursthall/models/src/order_item_details.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      892 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/wursthall/models/src/shared.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.057085 sqlmesh-0.7.0/examples/wursthall/seeds/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.101086 sqlmesh-0.7.0/examples/wursthall/seeds/src/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7416 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/wursthall/seeds/src/menu_item_details.csv
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.101086 sqlmesh-0.7.0/examples/wursthall/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      888 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/wursthall/tests/test_customer_d.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      955 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/wursthall/tests/test_order_item_f.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2113 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/mkdocs.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.101086 sqlmesh-0.7.0/pdoc/
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     1153 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/pdoc/cli.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.105086 sqlmesh-0.7.0/pdoc/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      131 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/pdoc/templates/module.html.jinja2
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.105086 sqlmesh-0.7.0/posts/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.105086 sqlmesh-0.7.0/posts/virtual_data_environments/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   318753 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/posts/virtual_data_environments/change_categorization.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   274526 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/posts/virtual_data_environments/isolated_rigid_envs.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   163619 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/posts/virtual_data_environments/partial_breaking.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   298971 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/posts/virtual_data_environments/stateful_envs.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   366545 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/posts/virtual_data_environments/virtual_envs.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)  1344487 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/posts/virtual_data_environments/virtual_envs_end_to_end.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18638 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/posts/virtual_data_environments.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      734 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/pytest.ini
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1443 2023-05-02 18:24:02.217090 sqlmesh-0.7.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3239 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.109087 sqlmesh-0.7.0/sqlmesh/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        3 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/.airflowignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3950 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      160 2023-05-02 18:24:01.000000 sqlmesh-0.7.0/sqlmesh/_version.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.109087 sqlmesh-0.7.0/sqlmesh/cli/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      898 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/cli/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4742 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/cli/example_project.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10941 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/cli/main.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1433 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/cli/options.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.117087 sqlmesh-0.7.0/sqlmesh/core/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      586 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/_typing.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.117087 sqlmesh-0.7.0/sqlmesh/core/audit/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      449 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/audit/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1071 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/audit/builtin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8136 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/audit/definition.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.117087 sqlmesh-0.7.0/sqlmesh/core/config/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      668 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/config/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4412 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/config/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1001 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/config/categorizer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      940 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/config/common.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21184 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/config/connection.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3351 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/config/loader.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1655 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/config/model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5611 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/config/root.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8421 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/config/scheduler.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    31743 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/console.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      826 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    36329 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/context.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8904 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/context_diff.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17484 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/dialect.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.121087 sqlmesh-0.7.0/sqlmesh/core/engine_adapter/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2626 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/engine_adapter/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      762 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/engine_adapter/_typing.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    29549 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/engine_adapter/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4191 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/engine_adapter/base_postgres.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4238 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/engine_adapter/base_spark.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15681 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/engine_adapter/bigquery.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      402 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/engine_adapter/databricks.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1939 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/engine_adapter/databricks_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1971 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/engine_adapter/duckdb.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2149 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/engine_adapter/postgres.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6673 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/engine_adapter/redshift.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1181 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/engine_adapter/shared.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2658 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/engine_adapter/snowflake.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4879 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/engine_adapter/spark.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1849 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/environment.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      742 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/hooks.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12673 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/loader.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19726 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/macros.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.125087 sqlmesh-0.7.0/sqlmesh/core/model/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      594 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/model/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1746 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/model/cache.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1300 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/model/common.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2417 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/model/decorator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    47510 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/model/definition.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8168 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/model/kind.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13069 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/model/meta.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2017 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/model/seed.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2314 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/notification_target.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.125087 sqlmesh-0.7.0/sqlmesh/core/plan/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      191 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/plan/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23956 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/plan/definition.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8565 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/plan/evaluator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12623 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/renderer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15386 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/scheduler.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20418 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/schema_diff.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.125087 sqlmesh-0.7.0/sqlmesh/core/snapshot/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      527 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/snapshot/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1990 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/snapshot/categorizer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    34694 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/snapshot/definition.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19245 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/snapshot/evaluator.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.125087 sqlmesh-0.7.0/sqlmesh/core/state_sync/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      692 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/state_sync/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13382 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/state_sync/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14349 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/state_sync/common.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20765 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/state_sync/engine_adapter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10834 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1412 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/user.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.129087 sqlmesh-0.7.0/sqlmesh/dbt/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       79 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/dbt/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9390 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/dbt/adapter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17485 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/dbt/basemodel.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11231 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/dbt/builtin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1762 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/dbt/column.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4978 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/dbt/common.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5087 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/dbt/context.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8044 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/dbt/loader.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9851 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/dbt/model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13257 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/dbt/package.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3701 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/dbt/profile.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4772 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/dbt/project.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      927 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/dbt/seed.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3137 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/dbt/source.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13618 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/dbt/target.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      291 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/dbt/util.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.129087 sqlmesh-0.7.0/sqlmesh/engines/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/engines/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4437 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/engines/commands.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.133087 sqlmesh-0.7.0/sqlmesh/engines/spark/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/engines/spark/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3414 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/engines/spark/app.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.133087 sqlmesh-0.7.0/sqlmesh/engines/spark/db_api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/engines/spark/db_api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      148 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/engines/spark/db_api/errors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2571 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/engines/spark/db_api/spark_session.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.133087 sqlmesh-0.7.0/sqlmesh/integrations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/integrations/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.133087 sqlmesh-0.7.0/sqlmesh/integrations/github/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/integrations/github/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2210 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/integrations/github/notification_operator_provider.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1726 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/integrations/github/notification_target.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1829 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/integrations/github/shared.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1553 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/integrations/llm.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13960 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/magics.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.133087 sqlmesh-0.7.0/sqlmesh/migrations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/migrations/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1749 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/migrations/v0001_init.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      103 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/migrations/v0002_remove_identify.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1183 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/migrations/v0003_move_batch_size.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      534 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/migrations/v0004_environmnent_add_finalized_at.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/py.typed
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.133087 sqlmesh-0.7.0/sqlmesh/schedulers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/schedulers/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.137087 sqlmesh-0.7.0/sqlmesh/schedulers/airflow/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/schedulers/airflow/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4020 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/schedulers/airflow/api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8128 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/schedulers/airflow/client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3888 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/schedulers/airflow/common.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19132 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/schedulers/airflow/dag_generator.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.137087 sqlmesh-0.7.0/sqlmesh/schedulers/airflow/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/schedulers/airflow/hooks/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2132 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/schedulers/airflow/hooks/bigquery.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      868 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/schedulers/airflow/hooks/redshift.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8508 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/schedulers/airflow/integration.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.141088 sqlmesh-0.7.0/sqlmesh/schedulers/airflow/operators/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/schedulers/airflow/operators/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1444 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/schedulers/airflow/operators/bigquery.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6307 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/schedulers/airflow/operators/databricks.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2549 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/schedulers/airflow/operators/hwm_sensor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      877 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/schedulers/airflow/operators/notification.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1322 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/schedulers/airflow/operators/postgres.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1211 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/schedulers/airflow/operators/redshift.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1340 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/schedulers/airflow/operators/snowflake.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5222 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/schedulers/airflow/operators/spark_submit.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11104 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/schedulers/airflow/operators/targets.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4660 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/schedulers/airflow/plan.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1292 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/schedulers/airflow/plugin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4139 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/schedulers/airflow/state_sync.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5213 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/schedulers/airflow/util.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.145088 sqlmesh-0.7.0/sqlmesh/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4386 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3593 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/utils/cache.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8053 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/utils/concurrency.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7530 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/utils/connection_pool.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      410 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/utils/conversions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4329 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/utils/dag.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7606 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/utils/date.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1244 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/utils/errors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16133 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/utils/jinja.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15093 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/utils/metaprogramming.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      888 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/utils/pandas.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1609 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/utils/pydantic.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1534 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/utils/rich.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6487 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/utils/transactional_file.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1419 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/utils/yaml.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.109087 sqlmesh-0.7.0/sqlmesh.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1956 2023-05-02 18:24:01.000000 sqlmesh-0.7.0/sqlmesh.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22014 2023-05-02 18:24:02.000000 sqlmesh-0.7.0/sqlmesh.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-02 18:24:01.000000 sqlmesh-0.7.0/sqlmesh.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      141 2023-05-02 18:24:01.000000 sqlmesh-0.7.0/sqlmesh.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      868 2023-05-02 18:24:01.000000 sqlmesh-0.7.0/sqlmesh.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2023-05-02 18:24:01.000000 sqlmesh-0.7.0/sqlmesh.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21020 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh.svg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.145088 sqlmesh-0.7.0/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      285 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/common_fixtures.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4037 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/conftest.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.149088 sqlmesh-0.7.0/tests/core/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.149088 sqlmesh-0.7.0/tests/core/engine_adapter/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/engine_adapter/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    28133 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/engine_adapter/test_base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2114 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/engine_adapter/test_base_postgres.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1270 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/engine_adapter/test_base_spark.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7171 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/engine_adapter/test_bigquery.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1253 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/engine_adapter/test_databricks.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2613 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/engine_adapter/test_duckdb.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1569 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/engine_adapter/test_postgres.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8036 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/engine_adapter/test_redshift.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3191 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/engine_adapter/test_spark.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7073 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/test_audit.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6611 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/test_config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      850 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/test_connection_config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10197 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/test_context.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2749 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/test_dialect.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      464 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/test_environment.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    26773 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/test_integration.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6500 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/test_macros.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25586 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/test_model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17081 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/test_plan.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3890 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/test_plan_evaluator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4647 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/test_scheduler.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    32235 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/test_schema_diff.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      857 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/test_seed.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    29629 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/test_snapshot.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10299 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/test_snapshot_evaluator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24610 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/test_state_sync.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.153088 sqlmesh-0.7.0/tests/dbt/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/dbt/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      739 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/dbt/conftest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2537 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/dbt/test_adapter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13195 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/dbt/test_config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17095 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/dbt/test_transformation.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.153088 sqlmesh-0.7.0/tests/engines/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/engines/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.153088 sqlmesh-0.7.0/tests/engines/spark/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/engines/spark/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      357 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/engines/spark/conftest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1503 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/engines/spark/test_db_api.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.061085 sqlmesh-0.7.0/tests/fixtures/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.061085 sqlmesh-0.7.0/tests/fixtures/dbt/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.153088 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.153088 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/analyses/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/analyses/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      291 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/config.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.061085 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/dbt_packages/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1055 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/dbt_project.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.153088 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/logs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10264 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/logs/dbt.log.legacy
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.153088 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/macros/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      941 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/macros/incremental.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/macros/log_value.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.157088 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      247 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/models/schema.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      334 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/models/top_waiters.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      389 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/models/waiter_as_customer_by_day.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      863 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/models/waiter_revenue_by_day.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      196 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/models/waiters.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.061085 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/packages/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.157088 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/packages/customers/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.157088 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/packages/customers/analyses/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/packages/customers/analyses/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      663 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/packages/customers/dbt_project.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.157088 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/packages/customers/macros/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      117 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/packages/customers/macros/current_engine.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       65 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/packages/customers/macros/distinct.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.157088 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/packages/customers/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1155 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/packages/customers/models/customer_revenue_by_day.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      108 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/packages/customers/models/customers.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      193 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/packages/customers/models/schema.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.157088 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/packages/customers/seeds/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/packages/customers/seeds/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.157088 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/packages/customers/snapshots/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/packages/customers/snapshots/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.157088 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/packages/customers/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/packages/customers/tests/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       41 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/packages.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      540 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/profiles.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1250 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/seed_sources.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.161088 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/seeds/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       42 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/seeds/properties.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       88 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/seeds/waiter_names.csv
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.161088 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/snapshots/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/snapshots/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.161088 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/source_data/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2327 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/source_data/items.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10472 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/source_data/order_items.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9746 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/source_data/orders.csv
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.161088 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/tests/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.161088 sqlmesh-0.7.0/tests/fixtures/migrations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9823 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/migrations/environments.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25229 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/migrations/snapshots.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.161088 sqlmesh-0.7.0/tests/integrations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/integrations/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.161088 sqlmesh-0.7.0/tests/integrations/github/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/integrations/github/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.161088 sqlmesh-0.7.0/tests/integrations/github/fixtures/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      816 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/integrations/github/fixtures/pull_request_review.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      477 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/integrations/github/test_notification_target.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.161088 sqlmesh-0.7.0/tests/schedulers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/schedulers/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.165088 sqlmesh-0.7.0/tests/schedulers/airflow/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/schedulers/airflow/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1414 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/schedulers/airflow/conftest.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.165088 sqlmesh-0.7.0/tests/schedulers/airflow/operators/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/schedulers/airflow/operators/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4442 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/schedulers/airflow/operators/test_hwm_sensor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4392 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/schedulers/airflow/operators/test_targets.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9920 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/schedulers/airflow/test_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1345 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/schedulers/airflow/test_end_to_end.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6222 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/schedulers/airflow/test_integration.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6054 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/schedulers/airflow/test_plan.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.169088 sqlmesh-0.7.0/tests/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1118 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/utils/test_cache.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3580 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/utils/test_concurrency.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6430 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/utils/test_connection_pool.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1381 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/utils/test_dag.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1818 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/utils/test_date.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      551 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/utils/test_filesystem.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5516 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/utils/test_jinja.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5790 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/utils/test_metaprogramming.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2501 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/utils/test_pandas.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      518 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/utils/test_pydantic.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2911 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/utils/test_transactional_file.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1194 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/utils/test_yaml.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.169088 sqlmesh-0.7.0/tests/web/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/web/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16232 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/web/test_main.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.169088 sqlmesh-0.7.0/web/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.173088 sqlmesh-0.7.0/web/client/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1104 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/.eslintrc.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       94 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/.gitignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      129 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/.prettierignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      403 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/.prettierrc.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.173088 sqlmesh-0.7.0/web/client/dist/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.177089 sqlmesh-0.7.0/web/client/dist/assets/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    74500 2023-05-02 18:23:49.000000 sqlmesh-0.7.0/web/client/dist/assets/CircularStd-Black-52659624.otf
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    74368 2023-05-02 18:23:49.000000 sqlmesh-0.7.0/web/client/dist/assets/CircularStd-Bold-0e6c076d.otf
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    74116 2023-05-02 18:23:49.000000 sqlmesh-0.7.0/web/client/dist/assets/CircularStd-Medium-2f373e53.otf
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24788 2023-05-02 18:23:49.000000 sqlmesh-0.7.0/web/client/dist/assets/Plan-683a0552.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    55004 2023-05-02 18:23:49.000000 sqlmesh-0.7.0/web/client/dist/assets/Publico-Black-e6bd2ea2.otf
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    57104 2023-05-02 18:23:49.000000 sqlmesh-0.7.0/web/client/dist/assets/Publico-Bold-c79acd56.otf
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    56836 2023-05-02 18:23:49.000000 sqlmesh-0.7.0/web/client/dist/assets/Publico-Medium-01b4a891.otf
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    43132 2023-05-02 18:23:49.000000 sqlmesh-0.7.0/web/client/dist/assets/index-b61dbb6f.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)  2636063 2023-05-02 18:23:49.000000 sqlmesh-0.7.0/web/client/dist/assets/index-f2c4b7c5.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2419 2023-05-02 18:23:49.000000 sqlmesh-0.7.0/web/client/dist/assets/worker-e891d118.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.177089 sqlmesh-0.7.0/web/client/dist/favicons/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2473 2023-05-02 18:23:46.000000 sqlmesh-0.7.0/web/client/dist/favicons/favicon.ico
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1150 2023-05-02 18:23:49.000000 sqlmesh-0.7.0/web/client/dist/index.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1076 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/index.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    37689 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/openapi.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      330 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/orval.config.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   408504 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/package-lock.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2389 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/package.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1642 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/playwright.config.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       82 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/postcss.config.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.065086 sqlmesh-0.7.0/web/client/public/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.177089 sqlmesh-0.7.0/web/client/public/favicons/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2473 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/public/favicons/favicon.ico
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.177089 sqlmesh-0.7.0/web/client/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.181089 sqlmesh-0.7.0/web/client/src/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1236 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/api/channels.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5243 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/api/index.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3247 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/api/instance.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.065086 sqlmesh-0.7.0/web/client/src/assets/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.065086 sqlmesh-0.7.0/web/client/src/assets/fonts/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.181089 sqlmesh-0.7.0/web/client/src/assets/fonts/Circular STD/
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    74500 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/assets/fonts/Circular STD/CircularStd-Black.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    74524 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/assets/fonts/Circular STD/CircularStd-BlackItalic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    74368 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/assets/fonts/Circular STD/CircularStd-Bold.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    73964 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/assets/fonts/Circular STD/CircularStd-BoldItalic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    68940 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/assets/fonts/Circular STD/CircularStd-Book.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    67284 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/assets/fonts/Circular STD/CircularStd-BookItalic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    74116 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/assets/fonts/Circular STD/CircularStd-Medium.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    73916 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/assets/fonts/Circular STD/CircularStd-MediumItalic.otf
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.189089 sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    55004 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/Publico-Black.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    56384 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/Publico-BlackItalic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    57104 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/Publico-Bold.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    62320 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/Publico-BoldItalic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    56652 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/Publico-Extrabold.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    61688 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/Publico-ExtraboldItalic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    57680 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/Publico-Italic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    53148 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/Publico-Light.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    57060 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/Publico-LightItalic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    56836 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/Publico-Medium.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    61460 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/Publico-MediumItalic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    52820 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/Publico-Roman.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    59176 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/PublicoText-Bold.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    63876 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/PublicoText-BoldItalic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    60768 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/PublicoText-Italic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    81732 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/PublicoText-Roman.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    60992 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/PublicoText-Semibold.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    64792 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/PublicoText-SemiboldItalic.otf
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.189089 sqlmesh-0.7.0/web/client/src/context/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4126 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/context/context.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6470 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/context/editor.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      923 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/context/fileTree.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2187 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/context/lineage.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2661 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/context/plan.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1562 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/context/theme.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.189089 sqlmesh-0.7.0/web/client/src/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      308 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/hooks/useActiveFocus.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      817 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/hooks/useLocalStorage.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9555 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/index.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.065086 sqlmesh-0.7.0/web/client/src/library/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.065086 sqlmesh-0.7.0/web/client/src/library/components/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.189089 sqlmesh-0.7.0/web/client/src/library/components/banner/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1705 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/banner/Banner.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.189089 sqlmesh-0.7.0/web/client/src/library/components/button/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4517 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/button/Button.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.193089 sqlmesh-0.7.0/web/client/src/library/components/button/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3516 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/button/tests/Button.spec.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.193089 sqlmesh-0.7.0/web/client/src/library/components/divider/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      856 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/divider/Divider.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.193089 sqlmesh-0.7.0/web/client/src/library/components/divider/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      632 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/divider/tests/Divider.spec.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.193089 sqlmesh-0.7.0/web/client/src/library/components/editor/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1992 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/editor/Editor.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5764 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/editor/Editor.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8518 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/editor/EditorCode.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2718 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/editor/EditorFooter.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1990 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/editor/EditorIndicator.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9819 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/editor/EditorInspector.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11905 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/editor/EditorPreview.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3527 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/editor/EditorTabs.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.193089 sqlmesh-0.7.0/web/client/src/library/components/editor/extensions/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5820 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/editor/extensions/SqlMeshDialect.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5744 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/editor/extensions/index.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1538 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/editor/help.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.193089 sqlmesh-0.7.0/web/client/src/library/components/fileTree/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10852 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/fileTree/Directory.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6045 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/fileTree/File.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2997 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/fileTree/FileTree.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      562 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/fileTree/help.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.197089 sqlmesh-0.7.0/web/client/src/library/components/graph/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      159 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/graph/Graph.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14454 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/graph/Graph.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7679 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/graph/help.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.197089 sqlmesh-0.7.0/web/client/src/library/components/ide/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4342 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/ide/ActivePlan.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4933 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/ide/IDE.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22356 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/ide/RunPlan.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.197089 sqlmesh-0.7.0/web/client/src/library/components/input/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2087 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/input/Input.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      688 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/input/InputToggle.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.197089 sqlmesh-0.7.0/web/client/src/library/components/loading/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      486 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/loading/Loading.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.197089 sqlmesh-0.7.0/web/client/src/library/components/logo/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2292 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/logo/Spinner.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4637 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/logo/SqlMesh.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8042 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/logo/Tobiko.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.197089 sqlmesh-0.7.0/web/client/src/library/components/modal/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1560 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/modal/Modal.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1953 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/modal/ModalConfirmation.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1447 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/modal/ModalDrawer.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.201089 sqlmesh-0.7.0/web/client/src/library/components/plan/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9269 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/plan/Plan.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6775 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/plan/PlanActions.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1312 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/plan/PlanBackfillDates.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10448 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/plan/PlanChangePreview.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4920 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/plan/PlanHeader.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15855 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/plan/PlanWizard.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9926 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/plan/PlanWizardStepOptions.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12528 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/plan/context.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3444 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/plan/help.spec.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2155 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/plan/help.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2599 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/plan/hooks.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.201089 sqlmesh-0.7.0/web/client/src/library/components/progress/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      713 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/progress/Progress.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.201089 sqlmesh-0.7.0/web/client/src/library/components/report/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1047 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/report/ReportTestsErrors.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.201089 sqlmesh-0.7.0/web/client/src/library/components/root/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      526 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/root/Footer.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1921 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/root/Header.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      247 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/root/Main.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      443 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/root/Root.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.201089 sqlmesh-0.7.0/web/client/src/library/components/splitPane/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      788 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/splitPane/SplitPane.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      541 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/splitPane/SplitPane.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.201089 sqlmesh-0.7.0/web/client/src/library/components/tasksOverview/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11713 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/tasksOverview/TasksOverview.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.201089 sqlmesh-0.7.0/web/client/src/library/components/toggle/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1453 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/toggle/Toggle.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1197 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/main.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.205089 sqlmesh-0.7.0/web/client/src/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1647 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/models/artifact.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3472 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/models/directory.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4190 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/models/environment.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2190 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/models/file.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      173 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/models/index.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      766 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/models/initial.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      200 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/routes.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.205089 sqlmesh-0.7.0/web/client/src/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       35 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/tests/setup.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      541 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/tests/utils.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.205089 sqlmesh-0.7.0/web/client/src/types/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      467 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/types/enum.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      137 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/types/index.d.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.205089 sqlmesh-0.7.0/web/client/src/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4102 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/utils/index.spec.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5413 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/utils/index.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.205089 sqlmesh-0.7.0/web/client/src/workers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      113 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/workers/index.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.205089 sqlmesh-0.7.0/web/client/src/workers/sqlglot/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1105 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/workers/sqlglot/sqlglot.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1578 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/workers/sqlglot/worker.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5879 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/tailwind.config.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.205089 sqlmesh-0.7.0/web/client/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      170 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/tests/initial.spec.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1141 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/tsconfig.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1297 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/vite.config.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.209089 sqlmesh-0.7.0/web/server/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/server/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.209089 sqlmesh-0.7.0/web/server/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/server/api/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.209089 sqlmesh-0.7.0/web/server/api/endpoints/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      784 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/server/api/endpoints/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4564 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/server/api/endpoints/commands.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      819 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/server/api/endpoints/context.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1858 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/server/api/endpoints/directories.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      721 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/server/api/endpoints/environments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      637 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/server/api/endpoints/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5383 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/server/api/endpoints/files.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3283 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/server/api/endpoints/lineage.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      962 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/server/api/endpoints/models.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3635 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/server/api/endpoints/plan.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3775 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/server/console.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1534 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/server/main.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5777 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/server/models.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      260 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/server/openapi.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2421 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/server/settings.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2114 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/server/sse.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2461 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/server/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      790 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/server/watcher.py
```

### Comparing `sqlmesh-0.6.4/.circleci/config.yml` & `sqlmesh-0.7.0/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/.circleci/continue_config.yml` & `sqlmesh-0.7.0/.circleci/continue_config.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/.gitignore` & `sqlmesh-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/.pre-commit-config.yaml` & `sqlmesh-0.7.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/LICENSE` & `sqlmesh-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/Makefile` & `sqlmesh-0.7.0/Makefile`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/PKG-INFO` & `sqlmesh-0.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlmesh
-Version: 0.6.4
+Version: 0.7.0
 Home-page: https://github.com/TobikoData/sqlmesh
 Author: TobikoData Inc.
 Author-email: engineering@tobikodata.com
 License: Apache License 2.0
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: SQL
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 Provides-Extra: bigquery
 Provides-Extra: databricks
 Provides-Extra: dev
 Provides-Extra: dbt
+Provides-Extra: llm
 Provides-Extra: postgres
 Provides-Extra: redshift
 Provides-Extra: snowflake
 Provides-Extra: web
 License-File: LICENSE
 
 ![SQLMesh logo](sqlmesh.svg)
```

### Comparing `sqlmesh-0.6.4/README.md` & `sqlmesh-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/docker-compose.yml` & `sqlmesh-0.7.0/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/docs/comparisons.md` & `sqlmesh-0.7.0/docs/comparisons.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/docs/concepts/architecture/serialization.md` & `sqlmesh-0.7.0/docs/concepts/architecture/serialization.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/docs/concepts/architecture/snapshots.md` & `sqlmesh-0.7.0/docs/concepts/architecture/snapshots.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/docs/concepts/audits.md` & `sqlmesh-0.7.0/docs/concepts/audits.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/docs/concepts/environments.md` & `sqlmesh-0.7.0/docs/concepts/environments.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/docs/concepts/glossary.md` & `sqlmesh-0.7.0/docs/concepts/glossary.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/docs/concepts/macros.md` & `sqlmesh-0.7.0/docs/concepts/macros.md`

 * *Files 3% similar despite different names*

```diff
@@ -46,14 +46,19 @@
 Variables:
 
 * date
     * @start_date
     * @end_date
     * @latest_date
 
+* datetime
+    * @start_dt
+    * @end_dt
+    * @latest_dt
+
 * ds
     * @start_ds
     * @end_ds
     * @latest_ds
 
 * ts
     * @start_ts
```

### Comparing `sqlmesh-0.6.4/docs/concepts/models/model_kinds.md` & `sqlmesh-0.7.0/docs/concepts/models/model_kinds.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/docs/concepts/models/overview.md` & `sqlmesh-0.7.0/docs/concepts/models/overview.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/docs/concepts/models/python_models.md` & `sqlmesh-0.7.0/docs/concepts/models/python_models.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/docs/concepts/models/seed_models.md` & `sqlmesh-0.7.0/docs/concepts/models/seed_models.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/docs/concepts/models/sql_models.md` & `sqlmesh-0.7.0/docs/concepts/models/sql_models.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/docs/concepts/overview.md` & `sqlmesh-0.7.0/docs/concepts/overview.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/docs/concepts/plans/model_versioning.png` & `sqlmesh-0.7.0/docs/concepts/plans/model_versioning.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/docs/concepts/plans.md` & `sqlmesh-0.7.0/docs/concepts/plans.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/docs/concepts/tests.md` & `sqlmesh-0.7.0/docs/concepts/tests.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/docs/development.md` & `sqlmesh-0.7.0/docs/development.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/docs/guides/connections.md` & `sqlmesh-0.7.0/docs/guides/connections.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/docs/guides/migrations.md` & `sqlmesh-0.7.0/docs/guides/migrations.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/docs/guides/models.md` & `sqlmesh-0.7.0/docs/guides/models.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/docs/guides/multi_repo.md` & `sqlmesh-0.7.0/docs/guides/multi_repo.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/docs/guides/projects.md` & `sqlmesh-0.7.0/docs/guides/projects.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/docs/guides/scheduling/airflow_successful_plan_apply.png` & `sqlmesh-0.7.0/docs/guides/scheduling/airflow_successful_plan_apply.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/docs/guides/scheduling/airflow_successful_setup.png` & `sqlmesh-0.7.0/docs/guides/scheduling/airflow_successful_setup.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/docs/guides/scheduling.md` & `sqlmesh-0.7.0/docs/guides/scheduling.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/docs/guides/testing.md` & `sqlmesh-0.7.0/docs/guides/testing.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/docs/index.md` & `sqlmesh-0.7.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/docs/integrations/airflow.md` & `sqlmesh-0.7.0/docs/integrations/airflow.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/docs/integrations/dbt.md` & `sqlmesh-0.7.0/docs/integrations/dbt.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/docs/integrations/engines.md` & `sqlmesh-0.7.0/docs/integrations/engines.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/docs/integrations/github.md` & `sqlmesh-0.7.0/docs/integrations/github.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/docs/prerequisites.md` & `sqlmesh-0.7.0/docs/prerequisites.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/docs/quick_start.md` & `sqlmesh-0.7.0/docs/quick_start.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/docs/reference/cli.md` & `sqlmesh-0.7.0/docs/reference/cli.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/docs/reference/configuration.md` & `sqlmesh-0.7.0/docs/reference/configuration.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/docs/reference/notebook.md` & `sqlmesh-0.7.0/docs/reference/notebook.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/docs/reference/overview.md` & `sqlmesh-0.7.0/docs/reference/overview.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/docs/sqlmesh.png` & `sqlmesh-0.7.0/docs/sqlmesh.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/examples/airflow/Dockerfile.template` & `sqlmesh-0.7.0/examples/airflow/Dockerfile.template`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/examples/airflow/Makefile` & `sqlmesh-0.7.0/examples/airflow/Makefile`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/examples/airflow/README.md` & `sqlmesh-0.7.0/examples/airflow/README.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/examples/airflow/docker_compose_decorator.py` & `sqlmesh-0.7.0/examples/airflow/docker_compose_decorator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/examples/airflow/spark_conf/hive-site.xml` & `sqlmesh-0.7.0/examples/airflow/spark_conf/hive-site.xml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/examples/sushi/config.py` & `sqlmesh-0.7.0/examples/sushi/config.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/examples/sushi/helper.py` & `sqlmesh-0.7.0/examples/sushi/helper.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/examples/sushi/macros/macros.py` & `sqlmesh-0.7.0/examples/sushi/macros/macros.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/examples/sushi/models/customer_revenue_by_day.sql` & `sqlmesh-0.7.0/examples/sushi/models/customer_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/examples/sushi/models/items.py` & `sqlmesh-0.7.0/examples/sushi/models/items.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/examples/sushi/models/order_items.py` & `sqlmesh-0.7.0/examples/sushi/models/order_items.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/examples/sushi/models/orders.py` & `sqlmesh-0.7.0/examples/sushi/models/orders.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/examples/sushi/models/waiter_revenue_by_day.sql` & `sqlmesh-0.7.0/examples/sushi/models/waiter_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/examples/sushi/tests/test_customer_revenue_by_day.yaml` & `sqlmesh-0.7.0/examples/sushi/tests/test_customer_revenue_by_day.yaml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/examples/sushi_dbt/macros/incremental.sql` & `sqlmesh-0.7.0/examples/sushi_dbt/macros/incremental.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/examples/sushi_dbt/models/customer_revenue_by_day.sql` & `sqlmesh-0.7.0/examples/sushi_dbt/models/customer_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/examples/sushi_dbt/models/waiter_revenue_by_day.sql` & `sqlmesh-0.7.0/examples/sushi_dbt/models/waiter_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/examples/sushi_dbt/packages/customers/dbt_project.yml` & `sqlmesh-0.7.0/examples/sushi_dbt/packages/customers/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/examples/sushi_dbt/profiles.yml` & `sqlmesh-0.7.0/examples/sushi_dbt/profiles.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/examples/sushi_dbt/seeds/items.csv` & `sqlmesh-0.7.0/examples/sushi_dbt/seeds/items.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/examples/sushi_dbt/seeds/order_items.csv` & `sqlmesh-0.7.0/examples/sushi_dbt/seeds/order_items.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/examples/sushi_dbt/seeds/orders.csv` & `sqlmesh-0.7.0/examples/sushi_dbt/seeds/orders.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/examples/wursthall/macros/macros.py` & `sqlmesh-0.7.0/examples/wursthall/macros/macros.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/examples/wursthall/models/db/order_f.py` & `sqlmesh-0.7.0/examples/wursthall/models/db/order_f.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/examples/wursthall/models/db/order_item_f.sql` & `sqlmesh-0.7.0/examples/wursthall/models/db/order_item_f.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/examples/wursthall/models/src/customer_details.py` & `sqlmesh-0.7.0/examples/wursthall/models/src/customer_details.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/examples/wursthall/models/src/order_item_details.py` & `sqlmesh-0.7.0/examples/wursthall/models/src/order_item_details.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/examples/wursthall/models/src/shared.py` & `sqlmesh-0.7.0/examples/wursthall/models/src/shared.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/examples/wursthall/seeds/src/menu_item_details.csv` & `sqlmesh-0.7.0/examples/wursthall/seeds/src/menu_item_details.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/examples/wursthall/tests/test_customer_d.yaml` & `sqlmesh-0.7.0/examples/wursthall/tests/test_customer_d.yaml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/examples/wursthall/tests/test_order_item_f.yaml` & `sqlmesh-0.7.0/examples/wursthall/tests/test_order_item_f.yaml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/mkdocs.yml` & `sqlmesh-0.7.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/pdoc/cli.py` & `sqlmesh-0.7.0/pdoc/cli.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/posts/virtual_data_environments/change_categorization.png` & `sqlmesh-0.7.0/posts/virtual_data_environments/change_categorization.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/posts/virtual_data_environments/isolated_rigid_envs.png` & `sqlmesh-0.7.0/posts/virtual_data_environments/isolated_rigid_envs.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/posts/virtual_data_environments/partial_breaking.png` & `sqlmesh-0.7.0/posts/virtual_data_environments/partial_breaking.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/posts/virtual_data_environments/stateful_envs.png` & `sqlmesh-0.7.0/posts/virtual_data_environments/stateful_envs.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/posts/virtual_data_environments/virtual_envs.png` & `sqlmesh-0.7.0/posts/virtual_data_environments/virtual_envs.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/posts/virtual_data_environments/virtual_envs_end_to_end.png` & `sqlmesh-0.7.0/posts/virtual_data_environments/virtual_envs_end_to_end.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/posts/virtual_data_environments.md` & `sqlmesh-0.7.0/posts/virtual_data_environments.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/pytest.ini` & `sqlmesh-0.7.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/setup.cfg` & `sqlmesh-0.7.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,17 @@
 
 [mypy-fsspec]
 ignore_missing_imports = True
 
 [mypy-psycopg2.*]
 ignore_missing_imports = True
 
+[mypy-langchain.*]
+ignore_missing_imports = True
+
 [autoflake]
 in-place = True
 expand-star-imports = True
 remove-all-unused-imports = True
 ignore-init-module-imports = True
 remove-duplicate-keys = True
 remove-unused-variables = True
```

### Comparing `sqlmesh-0.6.4/setup.py` & `sqlmesh-0.7.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -83,14 +83,18 @@
             "types-dateparser",
             "types-pytz",
             "types-requests==2.28.8",
         ],
         "dbt": [
             "dbt-core<1.5.0",
         ],
+        "llm": [
+            "langchain",
+            "openai",
+        ],
         "postgres": [
             "psycopg2",
         ],
         "redshift": [
             "redshift_connector",
         ],
         "snowflake": [
```

### Comparing `sqlmesh-0.6.4/sqlmesh/__init__.py` & `sqlmesh-0.7.0/sqlmesh/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/cli/__init__.py` & `sqlmesh-0.7.0/sqlmesh/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/cli/example_project.py` & `sqlmesh-0.7.0/sqlmesh/cli/example_project.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/cli/main.py` & `sqlmesh-0.7.0/sqlmesh/cli/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -374,9 +374,48 @@
 @click.pass_context
 @error_handler
 def migrate(ctx: click.Context) -> None:
     """Migrate SQLMesh to the current running version."""
     ctx.obj.migrate()
 
 
+@cli.command("prompt")
+@click.argument("prompt")
+@click.option(
+    "-e",
+    "--evaluate",
+    is_flag=True,
+    help="Evaluate the generated SQL query and display the results.",
+)
+@click.option(
+    "-t",
+    "--temperature",
+    type=float,
+    help="Sampling temperature. 0.0 - precise and predictable, 0.5 - balanced, 1.0 - creative. Default: 0.7",
+    default=0.7,
+)
+@opt.verbose
+@click.pass_context
+@error_handler
+def prompt(
+    ctx: click.Context, prompt: str, evaluate: bool, temperature: float, verbose: bool
+) -> None:
+    """Uses LLM to generate a SQL query from a prompt."""
+    from sqlmesh.integrations.llm import LLMIntegration
+
+    context = ctx.obj
+
+    llm_integration = LLMIntegration(
+        context.models.values(),
+        context.engine_adapter.dialect,
+        temperature=temperature,
+        verbose=verbose,
+    )
+    query = llm_integration.query(prompt)
+
+    context.console.log_status_update(query)
+    if evaluate:
+        context.console.log_success(context.fetchdf(query))
+
+
 if __name__ == "__main__":
     cli()
```

### Comparing `sqlmesh-0.6.4/sqlmesh/cli/options.py` & `sqlmesh-0.7.0/sqlmesh/cli/options.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/_typing.py` & `sqlmesh-0.7.0/sqlmesh/core/_typing.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/audit/builtin.py` & `sqlmesh-0.7.0/sqlmesh/core/audit/builtin.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/audit/definition.py` & `sqlmesh-0.7.0/sqlmesh/core/audit/definition.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/config/__init__.py` & `sqlmesh-0.7.0/sqlmesh/core/config/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/config/base.py` & `sqlmesh-0.7.0/sqlmesh/core/config/base.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/config/categorizer.py` & `sqlmesh-0.7.0/sqlmesh/core/config/categorizer.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/config/common.py` & `sqlmesh-0.7.0/sqlmesh/core/config/common.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/config/connection.py` & `sqlmesh-0.7.0/sqlmesh/core/config/connection.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/config/loader.py` & `sqlmesh-0.7.0/sqlmesh/core/config/loader.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/config/model.py` & `sqlmesh-0.7.0/sqlmesh/core/config/model.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/config/root.py` & `sqlmesh-0.7.0/sqlmesh/core/config/root.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/config/scheduler.py` & `sqlmesh-0.7.0/sqlmesh/core/config/scheduler.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/console.py` & `sqlmesh-0.7.0/sqlmesh/core/console.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/constants.py` & `sqlmesh-0.7.0/sqlmesh/core/constants.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/context.py` & `sqlmesh-0.7.0/sqlmesh/core/context.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/context_diff.py` & `sqlmesh-0.7.0/sqlmesh/core/context_diff.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/dialect.py` & `sqlmesh-0.7.0/sqlmesh/core/dialect.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/engine_adapter/__init__.py` & `sqlmesh-0.7.0/sqlmesh/core/engine_adapter/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/engine_adapter/_typing.py` & `sqlmesh-0.7.0/sqlmesh/core/engine_adapter/_typing.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/engine_adapter/base.py` & `sqlmesh-0.7.0/sqlmesh/core/engine_adapter/base.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/engine_adapter/base_postgres.py` & `sqlmesh-0.7.0/sqlmesh/core/engine_adapter/base_postgres.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/engine_adapter/base_spark.py` & `sqlmesh-0.7.0/sqlmesh/core/engine_adapter/base_spark.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/engine_adapter/bigquery.py` & `sqlmesh-0.7.0/sqlmesh/core/engine_adapter/bigquery.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/engine_adapter/databricks_api.py` & `sqlmesh-0.7.0/sqlmesh/core/engine_adapter/databricks_api.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/engine_adapter/duckdb.py` & `sqlmesh-0.7.0/sqlmesh/core/engine_adapter/duckdb.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/engine_adapter/postgres.py` & `sqlmesh-0.7.0/sqlmesh/core/engine_adapter/postgres.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/engine_adapter/redshift.py` & `sqlmesh-0.7.0/sqlmesh/core/engine_adapter/redshift.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/engine_adapter/shared.py` & `sqlmesh-0.7.0/sqlmesh/core/engine_adapter/shared.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/engine_adapter/snowflake.py` & `sqlmesh-0.7.0/sqlmesh/core/engine_adapter/snowflake.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/engine_adapter/spark.py` & `sqlmesh-0.7.0/sqlmesh/core/engine_adapter/spark.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/environment.py` & `sqlmesh-0.7.0/sqlmesh/core/environment.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/hooks.py` & `sqlmesh-0.7.0/sqlmesh/core/hooks.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/loader.py` & `sqlmesh-0.7.0/sqlmesh/core/loader.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/macros.py` & `sqlmesh-0.7.0/sqlmesh/core/macros.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/model/__init__.py` & `sqlmesh-0.7.0/sqlmesh/core/model/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/model/cache.py` & `sqlmesh-0.7.0/sqlmesh/core/model/cache.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/model/common.py` & `sqlmesh-0.7.0/sqlmesh/core/model/common.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/model/decorator.py` & `sqlmesh-0.7.0/sqlmesh/core/model/decorator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/model/definition.py` & `sqlmesh-0.7.0/sqlmesh/core/model/definition.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/model/kind.py` & `sqlmesh-0.7.0/sqlmesh/core/model/kind.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/model/meta.py` & `sqlmesh-0.7.0/sqlmesh/core/model/meta.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/model/seed.py` & `sqlmesh-0.7.0/sqlmesh/core/model/seed.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/notification_target.py` & `sqlmesh-0.7.0/sqlmesh/core/notification_target.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/plan/definition.py` & `sqlmesh-0.7.0/sqlmesh/core/plan/definition.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/plan/evaluator.py` & `sqlmesh-0.7.0/sqlmesh/core/plan/evaluator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/renderer.py` & `sqlmesh-0.7.0/sqlmesh/core/renderer.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/scheduler.py` & `sqlmesh-0.7.0/sqlmesh/core/scheduler.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/schema_diff.py` & `sqlmesh-0.7.0/sqlmesh/core/schema_diff.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/snapshot/__init__.py` & `sqlmesh-0.7.0/sqlmesh/core/snapshot/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/snapshot/categorizer.py` & `sqlmesh-0.7.0/sqlmesh/core/snapshot/categorizer.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/snapshot/definition.py` & `sqlmesh-0.7.0/sqlmesh/core/snapshot/definition.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/snapshot/evaluator.py` & `sqlmesh-0.7.0/sqlmesh/core/snapshot/evaluator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/state_sync/__init__.py` & `sqlmesh-0.7.0/sqlmesh/core/state_sync/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/state_sync/base.py` & `sqlmesh-0.7.0/sqlmesh/core/state_sync/base.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/state_sync/common.py` & `sqlmesh-0.7.0/sqlmesh/core/state_sync/common.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/state_sync/engine_adapter.py` & `sqlmesh-0.7.0/sqlmesh/core/state_sync/engine_adapter.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/test.py` & `sqlmesh-0.7.0/sqlmesh/core/test.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/core/user.py` & `sqlmesh-0.7.0/sqlmesh/core/user.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/dbt/adapter.py` & `sqlmesh-0.7.0/sqlmesh/dbt/adapter.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/dbt/basemodel.py` & `sqlmesh-0.7.0/sqlmesh/dbt/basemodel.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/dbt/builtin.py` & `sqlmesh-0.7.0/sqlmesh/dbt/builtin.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/dbt/column.py` & `sqlmesh-0.7.0/sqlmesh/dbt/column.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/dbt/common.py` & `sqlmesh-0.7.0/sqlmesh/dbt/common.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/dbt/context.py` & `sqlmesh-0.7.0/sqlmesh/dbt/context.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/dbt/loader.py` & `sqlmesh-0.7.0/sqlmesh/dbt/loader.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/dbt/model.py` & `sqlmesh-0.7.0/sqlmesh/dbt/model.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/dbt/package.py` & `sqlmesh-0.7.0/sqlmesh/dbt/package.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/dbt/profile.py` & `sqlmesh-0.7.0/sqlmesh/dbt/profile.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/dbt/project.py` & `sqlmesh-0.7.0/sqlmesh/dbt/project.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/dbt/seed.py` & `sqlmesh-0.7.0/sqlmesh/dbt/seed.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/dbt/source.py` & `sqlmesh-0.7.0/sqlmesh/dbt/source.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/dbt/target.py` & `sqlmesh-0.7.0/sqlmesh/dbt/target.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/engines/commands.py` & `sqlmesh-0.7.0/sqlmesh/engines/commands.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/engines/spark/app.py` & `sqlmesh-0.7.0/sqlmesh/engines/spark/app.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/engines/spark/db_api/spark_session.py` & `sqlmesh-0.7.0/sqlmesh/engines/spark/db_api/spark_session.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/integrations/github/notification_operator_provider.py` & `sqlmesh-0.7.0/sqlmesh/integrations/github/notification_operator_provider.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/integrations/github/notification_target.py` & `sqlmesh-0.7.0/sqlmesh/integrations/github/notification_target.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/integrations/github/shared.py` & `sqlmesh-0.7.0/sqlmesh/integrations/github/shared.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/magics.py` & `sqlmesh-0.7.0/sqlmesh/magics.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/migrations/v0001_init.py` & `sqlmesh-0.7.0/sqlmesh/migrations/v0001_init.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/migrations/v0003_move_batch_size.py` & `sqlmesh-0.7.0/sqlmesh/migrations/v0003_move_batch_size.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/migrations/v0004_environmnent_add_finalized_at.py` & `sqlmesh-0.7.0/sqlmesh/migrations/v0004_environmnent_add_finalized_at.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/schedulers/airflow/api.py` & `sqlmesh-0.7.0/sqlmesh/schedulers/airflow/api.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/schedulers/airflow/client.py` & `sqlmesh-0.7.0/sqlmesh/schedulers/airflow/client.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/schedulers/airflow/common.py` & `sqlmesh-0.7.0/sqlmesh/schedulers/airflow/common.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/schedulers/airflow/dag_generator.py` & `sqlmesh-0.7.0/sqlmesh/schedulers/airflow/dag_generator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/schedulers/airflow/hooks/bigquery.py` & `sqlmesh-0.7.0/sqlmesh/schedulers/airflow/hooks/bigquery.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/schedulers/airflow/hooks/redshift.py` & `sqlmesh-0.7.0/sqlmesh/schedulers/airflow/hooks/redshift.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/schedulers/airflow/integration.py` & `sqlmesh-0.7.0/sqlmesh/schedulers/airflow/integration.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/schedulers/airflow/operators/bigquery.py` & `sqlmesh-0.7.0/sqlmesh/schedulers/airflow/operators/bigquery.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/schedulers/airflow/operators/databricks.py` & `sqlmesh-0.7.0/sqlmesh/schedulers/airflow/operators/databricks.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/schedulers/airflow/operators/hwm_sensor.py` & `sqlmesh-0.7.0/sqlmesh/schedulers/airflow/operators/hwm_sensor.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/schedulers/airflow/operators/notification.py` & `sqlmesh-0.7.0/sqlmesh/schedulers/airflow/operators/notification.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/schedulers/airflow/operators/postgres.py` & `sqlmesh-0.7.0/sqlmesh/schedulers/airflow/operators/postgres.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/schedulers/airflow/operators/redshift.py` & `sqlmesh-0.7.0/sqlmesh/schedulers/airflow/operators/redshift.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/schedulers/airflow/operators/snowflake.py` & `sqlmesh-0.7.0/sqlmesh/schedulers/airflow/operators/snowflake.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/schedulers/airflow/operators/spark_submit.py` & `sqlmesh-0.7.0/sqlmesh/schedulers/airflow/operators/spark_submit.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/schedulers/airflow/operators/targets.py` & `sqlmesh-0.7.0/sqlmesh/schedulers/airflow/operators/targets.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/schedulers/airflow/plan.py` & `sqlmesh-0.7.0/sqlmesh/schedulers/airflow/plan.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/schedulers/airflow/plugin.py` & `sqlmesh-0.7.0/sqlmesh/schedulers/airflow/plugin.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/schedulers/airflow/state_sync.py` & `sqlmesh-0.7.0/sqlmesh/schedulers/airflow/state_sync.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/schedulers/airflow/util.py` & `sqlmesh-0.7.0/sqlmesh/schedulers/airflow/util.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/utils/__init__.py` & `sqlmesh-0.7.0/sqlmesh/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/utils/cache.py` & `sqlmesh-0.7.0/sqlmesh/utils/cache.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/utils/concurrency.py` & `sqlmesh-0.7.0/sqlmesh/utils/concurrency.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/utils/connection_pool.py` & `sqlmesh-0.7.0/sqlmesh/utils/connection_pool.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/utils/dag.py` & `sqlmesh-0.7.0/sqlmesh/utils/dag.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/utils/date.py` & `sqlmesh-0.7.0/sqlmesh/utils/date.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,40 +154,41 @@
         A date object with tz utc.
     """
     return to_datetime(value, relative_base).date()
 
 
 def date_dict(
     start: TimeLike, end: TimeLike, latest: TimeLike, only_latest: bool = False
-) -> t.Dict[str, t.Union[str, datetime, float, int]]:
+) -> t.Dict[str, t.Union[str, datetime, date, float, int]]:
     """Creates a kwarg dictionary of datetime variables for use in SQL Contexts.
 
     Keys are like start_date, start_ds, end_date, end_ds...
 
     Args:
         start: Start time.
         end: End time.
         latest: Latest time.
         only_latest: Only the latest timestamps will be returned.
 
     Returns:
         A dictionary with various keys pointing to datetime formats.
     """
-    kwargs: t.Dict[str, t.Union[str, datetime, float, int]] = {}
+    kwargs: t.Dict[str, t.Union[str, datetime, date, float, int]] = {}
 
     prefixes = [("latest", to_datetime(latest))]
 
     if not only_latest:
         prefixes.append(("start", to_datetime(start)))
         prefixes.append(("end", to_datetime(end)))
 
     for prefix, time_like in prefixes:
         dt = to_datetime(time_like)
         millis = to_timestamp(time_like)
-        kwargs[f"{prefix}_date"] = dt
+        kwargs[f"{prefix}_dt"] = dt
+        kwargs[f"{prefix}_date"] = to_date(dt)
         kwargs[f"{prefix}_ds"] = to_ds(time_like)
         kwargs[f"{prefix}_ts"] = dt.isoformat()
         kwargs[f"{prefix}_epoch"] = millis / 1000
         kwargs[f"{prefix}_millis"] = millis
     return kwargs
```

### Comparing `sqlmesh-0.6.4/sqlmesh/utils/errors.py` & `sqlmesh-0.7.0/sqlmesh/utils/errors.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/utils/jinja.py` & `sqlmesh-0.7.0/sqlmesh/utils/jinja.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/utils/metaprogramming.py` & `sqlmesh-0.7.0/sqlmesh/utils/metaprogramming.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/utils/pandas.py` & `sqlmesh-0.7.0/sqlmesh/utils/pandas.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/utils/pydantic.py` & `sqlmesh-0.7.0/sqlmesh/utils/pydantic.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/utils/rich.py` & `sqlmesh-0.7.0/sqlmesh/utils/rich.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/utils/transactional_file.py` & `sqlmesh-0.7.0/sqlmesh/utils/transactional_file.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh/utils/yaml.py` & `sqlmesh-0.7.0/sqlmesh/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/sqlmesh.egg-info/PKG-INFO` & `sqlmesh-0.7.0/sqlmesh.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlmesh
-Version: 0.6.4
+Version: 0.7.0
 Home-page: https://github.com/TobikoData/sqlmesh
 Author: TobikoData Inc.
 Author-email: engineering@tobikodata.com
 License: Apache License 2.0
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: SQL
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 Provides-Extra: bigquery
 Provides-Extra: databricks
 Provides-Extra: dev
 Provides-Extra: dbt
+Provides-Extra: llm
 Provides-Extra: postgres
 Provides-Extra: redshift
 Provides-Extra: snowflake
 Provides-Extra: web
 License-File: LICENSE
 
 ![SQLMesh logo](sqlmesh.svg)
```

### Comparing `sqlmesh-0.6.4/sqlmesh.egg-info/SOURCES.txt` & `sqlmesh-0.7.0/sqlmesh.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -263,14 +263,15 @@
 sqlmesh/engines/commands.py
 sqlmesh/engines/spark/__init__.py
 sqlmesh/engines/spark/app.py
 sqlmesh/engines/spark/db_api/__init__.py
 sqlmesh/engines/spark/db_api/errors.py
 sqlmesh/engines/spark/db_api/spark_session.py
 sqlmesh/integrations/__init__.py
+sqlmesh/integrations/llm.py
 sqlmesh/integrations/github/__init__.py
 sqlmesh/integrations/github/notification_operator_provider.py
 sqlmesh/integrations/github/notification_target.py
 sqlmesh/integrations/github/shared.py
 sqlmesh/migrations/__init__.py
 sqlmesh/migrations/v0001_init.py
 sqlmesh/migrations/v0002_remove_identify.py
```

### Comparing `sqlmesh-0.6.4/sqlmesh.egg-info/requires.txt` & `sqlmesh-0.7.0/sqlmesh.egg-info/requires.txt`

 * *Files 23% similar despite different names*

```diff
@@ -49,14 +49,18 @@
 sqlalchemy-stubs
 tenacity==8.1.0
 types-croniter
 types-dateparser
 types-pytz
 types-requests==2.28.8
 
+[llm]
+langchain
+openai
+
 [postgres]
 psycopg2
 
 [redshift]
 redshift_connector
 
 [snowflake]
```

### Comparing `sqlmesh-0.6.4/sqlmesh.svg` & `sqlmesh-0.7.0/sqlmesh.svg`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/conftest.py` & `sqlmesh-0.7.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/core/engine_adapter/test_base.py` & `sqlmesh-0.7.0/tests/core/engine_adapter/test_base.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/core/engine_adapter/test_base_postgres.py` & `sqlmesh-0.7.0/tests/core/engine_adapter/test_base_postgres.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/core/engine_adapter/test_base_spark.py` & `sqlmesh-0.7.0/tests/core/engine_adapter/test_base_spark.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/core/engine_adapter/test_bigquery.py` & `sqlmesh-0.7.0/tests/core/engine_adapter/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/core/engine_adapter/test_databricks.py` & `sqlmesh-0.7.0/tests/core/engine_adapter/test_databricks.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/core/engine_adapter/test_duckdb.py` & `sqlmesh-0.7.0/tests/core/engine_adapter/test_duckdb.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/core/engine_adapter/test_postgres.py` & `sqlmesh-0.7.0/tests/core/engine_adapter/test_postgres.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/core/engine_adapter/test_redshift.py` & `sqlmesh-0.7.0/tests/core/engine_adapter/test_redshift.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/core/engine_adapter/test_spark.py` & `sqlmesh-0.7.0/tests/core/engine_adapter/test_spark.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/core/test_audit.py` & `sqlmesh-0.7.0/tests/core/test_audit.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/core/test_config.py` & `sqlmesh-0.7.0/tests/core/test_config.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/core/test_connection_config.py` & `sqlmesh-0.7.0/tests/core/test_connection_config.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/core/test_context.py` & `sqlmesh-0.7.0/tests/core/test_context.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/core/test_dialect.py` & `sqlmesh-0.7.0/tests/core/test_dialect.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/core/test_integration.py` & `sqlmesh-0.7.0/tests/core/test_integration.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/core/test_macros.py` & `sqlmesh-0.7.0/tests/core/test_macros.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/core/test_model.py` & `sqlmesh-0.7.0/tests/core/test_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -546,29 +546,33 @@
         model.render_query(start="2020-10-28", end="2020-10-28"),
         """
         SELECT
           x.y AS y
         FROM x AS x
         WHERE
           x.y <= '2020-10-28'
+          AND x.y <= DATE_STR_TO_DATE('2020-10-28')
           AND x.y <= TIME_STR_TO_TIME('2020-10-28T23:59:59.999000+00:00')
           AND x.y >= '2020-10-28'
+          AND x.y >= DATE_STR_TO_DATE('2020-10-28')
           AND x.y >= TIME_STR_TO_TIME('2020-10-28T00:00:00+00:00')
         """,
     )
     assert_exp_eq(
         model.render_query(start="2020-10-28", end=to_datetime("2020-10-29")),
         """
         SELECT
           x.y AS y
         FROM x AS x
         WHERE
           x.y <= '2020-10-28'
+          AND x.y <= DATE_STR_TO_DATE('2020-10-28')
           AND x.y <= TIME_STR_TO_TIME('2020-10-28T23:59:59.999000+00:00')
           AND x.y >= '2020-10-28'
+          AND x.y >= DATE_STR_TO_DATE('2020-10-28')
           AND x.y >= TIME_STR_TO_TIME('2020-10-28T00:00:00+00:00')
         """,
     )
 
 
 def test_time_column():
     expressions = parse(
```

### Comparing `sqlmesh-0.6.4/tests/core/test_plan.py` & `sqlmesh-0.7.0/tests/core/test_plan.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/core/test_plan_evaluator.py` & `sqlmesh-0.7.0/tests/core/test_plan_evaluator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/core/test_scheduler.py` & `sqlmesh-0.7.0/tests/core/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/core/test_schema_diff.py` & `sqlmesh-0.7.0/tests/core/test_schema_diff.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/core/test_seed.py` & `sqlmesh-0.7.0/tests/core/test_seed.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/core/test_snapshot.py` & `sqlmesh-0.7.0/tests/core/test_snapshot.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/core/test_snapshot_evaluator.py` & `sqlmesh-0.7.0/tests/core/test_snapshot_evaluator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/core/test_state_sync.py` & `sqlmesh-0.7.0/tests/core/test_state_sync.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/dbt/conftest.py` & `sqlmesh-0.7.0/tests/dbt/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/dbt/test_adapter.py` & `sqlmesh-0.7.0/tests/dbt/test_adapter.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/dbt/test_config.py` & `sqlmesh-0.7.0/tests/dbt/test_config.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/dbt/test_transformation.py` & `sqlmesh-0.7.0/tests/dbt/test_transformation.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/engines/spark/test_db_api.py` & `sqlmesh-0.7.0/tests/engines/spark/test_db_api.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/dbt_project.yml` & `sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/logs/dbt.log.legacy` & `sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/logs/dbt.log.legacy`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/macros/incremental.sql` & `sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/macros/incremental.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/models/waiter_revenue_by_day.sql` & `sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/models/waiter_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/packages/customers/dbt_project.yml` & `sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/packages/customers/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/packages/customers/models/customer_revenue_by_day.sql` & `sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/packages/customers/models/customer_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/profiles.yml` & `sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/profiles.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/seed_sources.py` & `sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/seed_sources.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/source_data/items.csv` & `sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/source_data/items.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/source_data/order_items.csv` & `sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/source_data/order_items.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/fixtures/dbt/sushi_test/source_data/orders.csv` & `sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/source_data/orders.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/fixtures/migrations/environments.json` & `sqlmesh-0.7.0/tests/fixtures/migrations/environments.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/fixtures/migrations/snapshots.json` & `sqlmesh-0.7.0/tests/fixtures/migrations/snapshots.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/integrations/github/fixtures/pull_request_review.json` & `sqlmesh-0.7.0/tests/integrations/github/fixtures/pull_request_review.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/schedulers/airflow/conftest.py` & `sqlmesh-0.7.0/tests/schedulers/airflow/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/schedulers/airflow/operators/test_hwm_sensor.py` & `sqlmesh-0.7.0/tests/schedulers/airflow/operators/test_hwm_sensor.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/schedulers/airflow/operators/test_targets.py` & `sqlmesh-0.7.0/tests/schedulers/airflow/operators/test_targets.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/schedulers/airflow/test_client.py` & `sqlmesh-0.7.0/tests/schedulers/airflow/test_client.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/schedulers/airflow/test_end_to_end.py` & `sqlmesh-0.7.0/tests/schedulers/airflow/test_end_to_end.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/schedulers/airflow/test_integration.py` & `sqlmesh-0.7.0/tests/schedulers/airflow/test_integration.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/schedulers/airflow/test_plan.py` & `sqlmesh-0.7.0/tests/schedulers/airflow/test_plan.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/utils/test_cache.py` & `sqlmesh-0.7.0/tests/utils/test_cache.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/utils/test_concurrency.py` & `sqlmesh-0.7.0/tests/utils/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/utils/test_connection_pool.py` & `sqlmesh-0.7.0/tests/utils/test_connection_pool.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/utils/test_dag.py` & `sqlmesh-0.7.0/tests/utils/test_dag.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/utils/test_date.py` & `sqlmesh-0.7.0/tests/utils/test_date.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/utils/test_filesystem.py` & `sqlmesh-0.7.0/tests/utils/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/utils/test_jinja.py` & `sqlmesh-0.7.0/tests/utils/test_jinja.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/utils/test_metaprogramming.py` & `sqlmesh-0.7.0/tests/utils/test_metaprogramming.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/utils/test_pandas.py` & `sqlmesh-0.7.0/tests/utils/test_pandas.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/utils/test_pydantic.py` & `sqlmesh-0.7.0/tests/utils/test_pydantic.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/utils/test_transactional_file.py` & `sqlmesh-0.7.0/tests/utils/test_transactional_file.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/utils/test_yaml.py` & `sqlmesh-0.7.0/tests/utils/test_yaml.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/tests/web/test_main.py` & `sqlmesh-0.7.0/tests/web/test_main.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/.eslintrc.js` & `sqlmesh-0.7.0/web/client/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/dist/assets/CircularStd-Black-52659624.otf` & `sqlmesh-0.7.0/web/client/dist/assets/CircularStd-Black-52659624.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/dist/assets/CircularStd-Bold-0e6c076d.otf` & `sqlmesh-0.7.0/web/client/dist/assets/CircularStd-Bold-0e6c076d.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/dist/assets/CircularStd-Medium-2f373e53.otf` & `sqlmesh-0.7.0/web/client/dist/assets/CircularStd-Medium-2f373e53.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/dist/assets/Plan-683a0552.js` & `sqlmesh-0.7.0/web/client/dist/assets/Plan-683a0552.js`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/dist/assets/Publico-Black-e6bd2ea2.otf` & `sqlmesh-0.7.0/web/client/dist/assets/Publico-Black-e6bd2ea2.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/dist/assets/Publico-Bold-c79acd56.otf` & `sqlmesh-0.7.0/web/client/dist/assets/Publico-Bold-c79acd56.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/dist/assets/Publico-Medium-01b4a891.otf` & `sqlmesh-0.7.0/web/client/dist/assets/Publico-Medium-01b4a891.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/dist/assets/index-b61dbb6f.css` & `sqlmesh-0.7.0/web/client/dist/assets/index-b61dbb6f.css`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/dist/assets/index-f2c4b7c5.js` & `sqlmesh-0.7.0/web/client/dist/assets/index-f2c4b7c5.js`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/dist/assets/worker-e891d118.js` & `sqlmesh-0.7.0/web/client/dist/assets/worker-e891d118.js`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/dist/favicons/favicon.ico` & `sqlmesh-0.7.0/web/client/dist/favicons/favicon.ico`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/dist/index.html` & `sqlmesh-0.7.0/web/client/dist/index.html`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/index.html` & `sqlmesh-0.7.0/web/client/index.html`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/openapi.json` & `sqlmesh-0.7.0/web/client/openapi.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/package-lock.json` & `sqlmesh-0.7.0/web/client/package-lock.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/package.json` & `sqlmesh-0.7.0/web/client/package.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/playwright.config.ts` & `sqlmesh-0.7.0/web/client/playwright.config.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/public/favicons/favicon.ico` & `sqlmesh-0.7.0/web/client/public/favicons/favicon.ico`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/api/channels.ts` & `sqlmesh-0.7.0/web/client/src/api/channels.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/api/index.ts` & `sqlmesh-0.7.0/web/client/src/api/index.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/api/instance.ts` & `sqlmesh-0.7.0/web/client/src/api/instance.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/assets/fonts/Circular STD/CircularStd-Black.otf` & `sqlmesh-0.7.0/web/client/src/assets/fonts/Circular STD/CircularStd-Black.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/assets/fonts/Circular STD/CircularStd-BlackItalic.otf` & `sqlmesh-0.7.0/web/client/src/assets/fonts/Circular STD/CircularStd-BlackItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/assets/fonts/Circular STD/CircularStd-Bold.otf` & `sqlmesh-0.7.0/web/client/src/assets/fonts/Circular STD/CircularStd-Bold.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/assets/fonts/Circular STD/CircularStd-BoldItalic.otf` & `sqlmesh-0.7.0/web/client/src/assets/fonts/Circular STD/CircularStd-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/assets/fonts/Circular STD/CircularStd-Book.otf` & `sqlmesh-0.7.0/web/client/src/assets/fonts/Circular STD/CircularStd-Book.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/assets/fonts/Circular STD/CircularStd-BookItalic.otf` & `sqlmesh-0.7.0/web/client/src/assets/fonts/Circular STD/CircularStd-BookItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/assets/fonts/Circular STD/CircularStd-Medium.otf` & `sqlmesh-0.7.0/web/client/src/assets/fonts/Circular STD/CircularStd-Medium.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/assets/fonts/Circular STD/CircularStd-MediumItalic.otf` & `sqlmesh-0.7.0/web/client/src/assets/fonts/Circular STD/CircularStd-MediumItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/Publico-Black.otf` & `sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/Publico-Black.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/Publico-BlackItalic.otf` & `sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/Publico-BlackItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/Publico-Bold.otf` & `sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/Publico-Bold.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/Publico-BoldItalic.otf` & `sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/Publico-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/Publico-Extrabold.otf` & `sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/Publico-Extrabold.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/Publico-ExtraboldItalic.otf` & `sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/Publico-ExtraboldItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/Publico-Italic.otf` & `sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/Publico-Italic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/Publico-Light.otf` & `sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/Publico-Light.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/Publico-LightItalic.otf` & `sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/Publico-LightItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/Publico-Medium.otf` & `sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/Publico-Medium.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/Publico-MediumItalic.otf` & `sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/Publico-MediumItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/Publico-Roman.otf` & `sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/Publico-Roman.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/PublicoText-Bold.otf` & `sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/PublicoText-Bold.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/PublicoText-BoldItalic.otf` & `sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/PublicoText-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/PublicoText-Italic.otf` & `sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/PublicoText-Italic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/PublicoText-Roman.otf` & `sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/PublicoText-Roman.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/PublicoText-Semibold.otf` & `sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/PublicoText-Semibold.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/assets/fonts/Publico/PublicoText-SemiboldItalic.otf` & `sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/PublicoText-SemiboldItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/context/context.ts` & `sqlmesh-0.7.0/web/client/src/context/context.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/context/editor.ts` & `sqlmesh-0.7.0/web/client/src/context/editor.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/context/fileTree.ts` & `sqlmesh-0.7.0/web/client/src/context/fileTree.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/context/lineage.tsx` & `sqlmesh-0.7.0/web/client/src/context/lineage.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/context/plan.ts` & `sqlmesh-0.7.0/web/client/src/context/plan.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/context/theme.tsx` & `sqlmesh-0.7.0/web/client/src/context/theme.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/hooks/useLocalStorage.ts` & `sqlmesh-0.7.0/web/client/src/hooks/useLocalStorage.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/index.css` & `sqlmesh-0.7.0/web/client/src/index.css`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/library/components/banner/Banner.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/banner/Banner.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/library/components/button/Button.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/button/Button.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/library/components/button/tests/Button.spec.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/button/tests/Button.spec.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/library/components/divider/Divider.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/divider/Divider.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/library/components/divider/tests/Divider.spec.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/divider/tests/Divider.spec.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/library/components/editor/Editor.css` & `sqlmesh-0.7.0/web/client/src/library/components/editor/Editor.css`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/library/components/editor/Editor.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/editor/Editor.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/library/components/editor/EditorCode.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/editor/EditorCode.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/library/components/editor/EditorFooter.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/editor/EditorFooter.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/library/components/editor/EditorIndicator.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/editor/EditorIndicator.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/library/components/editor/EditorInspector.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/editor/EditorInspector.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/library/components/editor/EditorPreview.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/editor/EditorPreview.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/library/components/editor/EditorTabs.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/editor/EditorTabs.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/library/components/editor/extensions/SqlMeshDialect.ts` & `sqlmesh-0.7.0/web/client/src/library/components/editor/extensions/SqlMeshDialect.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/library/components/editor/extensions/index.ts` & `sqlmesh-0.7.0/web/client/src/library/components/editor/extensions/index.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/library/components/editor/help.ts` & `sqlmesh-0.7.0/web/client/src/library/components/editor/help.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/library/components/fileTree/Directory.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/fileTree/Directory.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/library/components/fileTree/File.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/fileTree/File.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/library/components/fileTree/FileTree.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/fileTree/FileTree.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/library/components/fileTree/help.ts` & `sqlmesh-0.7.0/web/client/src/library/components/fileTree/help.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/library/components/graph/Graph.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/graph/Graph.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/library/components/graph/help.ts` & `sqlmesh-0.7.0/web/client/src/library/components/graph/help.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/library/components/ide/ActivePlan.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/ide/ActivePlan.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/library/components/ide/IDE.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/ide/IDE.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/library/components/ide/RunPlan.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/ide/RunPlan.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/library/components/input/Input.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/input/Input.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/library/components/input/InputToggle.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/input/InputToggle.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/library/components/logo/Spinner.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/logo/Spinner.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/library/components/logo/SqlMesh.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/logo/SqlMesh.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/library/components/logo/Tobiko.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/logo/Tobiko.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/library/components/modal/Modal.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/modal/Modal.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/library/components/modal/ModalConfirmation.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/modal/ModalConfirmation.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/library/components/modal/ModalDrawer.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/modal/ModalDrawer.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/library/components/plan/Plan.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/plan/Plan.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/library/components/plan/PlanActions.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/plan/PlanActions.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/library/components/plan/PlanBackfillDates.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/plan/PlanBackfillDates.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/library/components/plan/PlanChangePreview.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/plan/PlanChangePreview.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/library/components/plan/PlanHeader.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/plan/PlanHeader.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/library/components/plan/PlanWizard.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/plan/PlanWizard.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/library/components/plan/PlanWizardStepOptions.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/plan/PlanWizardStepOptions.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/library/components/plan/context.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/plan/context.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/library/components/plan/help.spec.ts` & `sqlmesh-0.7.0/web/client/src/library/components/plan/help.spec.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/library/components/plan/help.ts` & `sqlmesh-0.7.0/web/client/src/library/components/plan/help.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/library/components/plan/hooks.ts` & `sqlmesh-0.7.0/web/client/src/library/components/plan/hooks.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/library/components/progress/Progress.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/progress/Progress.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/library/components/report/ReportTestsErrors.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/report/ReportTestsErrors.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/library/components/root/Footer.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/root/Footer.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/library/components/root/Header.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/root/Header.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/library/components/splitPane/SplitPane.css` & `sqlmesh-0.7.0/web/client/src/library/components/splitPane/SplitPane.css`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/library/components/splitPane/SplitPane.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/splitPane/SplitPane.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/library/components/tasksOverview/TasksOverview.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/tasksOverview/TasksOverview.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/library/components/toggle/Toggle.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/toggle/Toggle.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/main.tsx` & `sqlmesh-0.7.0/web/client/src/main.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/models/artifact.ts` & `sqlmesh-0.7.0/web/client/src/models/artifact.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/models/directory.ts` & `sqlmesh-0.7.0/web/client/src/models/directory.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/models/environment.ts` & `sqlmesh-0.7.0/web/client/src/models/environment.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/models/file.ts` & `sqlmesh-0.7.0/web/client/src/models/file.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/models/initial.ts` & `sqlmesh-0.7.0/web/client/src/models/initial.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/tests/utils.tsx` & `sqlmesh-0.7.0/web/client/src/tests/utils.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/utils/index.spec.ts` & `sqlmesh-0.7.0/web/client/src/utils/index.spec.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/utils/index.ts` & `sqlmesh-0.7.0/web/client/src/utils/index.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/workers/sqlglot/sqlglot.py` & `sqlmesh-0.7.0/web/client/src/workers/sqlglot/sqlglot.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/src/workers/sqlglot/worker.ts` & `sqlmesh-0.7.0/web/client/src/workers/sqlglot/worker.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/tailwind.config.js` & `sqlmesh-0.7.0/web/client/tailwind.config.js`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/tsconfig.json` & `sqlmesh-0.7.0/web/client/tsconfig.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/client/vite.config.ts` & `sqlmesh-0.7.0/web/client/vite.config.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/server/api/endpoints/__init__.py` & `sqlmesh-0.7.0/web/server/api/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/server/api/endpoints/commands.py` & `sqlmesh-0.7.0/web/server/api/endpoints/commands.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/server/api/endpoints/context.py` & `sqlmesh-0.7.0/web/server/api/endpoints/context.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/server/api/endpoints/directories.py` & `sqlmesh-0.7.0/web/server/api/endpoints/directories.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/server/api/endpoints/environments.py` & `sqlmesh-0.7.0/web/server/api/endpoints/environments.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/server/api/endpoints/events.py` & `sqlmesh-0.7.0/web/server/api/endpoints/events.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/server/api/endpoints/files.py` & `sqlmesh-0.7.0/web/server/api/endpoints/files.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/server/api/endpoints/lineage.py` & `sqlmesh-0.7.0/web/server/api/endpoints/lineage.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/server/api/endpoints/models.py` & `sqlmesh-0.7.0/web/server/api/endpoints/models.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/server/api/endpoints/plan.py` & `sqlmesh-0.7.0/web/server/api/endpoints/plan.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/server/console.py` & `sqlmesh-0.7.0/web/server/console.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/server/main.py` & `sqlmesh-0.7.0/web/server/main.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/server/models.py` & `sqlmesh-0.7.0/web/server/models.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/server/settings.py` & `sqlmesh-0.7.0/web/server/settings.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/server/sse.py` & `sqlmesh-0.7.0/web/server/sse.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/server/utils.py` & `sqlmesh-0.7.0/web/server/utils.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.4/web/server/watcher.py` & `sqlmesh-0.7.0/web/server/watcher.py`

 * *Files identical despite different names*

