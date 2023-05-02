# Comparing `tmp/OctoBot-Backtesting-1.8.2.tar.gz` & `tmp/OctoBot-Backtesting-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OctoBot-Backtesting-1.8.2.tar", last modified: Sat Apr 22 08:49:51 2023, max compression
+gzip compressed data, was "OctoBot-Backtesting-1.9.0.tar", last modified: Tue May  2 20:33:28 2023, max compression
```

## Comparing `OctoBot-Backtesting-1.8.2.tar` & `OctoBot-Backtesting-1.9.0.tar`

### file list

```diff
@@ -1,116 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:51.325968 OctoBot-Backtesting-1.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)     8311 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:51.317968 OctoBot-Backtesting-1.8.2/OctoBot_Backtesting.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-22 08:49:51.000000 OctoBot-Backtesting-1.8.2/OctoBot_Backtesting.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-04-22 08:49:51.000000 OctoBot-Backtesting-1.8.2/OctoBot_Backtesting.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 08:49:51.000000 OctoBot-Backtesting-1.8.2/OctoBot_Backtesting.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 08:49:51.000000 OctoBot-Backtesting-1.8.2/OctoBot_Backtesting.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-22 08:49:51.000000 OctoBot-Backtesting-1.8.2/OctoBot_Backtesting.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-22 08:49:51.000000 OctoBot-Backtesting-1.8.2/OctoBot_Backtesting.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-22 08:49:51.325968 OctoBot-Backtesting-1.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:51.317968 OctoBot-Backtesting-1.8.2/octobot_backtesting/
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:51.317968 OctoBot-Backtesting-1.8.2/octobot_backtesting/api/
--rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10582 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/api/backtesting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/api/data_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/api/data_file_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/api/exchange_data_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/api/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/backtest_data.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/backtest_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/backtesting.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/backtesting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/channels_manager.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/channels_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:51.317968 OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/data_collector.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/data_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:51.321968 OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/exchanges/
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/exchanges/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/exchanges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/exchanges/abstract_exchange_bot_snapshot_collector.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/exchanges/abstract_exchange_bot_snapshot_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/exchanges/abstract_exchange_history_collector.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/exchanges/abstract_exchange_history_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/exchanges/abstract_exchange_live_collector.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/exchanges/abstract_exchange_live_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/exchanges/exchange_collector.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     8622 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/exchanges/exchange_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:51.321968 OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/social/
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/social/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/social/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/social/social_collector.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/social/social_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:51.321968 OctoBot-Backtesting-1.8.2/octobot_backtesting/converters/
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/converters/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/converters/data_converter.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/converters/data_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:51.321968 OctoBot-Backtesting-1.8.2/octobot_backtesting/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/data/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/data/data_file_manager.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/data/data_file_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:51.321968 OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/data_importer.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/data_importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:51.321968 OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/exchanges/
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/exchanges/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/exchanges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/exchanges/exchange_importer.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    13833 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/exchanges/exchange_importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/exchanges/util.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/exchanges/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:51.321968 OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/social/
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/social/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/social/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/social/social_importer.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/social/social_importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:51.325968 OctoBot-Backtesting-1.8.2/octobot_backtesting/time/
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/time/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/time/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:51.325968 OctoBot-Backtesting-1.8.2/octobot_backtesting/time/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/time/channel/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/time/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/time/channel/time.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/time/channel/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/time/channel/time_updater.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/time/channel/time_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/time/time_manager.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/time/time_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:51.325968 OctoBot-Backtesting-1.8.2/octobot_backtesting/util/
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/util/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/util/backtesting_util.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/util/backtesting_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 08:49:51.325968 OctoBot-Backtesting-1.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:51.313968 OctoBot-Backtesting-1.8.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:51.325968 OctoBot-Backtesting-1.8.2/tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/tests/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/tests/api/test_backtesting.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/tests/api/test_data_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/tests/api/test_data_file_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/tests/api/test_exchange_data_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/tests/api/test_importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:51.325968 OctoBot-Backtesting-1.8.2/tests/importers/
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/tests/importers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/tests/importers/test_exchange_importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:51.325968 OctoBot-Backtesting-1.8.2/tests/producers/
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/tests/producers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:51.325968 OctoBot-Backtesting-1.8.2/tests/util/
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/tests/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/tests/util/test_backtesting_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:33:28.268707 OctoBot-Backtesting-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     8397 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:33:28.260707 OctoBot-Backtesting-1.9.0/OctoBot_Backtesting.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-02 20:33:28.000000 OctoBot-Backtesting-1.9.0/OctoBot_Backtesting.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-05-02 20:33:28.000000 OctoBot-Backtesting-1.9.0/OctoBot_Backtesting.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 20:33:28.000000 OctoBot-Backtesting-1.9.0/OctoBot_Backtesting.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 20:33:28.000000 OctoBot-Backtesting-1.9.0/OctoBot_Backtesting.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-02 20:33:28.000000 OctoBot-Backtesting-1.9.0/OctoBot_Backtesting.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-02 20:33:28.000000 OctoBot-Backtesting-1.9.0/OctoBot_Backtesting.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-02 20:33:28.268707 OctoBot-Backtesting-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:33:28.260707 OctoBot-Backtesting-1.9.0/octobot_backtesting/
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/octobot_backtesting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:33:28.260707 OctoBot-Backtesting-1.9.0/octobot_backtesting/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/octobot_backtesting/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10582 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/octobot_backtesting/api/backtesting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/octobot_backtesting/api/data_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/octobot_backtesting/api/data_file_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/octobot_backtesting/api/exchange_data_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/octobot_backtesting/api/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/octobot_backtesting/backtest_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/octobot_backtesting/backtesting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/octobot_backtesting/channels_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:33:28.260707 OctoBot-Backtesting-1.9.0/octobot_backtesting/collectors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/octobot_backtesting/collectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/octobot_backtesting/collectors/data_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:33:28.264706 OctoBot-Backtesting-1.9.0/octobot_backtesting/collectors/exchanges/
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/octobot_backtesting/collectors/exchanges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/octobot_backtesting/collectors/exchanges/abstract_exchange_bot_snapshot_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/octobot_backtesting/collectors/exchanges/abstract_exchange_history_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/octobot_backtesting/collectors/exchanges/abstract_exchange_live_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8622 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/octobot_backtesting/collectors/exchanges/exchange_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:33:28.264706 OctoBot-Backtesting-1.9.0/octobot_backtesting/collectors/social/
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/octobot_backtesting/collectors/social/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/octobot_backtesting/collectors/social/social_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/octobot_backtesting/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:33:28.264706 OctoBot-Backtesting-1.9.0/octobot_backtesting/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/octobot_backtesting/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/octobot_backtesting/converters/data_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:33:28.264706 OctoBot-Backtesting-1.9.0/octobot_backtesting/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/octobot_backtesting/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/octobot_backtesting/data/data_file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/octobot_backtesting/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/octobot_backtesting/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:33:28.264706 OctoBot-Backtesting-1.9.0/octobot_backtesting/importers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/octobot_backtesting/importers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/octobot_backtesting/importers/data_importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:33:28.264706 OctoBot-Backtesting-1.9.0/octobot_backtesting/importers/exchanges/
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/octobot_backtesting/importers/exchanges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13833 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/octobot_backtesting/importers/exchanges/exchange_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/octobot_backtesting/importers/exchanges/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:33:28.264706 OctoBot-Backtesting-1.9.0/octobot_backtesting/importers/social/
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/octobot_backtesting/importers/social/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/octobot_backtesting/importers/social/social_importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:33:28.264706 OctoBot-Backtesting-1.9.0/octobot_backtesting/time/
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/octobot_backtesting/time/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:33:28.264706 OctoBot-Backtesting-1.9.0/octobot_backtesting/time/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/octobot_backtesting/time/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/octobot_backtesting/time/channel/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/octobot_backtesting/time/channel/time_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/octobot_backtesting/time/time_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:33:28.264706 OctoBot-Backtesting-1.9.0/octobot_backtesting/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/octobot_backtesting/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/octobot_backtesting/util/backtesting_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 20:33:28.268707 OctoBot-Backtesting-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:33:28.256706 OctoBot-Backtesting-1.9.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:33:28.268707 OctoBot-Backtesting-1.9.0/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/tests/api/test_backtesting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/tests/api/test_data_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/tests/api/test_data_file_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/tests/api/test_exchange_data_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/tests/api/test_importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:33:28.268707 OctoBot-Backtesting-1.9.0/tests/importers/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/tests/importers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/tests/importers/test_exchange_importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:33:28.268707 OctoBot-Backtesting-1.9.0/tests/producers/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/tests/producers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:33:28.268707 OctoBot-Backtesting-1.9.0/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/tests/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-02 20:32:22.000000 OctoBot-Backtesting-1.9.0/tests/util/test_backtesting_util.py
```

### Comparing `OctoBot-Backtesting-1.8.2/CHANGELOG.md` & `OctoBot-Backtesting-1.9.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

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
 ## [1.8.2] - 2022-04-21
 ### Updated
 - [ExchangeCollector] handle exchange credentials
 
 ## [1.8.1] - 2022-04-17
 ### Updated
 - [ExchangeCollector] delete_all
