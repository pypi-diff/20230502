# Comparing `tmp/decide_exchange_model-2022.1.18.tar.gz` & `tmp/decide-exchange-model-2022.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decide_exchange_model-2022.1.18.tar", max compression
+gzip compressed data, was "dist/decide-exchange-model-2022.1.9.tar", last modified: Sun Mar  6 12:22:35 2022, max compression
```

## Comparing `decide_exchange_model-2022.1.18.tar` & `decide-exchange-model-2022.1.9.tar`

### file list

```diff
@@ -1,74 +1,93 @@
--rw-r--r--   0        0        0    35140 2023-05-02 11:44:21.020408 decide_exchange_model-2022.1.18/LICENSE
--rw-r--r--   0        0        0     1095 2023-05-02 11:44:21.020408 decide_exchange_model-2022.1.18/README.md
--rw-r--r--   0        0        0      271 2023-05-02 11:44:21.020408 decide_exchange_model-2022.1.18/decide/__init__.py
--rw-r--r--   0        0        0     6576 2023-05-02 11:44:21.020408 decide_exchange_model-2022.1.18/decide/cli.py
--rw-r--r--   0        0        0      606 2023-05-02 11:44:21.020408 decide_exchange_model-2022.1.18/decide/conftest.py
--rw-r--r--   0        0        0       92 2023-05-02 11:44:21.020408 decide_exchange_model-2022.1.18/decide/data/__init__.py
--rw-r--r--   0        0        0     5446 2023-05-02 11:44:21.020408 decide_exchange_model-2022.1.18/decide/data/database.py
--rw-r--r--   0        0        0     2772 2023-05-02 11:44:21.020408 decide_exchange_model-2022.1.18/decide/data/modelfactory.py
--rw-r--r--   0        0        0     6159 2023-05-02 11:44:21.020408 decide_exchange_model-2022.1.18/decide/data/reader.py
--rw-r--r--   0        0        0        0 2023-05-02 11:44:21.020408 decide_exchange_model-2022.1.18/decide/data/tests/__init__.py
--rw-r--r--   0        0        0      225 2023-05-02 11:44:21.020408 decide_exchange_model-2022.1.18/decide/data/tests/conftest.py
--rw-r--r--   0        0        0      940 2023-05-02 11:44:21.020408 decide_exchange_model-2022.1.18/decide/data/tests/test_database.py
--rw-r--r--   0        0        0     2822 2023-05-02 11:44:21.020408 decide_exchange_model-2022.1.18/decide/data/tests/test_modelfactory.py
--rw-r--r--   0        0        0     3081 2023-05-02 11:44:21.020408 decide_exchange_model-2022.1.18/decide/data/tests/test_read.py
--rw-r--r--   0        0        0     4399 2023-05-02 11:44:21.020408 decide_exchange_model-2022.1.18/decide/data/types.py
--rw-r--r--   0        0        0      668 2023-05-02 11:44:21.020408 decide_exchange_model-2022.1.18/decide/data/utils.py
--rw-r--r--   0        0        0       81 2023-05-02 11:44:21.020408 decide_exchange_model-2022.1.18/decide/gui.py
--rw-r--r--   0        0        0       91 2023-05-02 11:44:21.020408 decide_exchange_model-2022.1.18/decide/model/__init__.py
--rw-r--r--   0        0        0    32122 2023-05-02 11:44:21.020408 decide_exchange_model-2022.1.18/decide/model/base.py
--rw-r--r--   0        0        0     8914 2023-05-02 11:44:21.020408 decide_exchange_model-2022.1.18/decide/model/calculations.py
--rw-r--r--   0        0        0    22992 2023-05-02 11:44:21.020408 decide_exchange_model-2022.1.18/decide/model/equalgain.py
--rw-r--r--   0        0        0        0 2023-05-02 11:44:21.020408 decide_exchange_model-2022.1.18/decide/model/observers/__init__.py
--rw-r--r--   0        0        0     2611 2023-05-02 11:44:21.020408 decide_exchange_model-2022.1.18/decide/model/observers/exchanges_writer.py
--rw-r--r--   0        0        0    10957 2023-05-02 11:44:21.020408 decide_exchange_model-2022.1.18/decide/model/observers/externalities.py
--rw-r--r--   0        0        0    24383 2023-05-02 11:44:21.020408 decide_exchange_model-2022.1.18/decide/model/observers/issue_development.py
--rw-r--r--   0        0        0     1009 2023-05-02 11:44:21.020408 decide_exchange_model-2022.1.18/decide/model/observers/logger.py
--rw-r--r--   0        0        0     5379 2023-05-02 11:44:21.020408 decide_exchange_model-2022.1.18/decide/model/observers/observer.py
--rw-r--r--   0        0        0     8383 2023-05-02 11:44:21.020408 decide_exchange_model-2022.1.18/decide/model/observers/sqliteobserver.py
--rw-r--r--   0        0        0       53 2023-05-02 11:44:21.020408 decide_exchange_model-2022.1.18/decide/model/observers/tests/test_issue_development.py
--rw-r--r--   0        0        0    14517 2023-05-02 11:44:21.020408 decide_exchange_model-2022.1.18/decide/model/randomrate.py
--rw-r--r--   0        0        0        0 2023-05-02 11:44:21.020408 decide_exchange_model-2022.1.18/decide/model/test/__init__.py
--rw-r--r--   0        0        0     3124 2023-05-02 11:44:21.020408 decide_exchange_model-2022.1.18/decide/model/test/test_abstractExchangeActor.py
--rw-r--r--   0        0        0     1015 2023-05-02 11:44:21.020408 decide_exchange_model-2022.1.18/decide/model/test/test_actor.py
--rw-r--r--   0        0        0      637 2023-05-02 11:44:21.020408 decide_exchange_model-2022.1.18/decide/model/test/test_actorIssue.py
--rw-r--r--   0        0        0     4090 2023-05-02 11:44:21.020408 decide_exchange_model-2022.1.18/decide/model/test/test_calculations.py
--rw-r--r--   0        0        0     1275 2023-05-02 11:44:21.020408 decide_exchange_model-2022.1.18/decide/model/test/test_exchange.py
--rw-r--r--   0        0        0     2028 2023-05-02 11:44:21.020408 decide_exchange_model-2022.1.18/decide/model/test/test_issue.py
--rw-r--r--   0        0        0     2012 2023-05-02 11:44:21.020408 decide_exchange_model-2022.1.18/decide/model/test/test_model.py
--rw-r--r--   0        0        0       82 2023-05-02 11:44:21.020408 decide_exchange_model-2022.1.18/decide/model/test/test_randomizedequalgain.py
--rw-r--r--   0        0        0     2587 2023-05-02 11:44:21.024408 decide_exchange_model-2022.1.18/decide/model/utils.py
--rw-r--r--   0        0        0       11 2023-05-02 11:44:21.024408 decide_exchange_model-2022.1.18/decide/qt/__init__.py
--rw-r--r--   0        0        0        0 2023-05-02 11:44:21.024408 decide_exchange_model-2022.1.18/decide/qt/inputwindow/__init__.py
--rw-r--r--   0        0        0    11369 2023-05-02 11:44:21.024408 decide_exchange_model-2022.1.18/decide/qt/inputwindow/gui.py
--rw-r--r--   0        0        0     6309 2023-05-02 11:44:21.024408 decide_exchange_model-2022.1.18/decide/qt/inputwindow/models.py
--rw-r--r--   0        0        0      544 2023-05-02 11:44:21.024408 decide_exchange_model-2022.1.18/decide/qt/inputwindow/signals.py
--rw-r--r--   0        0        0        0 2023-05-02 11:44:21.024408 decide_exchange_model-2022.1.18/decide/qt/inputwindow/tests/__init__.py
--rw-r--r--   0        0        0     1125 2023-05-02 11:44:21.024408 decide_exchange_model-2022.1.18/decide/qt/inputwindow/tests/test_comment.py
--rw-r--r--   0        0        0      373 2023-05-02 11:44:21.024408 decide_exchange_model-2022.1.18/decide/qt/inputwindow/tests/test_load.py
--rw-r--r--   0        0        0    15336 2023-05-02 11:44:21.024408 decide_exchange_model-2022.1.18/decide/qt/inputwindow/widgets.py
--rw-r--r--   0        0        0        0 2023-05-02 11:44:21.024408 decide_exchange_model-2022.1.18/decide/qt/mainwindow/__init__.py
--rw-r--r--   0        0        0     3708 2023-05-02 11:44:21.024408 decide_exchange_model-2022.1.18/decide/qt/mainwindow/errordialog.py
--rw-r--r--   0        0        0     2401 2023-05-02 11:44:21.024408 decide_exchange_model-2022.1.18/decide/qt/mainwindow/errorgrid.py
--rw-r--r--   0        0        0    18598 2023-05-02 11:44:21.024408 decide_exchange_model-2022.1.18/decide/qt/mainwindow/gui.py
--rw-r--r--   0        0        0     1441 2023-05-02 11:44:21.024408 decide_exchange_model-2022.1.18/decide/qt/mainwindow/helpers.py
--rw-r--r--   0        0        0     7684 2023-05-02 11:44:21.024408 decide_exchange_model-2022.1.18/decide/qt/mainwindow/settings.py
--rw-r--r--   0        0        0      254 2023-05-02 11:44:21.024408 decide_exchange_model-2022.1.18/decide/qt/mainwindow/signals.py
--rw-r--r--   0        0        0        0 2023-05-02 11:44:21.024408 decide_exchange_model-2022.1.18/decide/qt/mainwindow/tests/__init__.py
--rw-r--r--   0        0        0      967 2023-05-02 11:44:21.024408 decide_exchange_model-2022.1.18/decide/qt/mainwindow/tests/test_settings.py
--rw-r--r--   0        0        0    11886 2023-05-02 11:44:21.024408 decide_exchange_model-2022.1.18/decide/qt/mainwindow/widgets.py
--rw-r--r--   0        0        0     1024 2023-05-02 11:44:21.024408 decide_exchange_model-2022.1.18/decide/qt/utils.py
--rw-r--r--   0        0        0       95 2023-05-02 11:44:21.024408 decide_exchange_model-2022.1.18/decide/results/__init__.py
--rw-r--r--   0        0        0     1893 2023-05-02 11:44:21.024408 decide_exchange_model-2022.1.18/decide/results/covariance.py
--rw-r--r--   0        0        0     2256 2023-05-02 11:44:21.024408 decide_exchange_model-2022.1.18/decide/results/descriptives.py
--rw-r--r--   0        0        0     3064 2023-05-02 11:44:21.024408 decide_exchange_model-2022.1.18/decide/results/externalities.py
--rw-r--r--   0        0        0     1843 2023-05-02 11:44:21.024408 decide_exchange_model-2022.1.18/decide/results/helpers.py
--rw-r--r--   0        0        0     2589 2023-05-02 11:44:21.024408 decide_exchange_model-2022.1.18/decide/results/issuecomparison.py
--rw-r--r--   0        0        0     4524 2023-05-02 11:44:21.024408 decide_exchange_model-2022.1.18/decide/results/nashbargainingsolution.py
--rw-r--r--   0        0        0        0 2023-05-02 11:44:21.024408 decide_exchange_model-2022.1.18/decide/tests/__init__.py
--rw-r--r--   0        0        0      595 2023-05-02 11:44:21.024408 decide_exchange_model-2022.1.18/decide/tests/cli_test.py
--rw-r--r--   0        0        0     7291 2023-05-02 11:44:21.024408 decide_exchange_model-2022.1.18/decide/tests/test_rex.py
--rw-r--r--   0        0        0     2948 2023-05-02 11:44:21.024408 decide_exchange_model-2022.1.18/decide/utils.py
--rw-r--r--   0        0        0      549 2023-05-02 11:44:21.024408 decide_exchange_model-2022.1.18/pyproject.toml
--rw-r--r--   0        0        0     2296 1970-01-01 00:00:00.000000 decide_exchange_model-2022.1.18/setup.py
--rw-r--r--   0        0        0     1751 1970-01-01 00:00:00.000000 decide_exchange_model-2022.1.18/PKG-INFO
+drwxrwxr-x   0 jelmert   (1000) jelmert   (1000)        0 2022-03-06 12:22:35.000000 decide-exchange-model-2022.1.9/
+-rw-rw-r--   0 jelmert   (1000) jelmert   (1000)      174 2022-03-06 12:22:35.000000 decide-exchange-model-2022.1.9/setup.cfg
+-rw-rw-r--   0 jelmert   (1000) jelmert   (1000)     1470 2022-03-06 12:22:35.000000 decide-exchange-model-2022.1.9/PKG-INFO
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)     1521 2022-03-06 12:16:12.000000 decide-exchange-model-2022.1.9/setup.py
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)     1095 2019-12-10 17:03:46.000000 decide-exchange-model-2022.1.9/README.md
+drwxrwxr-x   0 jelmert   (1000) jelmert   (1000)        0 2022-03-06 12:22:35.000000 decide-exchange-model-2022.1.9/decide/
+drwxrwxr-x   0 jelmert   (1000) jelmert   (1000)        0 2022-03-06 12:22:35.000000 decide-exchange-model-2022.1.9/decide/qt/
+drwxrwxr-x   0 jelmert   (1000) jelmert   (1000)        0 2022-03-06 12:22:35.000000 decide-exchange-model-2022.1.9/decide/qt/mainwindow/
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)     3708 2019-12-10 17:03:46.000000 decide-exchange-model-2022.1.9/decide/qt/mainwindow/errordialog.py
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)     2401 2019-12-10 17:03:46.000000 decide-exchange-model-2022.1.9/decide/qt/mainwindow/errorgrid.py
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)      254 2019-12-10 17:03:46.000000 decide-exchange-model-2022.1.9/decide/qt/mainwindow/signals.py
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)        0 2019-12-10 17:03:46.000000 decide-exchange-model-2022.1.9/decide/qt/mainwindow/__init__.py
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)     1441 2019-12-10 17:03:46.000000 decide-exchange-model-2022.1.9/decide/qt/mainwindow/helpers.py
+drwxrwxr-x   0 jelmert   (1000) jelmert   (1000)        0 2022-03-06 12:22:35.000000 decide-exchange-model-2022.1.9/decide/qt/mainwindow/tests/
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)        0 2019-12-10 17:03:46.000000 decide-exchange-model-2022.1.9/decide/qt/mainwindow/tests/__init__.py
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)      967 2019-12-10 17:03:46.000000 decide-exchange-model-2022.1.9/decide/qt/mainwindow/tests/test_settings.py
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)    12338 2020-12-16 14:15:19.000000 decide-exchange-model-2022.1.9/decide/qt/mainwindow/widgets.py
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)    18543 2020-12-16 14:39:27.000000 decide-exchange-model-2022.1.9/decide/qt/mainwindow/gui.py
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)     7684 2020-12-16 14:35:10.000000 decide-exchange-model-2022.1.9/decide/qt/mainwindow/settings.py
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)       11 2019-12-10 17:03:46.000000 decide-exchange-model-2022.1.9/decide/qt/__init__.py
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)     1024 2019-12-10 17:03:46.000000 decide-exchange-model-2022.1.9/decide/qt/utils.py
+drwxrwxr-x   0 jelmert   (1000) jelmert   (1000)        0 2022-03-06 12:22:35.000000 decide-exchange-model-2022.1.9/decide/qt/inputwindow/
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)      544 2019-12-10 17:03:46.000000 decide-exchange-model-2022.1.9/decide/qt/inputwindow/signals.py
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)        0 2019-12-10 17:03:46.000000 decide-exchange-model-2022.1.9/decide/qt/inputwindow/__init__.py
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)     6309 2019-12-13 11:01:05.000000 decide-exchange-model-2022.1.9/decide/qt/inputwindow/models.py
+drwxrwxr-x   0 jelmert   (1000) jelmert   (1000)        0 2022-03-06 12:22:35.000000 decide-exchange-model-2022.1.9/decide/qt/inputwindow/tests/
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)     1125 2019-12-10 17:03:46.000000 decide-exchange-model-2022.1.9/decide/qt/inputwindow/tests/test_comment.py
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)        0 2019-12-10 17:03:46.000000 decide-exchange-model-2022.1.9/decide/qt/inputwindow/tests/__init__.py
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)      373 2019-12-10 17:03:46.000000 decide-exchange-model-2022.1.9/decide/qt/inputwindow/tests/test_load.py
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)    15336 2019-12-10 17:03:46.000000 decide-exchange-model-2022.1.9/decide/qt/inputwindow/widgets.py
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)    11403 2020-03-02 13:58:31.000000 decide-exchange-model-2022.1.9/decide/qt/inputwindow/gui.py
+-rw-rw-r--   0 jelmert   (1000) jelmert   (1000)      270 2022-03-05 18:43:48.000000 decide-exchange-model-2022.1.9/decide/__init__.py
+drwxrwxr-x   0 jelmert   (1000) jelmert   (1000)        0 2022-03-06 12:22:35.000000 decide-exchange-model-2022.1.9/decide/data/
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)     6159 2020-04-03 07:19:55.000000 decide-exchange-model-2022.1.9/decide/data/reader.py
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)       92 2019-12-10 17:03:46.000000 decide-exchange-model-2022.1.9/decide/data/__init__.py
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)     2772 2021-04-07 13:20:46.000000 decide-exchange-model-2022.1.9/decide/data/modelfactory.py
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)     4399 2020-04-03 07:29:02.000000 decide-exchange-model-2022.1.9/decide/data/types.py
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)      668 2019-12-10 17:03:46.000000 decide-exchange-model-2022.1.9/decide/data/utils.py
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)     5446 2019-12-10 17:03:46.000000 decide-exchange-model-2022.1.9/decide/data/database.py
+drwxrwxr-x   0 jelmert   (1000) jelmert   (1000)        0 2022-03-06 12:22:35.000000 decide-exchange-model-2022.1.9/decide/data/tests/
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)        0 2019-12-10 17:03:46.000000 decide-exchange-model-2022.1.9/decide/data/tests/__init__.py
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)     3081 2020-04-03 07:29:13.000000 decide-exchange-model-2022.1.9/decide/data/tests/test_read.py
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)      225 2019-12-10 17:03:46.000000 decide-exchange-model-2022.1.9/decide/data/tests/conftest.py
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)      940 2019-12-10 17:03:46.000000 decide-exchange-model-2022.1.9/decide/data/tests/test_database.py
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)     2822 2019-12-10 17:03:46.000000 decide-exchange-model-2022.1.9/decide/data/tests/test_modelfactory.py
+-rw-rw-r--   0 jelmert   (1000) jelmert   (1000)     2948 2020-12-15 09:38:13.000000 decide-exchange-model-2022.1.9/decide/utils.py
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)      606 2019-12-10 17:03:46.000000 decide-exchange-model-2022.1.9/decide/conftest.py
+drwxrwxr-x   0 jelmert   (1000) jelmert   (1000)        0 2022-03-06 12:22:35.000000 decide-exchange-model-2022.1.9/decide/model/
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)       91 2019-12-10 17:03:46.000000 decide-exchange-model-2022.1.9/decide/model/__init__.py
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)     8914 2020-12-15 10:15:24.000000 decide-exchange-model-2022.1.9/decide/model/calculations.py
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)    14517 2019-12-10 17:03:46.000000 decide-exchange-model-2022.1.9/decide/model/randomrate.py
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)     2587 2020-12-15 10:15:24.000000 decide-exchange-model-2022.1.9/decide/model/utils.py
+drwxrwxr-x   0 jelmert   (1000) jelmert   (1000)        0 2022-03-06 12:22:35.000000 decide-exchange-model-2022.1.9/decide/model/test/
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)     1275 2021-04-07 13:28:29.000000 decide-exchange-model-2022.1.9/decide/model/test/test_exchange.py
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)     1015 2019-12-10 17:03:46.000000 decide-exchange-model-2022.1.9/decide/model/test/test_actor.py
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)     2012 2022-03-05 14:19:19.000000 decide-exchange-model-2022.1.9/decide/model/test/test_model.py
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)        0 2019-12-10 17:03:46.000000 decide-exchange-model-2022.1.9/decide/model/test/__init__.py
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)      637 2019-12-10 17:03:46.000000 decide-exchange-model-2022.1.9/decide/model/test/test_actorIssue.py
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)     3124 2021-04-07 13:33:17.000000 decide-exchange-model-2022.1.9/decide/model/test/test_abstractExchangeActor.py
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)     2028 2019-12-10 17:03:46.000000 decide-exchange-model-2022.1.9/decide/model/test/test_issue.py
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)     4090 2019-12-10 17:03:46.000000 decide-exchange-model-2022.1.9/decide/model/test/test_calculations.py
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)       82 2019-12-10 17:03:46.000000 decide-exchange-model-2022.1.9/decide/model/test/test_randomizedequalgain.py
+-rw-rw-r--   0 jelmert   (1000) jelmert   (1000)    22840 2022-03-01 08:02:44.000000 decide-exchange-model-2022.1.9/decide/model/equalgain.py
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)    32122 2021-04-07 13:32:44.000000 decide-exchange-model-2022.1.9/decide/model/base.py
+drwxrwxr-x   0 jelmert   (1000) jelmert   (1000)        0 2022-03-06 12:22:35.000000 decide-exchange-model-2022.1.9/decide/model/observers/
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)     2611 2019-12-10 17:03:46.000000 decide-exchange-model-2022.1.9/decide/model/observers/exchanges_writer.py
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)        0 2019-12-10 17:03:46.000000 decide-exchange-model-2022.1.9/decide/model/observers/__init__.py
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)     8383 2020-12-03 11:33:10.000000 decide-exchange-model-2022.1.9/decide/model/observers/sqliteobserver.py
+-rw-rw-r--   0 jelmert   (1000) jelmert   (1000)    24383 2021-03-31 06:58:27.000000 decide-exchange-model-2022.1.9/decide/model/observers/issue_development.py
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)     1009 2019-12-10 17:03:46.000000 decide-exchange-model-2022.1.9/decide/model/observers/logger.py
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)    10957 2019-12-10 17:03:46.000000 decide-exchange-model-2022.1.9/decide/model/observers/externalities.py
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)     5379 2019-12-10 17:03:46.000000 decide-exchange-model-2022.1.9/decide/model/observers/observer.py
+drwxrwxr-x   0 jelmert   (1000) jelmert   (1000)        0 2022-03-06 12:22:35.000000 decide-exchange-model-2022.1.9/decide/tests/
+-rw-rw-r--   0 jelmert   (1000) jelmert   (1000)     7291 2020-08-03 12:23:15.000000 decide-exchange-model-2022.1.9/decide/tests/test_rex.py
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)      595 2019-12-10 17:03:46.000000 decide-exchange-model-2022.1.9/decide/tests/cli_test.py
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)        0 2019-12-10 17:03:46.000000 decide-exchange-model-2022.1.9/decide/tests/__init__.py
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)       81 2019-12-10 17:03:46.000000 decide-exchange-model-2022.1.9/decide/gui.py
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)     6576 2020-12-16 14:11:40.000000 decide-exchange-model-2022.1.9/decide/cli.py
+drwxrwxr-x   0 jelmert   (1000) jelmert   (1000)        0 2022-03-06 12:22:35.000000 decide-exchange-model-2022.1.9/decide/results/
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)     2589 2020-12-03 10:41:21.000000 decide-exchange-model-2022.1.9/decide/results/issuecomparison.py
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)       95 2019-12-10 17:03:46.000000 decide-exchange-model-2022.1.9/decide/results/__init__.py
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)     1893 2020-12-03 11:26:15.000000 decide-exchange-model-2022.1.9/decide/results/covariance.py
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)     1843 2019-12-12 09:15:00.000000 decide-exchange-model-2022.1.9/decide/results/helpers.py
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)     3067 2020-01-10 08:33:44.000000 decide-exchange-model-2022.1.9/decide/results/externalities.py
+-rw-rw-r--   0 jelmert   (1000) jelmert   (1000)     4674 2022-03-05 15:41:46.000000 decide-exchange-model-2022.1.9/decide/results/nashbargainingsolution.py
+-rw-r--r--   0 jelmert   (1000) jelmert   (1000)     2259 2020-03-02 12:01:14.000000 decide-exchange-model-2022.1.9/decide/results/descriptives.py
+drwxrwxr-x   0 jelmert   (1000) jelmert   (1000)        0 2022-03-06 12:22:35.000000 decide-exchange-model-2022.1.9/decide_exchange_model.egg-info/
+-rw-rw-r--   0 jelmert   (1000) jelmert   (1000)        7 2022-03-06 12:22:35.000000 decide-exchange-model-2022.1.9/decide_exchange_model.egg-info/top_level.txt
+-rw-rw-r--   0 jelmert   (1000) jelmert   (1000)     2404 2022-03-06 12:22:35.000000 decide-exchange-model-2022.1.9/decide_exchange_model.egg-info/SOURCES.txt
+-rw-rw-r--   0 jelmert   (1000) jelmert   (1000)     1470 2022-03-06 12:22:35.000000 decide-exchange-model-2022.1.9/decide_exchange_model.egg-info/PKG-INFO
+-rw-rw-r--   0 jelmert   (1000) jelmert   (1000)       92 2022-03-06 12:22:35.000000 decide-exchange-model-2022.1.9/decide_exchange_model.egg-info/entry_points.txt
+-rw-rw-r--   0 jelmert   (1000) jelmert   (1000)        1 2022-03-06 12:22:35.000000 decide-exchange-model-2022.1.9/decide_exchange_model.egg-info/dependency_links.txt
+-rw-rw-r--   0 jelmert   (1000) jelmert   (1000)      139 2022-03-06 12:22:35.000000 decide-exchange-model-2022.1.9/decide_exchange_model.egg-info/requires.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `decide_exchange_model-2022.1.18/README.md` & `decide-exchange-model-2022.1.9/README.md`

 * *Files identical despite different names*

