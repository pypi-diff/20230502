# Comparing `tmp/bemserver-core-0.9.0.tar.gz` & `tmp/bemserver-core-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bemserver-core-0.9.0.tar", last modified: Tue Feb  7 11:06:52 2023, max compression
+gzip compressed data, was "bemserver-core-0.9.1.tar", last modified: Wed Feb  8 15:16:04 2023, max compression
```

## Comparing `bemserver-core-0.9.0.tar` & `bemserver-core-0.9.1.tar`

### file list

```diff
@@ -1,108 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:06:52.312072 bemserver-core-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-02-07 11:06:52.312072 bemserver-core-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:06:52.304071 bemserver-core-0.9.0/bemserver_core/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/bemserver_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/bemserver_core/alembic.ini
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/bemserver_core/authorization.polar
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/bemserver_core/authorization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/bemserver_core/celery.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/bemserver_core/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:06:52.304071 bemserver-core-0.9.0/bemserver_core/common/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/bemserver_core/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/bemserver_core/common/property_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     8831 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/bemserver_core/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/bemserver_core/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:06:52.304071 bemserver-core-0.9.0/bemserver_core/input_output/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/bemserver_core/input_output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/bemserver_core/input_output/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10582 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/bemserver_core/input_output/sites_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    19727 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/bemserver_core/input_output/timeseries_data_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/bemserver_core/input_output/timeseries_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:06:52.304071 bemserver-core-0.9.0/bemserver_core/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/bemserver_core/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/bemserver_core/migrations/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/bemserver_core/migrations/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:06:52.308071 bemserver-core-0.9.0/bemserver_core/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (123)    35257 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/bemserver_core/migrations/versions/0.1_v0_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/bemserver_core/migrations/versions/0.3.1_v0_3.1.py
--rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/bemserver_core/migrations/versions/0.3_v0_3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/bemserver_core/migrations/versions/0.4_v0_4.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/bemserver_core/migrations/versions/0.6_v0_6.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/bemserver_core/migrations/versions/0.8_v0_8.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:06:52.308071 bemserver-core-0.9.0/bemserver_core/model/
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/bemserver_core/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12855 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/bemserver_core/model/authorization.polar
--rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/bemserver_core/model/campaigns.py
--rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/bemserver_core/model/energy.py
--rw-r--r--   0 runner    (1001) docker     (123)    23795 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/bemserver_core/model/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/bemserver_core/model/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)    18214 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/bemserver_core/model/sites.py
--rw-r--r--   0 runner    (1001) docker     (123)    22318 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/bemserver_core/model/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/bemserver_core/model/timeseries_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/bemserver_core/model/users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:06:52.308071 bemserver-core-0.9.0/bemserver_core/process/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/bemserver_core/process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/bemserver_core/process/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/bemserver_core/process/completeness.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/bemserver_core/process/energy_consumption.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:06:52.308071 bemserver-core-0.9.0/bemserver_core/scheduled_tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/bemserver_core/scheduled_tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/bemserver_core/scheduled_tasks/authorization.polar
--rw-r--r--   0 runner    (1001) docker     (123)    10205 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/bemserver_core/scheduled_tasks/check_missing.py
--rw-r--r--   0 runner    (1001) docker     (123)    10840 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/bemserver_core/scheduled_tasks/check_outliers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/bemserver_core/scheduled_tasks/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/bemserver_core/time_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/bemserver_core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:06:52.304071 bemserver-core-0.9.0/bemserver_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-02-07 11:06:52.000000 bemserver-core-0.9.0/bemserver_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-02-07 11:06:52.000000 bemserver-core-0.9.0/bemserver_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 11:06:52.000000 bemserver-core-0.9.0/bemserver_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-02-07 11:06:52.000000 bemserver-core-0.9.0/bemserver_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-02-07 11:06:52.000000 bemserver-core-0.9.0/bemserver_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-07 11:06:52.000000 bemserver-core-0.9.0/bemserver_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:06:52.308071 bemserver-core-0.9.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/requirements/install.txt
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/requirements/tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-02-07 11:06:52.316072 bemserver-core-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:06:52.312072 bemserver-core-0.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:06:52.312072 bemserver-core-0.9.0/tests/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/tests/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/tests/common/test_property_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    28412 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:06:52.312072 bemserver-core-0.9.0/tests/input_output/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/tests/input_output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28052 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/tests/input_output/test_sites_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    91107 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/tests/input_output/test_timeseries_data_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    10180 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/tests/input_output/test_timeseries_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:06:52.312072 bemserver-core-0.9.0/tests/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/tests/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12029 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/tests/model/test_campaigns.py
--rw-r--r--   0 runner    (1001) docker     (123)     9244 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/tests/model/test_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)    41613 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/tests/model/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)    12157 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/tests/model/test_notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)    68629 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/tests/model/test_sites.py
--rw-r--r--   0 runner    (1001) docker     (123)    43567 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/tests/model/test_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)     8820 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/tests/model/test_users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:06:52.312072 bemserver-core-0.9.0/tests/process/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/tests/process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/tests/process/test_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)    15889 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/tests/process/test_completeness.py
--rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/tests/process/test_energy_consumption.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:06:52.312072 bemserver-core-0.9.0/tests/scheduled_tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/tests/scheduled_tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19586 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/tests/scheduled_tasks/test_check_missing.py
--rw-r--r--   0 runner    (1001) docker     (123)    20103 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/tests/scheduled_tasks/test_check_outliers.py
--rw-r--r--   0 runner    (1001) docker     (123)    22679 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/tests/scheduled_tasks/test_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/tests/test_authorization.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/tests/test_celery.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/tests/test_time_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-02-07 11:06:37.000000 bemserver-core-0.9.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:16:04.659967 bemserver-core-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-02-08 15:16:04.659967 bemserver-core-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:16:04.651967 bemserver-core-0.9.1/bemserver_core/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/bemserver_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/bemserver_core/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/bemserver_core/authorization.polar
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/bemserver_core/authorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/bemserver_core/celery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/bemserver_core/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:16:04.651967 bemserver-core-0.9.1/bemserver_core/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/bemserver_core/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/bemserver_core/common/property_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8831 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/bemserver_core/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/bemserver_core/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:16:04.651967 bemserver-core-0.9.1/bemserver_core/input_output/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/bemserver_core/input_output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/bemserver_core/input_output/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10582 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/bemserver_core/input_output/sites_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19727 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/bemserver_core/input_output/timeseries_data_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/bemserver_core/input_output/timeseries_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:16:04.651967 bemserver-core-0.9.1/bemserver_core/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/bemserver_core/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/bemserver_core/migrations/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/bemserver_core/migrations/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:16:04.651967 bemserver-core-0.9.1/bemserver_core/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)    35257 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/bemserver_core/migrations/versions/0.1_v0_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/bemserver_core/migrations/versions/0.3.1_v0_3.1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/bemserver_core/migrations/versions/0.3_v0_3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/bemserver_core/migrations/versions/0.4_v0_4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/bemserver_core/migrations/versions/0.6_v0_6.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/bemserver_core/migrations/versions/0.8_v0_8.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:16:04.655967 bemserver-core-0.9.1/bemserver_core/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/bemserver_core/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12855 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/bemserver_core/model/authorization.polar
+-rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/bemserver_core/model/campaigns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/bemserver_core/model/energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23795 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/bemserver_core/model/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/bemserver_core/model/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18214 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/bemserver_core/model/sites.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22318 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/bemserver_core/model/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/bemserver_core/model/timeseries_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/bemserver_core/model/users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:16:04.655967 bemserver-core-0.9.1/bemserver_core/process/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/bemserver_core/process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/bemserver_core/process/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/bemserver_core/process/completeness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/bemserver_core/process/energy_consumption.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:16:04.655967 bemserver-core-0.9.1/bemserver_core/scheduled_tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/bemserver_core/scheduled_tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/bemserver_core/scheduled_tasks/authorization.polar
+-rw-r--r--   0 runner    (1001) docker     (123)    10205 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/bemserver_core/scheduled_tasks/check_missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10840 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/bemserver_core/scheduled_tasks/check_outliers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/bemserver_core/scheduled_tasks/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/bemserver_core/time_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/bemserver_core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:16:04.651967 bemserver-core-0.9.1/bemserver_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-02-08 15:16:04.000000 bemserver-core-0.9.1/bemserver_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-02-08 15:16:04.000000 bemserver-core-0.9.1/bemserver_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 15:16:04.000000 bemserver-core-0.9.1/bemserver_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-02-08 15:16:04.000000 bemserver-core-0.9.1/bemserver_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-02-08 15:16:04.000000 bemserver-core-0.9.1/bemserver_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-08 15:16:04.000000 bemserver-core-0.9.1/bemserver_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:16:04.655967 bemserver-core-0.9.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/requirements/install.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/requirements/tests-min.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/requirements/tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-02-08 15:16:04.659967 bemserver-core-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:16:04.655967 bemserver-core-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:16:04.655967 bemserver-core-0.9.1/tests/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/tests/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/tests/common/test_property_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28412 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:16:04.655967 bemserver-core-0.9.1/tests/input_output/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/tests/input_output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28052 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/tests/input_output/test_sites_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91107 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/tests/input_output/test_timeseries_data_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10180 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/tests/input_output/test_timeseries_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:16:04.655967 bemserver-core-0.9.1/tests/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/tests/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12029 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/tests/model/test_campaigns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9244 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/tests/model/test_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41613 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/tests/model/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12157 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/tests/model/test_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68629 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/tests/model/test_sites.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43567 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/tests/model/test_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8820 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/tests/model/test_users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:16:04.659967 bemserver-core-0.9.1/tests/process/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/tests/process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/tests/process/test_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15889 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/tests/process/test_completeness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/tests/process/test_energy_consumption.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:16:04.659967 bemserver-core-0.9.1/tests/scheduled_tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/tests/scheduled_tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19586 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/tests/scheduled_tasks/test_check_missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20103 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/tests/scheduled_tasks/test_check_outliers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22679 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/tests/scheduled_tasks/test_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/tests/test_authorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/tests/test_celery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/tests/test_time_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-02-08 15:15:48.000000 bemserver-core-0.9.1/tox.ini
```

### Comparing `bemserver-core-0.9.0/LICENSE` & `bemserver-core-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/PKG-INFO` & `bemserver-core-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bemserver-core
-Version: 0.9.0
+Version: 0.9.1
 Summary: BEMServer core
 Home-page: https://github.com/BEMServer/bemserver-core
 Author: Nobatek/INEF4
 Author-email: jlafrechoux@nobatek.inef4.com
 License: AGPLv3+
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `bemserver-core-0.9.0/README.rst` & `bemserver-core-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/bemserver_core/__init__.py` & `bemserver-core-0.9.1/bemserver_core/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from . import model
 from . import database  # noqa
 from . import input_output  # noqa
 from . import scheduled_tasks
 
 
-__version__ = "0.9.0"
+__version__ = "0.9.1"
 
 
 class BEMServerCore:
     def __init__(self):
         self.auth_model_classes = (
             model.AUTH_MODEL_CLASSES + scheduled_tasks.AUTH_MODEL_CLASSES
         )
```