```

### Comparing `OctoBot-Backtesting-1.8.2/LICENSE` & `OctoBot-Backtesting-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.2/OctoBot_Backtesting.egg-info/PKG-INFO` & `OctoBot-Backtesting-1.9.0/OctoBot_Backtesting.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: OctoBot-Backtesting
-Version: 1.8.2
+Version: 1.9.0
 Summary: OctoBot project backtesting engine
 Home-page: https://github.com/Drakkar-Software/OctoBot-Backtesting
 Author: Drakkar-Software
-Author-email: drakkar-software@protonmail.com
+Author-email: contact@drakkar.software
 License: LGPL-3.0
-Description: UNKNOWN
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
```

### Comparing `OctoBot-Backtesting-1.8.2/OctoBot_Backtesting.egg-info/SOURCES.txt` & `OctoBot-Backtesting-1.9.0/OctoBot_Backtesting.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -6,84 +6,53 @@
 setup.py
 OctoBot_Backtesting.egg-info/PKG-INFO
 OctoBot_Backtesting.egg-info/SOURCES.txt
 OctoBot_Backtesting.egg-info/dependency_links.txt
 OctoBot_Backtesting.egg-info/not-zip-safe
 OctoBot_Backtesting.egg-info/requires.txt
 OctoBot_Backtesting.egg-info/top_level.txt
