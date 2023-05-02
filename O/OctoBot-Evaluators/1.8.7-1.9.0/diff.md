# Comparing `tmp/OctoBot-Evaluators-1.8.7.tar.gz` & `tmp/OctoBot-Evaluators-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OctoBot-Evaluators-1.8.7.tar", last modified: Mon Apr  3 14:43:13 2023, max compression
+gzip compressed data, was "OctoBot-Evaluators-1.9.0.tar", last modified: Tue May  2 20:32:12 2023, max compression
```

## Comparing `OctoBot-Evaluators-1.8.7.tar` & `OctoBot-Evaluators-1.9.0.tar`

### file list

```diff
@@ -1,87 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:43:13.906489 OctoBot-Evaluators-1.8.7/
--rw-r--r--   0 runner    (1001) docker     (123)     7442 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:43:13.894489 OctoBot-Evaluators-1.8.7/OctoBot_Evaluators.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-03 14:43:13.000000 OctoBot-Evaluators-1.8.7/OctoBot_Evaluators.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-04-03 14:43:13.000000 OctoBot-Evaluators-1.8.7/OctoBot_Evaluators.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 14:43:13.000000 OctoBot-Evaluators-1.8.7/OctoBot_Evaluators.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 14:43:13.000000 OctoBot-Evaluators-1.8.7/OctoBot_Evaluators.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-03 14:43:13.000000 OctoBot-Evaluators-1.8.7/OctoBot_Evaluators.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-03 14:43:13.000000 OctoBot-Evaluators-1.8.7/OctoBot_Evaluators.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-03 14:43:13.906489 OctoBot-Evaluators-1.8.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:43:13.894489 OctoBot-Evaluators-1.8.7/octobot_evaluators/
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/octobot_evaluators/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/octobot_evaluators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:43:13.894489 OctoBot-Evaluators-1.8.7/octobot_evaluators/api/
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/octobot_evaluators/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/octobot_evaluators/api/evaluators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/octobot_evaluators/api/initialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/octobot_evaluators/api/inspection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/octobot_evaluators/api/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/octobot_evaluators/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/octobot_evaluators/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/octobot_evaluators/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:43:13.898489 OctoBot-Evaluators-1.8.7/octobot_evaluators/evaluators/
--rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/octobot_evaluators/evaluators/TA_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/octobot_evaluators/evaluators/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/octobot_evaluators/evaluators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22529 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/octobot_evaluators/evaluators/abstract_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/octobot_evaluators/evaluators/abstract_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:43:13.902489 OctoBot-Evaluators-1.8.7/octobot_evaluators/evaluators/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/octobot_evaluators/evaluators/channel/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/octobot_evaluators/evaluators/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/octobot_evaluators/evaluators/channel/evaluator_channel.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/octobot_evaluators/evaluators/channel/evaluator_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/octobot_evaluators/evaluators/channel/evaluators.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     7214 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/octobot_evaluators/evaluators/channel/evaluators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/octobot_evaluators/evaluators/evaluator_factory.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    11820 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/octobot_evaluators/evaluators/evaluator_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/octobot_evaluators/evaluators/realtime_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17323 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/octobot_evaluators/evaluators/scripted_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/octobot_evaluators/evaluators/social_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)    26780 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/octobot_evaluators/evaluators/strategy_evaluator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:43:13.902489 OctoBot-Evaluators-1.8.7/octobot_evaluators/matrix/
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/octobot_evaluators/matrix/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/octobot_evaluators/matrix/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:43:13.902489 OctoBot-Evaluators-1.8.7/octobot_evaluators/matrix/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/octobot_evaluators/matrix/channel/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/octobot_evaluators/matrix/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/octobot_evaluators/matrix/channel/matrix.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     9731 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/octobot_evaluators/matrix/channel/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/octobot_evaluators/matrix/matrices.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/octobot_evaluators/matrix/matrices.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/octobot_evaluators/matrix/matrix.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/octobot_evaluators/matrix/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/octobot_evaluators/matrix/matrix_manager.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    15662 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/octobot_evaluators/matrix/matrix_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/octobot_evaluators/octobot_channel_consumer.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/octobot_evaluators/octobot_channel_consumer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:43:13.906489 OctoBot-Evaluators-1.8.7/octobot_evaluators/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/octobot_evaluators/util/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/octobot_evaluators/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/octobot_evaluators/util/evaluation_util.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/octobot_evaluators/util/evaluation_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 14:43:13.906489 OctoBot-Evaluators-1.8.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:43:13.890489 OctoBot-Evaluators-1.8.7/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:43:13.906489 OctoBot-Evaluators-1.8.7/tests/evaluators/
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/tests/evaluators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:43:13.906489 OctoBot-Evaluators-1.8.7/tests/evaluators/channel/
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/tests/evaluators/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/tests/evaluators/channel/test_evaluator_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)    13392 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/tests/evaluators/test_evaluator_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    12284 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/tests/evaluators/test_evaluator_factory_create_evaluators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:43:13.906489 OctoBot-Evaluators-1.8.7/tests/matrix/
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/tests/matrix/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:43:13.906489 OctoBot-Evaluators-1.8.7/tests/matrix/channel/
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/tests/matrix/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/tests/matrix/channel/test_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/tests/matrix/test_matrices.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/tests/matrix/test_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    41061 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/tests/matrix/test_matrix_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:43:13.906489 OctoBot-Evaluators-1.8.7/tests/util/
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/tests/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-03 14:42:43.000000 OctoBot-Evaluators-1.8.7/tests/util/test_evaluation_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:32:12.442050 OctoBot-Evaluators-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-05-02 20:31:12.000000 OctoBot-Evaluators-1.9.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-02 20:31:12.000000 OctoBot-Evaluators-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-02 20:31:12.000000 OctoBot-Evaluators-1.9.0/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:32:12.438050 OctoBot-Evaluators-1.9.0/OctoBot_Evaluators.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-05-02 20:32:12.000000 OctoBot-Evaluators-1.9.0/OctoBot_Evaluators.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-05-02 20:32:12.000000 OctoBot-Evaluators-1.9.0/OctoBot_Evaluators.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 20:32:12.000000 OctoBot-Evaluators-1.9.0/OctoBot_Evaluators.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 20:32:12.000000 OctoBot-Evaluators-1.9.0/OctoBot_Evaluators.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-02 20:32:12.000000 OctoBot-Evaluators-1.9.0/OctoBot_Evaluators.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-02 20:32:12.000000 OctoBot-Evaluators-1.9.0/OctoBot_Evaluators.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-05-02 20:32:12.442050 OctoBot-Evaluators-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-02 20:31:12.000000 OctoBot-Evaluators-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:32:12.438050 OctoBot-Evaluators-1.9.0/octobot_evaluators/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-02 20:31:12.000000 OctoBot-Evaluators-1.9.0/octobot_evaluators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:32:12.438050 OctoBot-Evaluators-1.9.0/octobot_evaluators/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-05-02 20:31:12.000000 OctoBot-Evaluators-1.9.0/octobot_evaluators/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-05-02 20:31:12.000000 OctoBot-Evaluators-1.9.0/octobot_evaluators/api/evaluators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-05-02 20:31:12.000000 OctoBot-Evaluators-1.9.0/octobot_evaluators/api/initialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-05-02 20:31:12.000000 OctoBot-Evaluators-1.9.0/octobot_evaluators/api/inspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-02 20:31:12.000000 OctoBot-Evaluators-1.9.0/octobot_evaluators/api/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-05-02 20:31:12.000000 OctoBot-Evaluators-1.9.0/octobot_evaluators/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-02 20:31:12.000000 OctoBot-Evaluators-1.9.0/octobot_evaluators/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-02 20:31:12.000000 OctoBot-Evaluators-1.9.0/octobot_evaluators/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:32:12.438050 OctoBot-Evaluators-1.9.0/octobot_evaluators/evaluators/
+-rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-05-02 20:31:12.000000 OctoBot-Evaluators-1.9.0/octobot_evaluators/evaluators/TA_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-05-02 20:31:12.000000 OctoBot-Evaluators-1.9.0/octobot_evaluators/evaluators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23071 2023-05-02 20:31:12.000000 OctoBot-Evaluators-1.9.0/octobot_evaluators/evaluators/abstract_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-02 20:31:12.000000 OctoBot-Evaluators-1.9.0/octobot_evaluators/evaluators/abstract_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:32:12.438050 OctoBot-Evaluators-1.9.0/octobot_evaluators/evaluators/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-02 20:31:12.000000 OctoBot-Evaluators-1.9.0/octobot_evaluators/evaluators/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-05-02 20:31:12.000000 OctoBot-Evaluators-1.9.0/octobot_evaluators/evaluators/channel/evaluator_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7214 2023-05-02 20:31:12.000000 OctoBot-Evaluators-1.9.0/octobot_evaluators/evaluators/channel/evaluators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11820 2023-05-02 20:31:12.000000 OctoBot-Evaluators-1.9.0/octobot_evaluators/evaluators/evaluator_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-02 20:31:12.000000 OctoBot-Evaluators-1.9.0/octobot_evaluators/evaluators/realtime_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17323 2023-05-02 20:31:12.000000 OctoBot-Evaluators-1.9.0/octobot_evaluators/evaluators/scripted_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-05-02 20:31:12.000000 OctoBot-Evaluators-1.9.0/octobot_evaluators/evaluators/social_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26780 2023-05-02 20:31:12.000000 OctoBot-Evaluators-1.9.0/octobot_evaluators/evaluators/strategy_evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:32:12.438050 OctoBot-Evaluators-1.9.0/octobot_evaluators/matrix/
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-02 20:31:12.000000 OctoBot-Evaluators-1.9.0/octobot_evaluators/matrix/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:32:12.442050 OctoBot-Evaluators-1.9.0/octobot_evaluators/matrix/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-02 20:31:12.000000 OctoBot-Evaluators-1.9.0/octobot_evaluators/matrix/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9731 2023-05-02 20:31:12.000000 OctoBot-Evaluators-1.9.0/octobot_evaluators/matrix/channel/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-02 20:31:12.000000 OctoBot-Evaluators-1.9.0/octobot_evaluators/matrix/matrices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-05-02 20:31:12.000000 OctoBot-Evaluators-1.9.0/octobot_evaluators/matrix/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15662 2023-05-02 20:31:12.000000 OctoBot-Evaluators-1.9.0/octobot_evaluators/matrix/matrix_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-05-02 20:31:12.000000 OctoBot-Evaluators-1.9.0/octobot_evaluators/octobot_channel_consumer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:32:12.442050 OctoBot-Evaluators-1.9.0/octobot_evaluators/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-05-02 20:31:12.000000 OctoBot-Evaluators-1.9.0/octobot_evaluators/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-05-02 20:31:12.000000 OctoBot-Evaluators-1.9.0/octobot_evaluators/util/evaluation_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-02 20:31:12.000000 OctoBot-Evaluators-1.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 20:32:12.442050 OctoBot-Evaluators-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-02 20:31:12.000000 OctoBot-Evaluators-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:32:12.434050 OctoBot-Evaluators-1.9.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:32:12.442050 OctoBot-Evaluators-1.9.0/tests/evaluators/
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-02 20:31:12.000000 OctoBot-Evaluators-1.9.0/tests/evaluators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:32:12.442050 OctoBot-Evaluators-1.9.0/tests/evaluators/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-02 20:31:12.000000 OctoBot-Evaluators-1.9.0/tests/evaluators/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-05-02 20:31:12.000000 OctoBot-Evaluators-1.9.0/tests/evaluators/channel/test_evaluator_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13392 2023-05-02 20:31:12.000000 OctoBot-Evaluators-1.9.0/tests/evaluators/test_evaluator_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12284 2023-05-02 20:31:12.000000 OctoBot-Evaluators-1.9.0/tests/evaluators/test_evaluator_factory_create_evaluators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:32:12.442050 OctoBot-Evaluators-1.9.0/tests/matrix/
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-02 20:31:12.000000 OctoBot-Evaluators-1.9.0/tests/matrix/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:32:12.442050 OctoBot-Evaluators-1.9.0/tests/matrix/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-02 20:31:12.000000 OctoBot-Evaluators-1.9.0/tests/matrix/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-05-02 20:31:12.000000 OctoBot-Evaluators-1.9.0/tests/matrix/channel/test_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-02 20:31:12.000000 OctoBot-Evaluators-1.9.0/tests/matrix/test_matrices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-02 20:31:12.000000 OctoBot-Evaluators-1.9.0/tests/matrix/test_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41061 2023-05-02 20:31:12.000000 OctoBot-Evaluators-1.9.0/tests/matrix/test_matrix_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:32:12.442050 OctoBot-Evaluators-1.9.0/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-02 20:31:12.000000 OctoBot-Evaluators-1.9.0/tests/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-02 20:31:12.000000 OctoBot-Evaluators-1.9.0/tests/util/test_evaluation_util.py
```

### Comparing `OctoBot-Evaluators-1.8.7/CHANGELOG.md` & `OctoBot-Evaluators-1.9.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [1.9.0] - 2023-05-02
+### Updated
+- Supported python versions
+### Removed
+- Cython
+
 ## [1.8.7] - 2023-04-03
 ### Added
 - [Evaluators] Split Initialize using _init_registered_topics 
 
 ## [1.8.6] - 2023-03-29
 ### Added
 - [Evaluators] enable_reevaluation()