### Comparing `bemserver-core-0.9.0/bemserver_core/alembic.ini` & `bemserver-core-0.9.1/bemserver_core/alembic.ini`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/bemserver_core/authorization.py` & `bemserver-core-0.9.1/bemserver_core/authorization.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/bemserver_core/celery.py` & `bemserver-core-0.9.1/bemserver_core/celery.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/bemserver_core/commands.py` & `bemserver-core-0.9.1/bemserver_core/commands.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/bemserver_core/common/property_type.py` & `bemserver-core-0.9.1/bemserver_core/common/property_type.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/bemserver_core/database.py` & `bemserver-core-0.9.1/bemserver_core/database.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/bemserver_core/exceptions.py` & `bemserver-core-0.9.1/bemserver_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/bemserver_core/input_output/base.py` & `bemserver-core-0.9.1/bemserver_core/input_output/base.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/bemserver_core/input_output/sites_io.py` & `bemserver-core-0.9.1/bemserver_core/input_output/sites_io.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/bemserver_core/input_output/timeseries_data_io.py` & `bemserver-core-0.9.1/bemserver_core/input_output/timeseries_data_io.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/bemserver_core/input_output/timeseries_io.py` & `bemserver-core-0.9.1/bemserver_core/input_output/timeseries_io.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/bemserver_core/migrations/env.py` & `bemserver-core-0.9.1/bemserver_core/migrations/env.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/bemserver_core/migrations/versions/0.1_v0_1.py` & `bemserver-core-0.9.1/bemserver_core/migrations/versions/0.1_v0_1.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/bemserver_core/migrations/versions/0.3.1_v0_3.1.py` & `bemserver-core-0.9.1/bemserver_core/migrations/versions/0.3.1_v0_3.1.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/bemserver_core/migrations/versions/0.3_v0_3.py` & `bemserver-core-0.9.1/bemserver_core/migrations/versions/0.3_v0_3.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/bemserver_core/migrations/versions/0.4_v0_4.py` & `bemserver-core-0.9.1/bemserver_core/migrations/versions/0.4_v0_4.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/bemserver_core/migrations/versions/0.6_v0_6.py` & `bemserver-core-0.9.1/bemserver_core/migrations/versions/0.6_v0_6.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/bemserver_core/migrations/versions/0.8_v0_8.py` & `bemserver-core-0.9.1/bemserver_core/migrations/versions/0.8_v0_8.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/bemserver_core/model/__init__.py` & `bemserver-core-0.9.1/bemserver_core/model/__init__.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/bemserver_core/model/authorization.polar` & `bemserver-core-0.9.1/bemserver_core/model/authorization.polar`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/bemserver_core/model/campaigns.py` & `bemserver-core-0.9.1/bemserver_core/model/campaigns.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/bemserver_core/model/energy.py` & `bemserver-core-0.9.1/bemserver_core/model/energy.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/bemserver_core/model/events.py` & `bemserver-core-0.9.1/bemserver_core/model/events.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/bemserver_core/model/notifications.py` & `bemserver-core-0.9.1/bemserver_core/model/notifications.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/bemserver_core/model/sites.py` & `bemserver-core-0.9.1/bemserver_core/model/sites.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/bemserver_core/model/timeseries.py` & `bemserver-core-0.9.1/bemserver_core/model/timeseries.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/bemserver_core/model/timeseries_data.py` & `bemserver-core-0.9.1/bemserver_core/model/timeseries_data.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/bemserver_core/model/users.py` & `bemserver-core-0.9.1/bemserver_core/model/users.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/bemserver_core/process/cleanup.py` & `bemserver-core-0.9.1/bemserver_core/process/cleanup.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/bemserver_core/process/completeness.py` & `bemserver-core-0.9.1/bemserver_core/process/completeness.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/bemserver_core/process/energy_consumption.py` & `bemserver-core-0.9.1/bemserver_core/process/energy_consumption.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/bemserver_core/scheduled_tasks/__init__.py` & `bemserver-core-0.9.1/bemserver_core/scheduled_tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/bemserver_core/scheduled_tasks/authorization.polar` & `bemserver-core-0.9.1/bemserver_core/scheduled_tasks/authorization.polar`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/bemserver_core/scheduled_tasks/check_missing.py` & `bemserver-core-0.9.1/bemserver_core/scheduled_tasks/check_missing.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/bemserver_core/scheduled_tasks/check_outliers.py` & `bemserver-core-0.9.1/bemserver_core/scheduled_tasks/check_outliers.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/bemserver_core/scheduled_tasks/cleanup.py` & `bemserver-core-0.9.1/bemserver_core/scheduled_tasks/cleanup.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/bemserver_core/time_utils.py` & `bemserver-core-0.9.1/bemserver_core/time_utils.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/bemserver_core/utils.py` & `bemserver-core-0.9.1/bemserver_core/utils.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/bemserver_core.egg-info/PKG-INFO` & `bemserver-core-0.9.1/bemserver_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bemserver-core
-Version: 0.9.0
+Version: 0.9.1
 Summary: BEMServer core
 Home-page: https://github.com/BEMServer/bemserver-core
 Author: Nobatek/INEF4
 Author-email: jlafrechoux@nobatek.inef4.com
 License: AGPLv3+
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `bemserver-core-0.9.0/bemserver_core.egg-info/SOURCES.txt` & `bemserver-core-0.9.1/bemserver_core.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 bemserver_core/scheduled_tasks/__init__.py
 bemserver_core/scheduled_tasks/authorization.polar
 bemserver_core/scheduled_tasks/check_missing.py
 bemserver_core/scheduled_tasks/check_outliers.py
 bemserver_core/scheduled_tasks/cleanup.py
 requirements/dev.txt
 requirements/install.txt
+requirements/tests-min.txt
 requirements/tests.txt
 tests/__init__.py
 tests/conftest.py
 tests/test_authorization.py
 tests/test_celery.py
 tests/test_commands.py
 tests/test_database.py
```