-octobot_backtesting/__init__.pxd
 octobot_backtesting/__init__.py
-octobot_backtesting/backtest_data.pxd
 octobot_backtesting/backtest_data.py
-octobot_backtesting/backtesting.pxd
 octobot_backtesting/backtesting.py
-octobot_backtesting/channels_manager.pxd
 octobot_backtesting/channels_manager.py
 octobot_backtesting/constants.py
 octobot_backtesting/enums.py
 octobot_backtesting/errors.py
 octobot_backtesting/api/__init__.py
 octobot_backtesting/api/backtesting.py
 octobot_backtesting/api/data_file.py
 octobot_backtesting/api/data_file_converters.py
 octobot_backtesting/api/exchange_data_collector.py
 octobot_backtesting/api/importer.py
-octobot_backtesting/collectors/__init__.pxd
 octobot_backtesting/collectors/__init__.py
-octobot_backtesting/collectors/data_collector.pxd
 octobot_backtesting/collectors/data_collector.py
-octobot_backtesting/collectors/exchanges/__init__.pxd
 octobot_backtesting/collectors/exchanges/__init__.py
-octobot_backtesting/collectors/exchanges/abstract_exchange_bot_snapshot_collector.pxd
 octobot_backtesting/collectors/exchanges/abstract_exchange_bot_snapshot_collector.py
-octobot_backtesting/collectors/exchanges/abstract_exchange_history_collector.pxd
 octobot_backtesting/collectors/exchanges/abstract_exchange_history_collector.py
-octobot_backtesting/collectors/exchanges/abstract_exchange_live_collector.pxd
 octobot_backtesting/collectors/exchanges/abstract_exchange_live_collector.py
-octobot_backtesting/collectors/exchanges/exchange_collector.pxd
 octobot_backtesting/collectors/exchanges/exchange_collector.py
-octobot_backtesting/collectors/social/__init__.pxd
 octobot_backtesting/collectors/social/__init__.py
-octobot_backtesting/collectors/social/social_collector.pxd
 octobot_backtesting/collectors/social/social_collector.py
-octobot_backtesting/converters/__init__.pxd
 octobot_backtesting/converters/__init__.py
-octobot_backtesting/converters/data_converter.pxd
 octobot_backtesting/converters/data_converter.py
-octobot_backtesting/data/__init__.pxd
 octobot_backtesting/data/__init__.py
-octobot_backtesting/data/data_file_manager.pxd
 octobot_backtesting/data/data_file_manager.py
-octobot_backtesting/importers/__init__.pxd
 octobot_backtesting/importers/__init__.py
-octobot_backtesting/importers/data_importer.pxd
 octobot_backtesting/importers/data_importer.py
-octobot_backtesting/importers/exchanges/__init__.pxd
 octobot_backtesting/importers/exchanges/__init__.py
-octobot_backtesting/importers/exchanges/exchange_importer.pxd
 octobot_backtesting/importers/exchanges/exchange_importer.py
-octobot_backtesting/importers/exchanges/util.pxd
 octobot_backtesting/importers/exchanges/util.py
-octobot_backtesting/importers/social/__init__.pxd
 octobot_backtesting/importers/social/__init__.py
-octobot_backtesting/importers/social/social_importer.pxd
 octobot_backtesting/importers/social/social_importer.py
-octobot_backtesting/time/__init__.pxd
 octobot_backtesting/time/__init__.py
-octobot_backtesting/time/time_manager.pxd
 octobot_backtesting/time/time_manager.py
-octobot_backtesting/time/channel/__init__.pxd
 octobot_backtesting/time/channel/__init__.py
-octobot_backtesting/time/channel/time.pxd
 octobot_backtesting/time/channel/time.py
-octobot_backtesting/time/channel/time_updater.pxd
 octobot_backtesting/time/channel/time_updater.py
-octobot_backtesting/util/__init__.pxd
 octobot_backtesting/util/__init__.py
-octobot_backtesting/util/backtesting_util.pxd
 octobot_backtesting/util/backtesting_util.py
 tests/api/__init__.py
 tests/api/test_backtesting.py
 tests/api/test_data_file.py
 tests/api/test_data_file_converters.py
 tests/api/test_exchange_data_collector.py
 tests/api/test_importer.py
```

### Comparing `OctoBot-Backtesting-1.8.2/PKG-INFO` & `OctoBot-Backtesting-1.9.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: OctoBot-Backtesting
-Version: 1.8.2
+Version: 1.9.0
 Summary: OctoBot project backtesting engine
 Home-page: https://github.com/Drakkar-Software/OctoBot-Backtesting
 Author: Drakkar-Software
-Author-email: drakkar-software@protonmail.com
+Author-email: contact@drakkar.software
 License: LGPL-3.0
