# Comparing `tmp/pulp-cli-0.8.0.tar.gz` & `tmp/pulp-cli-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulp-cli-0.8.0.tar", last modified: Fri Apr 30 15:25:18 2021, max compression
+gzip compressed data, was "pulp-cli-0.9.0.tar", last modified: Mon May 17 17:41:21 2021, max compression
```

## Comparing `pulp-cli-0.8.0.tar` & `pulp-cli-0.9.0.tar`

### file list

```diff
@@ -1,93 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-30 15:25:18.873650 pulp-cli-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)     2811 2021-04-30 15:25:18.873650 pulp-cli-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5160 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-30 15:25:18.865651 pulp-cli-0.8.0/pulp_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2811 2021-04-30 15:25:18.000000 pulp-cli-0.8.0/pulp_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2366 2021-04-30 15:25:18.000000 pulp-cli-0.8.0/pulp_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-30 15:25:18.000000 pulp-cli-0.8.0/pulp_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      272 2021-04-30 15:25:18.000000 pulp-cli-0.8.0/pulp_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       70 2021-04-30 15:25:18.000000 pulp-cli-0.8.0/pulp_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       25 2021-04-30 15:25:18.000000 pulp-cli-0.8.0/pulp_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-30 15:25:18.865651 pulp-cli-0.8.0/pulpcore/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-30 15:25:18.865651 pulp-cli-0.8.0/pulpcore/cli/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-30 15:25:18.865651 pulp-cli-0.8.0/pulpcore/cli/ansible/
--rw-r--r--   0 runner    (1001) docker     (121)      546 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/ansible/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3054 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/ansible/context.py
--rw-r--r--   0 runner    (1001) docker     (121)     5065 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/ansible/distribution.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/ansible/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     3056 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/ansible/remote.py
--rw-r--r--   0 runner    (1001) docker     (121)     3441 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/ansible/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-30 15:25:18.865651 pulp-cli-0.8.0/pulpcore/cli/common/
--rw-r--r--   0 runner    (1001) docker     (121)     5440 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    22323 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/common/context.py
--rw-r--r--   0 runner    (1001) docker     (121)      803 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/common/debug.py
--rw-r--r--   0 runner    (1001) docker     (121)    21655 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/common/generic.py
--rw-r--r--   0 runner    (1001) docker     (121)    10732 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/common/openapi.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/common/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-30 15:25:18.865651 pulp-cli-0.8.0/pulpcore/cli/container/
--rw-r--r--   0 runner    (1001) docker     (121)      622 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4424 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/container/context.py
--rw-r--r--   0 runner    (1001) docker     (121)     5689 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/container/distribution.py
--rw-r--r--   0 runner    (1001) docker     (121)     1126 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/container/namespace.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/container/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     1452 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/container/remote.py
--rw-r--r--   0 runner    (1001) docker     (121)     3156 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/container/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-30 15:25:18.869650 pulp-cli-0.8.0/pulpcore/cli/core/
--rw-r--r--   0 runner    (1001) docker     (121)     1280 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1219 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/core/access_policy.py
--rw-r--r--   0 runner    (1001) docker     (121)     1176 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/core/artifact.py
--rw-r--r--   0 runner    (1001) docker     (121)     4150 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/core/config.py
--rw-r--r--   0 runner    (1001) docker     (121)    13695 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/core/context.py
--rw-r--r--   0 runner    (1001) docker     (121)     3461 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/core/export.py
--rw-r--r--   0 runner    (1001) docker     (121)     3139 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/core/exporter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1602 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/core/generic.py
--rw-r--r--   0 runner    (1001) docker     (121)     4895 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/core/group.py
--rw-r--r--   0 runner    (1001) docker     (121)     2171 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/core/importer.py
--rw-r--r--   0 runner    (1001) docker     (121)      334 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/core/orphans.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/core/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)      948 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/core/repository.py
--rw-r--r--   0 runner    (1001) docker     (121)      502 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/core/show.py
--rw-r--r--   0 runner    (1001) docker     (121)      686 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/core/signing_service.py
--rw-r--r--   0 runner    (1001) docker     (121)     1550 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/core/status.py
--rw-r--r--   0 runner    (1001) docker     (121)     1808 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/core/task.py
--rw-r--r--   0 runner    (1001) docker     (121)      533 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/core/task_group.py
--rw-r--r--   0 runner    (1001) docker     (121)      868 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/core/user.py
--rw-r--r--   0 runner    (1001) docker     (121)      807 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/core/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-30 15:25:18.869650 pulp-cli-0.8.0/pulpcore/cli/file/
--rw-r--r--   0 runner    (1001) docker     (121)      697 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3172 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/file/content.py
--rw-r--r--   0 runner    (1001) docker     (121)     2874 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/file/context.py
--rw-r--r--   0 runner    (1001) docker     (121)     2069 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/file/distribution.py
--rw-r--r--   0 runner    (1001) docker     (121)     1663 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/file/publication.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/file/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     1510 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/file/remote.py
--rw-r--r--   0 runner    (1001) docker     (121)     8834 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/file/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-30 15:25:18.869650 pulp-cli-0.8.0/pulpcore/cli/migration/
--rw-r--r--   0 runner    (1001) docker     (121)      389 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/migration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1176 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/migration/context.py
--rw-r--r--   0 runner    (1001) docker     (121)     1510 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/migration/plan.py
--rw-r--r--   0 runner    (1001) docker     (121)      909 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/migration/pulp2.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/migration/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-30 15:25:18.873650 pulp-cli-0.8.0/pulpcore/cli/python/
--rw-r--r--   0 runner    (1001) docker     (121)      711 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2531 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/python/content.py
--rw-r--r--   0 runner    (1001) docker     (121)     3654 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/python/context.py
--rw-r--r--   0 runner    (1001) docker     (121)     1626 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/python/distribution.py
--rw-r--r--   0 runner    (1001) docker     (121)     1673 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/python/publication.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/python/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     1929 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/python/remote.py
--rw-r--r--   0 runner    (1001) docker     (121)     6340 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/python/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-30 15:25:18.873650 pulp-cli-0.8.0/pulpcore/cli/rpm/
--rw-r--r--   0 runner    (1001) docker     (121)      568 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/rpm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       86 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/rpm/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     2382 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/rpm/context.py
--rw-r--r--   0 runner    (1001) docker     (121)     2127 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/rpm/distribution.py
--rw-r--r--   0 runner    (1001) docker     (121)     1656 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/rpm/publication.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/rpm/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     1501 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/rpm/remote.py
--rw-r--r--   0 runner    (1001) docker     (121)     3687 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pulpcore/cli/rpm/repository.py
--rw-r--r--   0 runner    (1001) docker     (121)      688 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-30 15:25:18.873650 pulp-cli-0.8.0/pytest_pulp_cli/
--rw-r--r--   0 runner    (1001) docker     (121)     3228 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/pytest_pulp_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-04-30 15:25:18.873650 pulp-cli-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1755 2021-04-30 15:25:11.000000 pulp-cli-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-17 17:41:21.589575 pulp-cli-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)    17988 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     2811 2021-05-17 17:41:21.589575 pulp-cli-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5160 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-17 17:41:21.581574 pulp-cli-0.9.0/pulp_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2811 2021-05-17 17:41:21.000000 pulp-cli-0.9.0/pulp_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2376 2021-05-17 17:41:21.000000 pulp-cli-0.9.0/pulp_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-17 17:41:21.000000 pulp-cli-0.9.0/pulp_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      272 2021-05-17 17:41:21.000000 pulp-cli-0.9.0/pulp_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2021-05-17 17:41:21.000000 pulp-cli-0.9.0/pulp_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2021-05-17 17:41:21.000000 pulp-cli-0.9.0/pulp_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-17 17:41:21.581574 pulp-cli-0.9.0/pulpcore/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-17 17:41:21.581574 pulp-cli-0.9.0/pulpcore/cli/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-17 17:41:21.585574 pulp-cli-0.9.0/pulpcore/cli/ansible/
+-rw-r--r--   0 runner    (1001) docker     (121)      546 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/ansible/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3054 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/ansible/context.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5065 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/ansible/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/ansible/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)     3056 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/ansible/remote.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3484 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/ansible/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-17 17:41:21.585574 pulp-cli-0.9.0/pulpcore/cli/common/
+-rw-r--r--   0 runner    (1001) docker     (121)     4173 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6875 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/common/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23498 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/common/context.py
+-rw-r--r--   0 runner    (1001) docker     (121)      803 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/common/debug.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21674 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/common/generic.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11388 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/common/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/common/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-17 17:41:21.585574 pulp-cli-0.9.0/pulpcore/cli/container/
+-rw-r--r--   0 runner    (1001) docker     (121)      622 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4503 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/container/context.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5689 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/container/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1126 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/container/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/container/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)     1880 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/container/remote.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3156 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/container/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-17 17:41:21.585574 pulp-cli-0.9.0/pulpcore/cli/core/
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1219 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/core/access_policy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1176 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/core/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13695 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/core/context.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3461 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/core/export.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3139 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/core/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1602 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/core/generic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4895 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/core/group.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2171 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/core/importer.py
+-rw-r--r--   0 runner    (1001) docker     (121)      334 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/core/orphans.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/core/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)      948 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/core/repository.py
+-rw-r--r--   0 runner    (1001) docker     (121)      502 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/core/show.py
+-rw-r--r--   0 runner    (1001) docker     (121)      686 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/core/signing_service.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1550 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/core/status.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1808 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/core/task.py
+-rw-r--r--   0 runner    (1001) docker     (121)      533 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/core/task_group.py
+-rw-r--r--   0 runner    (1001) docker     (121)      868 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/core/user.py
+-rw-r--r--   0 runner    (1001) docker     (121)      807 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/core/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-17 17:41:21.589575 pulp-cli-0.9.0/pulpcore/cli/file/
+-rw-r--r--   0 runner    (1001) docker     (121)      735 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3172 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/file/content.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2874 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/file/context.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2069 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/file/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1663 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/file/publication.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/file/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)     1510 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/file/remote.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8894 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/file/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-17 17:41:21.589575 pulp-cli-0.9.0/pulpcore/cli/migration/
+-rw-r--r--   0 runner    (1001) docker     (121)      389 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/migration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1176 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/migration/context.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1510 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/migration/plan.py
+-rw-r--r--   0 runner    (1001) docker     (121)      909 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/migration/pulp2.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/migration/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-17 17:41:21.589575 pulp-cli-0.9.0/pulpcore/cli/python/
+-rw-r--r--   0 runner    (1001) docker     (121)      711 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2531 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/python/content.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3080 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/python/context.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2385 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/python/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1673 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/python/publication.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/python/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)     2325 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/python/remote.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6358 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/python/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-17 17:41:21.589575 pulp-cli-0.9.0/pulpcore/cli/rpm/
+-rw-r--r--   0 runner    (1001) docker     (121)      568 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/rpm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       86 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/rpm/common.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2382 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/rpm/context.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2127 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/rpm/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1656 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/rpm/publication.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/rpm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)     1501 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/rpm/remote.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3747 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pulpcore/cli/rpm/repository.py
+-rw-r--r--   0 runner    (1001) docker     (121)      688 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-17 17:41:21.589575 pulp-cli-0.9.0/pytest_pulp_cli/
+-rw-r--r--   0 runner    (1001) docker     (121)     3228 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/pytest_pulp_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-05-17 17:41:21.589575 pulp-cli-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1789 2021-05-17 17:41:13.000000 pulp-cli-0.9.0/setup.py
```

### Comparing `pulp-cli-0.8.0/PKG-INFO` & `pulp-cli-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulp-cli
-Version: 0.8.0
+Version: 0.9.0
 Summary: Command line interface to talk to pulpcore's REST API.
 Home-page: https://github.com/pulp/pulp-cli
 License: GPLv2+
 Description: # Pulp command line interface
         
         This is a command line interface for Pulp 3.