```

### Comparing `OctoBot-Evaluators-1.8.7/LICENSE` & `OctoBot-Evaluators-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `OctoBot-Evaluators-1.8.7/OctoBot_Evaluators.egg-info/PKG-INFO` & `OctoBot-Evaluators-1.9.0/OctoBot_Evaluators.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,46 +1,45 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: OctoBot-Evaluators
-Version: 1.8.7
+Version: 1.9.0
 Summary: OctoBot project evaluators package
 Home-page: https://github.com/Drakkar-Software/OctoBot-Evaluators
 Author: Drakkar-Software
-Author-email: drakkar-software@protonmail.com
+Author-email: contact@drakkar.software
 License: LGPL-3.0
-Description: # OctoBot-Evaluators [1.8.7](https://github.com/Drakkar-Software/OctoBot-Evaluators/blob/master/CHANGELOG.md)
-        [![Codacy Badge](https://api.codacy.com/project/badge/Grade/a0c08eab5d4c440aa6e3fc3061ad0520)](https://app.codacy.com/gh/Drakkar-Software/OctoBot-Evaluators?utm_source=github.com&utm_medium=referral&utm_content=Drakkar-Software/OctoBot-Evaluators&utm_campaign=Badge_Grade_Dashboard)
-        [![PyPI](https://img.shields.io/pypi/v/OctoBot-Evaluators.svg)](https://pypi.python.org/pypi/OctoBot-Evaluators/)
-        [![Coverage Status](https://coveralls.io/repos/github/Drakkar-Software/OctoBot-Evaluators/badge.svg)](https://coveralls.io/github/Drakkar-Software/OctoBot-Evaluators)
-        [![Github-Action-CI](https://github.com/Drakkar-Software/OctoBot-Evaluators/workflows/OctoBot-Evaluators-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot-Evaluators/actions)
-        [![Build Status](https://cloud.drone.io/api/badges/Drakkar-Software/OctoBot-Evaluators/status.svg)](https://cloud.drone.io/Drakkar-Software/OctoBot-Evaluators)
-        
-        # Where are evaluators and strategies ?
-        
-        Because OctoBot is modular, a wide range of evaluators and strategies are usable.
-        
-        Default evaluators and strategies are located here: [https://github.com/Drakkar-Software/OctoBot-Tentacles](https://github.com/Drakkar-Software/OctoBot-Tentacles).
-        
-        To install default evaluators and strategies in your OctoBot, run the following command: 
-        
-        ```bash
-        python start.py tentacles --install --all
-        ```
-        
-        
-        It is also possible to specify which module(s) to install by naming it(them). In this case only the modules available in the available packages can be installed.
-        ```
-        python start.py tentacles --install forum_evaluator john_smith_macd_evaluator advanced_twitter_evaluator
-        ```
-        
-        **You can find how to create your OctoBot evaluators and strategies [here](https://developer.octobot.info/guides/customize-your-octobot).**
-        
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Cython
 Requires-Python: >=3.8
+License-File: LICENSE
+
+# OctoBot-Evaluators [1.9.0](https://github.com/Drakkar-Software/OctoBot-Evaluators/blob/master/CHANGELOG.md)
+[![Codacy Badge](https://api.codacy.com/project/badge/Grade/a0c08eab5d4c440aa6e3fc3061ad0520)](https://app.codacy.com/gh/Drakkar-Software/OctoBot-Evaluators?utm_source=github.com&utm_medium=referral&utm_content=Drakkar-Software/OctoBot-Evaluators&utm_campaign=Badge_Grade_Dashboard)
+[![PyPI](https://img.shields.io/pypi/v/OctoBot-Evaluators.svg)](https://pypi.python.org/pypi/OctoBot-Evaluators/)
+[![Coverage Status](https://coveralls.io/repos/github/Drakkar-Software/OctoBot-Evaluators/badge.svg)](https://coveralls.io/github/Drakkar-Software/OctoBot-Evaluators)
+[![Github-Action-CI](https://github.com/Drakkar-Software/OctoBot-Evaluators/workflows/OctoBot-Evaluators-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot-Evaluators/actions)
+[![Build Status](https://cloud.drone.io/api/badges/Drakkar-Software/OctoBot-Evaluators/status.svg)](https://cloud.drone.io/Drakkar-Software/OctoBot-Evaluators)
+
+# Where are evaluators and strategies ?
+
+Because OctoBot is modular, a wide range of evaluators and strategies are usable.
+
+Default evaluators and strategies are located here: [https://github.com/Drakkar-Software/OctoBot-Tentacles](https://github.com/Drakkar-Software/OctoBot-Tentacles).
+
+To install default evaluators and strategies in your OctoBot, run the following command: 
+
+```bash
+python start.py tentacles --install --all
+```
+
+
+It is also possible to specify which module(s) to install by naming it(them). In this case only the modules available in the available packages can be installed.
+```
+python start.py tentacles --install forum_evaluator john_smith_macd_evaluator advanced_twitter_evaluator
+```
+
+**You can find how to create your OctoBot evaluators and strategies [here](https://developer.octobot.info/guides/customize-your-octobot).**
+
```