-Description: UNKNOWN
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
```

### Comparing `OctoBot-Backtesting-1.8.2/README.md` & `OctoBot-Backtesting-1.9.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# OctoBot-Backtesting [1.8.2](https://github.com/Drakkar-Software/OctoBot-Backtesting/blob/master/CHANGELOG.md)
+# OctoBot-Backtesting [1.9.0](https://github.com/Drakkar-Software/OctoBot-Backtesting/blob/master/CHANGELOG.md)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/aa0b156e99604b3c98923fffeaea6a49)](https://app.codacy.com/gh/Drakkar-Software/OctoBot-Backtesting?utm_source=github.com&utm_medium=referral&utm_content=Drakkar-Software/OctoBot-Backtesting&utm_campaign=Badge_Grade_Dashboard)
 [![PyPI](https://img.shields.io/pypi/v/OctoBot-Backtesting.svg)](https://pypi.python.org/pypi/OctoBot-Backtesting/)
 [![Coverage Status](https://coveralls.io/repos/github/Drakkar-Software/OctoBot-Backtesting/badge.svg?branch=master)](https://coveralls.io/github/Drakkar-Software/OctoBot-Backtesting?branch=master)
 [![Github-Action-CI](https://github.com/Drakkar-Software/OctoBot-Backtesting/workflows/OctoBot-Backtesting-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot-Backtesting/actions)
 [![Build Status](https://cloud.drone.io/api/badges/Drakkar-Software/OctoBot-Backtesting/status.svg)](https://cloud.drone.io/Drakkar-Software/OctoBot-Backtesting)
 
 OctoBot backtesting engine package.
```

### Comparing `OctoBot-Backtesting-1.8.2/octobot_backtesting/__init__.pxd` & `OctoBot-Backtesting-1.9.0/tests/api/test_exchange_data_collector.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# cython: language_level=3
 #  Drakkar-Software OctoBot-Backtesting
 #  Copyright (c) Drakkar-Software, All rights reserved.
 #
 #  This library is free software; you can redistribute it and/or
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
@@ -10,7 +9,12 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
+import octobot_backtesting.api as api
+
+
+def test_import():
+    assert api.exchange_historical_data_collector_factory is not None
```

### Comparing `OctoBot-Backtesting-1.8.2/octobot_backtesting/__init__.py` & `OctoBot-Backtesting-1.9.0/octobot_backtesting/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,10 +12,10 @@
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 import logging
 
 PROJECT_NAME = "OctoBot-Backtesting"
-VERSION = "1.8.2"
+VERSION = "1.9.0"
 
 logging.getLogger('aiosqlite').setLevel(logging.ERROR)
```

### Comparing `OctoBot-Backtesting-1.8.2/octobot_backtesting/api/__init__.py` & `OctoBot-Backtesting-1.9.0/octobot_backtesting/api/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.2/octobot_backtesting/api/backtesting.py` & `OctoBot-Backtesting-1.9.0/octobot_backtesting/api/backtesting.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.2/octobot_backtesting/api/data_file.py` & `OctoBot-Backtesting-1.9.0/octobot_backtesting/api/data_file.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.2/octobot_backtesting/api/data_file_converters.py` & `OctoBot-Backtesting-1.9.0/octobot_backtesting/api/data_file_converters.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.2/octobot_backtesting/api/exchange_data_collector.py` & `OctoBot-Backtesting-1.9.0/octobot_backtesting/api/exchange_data_collector.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.2/octobot_backtesting/api/importer.py` & `OctoBot-Backtesting-1.9.0/octobot_backtesting/api/importer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.2/octobot_backtesting/backtest_data.pxd` & `OctoBot-Backtesting-1.9.0/octobot_backtesting/importers/social/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,17 @@
-# cython: language_level=3
 #  Drakkar-Software OctoBot-Backtesting
 #  Copyright (c) Drakkar-Software, All rights reserved.
 #
 #  This library is free software; you can redistribute it and/or
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
 #
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-#  Lesser General License for more details.
+#  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 
-cdef class BacktestData:
-    cdef public list data_files
-    cdef public object config
-    cdef public object tentacles_config
-    cdef public dict importers_by_data_file
-    cdef public dict preloaded_candle_managers
-    cdef public object default_importer
+from octobot_backtesting.importers.social import social_importer
```

### Comparing `OctoBot-Backtesting-1.8.2/octobot_backtesting/backtest_data.py` & `OctoBot-Backtesting-1.9.0/octobot_backtesting/backtest_data.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.2/octobot_backtesting/backtesting.py` & `OctoBot-Backtesting-1.9.0/octobot_backtesting/backtesting.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.2/octobot_backtesting/channels_manager.py` & `OctoBot-Backtesting-1.9.0/octobot_backtesting/channels_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/__init__.pxd` & `OctoBot-Backtesting-1.9.0/octobot_backtesting/collectors/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# cython: language_level=3
 #  Drakkar-Software OctoBot-Backtesting
 #  Copyright (c) Drakkar-Software, All rights reserved.
 #
 #  This library is free software; you can redistribute it and/or
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
@@ -11,29 +10,29 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 
-from octobot_backtesting.collectors cimport data_collector
-from octobot_backtesting.collectors.data_collector cimport (
+from octobot_backtesting.collectors import data_collector
+from octobot_backtesting.collectors.data_collector import (
     DataCollector,
 )
 
-from octobot_backtesting.collectors cimport exchanges
-from octobot_backtesting.collectors.exchanges cimport (
+from octobot_backtesting.collectors import exchanges
+from octobot_backtesting.collectors.exchanges import (
     ExchangeDataCollector,
     AbstractExchangeBotSnapshotCollector,
     AbstractExchangeHistoryCollector,
     AbstractExchangeLiveCollector,
 )
 
-from octobot_backtesting.collectors cimport social
-from octobot_backtesting.collectors.social cimport (
+from octobot_backtesting.collectors import social
+from octobot_backtesting.collectors.social import (
     SocialDataCollector,
 )
 
 
 __all__ = [
     "DataCollector",
     "ExchangeDataCollector",
```

### Comparing `OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/__init__.py` & `OctoBot-Backtesting-1.9.0/octobot_backtesting/collectors/exchanges/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,34 +10,32 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 
-from octobot_backtesting.collectors import data_collector
-from octobot_backtesting.collectors.data_collector import (
-    DataCollector,
+from octobot_backtesting.collectors.exchanges import exchange_collector
+from octobot_backtesting.collectors.exchanges.exchange_collector import (
+    ExchangeDataCollector,
 )
 
-from octobot_backtesting.collectors import exchanges
-from octobot_backtesting.collectors.exchanges import (
-    ExchangeDataCollector,
+from octobot_backtesting.collectors.exchanges import abstract_exchange_bot_snapshot_collector
+from octobot_backtesting.collectors.exchanges import abstract_exchange_history_collector
+from octobot_backtesting.collectors.exchanges import abstract_exchange_live_collector
+
+from octobot_backtesting.collectors.exchanges.abstract_exchange_bot_snapshot_collector import (
     AbstractExchangeBotSnapshotCollector,
+)
+from octobot_backtesting.collectors.exchanges.abstract_exchange_history_collector import (
     AbstractExchangeHistoryCollector,
-    AbstractExchangeLiveCollector,
 )
-
-from octobot_backtesting.collectors import social
-from octobot_backtesting.collectors.social import (
-    SocialDataCollector,
+from octobot_backtesting.collectors.exchanges.abstract_exchange_live_collector import (
+    AbstractExchangeLiveCollector,
 )
 
-
 __all__ = [
-    "DataCollector",
     "ExchangeDataCollector",
     "AbstractExchangeBotSnapshotCollector",
     "AbstractExchangeHistoryCollector",
     "AbstractExchangeLiveCollector",
-    "SocialDataCollector",
 ]
```

### Comparing `OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/data_collector.py` & `OctoBot-Backtesting-1.9.0/octobot_backtesting/collectors/data_collector.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/exchanges/abstract_exchange_bot_snapshot_collector.pxd` & `OctoBot-Backtesting-1.9.0/octobot_backtesting/collectors/exchanges/abstract_exchange_bot_snapshot_collector.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# cython: language_level=3
 #  Drakkar-Software OctoBot-Backtesting
 #  Copyright (c) Drakkar-Software, All rights reserved.
 #
 #  This library is free software; you can redistribute it and/or
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
@@ -10,12 +9,12 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-cimport octobot_backtesting.collectors.exchanges as exchanges
+import octobot_backtesting.collectors.exchanges as exchanges
 
 
-cdef class AbstractExchangeBotSnapshotCollector(exchanges.ExchangeDataCollector):
+class AbstractExchangeBotSnapshotCollector(exchanges.ExchangeDataCollector):
     pass
```

### Comparing `OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/exchanges/abstract_exchange_bot_snapshot_collector.py` & `OctoBot-Backtesting-1.9.0/octobot_backtesting/collectors/exchanges/abstract_exchange_live_collector.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,12 +9,12 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-import octobot_backtesting.collectors.exchanges as exchanges
+import octobot_backtesting.collectors.exchanges.exchange_collector as exchange_collector
 
 
-class AbstractExchangeBotSnapshotCollector(exchanges.ExchangeDataCollector):
+class AbstractExchangeLiveCollector(exchange_collector.ExchangeDataCollector):
     pass
```

### Comparing `OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/exchanges/abstract_exchange_history_collector.pxd` & `OctoBot-Backtesting-1.9.0/octobot_backtesting/collectors/exchanges/abstract_exchange_history_collector.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-# cython: language_level=3
-#  Drakkar-Software OctoBot-Backtesting
+#  Drakkar-Software OctoBot
 #  Copyright (c) Drakkar-Software, All rights reserved.
 #
 #  This library is free software; you can redistribute it and/or
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
 #
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-cimport octobot_backtesting.collectors.exchanges as exchanges
+import octobot_backtesting.collectors.exchanges as exchanges
 
 
-cdef class AbstractExchangeHistoryCollector(exchanges.ExchangeDataCollector):
+class AbstractExchangeHistoryCollector(exchanges.ExchangeDataCollector):
     pass
```

### Comparing `OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/exchanges/abstract_exchange_history_collector.py` & `OctoBot-Backtesting-1.9.0/octobot_backtesting/collectors/social/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,25 @@
-#  Drakkar-Software OctoBot
+#  Drakkar-Software OctoBot-Backtesting
 #  Copyright (c) Drakkar-Software, All rights reserved.
 #
 #  This library is free software; you can redistribute it and/or
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
 #
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-import octobot_backtesting.collectors.exchanges as exchanges
 
+from octobot_backtesting.collectors.social import social_collector
 
-class AbstractExchangeHistoryCollector(exchanges.ExchangeDataCollector):
-    pass
+from octobot_backtesting.collectors.social.social_collector import (
+    SocialDataCollector,
+)
+
+__all__ = [
+    "SocialDataCollector",
+]
```

### Comparing `OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/exchanges/abstract_exchange_live_collector.py` & `OctoBot-Backtesting-1.9.0/octobot_backtesting/converters/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,12 +9,17 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-import octobot_backtesting.collectors.exchanges.exchange_collector as exchange_collector
 
+from octobot_backtesting.converters import data_converter
 
-class AbstractExchangeLiveCollector(exchange_collector.ExchangeDataCollector):
-    pass
+from octobot_backtesting.converters.data_converter import (
+    DataConverter,
+)
+
+__all__ = [
+    "DataConverter",
+]
```

### Comparing `OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/exchanges/exchange_collector.py` & `OctoBot-Backtesting-1.9.0/octobot_backtesting/collectors/exchanges/exchange_collector.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/social/__init__.pxd` & `OctoBot-Backtesting-1.9.0/octobot_backtesting/collectors/social/social_collector.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,30 @@
-# cython: language_level=3
-#  Drakkar-Software OctoBot-Backtesting
+#  Drakkar-Software OctoBot
 #  Copyright (c) Drakkar-Software, All rights reserved.
 #
 #  This library is free software; you can redistribute it and/or
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
 #
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
+import octobot_backtesting.collectors as collectors
 
-from octobot_backtesting.collectors.social cimport social_collector
 
-from octobot_backtesting.collectors.social.social_collector cimport (
-    SocialDataCollector,
-)
+class SocialDataCollector(collectors.DataCollector):
+    # IMPORTER = SocialDataImporter
 
-__all__ = [
-    "SocialDataCollector",
-]
+    def __init__(self, config, social_name):
+        super().__init__(config)
+        self.social_name = social_name
+        self.set_file_path()
+
+    async def initialize(self):
+        self.create_database()
+
+        # TODO initialize with service
```

### Comparing `OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/social/__init__.py` & `OctoBot-Backtesting-1.9.0/tests/api/test_importer.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,17 +9,12 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
+import octobot_backtesting.api as api
 
-from octobot_backtesting.collectors.social import social_collector
 
-from octobot_backtesting.collectors.social.social_collector import (
-    SocialDataCollector,
-)
-
-__all__ = [
-    "SocialDataCollector",
-]
+def test_import():
+    assert api.get_data_timestamp_interval is not None
```

### Comparing `OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/social/social_collector.pxd` & `OctoBot-Backtesting-1.9.0/octobot_backtesting/util/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,27 @@
-# cython: language_level=3
 #  Drakkar-Software OctoBot-Backtesting
 #  Copyright (c) Drakkar-Software, All rights reserved.
 #
 #  This library is free software; you can redistribute it and/or
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
 #
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-#  Lesser General License for more details.
+#  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 
-cimport octobot_backtesting.collectors as collectors
+from octobot_backtesting.util import backtesting_util
 
+from octobot_backtesting.util.backtesting_util import (
+    create_importer_from_backtesting_file_name,
+    get_default_importer,
+)
 
-cdef class SocialDataCollector(collectors.DataCollector):
-    cdef public str social_name
+__all__ = [
+    "create_importer_from_backtesting_file_name",
+    "get_default_importer",
+]
```

### Comparing `OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/social/social_collector.py` & `OctoBot-Backtesting-1.9.0/octobot_backtesting/errors.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-#  Drakkar-Software OctoBot
+#  Drakkar-Software OctoBot-Backtesting
 #  Copyright (c) Drakkar-Software, All rights reserved.
 #
 #  This library is free software; you can redistribute it and/or
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
 #
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-import octobot_backtesting.collectors as collectors
 
+class DataCollectorError(Exception):
+    pass
 
-class SocialDataCollector(collectors.DataCollector):
-    # IMPORTER = SocialDataImporter
 
-    def __init__(self, config, social_name):
-        super().__init__(config)
-        self.social_name = social_name
-        self.set_file_path()
+class IncompatibleDatafileError(Exception):
+    pass
 
-    async def initialize(self):
-        self.create_database()
 
-        # TODO initialize with service
+class MissingTimeFrame(Exception):
+    pass
+
+
+class BacktestingFileNotFound(Exception):
+    pass
```

### Comparing `OctoBot-Backtesting-1.8.2/octobot_backtesting/constants.py` & `OctoBot-Backtesting-1.9.0/octobot_backtesting/constants.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.2/octobot_backtesting/converters/__init__.py` & `OctoBot-Backtesting-1.9.0/octobot_backtesting/time/channel/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,16 +10,25 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 
-from octobot_backtesting.converters import data_converter
+from octobot_backtesting.time.channel import time
+from octobot_backtesting.time.channel import time_updater
 
-from octobot_backtesting.converters.data_converter import (
-    DataConverter,
+from octobot_backtesting.time.channel.time import (
+    TimeProducer,
+    TimeConsumer,
+    TimeChannel,
+)
+from octobot_backtesting.time.channel.time_updater import (
+    TimeUpdater,
 )
 
 __all__ = [
-    "DataConverter",
+    "TimeProducer",
+    "TimeConsumer",
+    "TimeChannel",
+    "TimeUpdater",
 ]
```

### Comparing `OctoBot-Backtesting-1.8.2/octobot_backtesting/converters/data_converter.pxd` & `OctoBot-Backtesting-1.9.0/octobot_backtesting/importers/social/social_importer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,15 @@
-# cython: language_level=3
 #  Drakkar-Software OctoBot-Backtesting
 #  Copyright (c) Drakkar-Software, All rights reserved.
 #
 #  This library is free software; you can redistribute it and/or
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
 #
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-#  Lesser General License for more details.
+#  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-
-cdef class DataConverter:
-    cdef object logger
-    cdef public str file_to_convert
-    cdef public str converted_file
```

### Comparing `OctoBot-Backtesting-1.8.2/octobot_backtesting/converters/data_converter.py` & `OctoBot-Backtesting-1.9.0/octobot_backtesting/converters/data_converter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.2/octobot_backtesting/data/__init__.py` & `OctoBot-Backtesting-1.9.0/octobot_backtesting/data/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.2/octobot_backtesting/data/data_file_manager.pxd` & `OctoBot-Backtesting-1.9.0/tests/api/test_data_file.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,20 @@
-# cython: language_level=3
 #  Drakkar-Software OctoBot-Backtesting
 #  Copyright (c) Drakkar-Software, All rights reserved.
 #
 #  This library is free software; you can redistribute it and/or
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
 #
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-#  Lesser General License for more details.
+#  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
+from octobot_backtesting.api.data_file import get_all_available_data_files
 
-cpdef object get_data_type(str file_name)
-cpdef str get_file_ending(object data_type)
-cpdef str get_date(int time_info)
-cpdef bint is_valid_ending(str ending)
-cpdef list get_all_available_data_files(str data_collector_path)
-cpdef object delete_data_file(str data_collector_path, str file_name)
+
+def test_get_all_available_data_files():
+    assert get_all_available_data_files() == []
```

### Comparing `OctoBot-Backtesting-1.8.2/octobot_backtesting/data/data_file_manager.py` & `OctoBot-Backtesting-1.9.0/octobot_backtesting/data/data_file_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.2/octobot_backtesting/enums.py` & `OctoBot-Backtesting-1.9.0/octobot_backtesting/enums.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.2/octobot_backtesting/errors.py` & `OctoBot-Backtesting-1.9.0/octobot_backtesting/time/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,22 +9,28 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
+from octobot_backtesting.time import time_manager
+from octobot_backtesting.time import channel
 
-class DataCollectorError(Exception):
-    pass
-
-
-class IncompatibleDatafileError(Exception):
-    pass
-
-
-class MissingTimeFrame(Exception):
-    pass
-
-
-class BacktestingFileNotFound(Exception):
-    pass
+from octobot_backtesting.time.time_manager import (
+    TimeManager,
+)
+
+from octobot_backtesting.time.channel import (
+    TimeProducer,
+    TimeConsumer,
+    TimeChannel,
+    TimeUpdater,
+)
+
+__all__ = [
+    "TimeManager",
+    "TimeProducer",
+    "TimeConsumer",
+    "TimeChannel",
+    "TimeUpdater",
+]
```

### Comparing `OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/__init__.pxd` & `OctoBot-Backtesting-1.9.0/octobot_backtesting/importers/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# cython: language_level=3
 #  Drakkar-Software OctoBot-Backtesting
 #  Copyright (c) Drakkar-Software, All rights reserved.
 #
 #  This library is free software; you can redistribute it and/or
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
@@ -11,23 +10,23 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 
-from octobot_backtesting.importers cimport data_importer
-from octobot_backtesting.importers.data_importer cimport (
+from octobot_backtesting.importers import data_importer
+from octobot_backtesting.importers.data_importer import (
     DataImporter,
 )
 
-from octobot_backtesting.importers cimport social
-from octobot_backtesting.importers cimport exchanges
+from octobot_backtesting.importers import social
+from octobot_backtesting.importers import exchanges
 
-from octobot_backtesting.importers.exchanges cimport (
+from octobot_backtesting.importers.exchanges import (
     ExchangeDataImporter,
     get_operations_from_timestamps,
     import_ohlcvs,
     import_tickers,
     import_order_books,
     import_recent_trades,
     import_klines,
```

### Comparing `OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/__init__.py` & `OctoBot-Backtesting-1.9.0/octobot_backtesting/importers/exchanges/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,34 +10,31 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 
-from octobot_backtesting.importers import data_importer
-from octobot_backtesting.importers.data_importer import (
-    DataImporter,
-)
-
-from octobot_backtesting.importers import social
-from octobot_backtesting.importers import exchanges
+from octobot_backtesting.importers.exchanges import exchange_importer
+from octobot_backtesting.importers.exchanges import util
 
-from octobot_backtesting.importers.exchanges import (
+from octobot_backtesting.importers.exchanges.exchange_importer import (
     ExchangeDataImporter,
+)
+
+from octobot_backtesting.importers.exchanges.util import (
     get_operations_from_timestamps,
     import_ohlcvs,
     import_tickers,
     import_order_books,
     import_recent_trades,
     import_klines,
 )
 
 __all__ = [
-    "DataImporter",
     "ExchangeDataImporter",
     "get_operations_from_timestamps",
     "import_ohlcvs",
     "import_tickers",
     "import_order_books",
     "import_recent_trades",
     "import_klines",
```

### Comparing `OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/data_importer.pxd` & `OctoBot-Backtesting-1.9.0/tests/api/test_data_file_converters.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,22 @@
-# cython: language_level=3
 #  Drakkar-Software OctoBot-Backtesting
 #  Copyright (c) Drakkar-Software, All rights reserved.
 #
 #  This library is free software; you can redistribute it and/or
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
 #
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-#  Lesser General License for more details.
+#  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-cimport octobot_commons.databases as databases
+import pytest
+from octobot_backtesting.api.data_file_converters import convert_data_file
 
-cdef class DataImporter:
-    cdef public dict config
 
-    cdef public object logger
-
-    cdef public bint should_stop
-
-    cdef public str version
-    cdef public str file_path
-
-    cdef public databases.SQLiteDatabase database
-
-    cpdef void load_database(self)
+@pytest.mark.asyncio
+async def test_convert_data_file_without_converter():
+    assert await convert_data_file(None) is None
```

### Comparing `OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/data_importer.py` & `OctoBot-Backtesting-1.9.0/octobot_backtesting/importers/data_importer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/exchanges/exchange_importer.py` & `OctoBot-Backtesting-1.9.0/octobot_backtesting/importers/exchanges/exchange_importer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/exchanges/util.py` & `OctoBot-Backtesting-1.9.0/octobot_backtesting/importers/exchanges/util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/social/__init__.pxd` & `OctoBot-Backtesting-1.9.0/tests/api/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# cython: language_level=3
 #  Drakkar-Software OctoBot-Backtesting
 #  Copyright (c) Drakkar-Software, All rights reserved.
 #
 #  This library is free software; you can redistribute it and/or
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
```

### Comparing `OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/social/__init__.py` & `OctoBot-Backtesting-1.9.0/tests/importers/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,9 +9,7 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-
-from octobot_backtesting.importers.social import social_importer
```

### Comparing `OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/social/social_importer.pxd` & `OctoBot-Backtesting-1.9.0/tests/producers/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-# cython: language_level=3
 #  Drakkar-Software OctoBot-Backtesting
 #  Copyright (c) Drakkar-Software, All rights reserved.
 #
 #  This library is free software; you can redistribute it and/or
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
 #
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-#  Lesser General License for more details.
+#  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
```

### Comparing `OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/social/social_importer.py` & `OctoBot-Backtesting-1.9.0/tests/util/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.2/octobot_backtesting/time/channel/__init__.py` & `OctoBot-Backtesting-1.9.0/tests/util/test_backtesting_util.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,26 +9,16 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
+import os
 
-from octobot_backtesting.time.channel import time
-from octobot_backtesting.time.channel import time_updater
+if not os.getenv('CYTHON_IGNORE'):
+    from octobot_backtesting.util.backtesting_util import _parse_class_name_from_backtesting_file
 
-from octobot_backtesting.time.channel.time import (
-    TimeProducer,
-    TimeConsumer,
-    TimeChannel,
-)
-from octobot_backtesting.time.channel.time_updater import (
-    TimeUpdater,
-)
 
-__all__ = [
-    "TimeProducer",
-    "TimeConsumer",
-    "TimeChannel",
-    "TimeUpdater",
-]
+def test_parse_class_name_from_backtesting_file():
+    if not os.getenv('CYTHON_IGNORE'):
+        assert _parse_class_name_from_backtesting_file("ExchangeHistoryDataCollector_1589740606.4862757") == "ExchangeHistoryDataCollector"
```

### Comparing `OctoBot-Backtesting-1.8.2/octobot_backtesting/time/channel/time.py` & `OctoBot-Backtesting-1.9.0/octobot_backtesting/time/channel/time.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.2/octobot_backtesting/time/channel/time_updater.py` & `OctoBot-Backtesting-1.9.0/octobot_backtesting/time/channel/time_updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.2/octobot_backtesting/time/time_manager.py` & `OctoBot-Backtesting-1.9.0/octobot_backtesting/time/time_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.2/octobot_backtesting/util/backtesting_util.py` & `OctoBot-Backtesting-1.9.0/octobot_backtesting/util/backtesting_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.2/tests/api/test_backtesting.py` & `OctoBot-Backtesting-1.9.0/tests/api/test_backtesting.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.2/tests/importers/test_exchange_importer.py` & `OctoBot-Backtesting-1.9.0/tests/importers/test_exchange_importer.py`

 * *Files identical despite different names*