### Comparing `bemserver-core-0.9.0/requirements/dev.txt` & `bemserver-core-0.9.1/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/requirements/install.txt` & `bemserver-core-0.9.1/requirements/install.txt`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/requirements/tests.txt` & `bemserver-core-0.9.1/requirements/tests.txt`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/setup.py` & `bemserver-core-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Get the long description from the README file
 with open("README.rst", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="bemserver-core",
-    version="0.9.0",
+    version="0.9.1",
     description="BEMServer core",
     long_description=long_description,
     url="https://github.com/BEMServer/bemserver-core",
     author="Nobatek/INEF4",
     author_email="jlafrechoux@nobatek.inef4.com",
     license="AGPLv3+",
     classifiers=[
@@ -28,15 +28,15 @@
             "License :: OSI Approved :: "
             "GNU Affero General Public License v3 or later (AGPLv3+)"
         ),
     ],
     python_requires=">=3.9",
     install_requires=[
         "psycopg2>=2.9.0",
-        "sqlalchemy>=2.0",
+        "sqlalchemy>=1.4.40",
         "pandas>=1.5.0",
         "passlib>=1.7.4",
         "argon2_cffi>=21.3.0",
         "oso>=0.26.0,<0.27",
         "alembic>=1.8.0",
         "click>=8.1.3",
         "celery>=5.2.0",
```

### Comparing `bemserver-core-0.9.0/tests/common/test_property_type.py` & `bemserver-core-0.9.1/tests/common/test_property_type.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/tests/conftest.py` & `bemserver-core-0.9.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/tests/input_output/test_sites_io.py` & `bemserver-core-0.9.1/tests/input_output/test_sites_io.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/tests/input_output/test_timeseries_data_io.py` & `bemserver-core-0.9.1/tests/input_output/test_timeseries_data_io.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/tests/input_output/test_timeseries_io.py` & `bemserver-core-0.9.1/tests/input_output/test_timeseries_io.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/tests/model/test_campaigns.py` & `bemserver-core-0.9.1/tests/model/test_campaigns.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/tests/model/test_energy.py` & `bemserver-core-0.9.1/tests/model/test_energy.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/tests/model/test_events.py` & `bemserver-core-0.9.1/tests/model/test_events.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/tests/model/test_notifications.py` & `bemserver-core-0.9.1/tests/model/test_notifications.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/tests/model/test_sites.py` & `bemserver-core-0.9.1/tests/model/test_sites.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/tests/model/test_timeseries.py` & `bemserver-core-0.9.1/tests/model/test_timeseries.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/tests/model/test_users.py` & `bemserver-core-0.9.1/tests/model/test_users.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/tests/process/test_cleanup.py` & `bemserver-core-0.9.1/tests/process/test_cleanup.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/tests/process/test_completeness.py` & `bemserver-core-0.9.1/tests/process/test_completeness.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/tests/process/test_energy_consumption.py` & `bemserver-core-0.9.1/tests/process/test_energy_consumption.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/tests/scheduled_tasks/test_check_missing.py` & `bemserver-core-0.9.1/tests/scheduled_tasks/test_check_missing.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/tests/scheduled_tasks/test_check_outliers.py` & `bemserver-core-0.9.1/tests/scheduled_tasks/test_check_outliers.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/tests/scheduled_tasks/test_cleanup.py` & `bemserver-core-0.9.1/tests/scheduled_tasks/test_cleanup.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/tests/test_authorization.py` & `bemserver-core-0.9.1/tests/test_authorization.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/tests/test_celery.py` & `bemserver-core-0.9.1/tests/test_celery.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/tests/test_commands.py` & `bemserver-core-0.9.1/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/tests/test_database.py` & `bemserver-core-0.9.1/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/tests/test_time_utils.py` & `bemserver-core-0.9.1/tests/test_time_utils.py`

 * *Files identical despite different names*

### Comparing `bemserver-core-0.9.0/tests/utils.py` & `bemserver-core-0.9.1/tests/utils.py`

 * *Files identical despite different names*