### Comparing `OctoBot-Evaluators-1.8.7/OctoBot_Evaluators.egg-info/SOURCES.txt` & `OctoBot-Evaluators-1.9.0/OctoBot_Evaluators.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -6,58 +6,43 @@
 setup.py
 OctoBot_Evaluators.egg-info/PKG-INFO
 OctoBot_Evaluators.egg-info/SOURCES.txt
 OctoBot_Evaluators.egg-info/dependency_links.txt
 OctoBot_Evaluators.egg-info/not-zip-safe
 OctoBot_Evaluators.egg-info/requires.txt
 OctoBot_Evaluators.egg-info/top_level.txt
-octobot_evaluators/__init__.pxd
 octobot_evaluators/__init__.py
 octobot_evaluators/constants.py
 octobot_evaluators/enums.py
 octobot_evaluators/errors.py
-octobot_evaluators/octobot_channel_consumer.pxd
 octobot_evaluators/octobot_channel_consumer.py
 octobot_evaluators/api/__init__.py
 octobot_evaluators/api/evaluators.py
 octobot_evaluators/api/initialization.py
 octobot_evaluators/api/inspection.py
 octobot_evaluators/api/matrix.py
 octobot_evaluators/evaluators/TA_evaluator.py
-octobot_evaluators/evaluators/__init__.pxd
 octobot_evaluators/evaluators/__init__.py
 octobot_evaluators/evaluators/abstract_evaluator.py
 octobot_evaluators/evaluators/abstract_util.py