### Comparing `decide_exchange_model-2022.1.18/decide/cli.py` & `decide-exchange-model-2022.1.9/decide/cli.py`

 * *Files identical despite different names*

### Comparing `decide_exchange_model-2022.1.18/decide/conftest.py` & `decide-exchange-model-2022.1.9/decide/conftest.py`

 * *Files identical despite different names*

### Comparing `decide_exchange_model-2022.1.18/decide/data/database.py` & `decide-exchange-model-2022.1.9/decide/data/database.py`

 * *Files identical despite different names*

### Comparing `decide_exchange_model-2022.1.18/decide/data/modelfactory.py` & `decide-exchange-model-2022.1.9/decide/data/modelfactory.py`

 * *Files identical despite different names*

### Comparing `decide_exchange_model-2022.1.18/decide/data/reader.py` & `decide-exchange-model-2022.1.9/decide/data/reader.py`

 * *Files identical despite different names*

### Comparing `decide_exchange_model-2022.1.18/decide/data/tests/test_database.py` & `decide-exchange-model-2022.1.9/decide/data/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `decide_exchange_model-2022.1.18/decide/data/tests/test_modelfactory.py` & `decide-exchange-model-2022.1.9/decide/data/tests/test_modelfactory.py`

 * *Files identical despite different names*