```

### Comparing `pulp-cli-0.8.0/README.md` & `pulp-cli-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pulp-cli-0.8.0/pulp_cli.egg-info/PKG-INFO` & `pulp-cli-0.9.0/pulp_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulp-cli
-Version: 0.8.0
+Version: 0.9.0
 Summary: Command line interface to talk to pulpcore's REST API.
 Home-page: https://github.com/pulp/pulp-cli
 License: GPLv2+
 Description: # Pulp command line interface
         
         This is a command line interface for Pulp 3.
```

### Comparing `pulp-cli-0.8.0/pulp_cli.egg-info/SOURCES.txt` & `pulp-cli-0.9.0/pulp_cli.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 pyproject.toml
 setup.py
 pulp_cli.egg-info/PKG-INFO
 pulp_cli.egg-info/SOURCES.txt
 pulp_cli.egg-info/dependency_links.txt
 pulp_cli.egg-info/entry_points.txt
@@ -10,14 +11,15 @@
 pulpcore/cli/ansible/__init__.py
 pulpcore/cli/ansible/context.py
 pulpcore/cli/ansible/distribution.py
 pulpcore/cli/ansible/py.typed
 pulpcore/cli/ansible/remote.py
 pulpcore/cli/ansible/repository.py
 pulpcore/cli/common/__init__.py
+pulpcore/cli/common/config.py
 pulpcore/cli/common/context.py
 pulpcore/cli/common/debug.py
 pulpcore/cli/common/generic.py
 pulpcore/cli/common/openapi.py
 pulpcore/cli/common/py.typed
 pulpcore/cli/container/__init__.py
 pulpcore/cli/container/context.py
@@ -25,15 +27,14 @@
 pulpcore/cli/container/namespace.py
 pulpcore/cli/container/py.typed
 pulpcore/cli/container/remote.py
 pulpcore/cli/container/repository.py
 pulpcore/cli/core/__init__.py
 pulpcore/cli/core/access_policy.py
 pulpcore/cli/core/artifact.py
-pulpcore/cli/core/config.py
 pulpcore/cli/core/context.py
 pulpcore/cli/core/export.py
 pulpcore/cli/core/exporter.py
 pulpcore/cli/core/generic.py
 pulpcore/cli/core/group.py
 pulpcore/cli/core/importer.py
 pulpcore/cli/core/orphans.py
```

### Comparing `pulp-cli-0.8.0/pulpcore/cli/ansible/__init__.py` & `pulp-cli-0.9.0/pulpcore/cli/ansible/__init__.py`

 * *Files identical despite different names*

### Comparing `pulp-cli-0.8.0/pulpcore/cli/ansible/context.py` & `pulp-cli-0.9.0/pulpcore/cli/ansible/context.py`

 * *Files identical despite different names*

### Comparing `pulp-cli-0.8.0/pulpcore/cli/ansible/distribution.py` & `pulp-cli-0.9.0/pulpcore/cli/ansible/distribution.py`

 * *Files identical despite different names*

### Comparing `pulp-cli-0.8.0/pulpcore/cli/ansible/remote.py` & `pulp-cli-0.9.0/pulpcore/cli/ansible/remote.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 def _requirements_callback(
     ctx: click.Context, param: click.Parameter, value: Any
 ) -> Optional[Union[str, Any]]:
     if value:
         if isinstance(ctx.obj, PulpAnsibleRoleRemoteContext):
             raise click.ClickException(f"Option {param.name} not valid for Role remote, see --help")
-        if param.name == "requirements-file":
+        if param.name == "requirements_file":
             return f"{yaml.safe_load(value)}"
         elif param.name == "requirements":
             return yaml.safe_load(f'"{value}"')
     return value
 
 
 @click.group()