-octobot_evaluators/evaluators/evaluator_factory.pxd
 octobot_evaluators/evaluators/evaluator_factory.py
 octobot_evaluators/evaluators/realtime_evaluator.py
 octobot_evaluators/evaluators/scripted_evaluator.py
 octobot_evaluators/evaluators/social_evaluator.py
 octobot_evaluators/evaluators/strategy_evaluator.py
-octobot_evaluators/evaluators/channel/__init__.pxd
 octobot_evaluators/evaluators/channel/__init__.py
-octobot_evaluators/evaluators/channel/evaluator_channel.pxd
 octobot_evaluators/evaluators/channel/evaluator_channel.py
-octobot_evaluators/evaluators/channel/evaluators.pxd
 octobot_evaluators/evaluators/channel/evaluators.py
-octobot_evaluators/matrix/__init__.pxd
 octobot_evaluators/matrix/__init__.py
-octobot_evaluators/matrix/matrices.pxd
 octobot_evaluators/matrix/matrices.py
-octobot_evaluators/matrix/matrix.pxd
 octobot_evaluators/matrix/matrix.py
-octobot_evaluators/matrix/matrix_manager.pxd
 octobot_evaluators/matrix/matrix_manager.py
-octobot_evaluators/matrix/channel/__init__.pxd
 octobot_evaluators/matrix/channel/__init__.py
-octobot_evaluators/matrix/channel/matrix.pxd
 octobot_evaluators/matrix/channel/matrix.py
-octobot_evaluators/util/__init__.pxd
 octobot_evaluators/util/__init__.py
-octobot_evaluators/util/evaluation_util.pxd
 octobot_evaluators/util/evaluation_util.py
 tests/evaluators/__init__.py
 tests/evaluators/test_evaluator_factory.py
 tests/evaluators/test_evaluator_factory_create_evaluators.py
 tests/evaluators/channel/__init__.py
 tests/evaluators/channel/test_evaluator_channel.py
 tests/matrix/__init__.py