### Comparing `decide_exchange_model-2022.1.18/decide/data/tests/test_read.py` & `decide-exchange-model-2022.1.9/decide/data/tests/test_read.py`

 * *Files identical despite different names*

### Comparing `decide_exchange_model-2022.1.18/decide/data/types.py` & `decide-exchange-model-2022.1.9/decide/data/types.py`

 * *Files identical despite different names*

### Comparing `decide_exchange_model-2022.1.18/decide/data/utils.py` & `decide-exchange-model-2022.1.9/decide/data/utils.py`

 * *Files identical despite different names*

### Comparing `decide_exchange_model-2022.1.18/decide/model/base.py` & `decide-exchange-model-2022.1.9/decide/model/base.py`

 * *Files identical despite different names*

### Comparing `decide_exchange_model-2022.1.18/decide/model/calculations.py` & `decide-exchange-model-2022.1.9/decide/model/calculations.py`

 * *Files identical despite different names*

### Comparing `decide_exchange_model-2022.1.18/decide/model/equalgain.py` & `decide-exchange-model-2022.1.9/decide/model/equalgain.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from decide.model import base, calculations
 
 
 class EqualGainExchangeActor(base.AbstractExchangeActor):
     """
     AbstractExchangeActor is the same actor...
     """
-    exchange: "EqualGainExchange"
 
     def __init__(
         self,
         model: "EqualGainModel",
         actor: base.Actor,
         demand_issue: base.Issue,
         supply_issue: base.Issue,
@@ -39,21 +38,20 @@
         self.u = u
         self.v = v
 
         self.opposite_actor.u = u
         self.opposite_actor.v = v
         self.opposite_actor.z = z
 
-        apply_equal_length = False
         # does this actor WIN or LOSE
         if v < 0.5:  # V < 0.5:
             # wins
             a = self.eu_max - eu
 
-            if apply_equal_length and a > eu:
+            if a > eu:
                 a = eu
             eui = eu + p * z * a
         else:
             # loses
             eui = eu - p * z * eu
 
         # calculate the expected utility of J
@@ -345,16 +343,14 @@
         self.opposite_actor.nbs_1 = self.opposite_actor.adjust_nbs(
             self.opposite_actor.y
         )
 
 
 class EqualGainExchange(base.AbstractExchange):
     actor_class = EqualGainExchangeActor
-    i: EqualGainExchangeActor
-    j: EqualGainExchangeActor
 
     def __init__(self, i, j, p, q, m, groups):
         self.i: EqualGainExchangeActor
         self.j: EqualGainExchangeActor
         super().__init__(i, j, p, q, m, groups)
 
     def calculate(self):
```

### Comparing `decide_exchange_model-2022.1.18/decide/model/observers/exchanges_writer.py` & `decide-exchange-model-2022.1.9/decide/model/observers/exchanges_writer.py`

 * *Files identical despite different names*

### Comparing `decide_exchange_model-2022.1.18/decide/model/observers/externalities.py` & `decide-exchange-model-2022.1.9/decide/model/observers/externalities.py`

 * *Files identical despite different names*

### Comparing `decide_exchange_model-2022.1.18/decide/model/observers/issue_development.py` & `decide-exchange-model-2022.1.9/decide/model/observers/issue_development.py`

 * *Files identical despite different names*

### Comparing `decide_exchange_model-2022.1.18/decide/model/observers/logger.py` & `decide-exchange-model-2022.1.9/decide/model/observers/logger.py`

 * *Files identical despite different names*

### Comparing `decide_exchange_model-2022.1.18/decide/model/observers/observer.py` & `decide-exchange-model-2022.1.9/decide/model/observers/observer.py`

 * *Files identical despite different names*

### Comparing `decide_exchange_model-2022.1.18/decide/model/observers/sqliteobserver.py` & `decide-exchange-model-2022.1.9/decide/model/observers/sqliteobserver.py`

 * *Files identical despite different names*

### Comparing `decide_exchange_model-2022.1.18/decide/model/randomrate.py` & `decide-exchange-model-2022.1.9/decide/model/randomrate.py`

 * *Files identical despite different names*

### Comparing `decide_exchange_model-2022.1.18/decide/model/test/test_abstractExchangeActor.py` & `decide-exchange-model-2022.1.9/decide/model/test/test_abstractExchangeActor.py`

 * *Files identical despite different names*

### Comparing `decide_exchange_model-2022.1.18/decide/model/test/test_actor.py` & `decide-exchange-model-2022.1.9/decide/model/test/test_actor.py`

 * *Files identical despite different names*

### Comparing `decide_exchange_model-2022.1.18/decide/model/test/test_actorIssue.py` & `decide-exchange-model-2022.1.9/decide/model/test/test_actorIssue.py`

 * *Files identical despite different names*

### Comparing `decide_exchange_model-2022.1.18/decide/model/test/test_calculations.py` & `decide-exchange-model-2022.1.9/decide/model/test/test_calculations.py`

 * *Files identical despite different names*

### Comparing `decide_exchange_model-2022.1.18/decide/model/test/test_exchange.py` & `decide-exchange-model-2022.1.9/decide/model/test/test_exchange.py`

 * *Files identical despite different names*

### Comparing `decide_exchange_model-2022.1.18/decide/model/test/test_issue.py` & `decide-exchange-model-2022.1.9/decide/model/test/test_issue.py`

 * *Files identical despite different names*

### Comparing `decide_exchange_model-2022.1.18/decide/model/test/test_model.py` & `decide-exchange-model-2022.1.9/decide/model/test/test_model.py`

 * *Files identical despite different names*

### Comparing `decide_exchange_model-2022.1.18/decide/model/utils.py` & `decide-exchange-model-2022.1.9/decide/model/utils.py`

 * *Files identical despite different names*

### Comparing `decide_exchange_model-2022.1.18/decide/qt/inputwindow/gui.py` & `decide-exchange-model-2022.1.9/decide/qt/inputwindow/gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,16 @@
         if file_path.startswith('http'):
             response = requests.get(file_path)
 
             file_path = file_path.split('/')[-1]
 
             download_dir = os.path.join(input_folder, 'downloads')
 
-            os.makedirs(download_dir, exist_ok=True)
+            if not os.path.isdir(download_dir):
+                os.mkdir(download_dir)
 
             with open(os.path.join(download_dir, file_path), 'wb') as file:
                 file.write(response.content)
 
         file = os.path.join(input_folder, file_path)
 
         if os.path.isfile(file):
```

### Comparing `decide_exchange_model-2022.1.18/decide/qt/inputwindow/models.py` & `decide-exchange-model-2022.1.9/decide/qt/inputwindow/models.py`

 * *Files identical despite different names*

### Comparing `decide_exchange_model-2022.1.18/decide/qt/inputwindow/signals.py` & `decide-exchange-model-2022.1.9/decide/qt/inputwindow/signals.py`

 * *Files identical despite different names*

### Comparing `decide_exchange_model-2022.1.18/decide/qt/inputwindow/tests/test_comment.py` & `decide-exchange-model-2022.1.9/decide/qt/inputwindow/tests/test_comment.py`

 * *Files identical despite different names*

### Comparing `decide_exchange_model-2022.1.18/decide/qt/inputwindow/widgets.py` & `decide-exchange-model-2022.1.9/decide/qt/inputwindow/widgets.py`

 * *Files identical despite different names*

### Comparing `decide_exchange_model-2022.1.18/decide/qt/mainwindow/errordialog.py` & `decide-exchange-model-2022.1.9/decide/qt/mainwindow/errordialog.py`

 * *Files identical despite different names*

### Comparing `decide_exchange_model-2022.1.18/decide/qt/mainwindow/errorgrid.py` & `decide-exchange-model-2022.1.9/decide/qt/mainwindow/errorgrid.py`

 * *Files identical despite different names*

### Comparing `decide_exchange_model-2022.1.18/decide/qt/mainwindow/gui.py` & `decide-exchange-model-2022.1.9/decide/qt/mainwindow/gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -301,19 +301,18 @@
 
         self.overview_widget.update_widget()
 
     def open_current_input_window_with_current_data(self):
 
         from decide.qt.inputwindow.gui import InputWindow, register_app
 
-        if self.settings and self.settings.input_filename:
-            ex = InputWindow(self)
-            ex.load(self.settings.input_filename)
+        ex = InputWindow(self)
+        ex.load(self.settings.input_filename)
 
-            register_app(ex)
+        register_app(ex)
 
     def select_output_dir(self):
         """
         Output directory
         """
         self.settings.output_directory = str(
             QtWidgets.QFileDialog.getExistingDirectory(self, "Select Directory")
@@ -373,16 +372,16 @@
                     from decide.qt.mainwindow.errorgrid import ErrorGrid
 
                     ex = ErrorGrid(data_file, self)
 
     def run_safe(self):
 
         self.worker = Worker(self.settings)
-        self.worker.moveToThread(self.thread)
         self.worker.finished.connect(self.finished)
+        self.worker.moveToThread(self.thread)
         self.worker.finished.connect(self.thread.quit)
         self.worker.update.connect(self.update_progress)
         self.thread.started.connect(self.worker.run_model)
         self.thread.start()
 
     def update_progress(self, variation, repetition, iteration, start_time):
 
@@ -505,22 +504,22 @@
     logging.basicConfig(
         filename=log_filename,
         filemode="a",
         level=logging.INFO,
         format=" %(asctime)s - %(levelname)s - %(message)s",
     )
 
-    qtapp = QtWidgets.QApplication([])
+    qtapp = QtWidgets.QApplication(sys.argv)
     qtapp.setQuitOnLastWindowClosed(True)
 
     app = DecideMainWindow()
 
     sys.excepthook = utils.exception_hook
 
-    qtapp.exec_()
+    sys.exit(qtapp.exec_())
 
 
 if __name__ == "__main__":
     main()
 
 
 def safe_settings_as_csv(settings: ProgramSettings, filename):
```

### Comparing `decide_exchange_model-2022.1.18/decide/qt/mainwindow/helpers.py` & `decide-exchange-model-2022.1.9/decide/qt/mainwindow/helpers.py`

 * *Files identical despite different names*

### Comparing `decide_exchange_model-2022.1.18/decide/qt/mainwindow/settings.py` & `decide-exchange-model-2022.1.9/decide/qt/mainwindow/settings.py`

 * *Files identical despite different names*

### Comparing `decide_exchange_model-2022.1.18/decide/qt/mainwindow/tests/test_settings.py` & `decide-exchange-model-2022.1.9/decide/qt/mainwindow/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `decide_exchange_model-2022.1.18/decide/qt/mainwindow/widgets.py` & `decide-exchange-model-2022.1.9/decide/qt/mainwindow/widgets.py`

 * *Files 4% similar despite different names*

```diff
@@ -286,14 +286,24 @@
 
         save_settings = QtWidgets.QAction("&Save settings", self)
         save_settings.triggered.connect(self.main_window.save_settings)
 
         output_dir_action = QtWidgets.QAction("&Set output directory", self)
         output_dir_action.triggered.connect(self.main_window.select_output_dir)
 
+        # output_menu.addAction(self.issue_development_csv)
+        # output_menu.addAction(self.externalities_csv)
+        # output_menu.addAction(self.exchanges_csv)
+        # output_menu.addSeparator()
+        # output_menu.addAction(self.summary_only)
+        # output_menu.addAction(self.output_sqlite)
+        # output_menu.addAction(self.voting_positions)
+        # output_menu.addSeparator()
+        # output_menu.addAction(output_dir_action)
+
         # debug = self.addMenu("Debug")
         log_action = QtWidgets.QAction("Show log window", self)
         log_action.triggered.connect(self.main_window.show_debug_dialog)
 
         file_menu.addAction(open_action)
         self.recently_opened_menu(file_menu)
         file_menu.addAction(self.open_data_view)
```

### Comparing `decide_exchange_model-2022.1.18/decide/qt/utils.py` & `decide-exchange-model-2022.1.9/decide/qt/utils.py`

 * *Files identical despite different names*

### Comparing `decide_exchange_model-2022.1.18/decide/results/covariance.py` & `decide-exchange-model-2022.1.9/decide/results/covariance.py`

 * *Files identical despite different names*

### Comparing `decide_exchange_model-2022.1.18/decide/results/descriptives.py` & `decide-exchange-model-2022.1.9/decide/results/descriptives.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 import os
 
 import pandas as pd
-from pandas.errors import DataError
+from pandas.core.base import DataError
 
 from decide import data_folder
 from decide.data.database import connection, Manager
 from decide.results.helpers import list_to_sql_param, handle_data_frame
 
 pd.set_option('display.max_rows', 500)
 pd.set_option('display.max_columns', 500)
```

### Comparing `decide_exchange_model-2022.1.18/decide/results/externalities.py` & `decide-exchange-model-2022.1.9/decide/results/externalities.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 import os
 
 import pandas as pd
-from pandas.errors import DataError
+from pandas.core.base import DataError
 
 from decide import data_folder
 from decide.data.database import connection, Manager
 from decide.results.helpers import list_to_sql_param, handle_data_frame
 
 pd.set_option('display.max_rows', 500)
 pd.set_option('display.max_columns', 500)
```

### Comparing `decide_exchange_model-2022.1.18/decide/results/helpers.py` & `decide-exchange-model-2022.1.9/decide/results/helpers.py`

 * *Files identical despite different names*

### Comparing `decide_exchange_model-2022.1.18/decide/results/issuecomparison.py` & `decide-exchange-model-2022.1.9/decide/results/issuecomparison.py`

 * *Files identical despite different names*

### Comparing `decide_exchange_model-2022.1.18/decide/results/nashbargainingsolution.py` & `decide-exchange-model-2022.1.9/decide/results/nashbargainingsolution.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,19 +17,22 @@
     df = pd.read_sql(
         """
     SELECT
       a.p as p,
       a.issue as issue,
       a.round as round,
       a.repetion as repetion,
-      a.numerator / a.denominator AS mds
+      (a.numerator / a.denominator) / a.step_size + a.lower AS mds
     FROM (SELECT
             sum(ai.position * ai.power * ai.salience) AS numerator,
             sum(ai.salience * ai.power)               AS denominator,
             r.pointer                                 AS repetion,
+            i.lower as lower,
+            i.upper as upper,            
+            100 / (i.upper - i.lower) as step_size,
             i2.pointer + 1                                AS round,
             m.p,
       i.name as issue
           FROM actorissue ai
             LEFT JOIN issue i ON ai.issue_id = i.id
             LEFT JOIN actor a ON ai.actor_id = a.id
             LEFT JOIN iteration i2 ON ai.iteration_id = i2.id
```

### Comparing `decide_exchange_model-2022.1.18/decide/tests/cli_test.py` & `decide-exchange-model-2022.1.9/decide/tests/cli_test.py`

 * *Files identical despite different names*

### Comparing `decide_exchange_model-2022.1.18/decide/tests/test_rex.py` & `decide-exchange-model-2022.1.9/decide/tests/test_rex.py`

 * *Files identical despite different names*

### Comparing `decide_exchange_model-2022.1.18/decide/utils.py` & `decide-exchange-model-2022.1.9/decide/utils.py`

 * *Files identical despite different names*

### Comparing `decide_exchange_model-2022.1.18/PKG-INFO` & `decide-exchange-model-2022.1.9/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,19 @@
 Metadata-Version: 2.1
 Name: decide-exchange-model
-Version: 2022.1.18
-Summary: Decide exchange model
-Author: Jelmer Draaijer
+Version: 2022.1.9
+Summary: Model of collective decision making
+Home-page: https://github.com/foarsitter/decide-exchange-model
+Author: jelmert
 Author-email: info@jelmert.nl
-Requires-Python: >=3.9,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: PyQt5 (==5.12.3)
-Requires-Dist: blinker (==1.5)
-Requires-Dist: matplotlib (==3.6.0)
-Requires-Dist: numpy (==1.23.4)
-Requires-Dist: pandas (==1.5.0)
-Requires-Dist: peewee (==3.14.4)
-Requires-Dist: typesystem (==0.2.2)
+License: GPL-3.0
+Description: [![Build Status](https://travis-ci.org/foarsitter/decide-exchange-model.svg?branch=master)](https://travis-ci.org/foarsitter/decide-exchange-model)
+        [![Code Climate](https://codeclimate.com/github/foarsitter/decide-exchange-model/badges/gpa.svg)](https://codeclimate.com/github/foarsitter/decide-exchange-model)
+        [![Test Coverage](https://codeclimate.com/github/foarsitter/decide-exchange-model/badges/coverage.svg)](https://codeclimate.com/github/foarsitter/decide-exchange-model/coverage)
+        [![PyPI](https://img.shields.io/pypi/v/decide-exchange-model.svg)](https://pypi.org/project/decide-exchange-model/)
+        [![Anaconda-Server Badge](https://anaconda.org/jelmert/decide-exchange-model/badges/version.svg)](https://anaconda.org/jelmert/decide-exchange-model)
+        [![Issue Count](https://codeclimate.com/github/foarsitter/decide-exchange-model/badges/issue_count.svg)](https://codeclimate.com/github/foarsitter/decide-exchange-model)
+        
+        # Decide Exchange Model
+        Equal Gain Model implementation in the Python programming language. Read the documentation on https://foarsitter.github.io/decide-exchange-model/
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
-
-[![Build Status](https://travis-ci.org/foarsitter/decide-exchange-model.svg?branch=master)](https://travis-ci.org/foarsitter/decide-exchange-model)
-[![Code Climate](https://codeclimate.com/github/foarsitter/decide-exchange-model/badges/gpa.svg)](https://codeclimate.com/github/foarsitter/decide-exchange-model)
-[![Test Coverage](https://codeclimate.com/github/foarsitter/decide-exchange-model/badges/coverage.svg)](https://codeclimate.com/github/foarsitter/decide-exchange-model/coverage)
-[![PyPI](https://img.shields.io/pypi/v/decide-exchange-model.svg)](https://pypi.org/project/decide-exchange-model/)
-[![Anaconda-Server Badge](https://anaconda.org/jelmert/decide-exchange-model/badges/version.svg)](https://anaconda.org/jelmert/decide-exchange-model)
-[![Issue Count](https://codeclimate.com/github/foarsitter/decide-exchange-model/badges/issue_count.svg)](https://codeclimate.com/github/foarsitter/decide-exchange-model)
-
-# Decide Exchange Model
-Equal Gain Model implementation in the Python programming language. Read the documentation on https://foarsitter.github.io/decide-exchange-model/
```