```

### Comparing `pulp-cli-0.8.0/pulpcore/cli/ansible/repository.py` & `pulp-cli-0.9.0/pulpcore/cli/ansible/repository.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from pulpcore.cli.ansible.context import (
     PulpAnsibleCollectionRemoteContext,
     PulpAnsibleRepositoryContext,
     PulpAnsibleRoleRemoteContext,
 )
 from pulpcore.cli.common.context import (
+    PluginRequirement,
     PulpContext,
     PulpRepositoryContext,
     pass_pulp_context,
     pass_repository_context,
 )
 from pulpcore.cli.common.generic import (
     create_command,
@@ -62,20 +63,20 @@
 
 
 lookup_options = [href_option, name_option]
 create_options = [
     click.option("--name", required=True),
     click.option("--description"),
     click.option("--remote", callback=_remote_callback, help=_("an optional remote")),
-    pulp_option("--retained-versions", needs_plugin="core", min_version="3.13.0.dev"),
+    pulp_option("--retained-versions", needs_plugins=[PluginRequirement("core", "3.13.0.dev")]),
 ]
 update_options = [
     click.option("--description"),
     click.option("--remote", callback=_remote_callback, help=_("new optional remote")),
-    pulp_option("--retained-versions", needs_plugin="core", min_version="3.13.0.dev"),
+    pulp_option("--retained-versions", needs_plugins=[PluginRequirement("core", "3.13.0.dev")]),
 ]
 
 repository.add_command(show_command(decorators=lookup_options))
 repository.add_command(list_command(decorators=[label_select_option]))
 repository.add_command(destroy_command(decorators=lookup_options))
 repository.add_command(version_command())
 repository.add_command(create_command(decorators=create_options))
```

### Comparing `pulp-cli-0.8.0/pulpcore/cli/common/__init__.py` & `pulp-cli-0.9.0/pulpcore/cli/common/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,30 @@
 import gettext
 import os
 import sys
-from typing import Any, Callable, Dict, Optional
+from typing import Any, Optional
 
 import click
 import pkg_resources
 import toml
 from click_shell import make_click_shell
 
+from pulpcore.cli.common.config import CONFIG_LOCATION, config, config_options, validate_config
 from pulpcore.cli.common.context import PulpContext
 from pulpcore.cli.common.debug import debug
 
 _ = gettext.gettext
-__version__ = "0.8.0"
+__version__ = "0.9.0"
 
 
 ##############################################################################
 # Main entry point
 
 
 PROFILE_KEY = f"{__name__}.profile"
-FORMAT_CHOICES = ["json", "yaml", "none"]
-
-
-def _validate_config(config: Dict[str, Any]) -> bool:
-    if "format" in config and config["format"].lower() not in FORMAT_CHOICES:
-        raise ValueError(_("'format' is not one of {}").format(FORMAT_CHOICES))
-    return True
 
 
 def _config_profile_callback(ctx: click.Context, param: Any, value: Optional[str]) -> Optional[str]:
     if value is not None:
         ctx.meta[PROFILE_KEY] = value
     return value
 
@@ -39,64 +33,37 @@
     if ctx.default_map:
         return
 
     try:
         if value:
             config = toml.load(value)
         else:
-            default_config_path = os.path.join(click.utils.get_app_dir("pulp"), "settings.toml")
-
             try:
-                config = toml.load(default_config_path)
+                config = toml.load(CONFIG_LOCATION)
             except FileNotFoundError:
                 # No config, but also none requested
                 return
         profile: str = "cli"
         if PROFILE_KEY in ctx.meta:
             profile = "cli-" + ctx.meta[PROFILE_KEY]
         try:
-            _validate_config(config[profile])
+            validate_config(config[profile])
             ctx.default_map = config[profile]
         except KeyError:
             raise click.ClickException(
                 _("Profile named '{profile}' not found.").format(profile=profile)
             )
     except ValueError as e:
         if sys.stdout.isatty():
             click.echo(_("Config file failed to parse. ({}).").format(e), err=True)
             if click.confirm(_("Continue without config?")):
                 return
         raise click.ClickException(_("Aborted."))
 
 
-CONFIG_OPTIONS = [
-    click.option("--base-url", default="https://localhost", help=_("API base url")),
-    click.option("--username", help=_("Username on pulp server")),
-    click.option("--password", help=_("Password on pulp server")),
-    click.option("--cert", help=_("Path to client certificate")),
-    click.option(
-        "--key",
-        help=_("Path to client private key. Not required if client cert contains this."),
-    ),
-    click.option("--verify-ssl/--no-verify-ssl", default=True, help=_("Verify SSL connection")),
-    click.option(
-        "--format",
-        type=click.Choice(FORMAT_CHOICES, case_sensitive=False),
-        default="json",
-        help=_("Format of the response"),
-    ),
-]
-
-
-def config_options(command: Callable[..., Any]) -> Callable[..., Any]:
-    for option in reversed(CONFIG_OPTIONS):
-        command = option(command)
-    return command
-
-
 @click.group()
 @click.version_option(prog_name=_("pulp3 command line interface"))
 @click.option(
     "--profile",
     "-p",
     help=_("Config profile to use"),
     callback=_config_profile_callback,
@@ -120,17 +87,14 @@
 @click.option(
     "-b",
     "--background",
     is_flag=True,
     help=_("Start tasks in the background instead of awaiting them"),
 )
 @click.option("--refresh-api", is_flag=True, help=_("Invalidate cached API docs"))
-@click.option(
-    "--dry-run", is_flag=True, help=_("Trace commands without performing any unsafe HTTP calls")
-)
 @config_options
 @click.pass_context
 def main(
     ctx: click.Context,
     base_url: str,
     username: Optional[str],
     password: Optional[str],
@@ -158,14 +122,15 @@
         refresh_cache=refresh_api,
         safe_calls_only=dry_run,
         debug_callback=_debug_callback,
     )
     ctx.obj = PulpContext(api_kwargs=api_kwargs, format=format, background_tasks=background)
 
 
+main.add_command(config)
 main.add_command(debug)
 
 
 @main.command("shell")
 @click.pass_context
 def pulp_shell(ctx: click.Context) -> None:
     """Activate an interactive shell-mode"""
```

### Comparing `pulp-cli-0.8.0/pulpcore/cli/common/context.py` & `pulp-cli-0.9.0/pulpcore/cli/common/context.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,26 @@
 import datetime
 import gettext
 import json
 import sys
 import time
-from typing import IO, Any, ClassVar, Dict, List, NamedTuple, Optional, Set, Tuple, Type, Union
+from typing import (
+    IO,
+    Any,
+    ClassVar,
+    Dict,
+    List,
+    NamedTuple,
+    Optional,
+    Set,
+    Tuple,
+    Type,
+    Union,
+    overload,
+)
 
 import click
 import yaml
 from packaging.version import parse as parse_version
 from requests import HTTPError
 from urllib3.util import parse_url
 
@@ -34,15 +47,15 @@
 RepositoryVersionDefinition = Tuple[str, str, int]  # name, pulp_type, version
 
 
 class PluginRequirement(NamedTuple):
     name: str
     min: Optional[str] = None
     max: Optional[str] = None
-    feature: Optional[str] = _("this command")
+    feature: Optional[str] = None
 
 
 new_component_names_to_pre_3_11_names: Dict[str, str] = dict(
     ansible="pulp_ansible",
     container="pulp_container",
     core="pulpcore",
     deb="pulp_deb",
@@ -176,60 +189,106 @@
                     task = self.api.call("tasks_read", parameters={"task_href": task_href})
                 else:
                     raise NotImplementedError(f"Unknown task state: {task['state']}")
             raise click.ClickException("Task timed out")
         except KeyboardInterrupt:
             raise PulpNoWait(f"Task {task_href} sent to background.")
 
+    @overload
+    def has_plugin(
+        self,
+        plugin: str,
+        min_version: Optional[str] = None,
+        max_version: Optional[str] = None,
+    ) -> bool:
+        ...
+
+    @overload
+    def has_plugin(
+        self,
+        plugin: PluginRequirement,
+        min_version: None = None,
+        max_version: None = None,
+    ) -> bool:
+        ...
+
     def has_plugin(
-        self, name: str, min_version: Optional[str] = None, max_version: Optional[str] = None
+        self,
+        plugin: Union[PluginRequirement, str],
+        min_version: Optional[str] = None,
+        max_version: Optional[str] = None,
     ) -> bool:
+        if not isinstance(plugin, PluginRequirement):
+            plugin = PluginRequirement(plugin, min_version, max_version)
         if not self.component_versions:
             # Prior to 3.9 we do not have this information
             # assume yes if no version constraint is specified
-            return (min_version is None) and (max_version is None)
-        version: Optional[str] = self.component_versions.get(name)
+            return (plugin.min is None) and (plugin.max is None)
+        version: Optional[str] = self.component_versions.get(plugin.name)
         if version is None:
-            pre_3_11_name: str = new_component_names_to_pre_3_11_names.get(name, "")
+            pre_3_11_name: str = new_component_names_to_pre_3_11_names.get(plugin.name, "")
             version = self.component_versions.get(pre_3_11_name)
             if version is None:
                 return False
-        if min_version is not None:
-            if parse_version(version) < parse_version(min_version):
+        if plugin.min is not None:
+            if parse_version(version) < parse_version(plugin.min):
                 return False
-        if max_version is not None:
-            if parse_version(version) >= parse_version(max_version):
+        if plugin.max is not None:
+            if parse_version(version) >= parse_version(plugin.max):
                 return False
         return True
 
+    @overload
+    def needs_plugin(
+        self,
+        plugin: str,
+        min_version: Optional[str] = None,
+        max_version: Optional[str] = None,
+        feature: Optional[str] = None,
+    ) -> None:
+        ...
+
+    @overload
+    def needs_plugin(
+        self,
+        plugin: PluginRequirement,
+        min_version: None = None,
+        max_version: None = None,
+        feature: None = None,
+    ) -> None:
+        ...
+
     def needs_plugin(
         self,
-        name: str,
+        plugin: Union[PluginRequirement, str],
         min_version: Optional[str] = None,
         max_version: Optional[str] = None,
-        feature: Optional[str] = _("this command"),
+        feature: Optional[str] = None,
     ) -> None:
+        if not isinstance(plugin, PluginRequirement):
+            plugin = PluginRequirement(plugin, min_version, max_version, feature)
         if self._api is not None:
-            if not self.has_plugin(name, min_version, max_version):
-                specifier = name
+            if not self.has_plugin(plugin):
+                specifier = plugin.name
                 separator = ""
-                if min_version is not None:
-                    specifier += f">={min_version}"
+                if plugin.min is not None:
+                    specifier += f">={plugin.min}"
                     separator = ","
-                if max_version is not None:
-                    specifier += f"{separator}<{max_version}"
+                if plugin.max is not None:
+                    specifier += f"{separator}<{plugin.max}"
+                feature = plugin.feature or _("this command")
                 raise click.ClickException(
                     _(
                         "The server does not have '{specifier}' installed,"
                         " which is needed to use {feature}."
                     ).format(specifier=specifier, feature=feature)
                 )
         else:
             # Schedule for later checking
-            self._needed_plugins.append(PluginRequirement(name, min_version, max_version, feature))
+            self._needed_plugins.append(plugin)
 
 
 class PulpEntityContext:
     """
     Base class for entity specific contexts.
     This class provides the basic CRUD commands and ties its instances to the global
     PulpContext for api access.
```

### Comparing `pulp-cli-0.8.0/pulpcore/cli/common/debug.py` & `pulp-cli-0.9.0/pulpcore/cli/common/debug.py`

 * *Files identical despite different names*

### Comparing `pulp-cli-0.8.0/pulpcore/cli/common/generic.py` & `pulp-cli-0.9.0/pulpcore/cli/common/generic.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,35 +37,35 @@
         super().format_help_text(ctx, formatter)
 
 
 class PulpOption(click.Option):
     def __init__(
         self,
         *args: Any,
-        needs_plugin: Optional[str] = None,
-        min_version: Optional[str] = None,
-        max_version: Optional[str] = None,
+        needs_plugins: Optional[List[PluginRequirement]] = None,
         **kwargs: Any,
     ):
-        if min_version or max_version:
-            assert needs_plugin, "Must supply required_version if min or max_version supplied."
-        self.needs_plugin = needs_plugin
-        self.min_version = min_version
-        self.max_version = max_version
+        self.needs_plugins = needs_plugins
         super().__init__(*args, **kwargs)
 
     def process_value(self, ctx: click.Context, value: Any) -> Any:
-        if value is not None and self.needs_plugin:
+        if value is not None and self.needs_plugins:
             pulp_ctx = ctx.find_object(PulpContext)
-            pulp_ctx.needs_plugin(
-                self.needs_plugin,
-                self.min_version,
-                self.max_version,
-                _("the {name} option").format(name=self.name),
-            )
+            for plugin_requirement in self.needs_plugins:
+                if plugin_requirement.feature:
+                    feature = plugin_requirement.feature
+                else:
+                    feature = _("the {name} option").format(name=self.name)
+
+                pulp_ctx.needs_plugin(
+                    plugin_requirement.name,
+                    plugin_requirement.min,
+                    plugin_requirement.max,
+                    feature,
+                )
         return super().process_value(ctx, value)
 
     def get_help_record(self, ctx: click.Context) -> Tuple[str, str]:
         synopsis, help_text = super().get_help_record(ctx)
         entity_ctx: PulpEntityContext = ctx.find_object(PulpEntityContext)
         help_text = help_text.format(entity=entity_ctx.ENTITY, entities=entity_ctx.ENTITIES)
         return synopsis, help_text
@@ -139,31 +139,32 @@
 
 def _version_callback(
     ctx: click.Context, param: click.Parameter, value: Optional[int]
 ) -> Optional[int]:
     entity_ctx: PulpEntityContext = ctx.find_object(PulpEntityContext)
     repository_ctx: PulpRepositoryContext = ctx.find_object(PulpRepositoryContext)
     if value is not None:
-        entity_ctx.pulp_href = repository_ctx.entity["versions_href"] + str(value)
+        entity_ctx.pulp_href = f"{repository_ctx.entity['versions_href']}{value}/"
     else:
         entity_ctx.pulp_href = repository_ctx.entity["latest_version_href"]
     return value
 
 
 def load_json_callback(
     ctx: click.Context,
     param: click.Parameter,
     value: Optional[str],
 ) -> Any:
     """Load JSON from input string or from file if string starts with @."""
     json_object: Any
     json_string: Union[str, bytes]
 
-    if value is None:
-        return None
+    # pass None and "" verbatim
+    if not value:
+        return value
 
     if value.startswith("@"):
         json_file = value[1:]
         try:
             with click.open_file(json_file, "rb") as fp:
                 json_string = fp.read()
         except OSError:
```

### Comparing `pulp-cli-0.8.0/pulpcore/cli/common/openapi.py` & `pulp-cli-0.9.0/pulpcore/cli/common/openapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,15 @@
             self._session.cert = (cert, key)
         elif cert:
             self._session.cert = cert
         elif key:
             raise OpenAPIError("Cert is required if key is set.")
         self._session.headers.update(headers)
         self._session.verify = validate_certs
+        self._session.max_redirects = 0
 
         self.load_api(refresh_cache=refresh_cache)
 
     def load_api(self, refresh_cache: bool = False) -> None:
         # TODO: Find a way to invalidate caches on upstream change
         xdg_cache_home: str = os.environ.get("XDG_CACHE_HOME") or "~/.cache"
         apidoc_cache: str = os.path.join(
@@ -215,15 +216,23 @@
         if response.status_code == 204:
             return "{}"
 
         try:
             response_spec = method_spec["responses"][str(response.status_code)]
         except KeyError:
             # Fallback 201 -> 200
-            response_spec = method_spec["responses"][str(100 * int(response.status_code / 100))]
+            try:
+                response_spec = method_spec["responses"][str(100 * int(response.status_code / 100))]
+            except KeyError:
+                raise OpenAPIError(
+                    _("Unexpected response '{code}' (expected '{expected}').").format(
+                        code=response.status_code,
+                        expected=(", ").join(method_spec["responses"].keys()),
+                    )
+                )
         if "application/json" in response_spec["content"]:
             return response.json()
         return None
 
     def call(
         self,
         operation_id: str,
@@ -273,12 +282,18 @@
             raise OpenAPIError("Call aborted due to safe mode")
         try:
             response: requests.Response = self._session.request(
                 method, url, data=data, headers=headers
             )
         except requests.ConnectionError as e:
             raise OpenAPIError(str(e))
+        except requests.exceptions.TooManyRedirects as e:
+            raise OpenAPIError(
+                _("Received redirect to '{url}'. Please check your CLI configuration.").format(
+                    url=e.response.headers["location"]
+                )
+            )
         self.debug_callback(1, f"Response: {response.status_code}")
         if response.text:
             self.debug_callback(3, f"{response.text}")
         response.raise_for_status()
         return self.parse_response(method_spec, response)
```

### Comparing `pulp-cli-0.8.0/pulpcore/cli/container/__init__.py` & `pulp-cli-0.9.0/pulpcore/cli/container/__init__.py`

 * *Files identical despite different names*

### Comparing `pulp-cli-0.8.0/pulpcore/cli/container/context.py` & `pulp-cli-0.9.0/pulpcore/cli/container/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,15 @@
     ENTITY = "container remote"
     ENTITIES = "container remotes"
     HREF = "container_container_remote_href"
     LIST_ID = "remotes_container_container_list"
     CREATE_ID = "remotes_container_container_create"
     UPDATE_ID = "remotes_container_container_partial_update"
     DELETE_ID = "remotes_container_container_delete"
+    NULLABLES = PulpRemoteContext.NULLABLES | {"include_tags", "exclude_tags"}
 
 
 class PulpContainerRepositoryVersionContext(PulpRepositoryVersionContext):
     HREF = "container_container_repository_version_href"
     REPOSITORY_HREF = "container_container_repository_href"
     LIST_ID = "repositories_container_container_versions_list"
     READ_ID = "repositories_container_container_versions_read"
```

### Comparing `pulp-cli-0.8.0/pulpcore/cli/container/distribution.py` & `pulp-cli-0.9.0/pulpcore/cli/container/distribution.py`

 * *Files identical despite different names*

### Comparing `pulp-cli-0.8.0/pulpcore/cli/container/namespace.py` & `pulp-cli-0.9.0/pulpcore/cli/container/namespace.py`

 * *Files identical despite different names*

### Comparing `pulp-cli-0.8.0/pulpcore/cli/container/remote.py` & `pulp-cli-0.9.0/pulpcore/cli/file/remote.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,42 +12,44 @@
     label_command,
     label_select_option,
     list_command,
     name_option,
     show_command,
     update_command,
 )
-from pulpcore.cli.container.context import PulpContainerRemoteContext
+from pulpcore.cli.file.context import PulpFileRemoteContext
 
 _ = gettext.gettext
 
 
 @click.group()
 @click.option(
     "-t",
     "--type",
     "remote_type",
-    type=click.Choice(["container"], case_sensitive=False),
-    default="container",
+    type=click.Choice(["file"], case_sensitive=False),
+    default="file",
 )
 @pass_pulp_context
 @click.pass_context
 def remote(ctx: click.Context, pulp_ctx: PulpContext, remote_type: str) -> None:
-    if remote_type == "container":
-        ctx.obj = PulpContainerRemoteContext(pulp_ctx)
+    if remote_type == "file":
+        ctx.obj = PulpFileRemoteContext(pulp_ctx)
     else:
         raise NotImplementedError()
 
 
 lookup_options = [href_option, name_option]
-remote_options = [
-    click.option("--upstream-name", required=True),
+file_remote_options = [
+    click.option(
+        "--policy", type=click.Choice(["immediate", "on_demand", "streamed"], case_sensitive=False)
+    ),
 ]
 
 remote.add_command(list_command(decorators=[label_select_option]))
 remote.add_command(show_command(decorators=lookup_options))
-remote.add_command(create_command(decorators=common_remote_create_options + remote_options))
+remote.add_command(create_command(decorators=common_remote_create_options + file_remote_options))
 remote.add_command(
-    update_command(decorators=lookup_options + common_remote_update_options + remote_options)
+    update_command(decorators=lookup_options + common_remote_update_options + file_remote_options)
 )
 remote.add_command(destroy_command(decorators=lookup_options))
 remote.add_command(label_command())
```

### Comparing `pulp-cli-0.8.0/pulpcore/cli/container/repository.py` & `pulp-cli-0.9.0/pulpcore/cli/container/repository.py`

 * *Files identical despite different names*

### Comparing `pulp-cli-0.8.0/pulpcore/cli/core/__init__.py` & `pulp-cli-0.9.0/pulpcore/cli/core/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import gettext
 
 from pulpcore.cli.common import main
 from pulpcore.cli.core.access_policy import access_policy
 from pulpcore.cli.core.artifact import artifact
-from pulpcore.cli.core.config import config
 from pulpcore.cli.core.export import export
 from pulpcore.cli.core.exporter import exporter
 from pulpcore.cli.core.group import group
 from pulpcore.cli.core.importer import importer
 from pulpcore.cli.core.orphans import orphans
 from pulpcore.cli.core.repository import repository
 from pulpcore.cli.core.show import show
@@ -19,15 +18,14 @@
 from pulpcore.cli.core.worker import worker
 
 _ = gettext.gettext
 
 # Register commands with cli
 main.add_command(access_policy)
 main.add_command(artifact)
-main.add_command(config)
 main.add_command(export)
 main.add_command(exporter)
 main.add_command(group)
 main.add_command(importer)
 main.add_command(orphans)
 main.add_command(repository)
 main.add_command(show)
```

### Comparing `pulp-cli-0.8.0/pulpcore/cli/core/access_policy.py` & `pulp-cli-0.9.0/pulpcore/cli/core/access_policy.py`

 * *Files identical despite different names*

### Comparing `pulp-cli-0.8.0/pulpcore/cli/core/artifact.py` & `pulp-cli-0.9.0/pulpcore/cli/core/artifact.py`

 * *Files identical despite different names*

### Comparing `pulp-cli-0.8.0/pulpcore/cli/core/context.py` & `pulp-cli-0.9.0/pulpcore/cli/core/context.py`

 * *Files identical despite different names*

### Comparing `pulp-cli-0.8.0/pulpcore/cli/core/export.py` & `pulp-cli-0.9.0/pulpcore/cli/core/export.py`

 * *Files identical despite different names*

### Comparing `pulp-cli-0.8.0/pulpcore/cli/core/exporter.py` & `pulp-cli-0.9.0/pulpcore/cli/core/exporter.py`

 * *Files identical despite different names*

### Comparing `pulp-cli-0.8.0/pulpcore/cli/core/generic.py` & `pulp-cli-0.9.0/pulpcore/cli/core/generic.py`

 * *Files identical despite different names*

### Comparing `pulp-cli-0.8.0/pulpcore/cli/core/group.py` & `pulp-cli-0.9.0/pulpcore/cli/core/group.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,9 +153,9 @@
 @groupname_option
 @click.option("--username", required=True)
 @pass_entity_context
 @pass_pulp_context
 def remove_user(pulp_ctx: PulpContext, entity_ctx: PulpGroupUserContext, username: str) -> None:
     user_href = PulpUserContext(pulp_ctx).find(username=username)["pulp_href"]
     user_pk = user_href.split("/")[-2]
-    group_user_href = entity_ctx.group_ctx.pulp_href + "users/" + user_pk
+    group_user_href = f"{entity_ctx.group_ctx.pulp_href}users/{user_pk}/"
     entity_ctx.delete(group_user_href)
```

### Comparing `pulp-cli-0.8.0/pulpcore/cli/core/importer.py` & `pulp-cli-0.9.0/pulpcore/cli/core/importer.py`

 * *Files identical despite different names*

### Comparing `pulp-cli-0.8.0/pulpcore/cli/core/repository.py` & `pulp-cli-0.9.0/pulpcore/cli/core/repository.py`

 * *Files identical despite different names*

### Comparing `pulp-cli-0.8.0/pulpcore/cli/core/signing_service.py` & `pulp-cli-0.9.0/pulpcore/cli/core/signing_service.py`

 * *Files identical despite different names*

### Comparing `pulp-cli-0.8.0/pulpcore/cli/core/status.py` & `pulp-cli-0.9.0/pulpcore/cli/core/status.py`

 * *Files identical despite different names*

### Comparing `pulp-cli-0.8.0/pulpcore/cli/core/task.py` & `pulp-cli-0.9.0/pulpcore/cli/core/task.py`

 * *Files identical despite different names*

### Comparing `pulp-cli-0.8.0/pulpcore/cli/core/task_group.py` & `pulp-cli-0.9.0/pulpcore/cli/core/task_group.py`

 * *Files identical despite different names*

### Comparing `pulp-cli-0.8.0/pulpcore/cli/core/user.py` & `pulp-cli-0.9.0/pulpcore/cli/core/user.py`

 * *Files identical despite different names*

### Comparing `pulp-cli-0.8.0/pulpcore/cli/core/worker.py` & `pulp-cli-0.9.0/pulpcore/cli/core/worker.py`

 * *Files identical despite different names*

### Comparing `pulp-cli-0.8.0/pulpcore/cli/file/__init__.py` & `pulp-cli-0.9.0/pulpcore/cli/file/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import gettext
 
 from pulpcore.cli.common import main
-from pulpcore.cli.common.context import PulpContext, pass_pulp_context
+from pulpcore.cli.common.context import PluginRequirement, PulpContext, pass_pulp_context
 from pulpcore.cli.file.content import content
 from pulpcore.cli.file.distribution import distribution
 from pulpcore.cli.file.publication import publication
 from pulpcore.cli.file.remote import remote
 from pulpcore.cli.file.repository import repository
 
 _ = gettext.gettext
 
 
 @main.group(name="file")
 @pass_pulp_context
 def file_group(pulp_ctx: PulpContext) -> None:
-    pulp_ctx.needs_plugin("file")
+    pulp_ctx.needs_plugin(PluginRequirement("file"))
 
 
 file_group.add_command(repository)
 file_group.add_command(remote)
 file_group.add_command(publication)
 file_group.add_command(distribution)
 file_group.add_command(content)
```

### Comparing `pulp-cli-0.8.0/pulpcore/cli/file/content.py` & `pulp-cli-0.9.0/pulpcore/cli/file/content.py`

 * *Files identical despite different names*

### Comparing `pulp-cli-0.8.0/pulpcore/cli/file/context.py` & `pulp-cli-0.9.0/pulpcore/cli/file/context.py`

 * *Files identical despite different names*

### Comparing `pulp-cli-0.8.0/pulpcore/cli/file/distribution.py` & `pulp-cli-0.9.0/pulpcore/cli/file/distribution.py`

 * *Files identical despite different names*

### Comparing `pulp-cli-0.8.0/pulpcore/cli/file/publication.py` & `pulp-cli-0.9.0/pulpcore/cli/file/publication.py`

 * *Files identical despite different names*

### Comparing `pulp-cli-0.8.0/pulpcore/cli/file/remote.py` & `pulp-cli-0.9.0/pulpcore/cli/rpm/remote.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,44 +12,44 @@
     label_command,
     label_select_option,
     list_command,
     name_option,
     show_command,
     update_command,
 )
-from pulpcore.cli.file.context import PulpFileRemoteContext
+from pulpcore.cli.rpm.context import PulpRpmRemoteContext
 
 _ = gettext.gettext
 
 
 @click.group()
 @click.option(
     "-t",
     "--type",
     "remote_type",
-    type=click.Choice(["file"], case_sensitive=False),
-    default="file",
+    type=click.Choice(["rpm"], case_sensitive=False),
+    default="rpm",
 )
 @pass_pulp_context
 @click.pass_context
 def remote(ctx: click.Context, pulp_ctx: PulpContext, remote_type: str) -> None:
-    if remote_type == "file":
-        ctx.obj = PulpFileRemoteContext(pulp_ctx)
+    if remote_type == "rpm":
+        ctx.obj = PulpRpmRemoteContext(pulp_ctx)
     else:
         raise NotImplementedError()
 
 
 lookup_options = [href_option, name_option]
-file_remote_options = [
+rpm_remote_options = [
     click.option(
         "--policy", type=click.Choice(["immediate", "on_demand", "streamed"], case_sensitive=False)
     ),
 ]
 
 remote.add_command(list_command(decorators=[label_select_option]))
 remote.add_command(show_command(decorators=lookup_options))
-remote.add_command(create_command(decorators=common_remote_create_options + file_remote_options))
+remote.add_command(create_command(decorators=common_remote_create_options + rpm_remote_options))
 remote.add_command(
-    update_command(decorators=lookup_options + common_remote_update_options + file_remote_options)
+    update_command(decorators=lookup_options + common_remote_update_options + rpm_remote_options)
 )
 remote.add_command(destroy_command(decorators=lookup_options))
 remote.add_command(label_command())
```

### Comparing `pulp-cli-0.8.0/pulpcore/cli/file/repository.py` & `pulp-cli-0.9.0/pulpcore/cli/file/repository.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import gettext
 from typing import Any, Dict, List, Optional, Union
 
 import click
 
 from pulpcore.cli.common.context import (
+    PluginRequirement,
     PulpContext,
     PulpEntityContext,
     PulpRepositoryContext,
     pass_pulp_context,
     pass_repository_context,
 )
 from pulpcore.cli.common.generic import (
@@ -76,17 +77,19 @@
 lookup_options = [href_option, name_option]
 nested_lookup_options = [repository_href_option, repository_option]
 update_options = [
     click.option("--description"),
     click.option("--remote", callback=_remote_callback),
     click.option("--manifest"),
     pulp_option(
-        "--autopublish/--no-autopublish", needs_plugin="file", min_version="1.7.0", default=None
+        "--autopublish/--no-autopublish",
+        needs_plugins=[PluginRequirement("file", "1.7.0")],
+        default=None,
     ),
-    pulp_option("--retained-versions", needs_plugin="core", min_version="3.13.0.dev"),
+    pulp_option("--retained-versions", needs_plugins=[PluginRequirement("core", "3.13.0.dev")]),
 ]
 create_options = update_options + [
     click.option("--name", required=True),
 ]
 file_options = [
     click.option("--sha256", cls=GroupOption, expose_value=False, group=["relative_path"]),
     click.option(
```

### Comparing `pulp-cli-0.8.0/pulpcore/cli/migration/context.py` & `pulp-cli-0.9.0/pulpcore/cli/migration/context.py`

 * *Files identical despite different names*

### Comparing `pulp-cli-0.8.0/pulpcore/cli/migration/plan.py` & `pulp-cli-0.9.0/pulpcore/cli/migration/plan.py`

 * *Files identical despite different names*

### Comparing `pulp-cli-0.8.0/pulpcore/cli/migration/pulp2.py` & `pulp-cli-0.9.0/pulpcore/cli/migration/pulp2.py`

 * *Files identical despite different names*

### Comparing `pulp-cli-0.8.0/pulpcore/cli/python/__init__.py` & `pulp-cli-0.9.0/pulpcore/cli/python/__init__.py`

 * *Files identical despite different names*

### Comparing `pulp-cli-0.8.0/pulpcore/cli/python/content.py` & `pulp-cli-0.9.0/pulpcore/cli/python/content.py`

 * *Files identical despite different names*

### Comparing `pulp-cli-0.8.0/pulpcore/cli/python/context.py` & `pulp-cli-0.9.0/pulpcore/cli/python/context.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import ClassVar
 
 from pulpcore.cli.common.context import (
     EntityDefinition,
-    PluginRequirement,
     PulpContentContext,
     PulpEntityContext,
     PulpRemoteContext,
     PulpRepositoryContext,
     PulpRepositoryVersionContext,
 )
 
@@ -25,15 +24,15 @@
     ENTITIES = "python distributions"
     HREF = "python_python_distribution_href"
     LIST_ID = "distributions_python_pypi_list"
     READ_ID = "distributions_python_pypi_read"
     CREATE_ID = "distributions_python_pypi_create"
     UPDATE_ID = "distributions_python_pypi_partial_update"
     DELETE_ID = "distributions_python_pypi_delete"
-    NULLABLES = {"publication"}
+    NULLABLES = {"publication", "repository"}
 
 
 class PulpPythonPublicationContext(PulpEntityContext):
     ENTITY = "python publication"
     ENTITIES = "python publications"
     HREF = "python_python_publication_href"
     LIST_ID = "publications_python_pypi_list"
@@ -55,27 +54,14 @@
     ENTITIES = "python remotes"
     HREF = "python_python_remote_href"
     LIST_ID = "remotes_python_python_list"
     CREATE_ID = "remotes_python_python_create"
     BANDERSNATCH_ID: ClassVar[str] = "remotes_python_python_from_bandersnatch"
     UPDATE_ID = "remotes_python_python_partial_update"
     DELETE_ID = "remotes_python_python_delete"
-    field_versions = {
-        "keep_latest_packages": [PluginRequirement("python", "3.2.0")],
-        "exclude_platforms": [PluginRequirement("python", "3.2.0")],
-        "package_types": [PluginRequirement("python", "3.2.0")],
-    }
-
-    def preprocess_body(self, body: EntityDefinition) -> EntityDefinition:
-        body = super().preprocess_body(body)
-        for field in body.keys():
-            if field in self.field_versions:
-                for item in self.field_versions[field]:
-                    self.pulp_ctx.needs_plugin(*item)
-        return body
 
 
 class PulpPythonRepositoryVersionContext(PulpRepositoryVersionContext):
     HREF = "python_python_repository_version_href"
     REPOSITORY_HREF = "python_python_repository_href"
     LIST_ID = "repositories_python_python_versions_list"
     READ_ID = "repositories_python_python_versions_read"
```

### Comparing `pulp-cli-0.8.0/pulpcore/cli/python/distribution.py` & `pulp-cli-0.9.0/pulpcore/cli/rpm/publication.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,57 @@
+import gettext
+from typing import Optional, Union
+
 import click
 
-from pulpcore.cli.common.context import PulpContext, pass_pulp_context
+from pulpcore.cli.common.context import PulpContext, PulpEntityContext, pass_pulp_context
 from pulpcore.cli.common.generic import (
-    base_path_contains_option,
-    base_path_option,
     create_command,
     destroy_command,
     href_option,
-    label_command,
-    label_select_option,
     list_command,
-    name_option,
     show_command,
-    update_command,
 )
-from pulpcore.cli.python.context import PulpPythonDistributionContext
+from pulpcore.cli.rpm.context import PulpRpmPublicationContext, PulpRpmRepositoryContext
+
+_ = gettext.gettext
+
+
+def _repository_callback(
+    ctx: click.Context, param: click.Parameter, value: Optional[str]
+) -> Optional[Union[str, PulpEntityContext]]:
+    # Pass None and "" verbatim
+    if value:
+        pulp_ctx: PulpContext = ctx.find_object(PulpContext)
+        return PulpRpmRepositoryContext(pulp_ctx, entity={"name": value})
+    return value
 
 
 @click.group()
 @click.option(
     "-t",
     "--type",
-    "distribution_type",
-    type=click.Choice(["python"], case_sensitive=False),
-    default="python",
+    "publication_type",
+    type=click.Choice(["rpm"], case_sensitive=False),
+    default="rpm",
 )
 @pass_pulp_context
 @click.pass_context
-def distribution(ctx: click.Context, pulp_ctx: PulpContext, distribution_type: str) -> None:
-    if distribution_type == "python":
-        ctx.obj = PulpPythonDistributionContext(pulp_ctx)
+def publication(ctx: click.Context, pulp_ctx: PulpContext, publication_type: str) -> None:
+    if publication_type == "rpm":
+        ctx.obj = PulpRpmPublicationContext(pulp_ctx)
     else:
         raise NotImplementedError()
 
 
-filter_options = [label_select_option, base_path_option, base_path_contains_option]
-lookup_options = [href_option, name_option]
+lookup_options = [href_option]
 create_options = [
-    click.option("--name", required=True),
-    click.option("--base-path", required=True),
-    click.option("--publication"),
-]
-update_options = [
-    click.option("--base-path"),
-    click.option("--publication"),
+    click.option("--repository", required=True, callback=_repository_callback),
+    click.option(
+        "--version", type=int, help=_("a repository version number, leave blank for latest")
+    ),
 ]
 
-distribution.add_command(list_command(decorators=filter_options))
-distribution.add_command(show_command(decorators=lookup_options))
-distribution.add_command(destroy_command(decorators=lookup_options))
-distribution.add_command(create_command(decorators=create_options))
-distribution.add_command(update_command(decorators=lookup_options + update_options))
-distribution.add_command(label_command())
+publication.add_command(list_command())
+publication.add_command(show_command(decorators=lookup_options))
+publication.add_command(create_command(decorators=create_options))
+publication.add_command(destroy_command(decorators=lookup_options))
```

### Comparing `pulp-cli-0.8.0/pulpcore/cli/python/publication.py` & `pulp-cli-0.9.0/pulpcore/cli/python/publication.py`

 * *Files identical despite different names*

### Comparing `pulp-cli-0.8.0/pulpcore/cli/python/remote.py` & `pulp-cli-0.9.0/pulpcore/cli/python/remote.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import gettext
 
 import click
 
-from pulpcore.cli.common.context import PulpContext, pass_pulp_context
+from pulpcore.cli.common.context import PluginRequirement, PulpContext, pass_pulp_context
 from pulpcore.cli.common.generic import (
     common_remote_create_options,
     common_remote_update_options,
     create_command,
     destroy_command,
     href_option,
     label_command,
     label_select_option,
     list_command,
     load_json_callback,
     name_option,
+    pulp_option,
     show_command,
     update_command,
 )
 from pulpcore.cli.python.context import PulpPythonRemoteContext
 
 _ = gettext.gettext
 
@@ -37,20 +38,33 @@
         ctx.obj = PulpPythonRemoteContext(pulp_ctx)
     else:
         raise NotImplementedError()
 
 
 lookup_options = [href_option, name_option]
 python_remote_options = [
+    click.option(
+        "--policy", type=click.Choice(["immediate", "on_demand", "streamed"], case_sensitive=False)
+    ),
     click.option("--includes", callback=load_json_callback, help=_("Package allowlist")),
     click.option("--excludes", callback=load_json_callback, help=_("Package blocklist")),
     click.option("--prereleases", type=click.BOOL, default=True),
-    click.option("--keep-latest-packages", type=int),
-    click.option("--package-types", callback=load_json_callback),
-    click.option("--exclude-platforms", callback=load_json_callback),
+    pulp_option(
+        "--keep-latest-packages", type=int, needs_plugins=[PluginRequirement("python", "3.2.0")]
+    ),
+    pulp_option(
+        "--package-types",
+        callback=load_json_callback,
+        needs_plugins=[PluginRequirement("python", "3.2.0")],
+    ),
+    pulp_option(
+        "--exclude-platforms",
+        callback=load_json_callback,
+        needs_plugins=[PluginRequirement("python", "3.2.0")],
+    ),
 ]
 remote.add_command(list_command(decorators=[label_select_option]))
 remote.add_command(show_command(decorators=lookup_options))
 remote.add_command(destroy_command(decorators=lookup_options))
 remote.add_command(create_command(decorators=common_remote_create_options + python_remote_options))
 remote.add_command(
     update_command(decorators=lookup_options + common_remote_update_options + python_remote_options)
```

### Comparing `pulp-cli-0.8.0/pulpcore/cli/python/repository.py` & `pulp-cli-0.9.0/pulpcore/cli/python/repository.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from gettext import gettext
 from typing import Optional, Union
 
 import click
 
 from pulpcore.cli.common.context import (
+    PluginRequirement,
     PulpContext,
     PulpEntityContext,
     PulpRepositoryContext,
     pass_pulp_context,
     pass_repository_context,
 )
 from pulpcore.cli.common.generic import (
@@ -67,25 +68,25 @@
     if repo_type == "python":
         ctx.obj = PulpPythonRepositoryContext(pulp_ctx)
     else:
         raise NotImplementedError()
 
 
 lookup_options = [href_option, name_option]
-create_options = [
-    click.option("--name", required=True),
-    click.option("--description"),
-    click.option("--remote", callback=_remote_callback),
-    pulp_option("--retained-versions", needs_plugin="core", min_version="3.13.0.dev"),
-]
 update_options = [
     click.option("--description"),
     click.option("--remote", callback=_remote_callback),
-    pulp_option("--retained-versions", needs_plugin="core", min_version="3.13.0.dev"),
+    pulp_option("--retained-versions", needs_plugins=[PluginRequirement("core", "3.13.0.dev")]),
+    pulp_option(
+        "--autopublish/--no-autopublish",
+        needs_plugins=[PluginRequirement("python", "3.3.0.dev")],
+        default=None,
+    ),
 ]
+create_options = [click.option("--name", required=True)] + update_options
 package_option = click.option(
     "--filename",
     callback=_content_callback,
     expose_value=False,
     help=_("Filename of the python package"),
 )
 content_json_callback = create_content_json_callback(PulpPythonContentContext)
```

### Comparing `pulp-cli-0.8.0/pulpcore/cli/rpm/__init__.py` & `pulp-cli-0.9.0/pulpcore/cli/rpm/__init__.py`

 * *Files identical despite different names*

### Comparing `pulp-cli-0.8.0/pulpcore/cli/rpm/context.py` & `pulp-cli-0.9.0/pulpcore/cli/rpm/context.py`

 * *Files identical despite different names*

### Comparing `pulp-cli-0.8.0/pulpcore/cli/rpm/distribution.py` & `pulp-cli-0.9.0/pulpcore/cli/rpm/distribution.py`

 * *Files identical despite different names*

### Comparing `pulp-cli-0.8.0/pulpcore/cli/rpm/publication.py` & `pulp-cli-0.9.0/pulpcore/cli/rpm/repository.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,57 +1,124 @@
 import gettext
-from typing import Optional, Union
+from typing import Any, Dict, Optional, Union
 
 import click
 
-from pulpcore.cli.common.context import PulpContext, PulpEntityContext, pass_pulp_context
+from pulpcore.cli.common.context import (
+    PluginRequirement,
+    PulpContext,
+    PulpEntityContext,
+    PulpRepositoryContext,
+    pass_pulp_context,
+    pass_repository_context,
+)
 from pulpcore.cli.common.generic import (
     create_command,
     destroy_command,
     href_option,
+    label_command,
+    label_select_option,
     list_command,
+    name_option,
+    pulp_option,
     show_command,
+    update_command,
+    version_command,
 )
-from pulpcore.cli.rpm.context import PulpRpmPublicationContext, PulpRpmRepositoryContext
+from pulpcore.cli.rpm.common import CHECKSUM_CHOICES
+from pulpcore.cli.rpm.context import PulpRpmRemoteContext, PulpRpmRepositoryContext
 
 _ = gettext.gettext
 
 
-def _repository_callback(
+def _remote_callback(
     ctx: click.Context, param: click.Parameter, value: Optional[str]
 ) -> Optional[Union[str, PulpEntityContext]]:
     # Pass None and "" verbatim
     if value:
         pulp_ctx: PulpContext = ctx.find_object(PulpContext)
-        return PulpRpmRepositoryContext(pulp_ctx, entity={"name": value})
+        return PulpRpmRemoteContext(pulp_ctx, entity={"name": value})
     return value
 
 
 @click.group()
 @click.option(
     "-t",
     "--type",
-    "publication_type",
+    "repo_type",
     type=click.Choice(["rpm"], case_sensitive=False),
     default="rpm",
 )
 @pass_pulp_context
 @click.pass_context
-def publication(ctx: click.Context, pulp_ctx: PulpContext, publication_type: str) -> None:
-    if publication_type == "rpm":
-        ctx.obj = PulpRpmPublicationContext(pulp_ctx)
+def repository(ctx: click.Context, pulp_ctx: PulpContext, repo_type: str) -> None:
+    if repo_type == "rpm":
+        ctx.obj = PulpRpmRepositoryContext(pulp_ctx)
     else:
         raise NotImplementedError()
 
 
-lookup_options = [href_option]
-create_options = [
-    click.option("--repository", required=True, callback=_repository_callback),
+lookup_options = [href_option, name_option]
+update_options = [
+    click.option("--description"),
+    click.option("--retain-package-versions", type=int),
+    click.option("--remote", callback=_remote_callback),
+    click.option(
+        "--metadata-checksum-type", type=click.Choice(CHECKSUM_CHOICES, case_sensitive=False)
+    ),
     click.option(
-        "--version", type=int, help=_("a repository version number, leave blank for latest")
+        "--package-checksum-type", type=click.Choice(CHECKSUM_CHOICES, case_sensitive=False)
     ),
+    click.option("--gpgcheck", type=click.Choice(("0", "1"))),
+    click.option("--repo-gpgcheck", type=click.Choice(("0", "1"))),
+    click.option("--sqlite-metadata/--no-sqlite-metadata", default=None),
+    pulp_option(
+        "--autopublish/--no-autopublish",
+        needs_plugins=[PluginRequirement("rpm", "3.11.0.dev")],
+        default=None,
+    ),
+    pulp_option("--retained-versions", needs_plugins=[PluginRequirement("core", "3.13.0.dev")]),
 ]
+create_options = update_options + [click.option("--name", required=True)]
 
-publication.add_command(list_command())
-publication.add_command(show_command(decorators=lookup_options))
-publication.add_command(create_command(decorators=create_options))
-publication.add_command(destroy_command(decorators=lookup_options))
+repository.add_command(list_command(decorators=[label_select_option]))
+repository.add_command(show_command(decorators=lookup_options))
+repository.add_command(create_command(decorators=create_options))
+repository.add_command(update_command(decorators=lookup_options + update_options))
+repository.add_command(destroy_command(decorators=lookup_options))
+repository.add_command(version_command())
+repository.add_command(label_command())
+
+
+@repository.command()
+@click.option("--name", required=True)
+@click.option("--mirror/--no-mirror", default=None)
+@click.option("--remote")
+@pass_repository_context
+@pass_pulp_context
+def sync(
+    pulp_ctx: PulpContext,
+    repository_ctx: PulpRepositoryContext,
+    name: str,
+    remote: Optional[str],
+    mirror: Optional[bool],
+) -> None:
+    repository = repository_ctx.find(name=name)
+    repository_href = repository["pulp_href"]
+
+    body: Dict[str, Any] = {}
+
+    if mirror:
+        body["mirror"] = mirror
+
+    if remote:
+        remote_href: str = PulpRpmRemoteContext(pulp_ctx).find(name=remote)["pulp_href"]
+        body["remote"] = remote_href
+    elif repository["remote"] is None:
+        raise click.ClickException(
+            f"Repository '{name}' does not have a default remote. Please specify with '--remote'."
+        )
+
+    repository_ctx.sync(
+        href=repository_href,
+        body=body,
+    )
```

### Comparing `pulp-cli-0.8.0/pyproject.toml` & `pulp-cli-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pulp-cli-0.8.0/pytest_pulp_cli/__init__.py` & `pulp-cli-0.9.0/pytest_pulp_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `pulp-cli-0.8.0/setup.py` & `pulp-cli-0.9.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,25 +12,25 @@
 
 setup(
     name="pulp-cli",
     description="Command line interface to talk to pulpcore's REST API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pulp/pulp-cli",
-    version="0.8.0",
+    version="0.9.0",
     packages=packages,
     package_data={package: ["py.typed"] for package in packages},
     python_requires=">=3.6",
     install_requires=[
-        "click",
-        "click-shell",
+        "click<8.0.0",
+        "click-shell~=2.0",
         "packaging",
-        "PyYAML",
-        "requests",
-        "toml",
+        "PyYAML~=5.4.1",
+        "requests~=2.25.1",
+        "toml==0.10.2",
     ],
     extras_require={
         "pygments": ["pygments"],
     },
     entry_points={
         "console_scripts": "pulp=pulpcore.cli.common:main",
         "pulp_cli.plugins": [
```