```

### Comparing `OctoBot-Evaluators-1.8.7/PKG-INFO` & `OctoBot-Evaluators-1.9.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,46 +1,45 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: OctoBot-Evaluators
-Version: 1.8.7
+Version: 1.9.0
 Summary: OctoBot project evaluators package
 Home-page: https://github.com/Drakkar-Software/OctoBot-Evaluators
 Author: Drakkar-Software
-Author-email: drakkar-software@protonmail.com
+Author-email: contact@drakkar.software
 License: LGPL-3.0
-Description: # OctoBot-Evaluators [1.8.7](https://github.com/Drakkar-Software/OctoBot-Evaluators/blob/master/CHANGELOG.md)
-        [![Codacy Badge](https://api.codacy.com/project/badge/Grade/a0c08eab5d4c440aa6e3fc3061ad0520)](https://app.codacy.com/gh/Drakkar-Software/OctoBot-Evaluators?utm_source=github.com&utm_medium=referral&utm_content=Drakkar-Software/OctoBot-Evaluators&utm_campaign=Badge_Grade_Dashboard)
-        [![PyPI](https://img.shields.io/pypi/v/OctoBot-Evaluators.svg)](https://pypi.python.org/pypi/OctoBot-Evaluators/)
-        [![Coverage Status](https://coveralls.io/repos/github/Drakkar-Software/OctoBot-Evaluators/badge.svg)](https://coveralls.io/github/Drakkar-Software/OctoBot-Evaluators)
-        [![Github-Action-CI](https://github.com/Drakkar-Software/OctoBot-Evaluators/workflows/OctoBot-Evaluators-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot-Evaluators/actions)
-        [![Build Status](https://cloud.drone.io/api/badges/Drakkar-Software/OctoBot-Evaluators/status.svg)](https://cloud.drone.io/Drakkar-Software/OctoBot-Evaluators)
-        
-        # Where are evaluators and strategies ?
-        
-        Because OctoBot is modular, a wide range of evaluators and strategies are usable.
-        
-        Default evaluators and strategies are located here: [https://github.com/Drakkar-Software/OctoBot-Tentacles](https://github.com/Drakkar-Software/OctoBot-Tentacles).
-        
-        To install default evaluators and strategies in your OctoBot, run the following command: 
-        
-        ```bash
-        python start.py tentacles --install --all
-        ```
-        
-        
-        It is also possible to specify which module(s) to install by naming it(them). In this case only the modules available in the available packages can be installed.
-        ```
-        python start.py tentacles --install forum_evaluator john_smith_macd_evaluator advanced_twitter_evaluator
-        ```
-        
-        **You can find how to create your OctoBot evaluators and strategies [here](https://developer.octobot.info/guides/customize-your-octobot).**
-        
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Cython
 Requires-Python: >=3.8
+License-File: LICENSE
+
+# OctoBot-Evaluators [1.9.0](https://github.com/Drakkar-Software/OctoBot-Evaluators/blob/master/CHANGELOG.md)
+[![Codacy Badge](https://api.codacy.com/project/badge/Grade/a0c08eab5d4c440aa6e3fc3061ad0520)](https://app.codacy.com/gh/Drakkar-Software/OctoBot-Evaluators?utm_source=github.com&utm_medium=referral&utm_content=Drakkar-Software/OctoBot-Evaluators&utm_campaign=Badge_Grade_Dashboard)
+[![PyPI](https://img.shields.io/pypi/v/OctoBot-Evaluators.svg)](https://pypi.python.org/pypi/OctoBot-Evaluators/)
+[![Coverage Status](https://coveralls.io/repos/github/Drakkar-Software/OctoBot-Evaluators/badge.svg)](https://coveralls.io/github/Drakkar-Software/OctoBot-Evaluators)
+[![Github-Action-CI](https://github.com/Drakkar-Software/OctoBot-Evaluators/workflows/OctoBot-Evaluators-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot-Evaluators/actions)
+[![Build Status](https://cloud.drone.io/api/badges/Drakkar-Software/OctoBot-Evaluators/status.svg)](https://cloud.drone.io/Drakkar-Software/OctoBot-Evaluators)
+
+# Where are evaluators and strategies ?
+
+Because OctoBot is modular, a wide range of evaluators and strategies are usable.
+
+Default evaluators and strategies are located here: [https://github.com/Drakkar-Software/OctoBot-Tentacles](https://github.com/Drakkar-Software/OctoBot-Tentacles).
+
+To install default evaluators and strategies in your OctoBot, run the following command: 
+
+```bash
+python start.py tentacles --install --all
+```
+
+
+It is also possible to specify which module(s) to install by naming it(them). In this case only the modules available in the available packages can be installed.
+```
+python start.py tentacles --install forum_evaluator john_smith_macd_evaluator advanced_twitter_evaluator
+```
+
+**You can find how to create your OctoBot evaluators and strategies [here](https://developer.octobot.info/guides/customize-your-octobot).**
+
```

### Comparing `OctoBot-Evaluators-1.8.7/README.md` & `OctoBot-Evaluators-1.9.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# OctoBot-Evaluators [1.8.7](https://github.com/Drakkar-Software/OctoBot-Evaluators/blob/master/CHANGELOG.md)
+# OctoBot-Evaluators [1.9.0](https://github.com/Drakkar-Software/OctoBot-Evaluators/blob/master/CHANGELOG.md)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/a0c08eab5d4c440aa6e3fc3061ad0520)](https://app.codacy.com/gh/Drakkar-Software/OctoBot-Evaluators?utm_source=github.com&utm_medium=referral&utm_content=Drakkar-Software/OctoBot-Evaluators&utm_campaign=Badge_Grade_Dashboard)
 [![PyPI](https://img.shields.io/pypi/v/OctoBot-Evaluators.svg)](https://pypi.python.org/pypi/OctoBot-Evaluators/)
 [![Coverage Status](https://coveralls.io/repos/github/Drakkar-Software/OctoBot-Evaluators/badge.svg)](https://coveralls.io/github/Drakkar-Software/OctoBot-Evaluators)
 [![Github-Action-CI](https://github.com/Drakkar-Software/OctoBot-Evaluators/workflows/OctoBot-Evaluators-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot-Evaluators/actions)
 [![Build Status](https://cloud.drone.io/api/badges/Drakkar-Software/OctoBot-Evaluators/status.svg)](https://cloud.drone.io/Drakkar-Software/OctoBot-Evaluators)
 
 # Where are evaluators and strategies ?
```

### Comparing `OctoBot-Evaluators-1.8.7/octobot_evaluators/__init__.pxd` & `OctoBot-Evaluators-1.9.0/tests/evaluators/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Evaluators-1.8.7/octobot_evaluators/__init__.py` & `OctoBot-Evaluators-1.9.0/tests/evaluators/channel/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,10 +9,7 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-
-PROJECT_NAME = "OctoBot-Evaluators"
-VERSION = "1.8.7"  # major.minor.revision
```

### Comparing `OctoBot-Evaluators-1.8.7/octobot_evaluators/api/__init__.py` & `OctoBot-Evaluators-1.9.0/octobot_evaluators/api/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Evaluators-1.8.7/octobot_evaluators/api/evaluators.py` & `OctoBot-Evaluators-1.9.0/octobot_evaluators/api/evaluators.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Evaluators-1.8.7/octobot_evaluators/api/initialization.py` & `OctoBot-Evaluators-1.9.0/octobot_evaluators/api/initialization.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Evaluators-1.8.7/octobot_evaluators/api/inspection.py` & `OctoBot-Evaluators-1.9.0/octobot_evaluators/api/inspection.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Evaluators-1.8.7/octobot_evaluators/api/matrix.py` & `OctoBot-Evaluators-1.9.0/octobot_evaluators/api/matrix.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Evaluators-1.8.7/octobot_evaluators/constants.py` & `OctoBot-Evaluators-1.9.0/octobot_evaluators/constants.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Evaluators-1.8.7/octobot_evaluators/enums.py` & `OctoBot-Evaluators-1.9.0/octobot_evaluators/enums.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Evaluators-1.8.7/octobot_evaluators/errors.py` & `OctoBot-Evaluators-1.9.0/octobot_evaluators/errors.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Evaluators-1.8.7/octobot_evaluators/evaluators/TA_evaluator.py` & `OctoBot-Evaluators-1.9.0/octobot_evaluators/evaluators/TA_evaluator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Evaluators-1.8.7/octobot_evaluators/evaluators/__init__.pxd` & `OctoBot-Evaluators-1.9.0/octobot_evaluators/evaluators/channel/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,37 +10,45 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 
-from octobot_evaluators.evaluators cimport channel
-from octobot_evaluators.evaluators.channel cimport (
-    EvaluatorsChannelConsumer,
-    EvaluatorChannelSupervisedConsumer,
-    EvaluatorsChannelProducer,
-    EvaluatorsChannel,
+from octobot_evaluators.evaluators.channel import evaluator_channel
+from octobot_evaluators.evaluators.channel.evaluator_channel import (
     EvaluatorChannelConsumer,
+    EvaluatorChannelSupervisedConsumer,
     EvaluatorChannelProducer,
     EvaluatorChannel,
     set_chan,
     get_evaluator_channels,
     del_evaluator_channel_container,
     get_chan,
     del_chan,
+    trigger_technical_evaluators_re_evaluation_with_updated_data,
+)
+from octobot_evaluators.evaluators.channel import evaluators
+from octobot_evaluators.evaluators.channel.evaluators import (
+    EvaluatorsChannelConsumer,
+    EvaluatorsChannelProducer,
+    EvaluatorsChannel,
 )
 
 __all__ = [
-    "EvaluatorsChannelConsumer",
+    "EvaluatorChannelConsumer",
     "EvaluatorChannelSupervisedConsumer",
-    "EvaluatorsChannelProducer",
-    "EvaluatorsChannel",
+    "EvaluatorChannelProducer",
+    "EvaluatorChannel",
     "EvaluatorChannelConsumer",
     "EvaluatorChannelProducer",
     "EvaluatorChannel",
     "set_chan",
     "get_evaluator_channels",
     "del_evaluator_channel_container",
     "get_chan",
     "del_chan",
+    "trigger_technical_evaluators_re_evaluation_with_updated_data",
+    "EvaluatorsChannelConsumer",
+    "EvaluatorsChannelProducer",
+    "EvaluatorsChannel",
 ]
```

### Comparing `OctoBot-Evaluators-1.8.7/octobot_evaluators/evaluators/__init__.py` & `OctoBot-Evaluators-1.9.0/octobot_evaluators/evaluators/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Evaluators-1.8.7/octobot_evaluators/evaluators/abstract_evaluator.py` & `OctoBot-Evaluators-1.9.0/octobot_evaluators/evaluators/abstract_evaluator.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,14 +209,27 @@
         trigger_timeframes = self.get_trigger_time_frames()
         if trigger_timeframes != common_constants.CONFIG_WILDCARD:
             available_time_frames = [tf
                                      for tf in available_time_frames
                                      if tf in trigger_timeframes]
         return currencies, symbols, available_time_frames
 
+    def _is_in_backtesting(self):
+        try:
+            import octobot_trading.api as exchange_api
+            return exchange_api.get_is_backtesting(
+                exchange_api.get_exchange_manager_from_exchange_name_and_id(
+                    self.exchange_name,
+                    exchange_api.get_exchange_id_from_matrix_id(self.exchange_name, self.matrix_id)
+                )
+            )
+        except ImportError as e:
+            self.logger.error(f"Can't connect check if backtesting is enabled {e}")
+        return False
+
     async def initialize(self, all_symbols_by_crypto_currencies, time_frames, real_time_time_frames, bot_id):
         await self.reload_config(bot_id)
         currencies, symbols, time_frames = self._get_tentacle_registration_topic(
             all_symbols_by_crypto_currencies, time_frames, real_time_time_frames
         )
         await self._init_registered_topics(all_symbols_by_crypto_currencies, currencies, symbols, time_frames)
```

### Comparing `OctoBot-Evaluators-1.8.7/octobot_evaluators/evaluators/abstract_util.py` & `OctoBot-Evaluators-1.9.0/octobot_evaluators/evaluators/abstract_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Evaluators-1.8.7/octobot_evaluators/evaluators/channel/evaluator_channel.py` & `OctoBot-Evaluators-1.9.0/octobot_evaluators/evaluators/channel/evaluator_channel.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Evaluators-1.8.7/octobot_evaluators/evaluators/channel/evaluators.py` & `OctoBot-Evaluators-1.9.0/octobot_evaluators/evaluators/channel/evaluators.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Evaluators-1.8.7/octobot_evaluators/evaluators/evaluator_factory.py` & `OctoBot-Evaluators-1.9.0/octobot_evaluators/evaluators/evaluator_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Evaluators-1.8.7/octobot_evaluators/evaluators/realtime_evaluator.py` & `OctoBot-Evaluators-1.9.0/octobot_evaluators/evaluators/realtime_evaluator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Evaluators-1.8.7/octobot_evaluators/evaluators/scripted_evaluator.py` & `OctoBot-Evaluators-1.9.0/octobot_evaluators/evaluators/scripted_evaluator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Evaluators-1.8.7/octobot_evaluators/evaluators/social_evaluator.py` & `OctoBot-Evaluators-1.9.0/octobot_evaluators/evaluators/social_evaluator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Evaluators-1.8.7/octobot_evaluators/evaluators/strategy_evaluator.py` & `OctoBot-Evaluators-1.9.0/octobot_evaluators/evaluators/strategy_evaluator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Evaluators-1.8.7/octobot_evaluators/matrix/__init__.pxd` & `OctoBot-Evaluators-1.9.0/octobot_evaluators/matrix/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,22 +10,28 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 
-from octobot_evaluators.matrix cimport matrix_manager
-from octobot_evaluators.matrix cimport matrices
-from octobot_evaluators.matrix cimport matrix
+from octobot_evaluators.matrix import matrix
+from octobot_evaluators.matrix.matrix import (
+    Matrix,
+)
+
+from octobot_evaluators.matrix import matrix_manager
+from octobot_evaluators.matrix import matrices
+from octobot_evaluators.matrix import channel
 
-from octobot_evaluators.matrix.matrix_manager cimport (
+from octobot_evaluators.matrix.matrix_manager import (
     get_matrix,
     set_tentacle_value,
     get_tentacle_node,
+    delete_tentacle_node,
     get_tentacle_value,
     get_tentacle_eval_time,
     get_matrix_default_value_path,
     get_tentacle_nodes,
     get_node_children_by_names_at_path,
     get_tentacles_value_nodes,
     get_latest_eval_time,
@@ -33,33 +39,29 @@
     get_tentacle_value_path,
     get_evaluations_by_evaluator,
     get_available_time_frames,
     get_available_symbols,
     is_tentacle_value_valid,
     is_tentacles_values_valid,
 )
-from octobot_evaluators.matrix.matrices cimport (
+from octobot_evaluators.matrix.matrices import (
     Matrices,
 )
-from octobot_evaluators.matrix.matrix cimport (
-    Matrix,
-)
-
-from octobot_evaluators.matrix cimport channel
-from octobot_evaluators.matrix.channel cimport (
+from octobot_evaluators.matrix.channel import (
     MatrixChannelConsumer,
     MatrixChannelSupervisedConsumer,
     MatrixChannelProducer,
     MatrixChannel,
 )
 
 __all__ = [
     "get_matrix",
     "set_tentacle_value",
     "get_tentacle_node",
+    "delete_tentacle_node",
     "get_tentacle_value",
     "get_tentacle_eval_time",
     "get_matrix_default_value_path",
     "get_tentacle_nodes",
     "get_node_children_by_names_at_path",
     "get_tentacles_value_nodes",
     "get_latest_eval_time",
```

### Comparing `OctoBot-Evaluators-1.8.7/octobot_evaluators/matrix/channel/__init__.pxd` & `OctoBot-Evaluators-1.9.0/octobot_evaluators/matrix/channel/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 
-from octobot_evaluators.matrix.channel cimport matrix
+from octobot_evaluators.matrix.channel import matrix
 
-from octobot_evaluators.matrix.channel.matrix cimport (
+from octobot_evaluators.matrix.channel.matrix import (
     MatrixChannelConsumer,
     MatrixChannelSupervisedConsumer,
     MatrixChannelProducer,
     MatrixChannel,
 )
 
 __all__ = [
```

### Comparing `OctoBot-Evaluators-1.8.7/octobot_evaluators/matrix/channel/matrix.py` & `OctoBot-Evaluators-1.9.0/octobot_evaluators/matrix/channel/matrix.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Evaluators-1.8.7/octobot_evaluators/matrix/matrices.pxd` & `OctoBot-Evaluators-1.9.0/octobot_evaluators/matrix/matrices.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# cython: language_level=3
 #  Drakkar-Software OctoBot-Evaluators
 #  Copyright (c) Drakkar-Software, All rights reserved.
 #
 #  This library is free software; you can redistribute it and/or
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
@@ -10,17 +9,30 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-cimport octobot_commons.singleton as singleton
+import octobot_commons.logging as logging
+import octobot_commons.singleton as singleton
 
-cimport octobot_evaluators.matrix as matrix
+import octobot_evaluators.matrix as matrix 
 
-cdef class Matrices(singleton.Singleton):
-    cdef public dict matrices
 
-    cpdef void add_matrix(self, matrix.Matrix matrix)
-    cpdef matrix.Matrix get_matrix(self, str matrix_id)
-    cpdef void del_matrix(self, str matrix_id)
+class Matrices(singleton.Singleton):
+    def __init__(self):
+        self.matrices: dict = {}
+
+    def add_matrix(self, matrix) -> None:
+        if matrix.matrix_id not in self.matrices:
+            self.matrices[matrix.matrix_id] = matrix
+
+    def get_matrix(self, matrix_id) -> matrix.Matrix:
+        return self.matrices[matrix_id]
+
+    def del_matrix(self, matrix_id) -> None:
+        try:
+            if self.matrices[matrix_id]:
+                self.matrices.pop(matrix_id, None)
+        except KeyError:
+            logging.get_logger(self.__class__.__name__).warning(f"Can't del matrix with id {matrix_id}")
```

### Comparing `OctoBot-Evaluators-1.8.7/octobot_evaluators/matrix/matrix.py` & `OctoBot-Evaluators-1.9.0/octobot_evaluators/matrix/matrix.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Evaluators-1.8.7/octobot_evaluators/matrix/matrix_manager.py` & `OctoBot-Evaluators-1.9.0/octobot_evaluators/matrix/matrix_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Evaluators-1.8.7/octobot_evaluators/octobot_channel_consumer.pxd` & `OctoBot-Evaluators-1.9.0/tests/matrix/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# cython: language_level=3
 #  Drakkar-Software OctoBot-Evaluators
 #  Copyright (c) Drakkar-Software, All rights reserved.
 #
 #  This library is free software; you can redistribute it and/or
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
```

### Comparing `OctoBot-Evaluators-1.8.7/octobot_evaluators/octobot_channel_consumer.py` & `OctoBot-Evaluators-1.9.0/octobot_evaluators/octobot_channel_consumer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Evaluators-1.8.7/octobot_evaluators/util/__init__.pxd` & `OctoBot-Evaluators-1.9.0/octobot_evaluators/util/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,24 +10,25 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 
-from octobot_evaluators.util cimport evaluation_util
+from octobot_evaluators.util import evaluation_util
 
-from octobot_evaluators.util.evaluation_util cimport (
+from octobot_evaluators.util.evaluation_util import (
     get_eval_time,
     get_shortest_time_frame,
     local_trading_context,
     local_cache_client,
     get_required_candles_count,
 )
 
 __all__ = [
     "get_eval_time",
     "get_shortest_time_frame",
     "local_trading_context",
     "local_cache_client",
     "get_required_candles_count",
 ]
+
```

### Comparing `OctoBot-Evaluators-1.8.7/octobot_evaluators/util/evaluation_util.py` & `OctoBot-Evaluators-1.9.0/octobot_evaluators/util/evaluation_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Evaluators-1.8.7/tests/evaluators/__init__.py` & `OctoBot-Evaluators-1.9.0/tests/matrix/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Evaluators-1.8.7/tests/evaluators/channel/__init__.py` & `OctoBot-Evaluators-1.9.0/tests/util/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Evaluators-1.8.7/tests/evaluators/channel/test_evaluator_channel.py` & `OctoBot-Evaluators-1.9.0/tests/evaluators/channel/test_evaluator_channel.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Evaluators-1.8.7/tests/evaluators/test_evaluator_factory.py` & `OctoBot-Evaluators-1.9.0/tests/evaluators/test_evaluator_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Evaluators-1.8.7/tests/evaluators/test_evaluator_factory_create_evaluators.py` & `OctoBot-Evaluators-1.9.0/tests/evaluators/test_evaluator_factory_create_evaluators.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Evaluators-1.8.7/tests/matrix/__init__.py` & `OctoBot-Evaluators-1.9.0/octobot_evaluators/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,7 +9,10 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
+
+PROJECT_NAME = "OctoBot-Evaluators"
+VERSION = "1.9.0"  # major.minor.revision
```

### Comparing `OctoBot-Evaluators-1.8.7/tests/matrix/channel/test_matrix.py` & `OctoBot-Evaluators-1.9.0/tests/matrix/channel/test_matrix.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Evaluators-1.8.7/tests/matrix/test_matrices.py` & `OctoBot-Evaluators-1.9.0/tests/matrix/test_matrices.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Evaluators-1.8.7/tests/matrix/test_matrix.py` & `OctoBot-Evaluators-1.9.0/tests/matrix/test_matrix.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Evaluators-1.8.7/tests/matrix/test_matrix_manager.py` & `OctoBot-Evaluators-1.9.0/tests/matrix/test_matrix_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Evaluators-1.8.7/tests/util/test_evaluation_util.py` & `OctoBot-Evaluators-1.9.0/tests/util/test_evaluation_util.py`

 * *Files identical despite different names*

