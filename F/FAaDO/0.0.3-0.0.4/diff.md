# Comparing `tmp/FAaDO-0.0.3.tar.gz` & `tmp/FAaDO-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FAaDO-0.0.3.tar", last modified: Tue May  2 15:15:51 2023, max compression
+gzip compressed data, was "FAaDO-0.0.4.tar", last modified: Tue May  2 17:36:27 2023, max compression
```

## Comparing `FAaDO-0.0.3.tar` & `FAaDO-0.0.4.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 15:15:51.540432 FAaDO-0.0.3/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 15:15:51.540432 FAaDO-0.0.3/FAaDO.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)      234 2023-05-02 15:15:51.000000 FAaDO-0.0.3/FAaDO.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     4148 2023-05-02 15:15:51.000000 FAaDO-0.0.3/FAaDO.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-02 15:15:51.000000 FAaDO-0.0.3/FAaDO.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       47 2023-05-02 15:15:51.000000 FAaDO-0.0.3/FAaDO.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1000) user      (1000)       85 2023-05-02 15:15:51.000000 FAaDO-0.0.3/FAaDO.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       12 2023-05-02 15:15:51.000000 FAaDO-0.0.3/FAaDO.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)      234 2023-05-02 15:15:51.540432 FAaDO-0.0.3/PKG-INFO
--rwxrwxr-x   0 user      (1000) user      (1000)      442 2023-02-23 14:30:12.000000 FAaDO-0.0.3/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 15:15:51.528431 FAaDO-0.0.3/docker/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-02-22 17:07:13.000000 FAaDO-0.0.3/docker/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 15:15:51.528431 FAaDO-0.0.3/fado/
--rw-rw-r--   0 user      (1000) user      (1000)      577 2023-02-24 20:54:56.000000 FAaDO-0.0.3/fado/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 15:15:51.528431 FAaDO-0.0.3/fado/builder/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-02-17 16:37:39.000000 FAaDO-0.0.3/fado/builder/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 15:15:51.528431 FAaDO-0.0.3/fado/builder/crypto/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-02-22 20:45:49.000000 FAaDO-0.0.3/fado/builder/crypto/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 15:15:51.528431 FAaDO-0.0.3/fado/builder/data/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-02-17 16:40:48.000000 FAaDO-0.0.3/fado/builder/data/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      762 2023-02-27 21:20:44.000000 FAaDO-0.0.3/fado/builder/data/dataset.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 15:15:51.528431 FAaDO-0.0.3/fado/builder/data/download/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-02-20 16:37:36.000000 FAaDO-0.0.3/fado/builder/data/download/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      117 2023-02-22 20:36:23.000000 FAaDO-0.0.3/fado/builder/data/download/downloader.py
--rw-rw-r--   0 user      (1000) user      (1000)     1468 2023-03-21 00:49:45.000000 FAaDO-0.0.3/fado/builder/data/download/leaf_downloader.py
--rw-rw-r--   0 user      (1000) user      (1000)     2165 2023-03-21 00:49:28.000000 FAaDO-0.0.3/fado/builder/data/download/nlafl_downloader.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 15:15:51.528431 FAaDO-0.0.3/fado/builder/data/leaf/
--rwxrwxr-x   0 user      (1000) user      (1000)        0 2023-03-21 00:49:45.000000 FAaDO-0.0.3/fado/builder/data/leaf/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1466 2023-03-21 00:49:45.000000 FAaDO-0.0.3/fado/builder/data/leaf/leaf_transformer.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 15:15:51.532431 FAaDO-0.0.3/fado/builder/data/leaf/utils/
--rwxrwxr-x   0 user      (1000) user      (1000)        0 2023-03-21 00:49:45.000000 FAaDO-0.0.3/fado/builder/data/leaf/utils/__init__.py
--rwxrwxr-x   0 user      (1000) user      (1000)      148 2023-03-21 00:49:45.000000 FAaDO-0.0.3/fado/builder/data/leaf/utils/constants.py
--rwxrwxr-x   0 user      (1000) user      (1000)     2288 2023-03-21 00:49:45.000000 FAaDO-0.0.3/fado/builder/data/leaf/utils/remove_users.py
--rwxrwxr-x   0 user      (1000) user      (1000)     6761 2023-03-21 00:49:45.000000 FAaDO-0.0.3/fado/builder/data/leaf/utils/sample.py
--rwxrwxr-x   0 user      (1000) user      (1000)     9200 2023-03-21 00:49:45.000000 FAaDO-0.0.3/fado/builder/data/leaf/utils/split_data.py
--rwxrwxr-x   0 user      (1000) user      (1000)     2786 2023-03-21 00:49:45.000000 FAaDO-0.0.3/fado/builder/data/leaf/utils/stats.py
--rwxrwxr-x   0 user      (1000) user      (1000)      839 2023-03-21 00:49:45.000000 FAaDO-0.0.3/fado/builder/data/leaf/utils/util.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 15:15:51.532431 FAaDO-0.0.3/fado/builder/data/shape/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-02-20 18:18:12.000000 FAaDO-0.0.3/fado/builder/data/shape/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     4003 2023-03-21 00:49:45.000000 FAaDO-0.0.3/fado/builder/data/shape/leaf_shaper.py
--rw-rw-r--   0 user      (1000) user      (1000)    13753 2023-03-21 00:49:28.000000 FAaDO-0.0.3/fado/builder/data/shape/nlafl_shaper.py
--rw-rw-r--   0 user      (1000) user      (1000)      110 2023-02-22 20:36:04.000000 FAaDO-0.0.3/fado/builder/data/shape/shaper.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 15:15:51.532431 FAaDO-0.0.3/fado/builder/default/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-02-22 20:47:19.000000 FAaDO-0.0.3/fado/builder/default/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 15:15:51.532431 FAaDO-0.0.3/fado/cli/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-02-17 16:43:23.000000 FAaDO-0.0.3/fado/cli/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 15:15:51.532431 FAaDO-0.0.3/fado/cli/arguments/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-02-17 16:43:41.000000 FAaDO-0.0.3/fado/cli/arguments/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2550 2023-05-02 13:31:18.000000 FAaDO-0.0.3/fado/cli/arguments/arguments.py
--rw-rw-r--   0 user      (1000) user      (1000)    12366 2023-05-02 14:38:23.000000 FAaDO-0.0.3/fado/cli/fado_run.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 15:15:51.532431 FAaDO-0.0.3/fado/constants/
--rw-rw-r--   0 user      (1000) user      (1000)     1769 2023-05-02 15:15:36.000000 FAaDO-0.0.3/fado/constants/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 15:15:51.532431 FAaDO-0.0.3/fado/runner/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-02-17 16:37:47.000000 FAaDO-0.0.3/fado/runner/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2390 2023-03-21 23:47:32.000000 FAaDO-0.0.3/fado/runner/clients_run.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 15:15:51.532431 FAaDO-0.0.3/fado/runner/communication/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-02-17 16:41:21.000000 FAaDO-0.0.3/fado/runner/communication/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      518 2023-02-18 14:22:44.000000 FAaDO-0.0.3/fado/runner/communication/base_com_manager.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 15:15:51.532431 FAaDO-0.0.3/fado/runner/communication/config/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-02-23 10:19:37.000000 FAaDO-0.0.3/fado/runner/communication/config/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1337 2023-03-21 13:49:39.000000 FAaDO-0.0.3/fado/runner/communication/config/config_clients_network.py
--rw-rw-r--   0 user      (1000) user      (1000)      458 2023-02-25 18:35:31.000000 FAaDO-0.0.3/fado/runner/communication/config/config_router_network.py
--rw-rw-r--   0 user      (1000) user      (1000)      515 2023-02-23 13:58:31.000000 FAaDO-0.0.3/fado/runner/communication/config/config_server_network.py
--rw-rw-r--   0 user      (1000) user      (1000)      475 2023-02-18 14:22:44.000000 FAaDO-0.0.3/fado/runner/communication/fl_com_manager.py
--rw-rw-r--   0 user      (1000) user      (1000)     2457 2023-03-21 19:28:53.000000 FAaDO-0.0.3/fado/runner/communication/message.py
--rw-rw-r--   0 user      (1000) user      (1000)      140 2023-03-21 22:03:07.000000 FAaDO-0.0.3/fado/runner/communication/observer.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 15:15:51.532431 FAaDO-0.0.3/fado/runner/communication/secure_sockets/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-02-17 18:34:47.000000 FAaDO-0.0.3/fado/runner/communication/secure_sockets/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 15:15:51.540432 FAaDO-0.0.3/fado/runner/communication/sockets/
--rw-rw-r--   0 user      (1000) user      (1000)       63 2023-02-17 18:25:54.000000 FAaDO-0.0.3/fado/runner/communication/sockets/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     3427 2023-03-24 16:54:24.000000 FAaDO-0.0.3/fado/runner/communication/sockets/client_com_manager.py
--rw-rw-r--   0 user      (1000) user      (1000)     4665 2023-04-28 16:27:35.000000 FAaDO-0.0.3/fado/runner/communication/sockets/server_com_manager.py
--rw-rw-r--   0 user      (1000) user      (1000)     3286 2023-04-28 16:24:39.000000 FAaDO-0.0.3/fado/runner/communication/sockets/server_pub_info_manager.py
--rw-rw-r--   0 user      (1000) user      (1000)      189 2023-02-18 14:24:50.000000 FAaDO-0.0.3/fado/runner/communication/sockets/test_sockets.py
--rw-rw-r--   0 user      (1000) user      (1000)      270 2023-02-21 19:38:05.000000 FAaDO-0.0.3/fado/runner/communication/sockets/utils.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 15:15:51.540432 FAaDO-0.0.3/fado/runner/data/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-02-21 18:51:45.000000 FAaDO-0.0.3/fado/runner/data/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 15:15:51.540432 FAaDO-0.0.3/fado/runner/data/load/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-02-17 16:48:26.000000 FAaDO-0.0.3/fado/runner/data/load/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      629 2023-03-21 00:49:45.000000 FAaDO-0.0.3/fado/runner/data/load/attacker_data_loader.py
--rw-rw-r--   0 user      (1000) user      (1000)      842 2023-02-27 21:10:16.000000 FAaDO-0.0.3/fado/runner/data/load/base_data_loader.py
--rw-rw-r--   0 user      (1000) user      (1000)      782 2023-03-21 00:49:45.000000 FAaDO-0.0.3/fado/runner/data/load/client_data_loader.py
--rw-rw-r--   0 user      (1000) user      (1000)     1307 2023-03-21 00:49:45.000000 FAaDO-0.0.3/fado/runner/data/load/server_data_loader.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 15:15:51.540432 FAaDO-0.0.3/fado/runner/fl/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-02-17 16:51:10.000000 FAaDO-0.0.3/fado/runner/fl/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 15:15:51.540432 FAaDO-0.0.3/fado/runner/fl/aggregate/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-02-17 16:38:31.000000 FAaDO-0.0.3/fado/runner/fl/aggregate/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      629 2023-05-02 13:42:58.000000 FAaDO-0.0.3/fado/runner/fl/aggregate/aggregator_manager.py
--rw-rw-r--   0 user      (1000) user      (1000)      302 2023-02-19 23:05:47.000000 FAaDO-0.0.3/fado/runner/fl/aggregate/base_aggregator.py
--rw-rw-r--   0 user      (1000) user      (1000)      934 2023-03-21 01:56:16.000000 FAaDO-0.0.3/fado/runner/fl/aggregate/mean_aggregator.py
--rw-rw-r--   0 user      (1000) user      (1000)     2414 2023-03-21 13:55:56.000000 FAaDO-0.0.3/fado/runner/fl/fl_client.py
--rw-rw-r--   0 user      (1000) user      (1000)     7013 2023-03-24 18:46:04.000000 FAaDO-0.0.3/fado/runner/fl/fl_server.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 15:15:51.540432 FAaDO-0.0.3/fado/runner/fl/select/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-02-19 18:39:22.000000 FAaDO-0.0.3/fado/runner/fl/select/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      196 2023-02-19 21:29:46.000000 FAaDO-0.0.3/fado/runner/fl/select/base_participant_selector.py
--rw-rw-r--   0 user      (1000) user      (1000)      655 2023-05-02 13:42:06.000000 FAaDO-0.0.3/fado/runner/fl/select/participant_selector_manager.py
--rw-rw-r--   0 user      (1000) user      (1000)      296 2023-02-19 21:30:49.000000 FAaDO-0.0.3/fado/runner/fl/select/random_participant_selector.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 15:15:51.540432 FAaDO-0.0.3/fado/runner/ml/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-02-17 16:38:20.000000 FAaDO-0.0.3/fado/runner/ml/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 15:15:51.540432 FAaDO-0.0.3/fado/runner/ml/model/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-02-17 16:38:42.000000 FAaDO-0.0.3/fado/runner/ml/model/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 15:15:51.540432 FAaDO-0.0.3/fado/runner/ml/model/built_in/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-02-18 16:39:23.000000 FAaDO-0.0.3/fado/runner/ml/model/built_in/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     5362 2023-03-21 02:44:23.000000 FAaDO-0.0.3/fado/runner/ml/model/built_in/mnist_conv_torch.py
--rw-rw-r--   0 user      (1000) user      (1000)     3267 2023-03-21 00:49:28.000000 FAaDO-0.0.3/fado/runner/ml/model/built_in/nlafl_dbpedia_tf.py
--rw-rw-r--   0 user      (1000) user      (1000)     3085 2023-03-21 00:49:28.000000 FAaDO-0.0.3/fado/runner/ml/model/built_in/nlafl_emnist_tf.py
--rw-rw-r--   0 user      (1000) user      (1000)     4090 2023-03-23 22:15:30.000000 FAaDO-0.0.3/fado/runner/ml/model/built_in/nlafl_emnist_torch.py
--rw-rw-r--   0 user      (1000) user      (1000)     3083 2023-03-21 00:49:28.000000 FAaDO-0.0.3/fado/runner/ml/model/built_in/nlafl_fashionmnist_tf.py
--rw-rw-r--   0 user      (1000) user      (1000)      325 2023-03-14 21:13:54.000000 FAaDO-0.0.3/fado/runner/ml/model/fado_module.py
--rw-rw-r--   0 user      (1000) user      (1000)     1333 2023-05-02 13:08:45.000000 FAaDO-0.0.3/fado/runner/ml/model/module_manager.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 15:15:51.540432 FAaDO-0.0.3/fado/runner/output/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-02-24 16:15:24.000000 FAaDO-0.0.3/fado/runner/output/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      869 2023-03-21 00:49:28.000000 FAaDO-0.0.3/fado/runner/output/results.py
--rw-rw-r--   0 user      (1000) user      (1000)     1160 2023-03-21 00:49:28.000000 FAaDO-0.0.3/fado/runner/output/table.py
--rw-rw-r--   0 user      (1000) user      (1000)     3784 2023-04-28 16:36:18.000000 FAaDO-0.0.3/fado/runner/router_run.py
--rw-rw-r--   0 user      (1000) user      (1000)     1883 2023-03-21 22:01:20.000000 FAaDO-0.0.3/fado/runner/server_run.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 15:15:51.540432 FAaDO-0.0.3/fado/security/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-02-17 16:39:23.000000 FAaDO-0.0.3/fado/security/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 15:15:51.540432 FAaDO-0.0.3/fado/security/attack/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-02-17 16:39:38.000000 FAaDO-0.0.3/fado/security/attack/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 15:15:51.540432 FAaDO-0.0.3/fado/security/attack/client/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-03-21 00:49:28.000000 FAaDO-0.0.3/fado/security/attack/client/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      246 2023-03-21 00:49:28.000000 FAaDO-0.0.3/fado/security/attack/client/attack_base.py
--rw-rw-r--   0 user      (1000) user      (1000)     1089 2023-03-21 00:49:28.000000 FAaDO-0.0.3/fado/security/attack/client/nlafl_poison_attacker.py
--rw-rw-r--   0 user      (1000) user      (1000)      502 2023-03-21 00:49:28.000000 FAaDO-0.0.3/fado/security/attack/client/random_attacker.py
--rw-rw-r--   0 user      (1000) user      (1000)      990 2023-05-02 13:09:20.000000 FAaDO-0.0.3/fado/security/attack/client/server_attack_manager.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 15:15:51.540432 FAaDO-0.0.3/fado/security/attack/network/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-02-27 13:32:47.000000 FAaDO-0.0.3/fado/security/attack/network/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      596 2023-03-21 00:59:27.000000 FAaDO-0.0.3/fado/security/attack/network/network_attack_manager.py
--rw-rw-r--   0 user      (1000) user      (1000)     6868 2023-04-28 16:35:12.000000 FAaDO-0.0.3/fado/security/attack/network/nlafl_attacker.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 15:15:51.540432 FAaDO-0.0.3/fado/security/defend/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-02-17 16:39:45.000000 FAaDO-0.0.3/fado/security/defend/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 15:15:51.540432 FAaDO-0.0.3/fado/security/defend/server/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-03-21 00:49:28.000000 FAaDO-0.0.3/fado/security/defend/server/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1252 2023-03-21 00:49:28.000000 FAaDO-0.0.3/fado/security/defend/server/clipping_defender.py
--rw-rw-r--   0 user      (1000) user      (1000)      237 2023-03-21 00:49:28.000000 FAaDO-0.0.3/fado/security/defend/server/server_defense_base.py
--rw-rw-r--   0 user      (1000) user      (1000)      593 2023-03-21 00:49:28.000000 FAaDO-0.0.3/fado/security/defend/server/server_defense_manager.py
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-05-02 15:15:51.540432 FAaDO-0.0.3/setup.cfg
--rwxrwxr-x   0 user      (1000) user      (1000)      768 2023-05-02 15:14:04.000000 FAaDO-0.0.3/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 17:36:27.859312 FAaDO-0.0.4/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 17:36:27.859312 FAaDO-0.0.4/FAaDO.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)      234 2023-05-02 17:36:27.000000 FAaDO-0.0.4/FAaDO.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     4148 2023-05-02 17:36:27.000000 FAaDO-0.0.4/FAaDO.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-02 17:36:27.000000 FAaDO-0.0.4/FAaDO.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       47 2023-05-02 17:36:27.000000 FAaDO-0.0.4/FAaDO.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       87 2023-05-02 17:36:27.000000 FAaDO-0.0.4/FAaDO.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       12 2023-05-02 17:36:27.000000 FAaDO-0.0.4/FAaDO.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      234 2023-05-02 17:36:27.859312 FAaDO-0.0.4/PKG-INFO
+-rwxrwxr-x   0 user      (1000) user      (1000)     2348 2023-05-02 16:10:01.000000 FAaDO-0.0.4/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 17:36:27.843311 FAaDO-0.0.4/docker/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-02-22 17:07:13.000000 FAaDO-0.0.4/docker/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 17:36:27.843311 FAaDO-0.0.4/fado/
+-rw-rw-r--   0 user      (1000) user      (1000)      577 2023-02-24 20:54:56.000000 FAaDO-0.0.4/fado/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 17:36:27.843311 FAaDO-0.0.4/fado/builder/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-02-17 16:37:39.000000 FAaDO-0.0.4/fado/builder/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 17:36:27.843311 FAaDO-0.0.4/fado/builder/crypto/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-02-22 20:45:49.000000 FAaDO-0.0.4/fado/builder/crypto/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 17:36:27.843311 FAaDO-0.0.4/fado/builder/data/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-02-17 16:40:48.000000 FAaDO-0.0.4/fado/builder/data/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      762 2023-02-27 21:20:44.000000 FAaDO-0.0.4/fado/builder/data/dataset.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 17:36:27.843311 FAaDO-0.0.4/fado/builder/data/download/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-02-20 16:37:36.000000 FAaDO-0.0.4/fado/builder/data/download/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      117 2023-02-22 20:36:23.000000 FAaDO-0.0.4/fado/builder/data/download/downloader.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1468 2023-03-21 00:49:45.000000 FAaDO-0.0.4/fado/builder/data/download/leaf_downloader.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2165 2023-03-21 00:49:28.000000 FAaDO-0.0.4/fado/builder/data/download/nlafl_downloader.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 17:36:27.843311 FAaDO-0.0.4/fado/builder/data/leaf/
+-rwxrwxr-x   0 user      (1000) user      (1000)        0 2023-03-21 00:49:45.000000 FAaDO-0.0.4/fado/builder/data/leaf/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1466 2023-03-21 00:49:45.000000 FAaDO-0.0.4/fado/builder/data/leaf/leaf_transformer.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 17:36:27.847311 FAaDO-0.0.4/fado/builder/data/leaf/utils/
+-rwxrwxr-x   0 user      (1000) user      (1000)        0 2023-03-21 00:49:45.000000 FAaDO-0.0.4/fado/builder/data/leaf/utils/__init__.py
+-rwxrwxr-x   0 user      (1000) user      (1000)      148 2023-03-21 00:49:45.000000 FAaDO-0.0.4/fado/builder/data/leaf/utils/constants.py
+-rwxrwxr-x   0 user      (1000) user      (1000)     2288 2023-03-21 00:49:45.000000 FAaDO-0.0.4/fado/builder/data/leaf/utils/remove_users.py
+-rwxrwxr-x   0 user      (1000) user      (1000)     6761 2023-03-21 00:49:45.000000 FAaDO-0.0.4/fado/builder/data/leaf/utils/sample.py
+-rwxrwxr-x   0 user      (1000) user      (1000)     9200 2023-03-21 00:49:45.000000 FAaDO-0.0.4/fado/builder/data/leaf/utils/split_data.py
+-rwxrwxr-x   0 user      (1000) user      (1000)     2786 2023-03-21 00:49:45.000000 FAaDO-0.0.4/fado/builder/data/leaf/utils/stats.py
+-rwxrwxr-x   0 user      (1000) user      (1000)      839 2023-03-21 00:49:45.000000 FAaDO-0.0.4/fado/builder/data/leaf/utils/util.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 17:36:27.847311 FAaDO-0.0.4/fado/builder/data/shape/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-02-20 18:18:12.000000 FAaDO-0.0.4/fado/builder/data/shape/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4003 2023-03-21 00:49:45.000000 FAaDO-0.0.4/fado/builder/data/shape/leaf_shaper.py
+-rw-rw-r--   0 user      (1000) user      (1000)    13753 2023-03-21 00:49:28.000000 FAaDO-0.0.4/fado/builder/data/shape/nlafl_shaper.py
+-rw-rw-r--   0 user      (1000) user      (1000)      110 2023-02-22 20:36:04.000000 FAaDO-0.0.4/fado/builder/data/shape/shaper.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 17:36:27.847311 FAaDO-0.0.4/fado/builder/default/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-02-22 20:47:19.000000 FAaDO-0.0.4/fado/builder/default/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 17:36:27.847311 FAaDO-0.0.4/fado/cli/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-02-17 16:43:23.000000 FAaDO-0.0.4/fado/cli/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 17:36:27.847311 FAaDO-0.0.4/fado/cli/arguments/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-02-17 16:43:41.000000 FAaDO-0.0.4/fado/cli/arguments/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2550 2023-05-02 13:31:18.000000 FAaDO-0.0.4/fado/cli/arguments/arguments.py
+-rw-rw-r--   0 user      (1000) user      (1000)    13552 2023-05-02 16:18:16.000000 FAaDO-0.0.4/fado/cli/fado_run.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 17:36:27.847311 FAaDO-0.0.4/fado/constants/
+-rw-rw-r--   0 user      (1000) user      (1000)     1769 2023-05-02 17:36:21.000000 FAaDO-0.0.4/fado/constants/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 17:36:27.847311 FAaDO-0.0.4/fado/runner/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-02-17 16:37:47.000000 FAaDO-0.0.4/fado/runner/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2390 2023-03-21 23:47:32.000000 FAaDO-0.0.4/fado/runner/clients_run.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 17:36:27.847311 FAaDO-0.0.4/fado/runner/communication/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-02-17 16:41:21.000000 FAaDO-0.0.4/fado/runner/communication/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      518 2023-02-18 14:22:44.000000 FAaDO-0.0.4/fado/runner/communication/base_com_manager.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 17:36:27.847311 FAaDO-0.0.4/fado/runner/communication/config/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-02-23 10:19:37.000000 FAaDO-0.0.4/fado/runner/communication/config/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1337 2023-03-21 13:49:39.000000 FAaDO-0.0.4/fado/runner/communication/config/config_clients_network.py
+-rw-rw-r--   0 user      (1000) user      (1000)      458 2023-02-25 18:35:31.000000 FAaDO-0.0.4/fado/runner/communication/config/config_router_network.py
+-rw-rw-r--   0 user      (1000) user      (1000)      515 2023-02-23 13:58:31.000000 FAaDO-0.0.4/fado/runner/communication/config/config_server_network.py
+-rw-rw-r--   0 user      (1000) user      (1000)      475 2023-02-18 14:22:44.000000 FAaDO-0.0.4/fado/runner/communication/fl_com_manager.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2457 2023-03-21 19:28:53.000000 FAaDO-0.0.4/fado/runner/communication/message.py
+-rw-rw-r--   0 user      (1000) user      (1000)      140 2023-03-21 22:03:07.000000 FAaDO-0.0.4/fado/runner/communication/observer.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 17:36:27.847311 FAaDO-0.0.4/fado/runner/communication/secure_sockets/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-02-17 18:34:47.000000 FAaDO-0.0.4/fado/runner/communication/secure_sockets/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 17:36:27.851311 FAaDO-0.0.4/fado/runner/communication/sockets/
+-rw-rw-r--   0 user      (1000) user      (1000)       63 2023-02-17 18:25:54.000000 FAaDO-0.0.4/fado/runner/communication/sockets/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3427 2023-03-24 16:54:24.000000 FAaDO-0.0.4/fado/runner/communication/sockets/client_com_manager.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4665 2023-04-28 16:27:35.000000 FAaDO-0.0.4/fado/runner/communication/sockets/server_com_manager.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3286 2023-04-28 16:24:39.000000 FAaDO-0.0.4/fado/runner/communication/sockets/server_pub_info_manager.py
+-rw-rw-r--   0 user      (1000) user      (1000)      189 2023-02-18 14:24:50.000000 FAaDO-0.0.4/fado/runner/communication/sockets/test_sockets.py
+-rw-rw-r--   0 user      (1000) user      (1000)      270 2023-02-21 19:38:05.000000 FAaDO-0.0.4/fado/runner/communication/sockets/utils.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 17:36:27.851311 FAaDO-0.0.4/fado/runner/data/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-02-21 18:51:45.000000 FAaDO-0.0.4/fado/runner/data/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 17:36:27.851311 FAaDO-0.0.4/fado/runner/data/load/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-02-17 16:48:26.000000 FAaDO-0.0.4/fado/runner/data/load/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      629 2023-03-21 00:49:45.000000 FAaDO-0.0.4/fado/runner/data/load/attacker_data_loader.py
+-rw-rw-r--   0 user      (1000) user      (1000)      842 2023-02-27 21:10:16.000000 FAaDO-0.0.4/fado/runner/data/load/base_data_loader.py
+-rw-rw-r--   0 user      (1000) user      (1000)      782 2023-03-21 00:49:45.000000 FAaDO-0.0.4/fado/runner/data/load/client_data_loader.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1307 2023-03-21 00:49:45.000000 FAaDO-0.0.4/fado/runner/data/load/server_data_loader.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 17:36:27.851311 FAaDO-0.0.4/fado/runner/fl/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-02-17 16:51:10.000000 FAaDO-0.0.4/fado/runner/fl/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 17:36:27.851311 FAaDO-0.0.4/fado/runner/fl/aggregate/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-02-17 16:38:31.000000 FAaDO-0.0.4/fado/runner/fl/aggregate/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      629 2023-05-02 13:42:58.000000 FAaDO-0.0.4/fado/runner/fl/aggregate/aggregator_manager.py
+-rw-rw-r--   0 user      (1000) user      (1000)      302 2023-02-19 23:05:47.000000 FAaDO-0.0.4/fado/runner/fl/aggregate/base_aggregator.py
+-rw-rw-r--   0 user      (1000) user      (1000)      934 2023-03-21 01:56:16.000000 FAaDO-0.0.4/fado/runner/fl/aggregate/mean_aggregator.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2414 2023-03-21 13:55:56.000000 FAaDO-0.0.4/fado/runner/fl/fl_client.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7013 2023-03-24 18:46:04.000000 FAaDO-0.0.4/fado/runner/fl/fl_server.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 17:36:27.851311 FAaDO-0.0.4/fado/runner/fl/select/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-02-19 18:39:22.000000 FAaDO-0.0.4/fado/runner/fl/select/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      196 2023-02-19 21:29:46.000000 FAaDO-0.0.4/fado/runner/fl/select/base_participant_selector.py
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-05-02 13:42:06.000000 FAaDO-0.0.4/fado/runner/fl/select/participant_selector_manager.py
+-rw-rw-r--   0 user      (1000) user      (1000)      296 2023-02-19 21:30:49.000000 FAaDO-0.0.4/fado/runner/fl/select/random_participant_selector.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 17:36:27.851311 FAaDO-0.0.4/fado/runner/ml/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-02-17 16:38:20.000000 FAaDO-0.0.4/fado/runner/ml/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 17:36:27.851311 FAaDO-0.0.4/fado/runner/ml/model/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-02-17 16:38:42.000000 FAaDO-0.0.4/fado/runner/ml/model/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 17:36:27.855311 FAaDO-0.0.4/fado/runner/ml/model/built_in/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-02-18 16:39:23.000000 FAaDO-0.0.4/fado/runner/ml/model/built_in/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5362 2023-03-21 02:44:23.000000 FAaDO-0.0.4/fado/runner/ml/model/built_in/mnist_conv_torch.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3267 2023-03-21 00:49:28.000000 FAaDO-0.0.4/fado/runner/ml/model/built_in/nlafl_dbpedia_tf.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3085 2023-03-21 00:49:28.000000 FAaDO-0.0.4/fado/runner/ml/model/built_in/nlafl_emnist_tf.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4090 2023-03-23 22:15:30.000000 FAaDO-0.0.4/fado/runner/ml/model/built_in/nlafl_emnist_torch.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3083 2023-03-21 00:49:28.000000 FAaDO-0.0.4/fado/runner/ml/model/built_in/nlafl_fashionmnist_tf.py
+-rw-rw-r--   0 user      (1000) user      (1000)      325 2023-03-14 21:13:54.000000 FAaDO-0.0.4/fado/runner/ml/model/fado_module.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1334 2023-05-02 17:33:12.000000 FAaDO-0.0.4/fado/runner/ml/model/module_manager.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 17:36:27.855311 FAaDO-0.0.4/fado/runner/output/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-02-24 16:15:24.000000 FAaDO-0.0.4/fado/runner/output/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      869 2023-03-21 00:49:28.000000 FAaDO-0.0.4/fado/runner/output/results.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1160 2023-03-21 00:49:28.000000 FAaDO-0.0.4/fado/runner/output/table.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3784 2023-04-28 16:36:18.000000 FAaDO-0.0.4/fado/runner/router_run.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1883 2023-03-21 22:01:20.000000 FAaDO-0.0.4/fado/runner/server_run.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 17:36:27.855311 FAaDO-0.0.4/fado/security/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-02-17 16:39:23.000000 FAaDO-0.0.4/fado/security/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 17:36:27.855311 FAaDO-0.0.4/fado/security/attack/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-02-17 16:39:38.000000 FAaDO-0.0.4/fado/security/attack/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 17:36:27.855311 FAaDO-0.0.4/fado/security/attack/client/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-03-21 00:49:28.000000 FAaDO-0.0.4/fado/security/attack/client/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      246 2023-03-21 00:49:28.000000 FAaDO-0.0.4/fado/security/attack/client/attack_base.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1089 2023-03-21 00:49:28.000000 FAaDO-0.0.4/fado/security/attack/client/nlafl_poison_attacker.py
+-rw-rw-r--   0 user      (1000) user      (1000)      502 2023-03-21 00:49:28.000000 FAaDO-0.0.4/fado/security/attack/client/random_attacker.py
+-rw-rw-r--   0 user      (1000) user      (1000)      990 2023-05-02 13:09:20.000000 FAaDO-0.0.4/fado/security/attack/client/server_attack_manager.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 17:36:27.855311 FAaDO-0.0.4/fado/security/attack/network/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-02-27 13:32:47.000000 FAaDO-0.0.4/fado/security/attack/network/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      596 2023-03-21 00:59:27.000000 FAaDO-0.0.4/fado/security/attack/network/network_attack_manager.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6868 2023-04-28 16:35:12.000000 FAaDO-0.0.4/fado/security/attack/network/nlafl_attacker.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 17:36:27.855311 FAaDO-0.0.4/fado/security/defend/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-02-17 16:39:45.000000 FAaDO-0.0.4/fado/security/defend/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 17:36:27.859312 FAaDO-0.0.4/fado/security/defend/server/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-03-21 00:49:28.000000 FAaDO-0.0.4/fado/security/defend/server/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1252 2023-03-21 00:49:28.000000 FAaDO-0.0.4/fado/security/defend/server/clipping_defender.py
+-rw-rw-r--   0 user      (1000) user      (1000)      237 2023-03-21 00:49:28.000000 FAaDO-0.0.4/fado/security/defend/server/server_defense_base.py
+-rw-rw-r--   0 user      (1000) user      (1000)      593 2023-03-21 00:49:28.000000 FAaDO-0.0.4/fado/security/defend/server/server_defense_manager.py
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-05-02 17:36:27.859312 FAaDO-0.0.4/setup.cfg
+-rwxrwxr-x   0 user      (1000) user      (1000)      770 2023-05-02 17:36:13.000000 FAaDO-0.0.4/setup.py
```

### Comparing `FAaDO-0.0.3/FAaDO.egg-info/SOURCES.txt` & `FAaDO-0.0.4/FAaDO.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FAaDO-0.0.3/fado/__init__.py` & `FAaDO-0.0.4/fado/__init__.py`

 * *Files identical despite different names*

### Comparing `FAaDO-0.0.3/fado/builder/data/dataset.py` & `FAaDO-0.0.4/fado/builder/data/dataset.py`

 * *Files identical despite different names*

### Comparing `FAaDO-0.0.3/fado/builder/data/download/leaf_downloader.py` & `FAaDO-0.0.4/fado/builder/data/download/leaf_downloader.py`

 * *Files identical despite different names*

### Comparing `FAaDO-0.0.3/fado/builder/data/download/nlafl_downloader.py` & `FAaDO-0.0.4/fado/builder/data/download/nlafl_downloader.py`

 * *Files identical despite different names*

### Comparing `FAaDO-0.0.3/fado/builder/data/leaf/leaf_transformer.py` & `FAaDO-0.0.4/fado/builder/data/leaf/leaf_transformer.py`

 * *Files identical despite different names*

### Comparing `FAaDO-0.0.3/fado/builder/data/leaf/utils/remove_users.py` & `FAaDO-0.0.4/fado/builder/data/leaf/utils/remove_users.py`

 * *Files identical despite different names*

### Comparing `FAaDO-0.0.3/fado/builder/data/leaf/utils/sample.py` & `FAaDO-0.0.4/fado/builder/data/leaf/utils/sample.py`

 * *Files identical despite different names*

### Comparing `FAaDO-0.0.3/fado/builder/data/leaf/utils/split_data.py` & `FAaDO-0.0.4/fado/builder/data/leaf/utils/split_data.py`

 * *Files identical despite different names*

### Comparing `FAaDO-0.0.3/fado/builder/data/leaf/utils/stats.py` & `FAaDO-0.0.4/fado/builder/data/leaf/utils/stats.py`

 * *Files identical despite different names*

### Comparing `FAaDO-0.0.3/fado/builder/data/leaf/utils/util.py` & `FAaDO-0.0.4/fado/builder/data/leaf/utils/util.py`

 * *Files identical despite different names*

### Comparing `FAaDO-0.0.3/fado/builder/data/shape/leaf_shaper.py` & `FAaDO-0.0.4/fado/builder/data/shape/leaf_shaper.py`

 * *Files identical despite different names*

### Comparing `FAaDO-0.0.3/fado/builder/data/shape/nlafl_shaper.py` & `FAaDO-0.0.4/fado/builder/data/shape/nlafl_shaper.py`

 * *Files identical despite different names*

### Comparing `FAaDO-0.0.3/fado/cli/arguments/arguments.py` & `FAaDO-0.0.4/fado/cli/arguments/arguments.py`

 * *Files identical despite different names*

### Comparing `FAaDO-0.0.3/fado/cli/fado_run.py` & `FAaDO-0.0.4/fado/cli/fado_run.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     parser.add_argument('-f', dest='yaml_file', type=str, help='Specify a custom yaml configuration file',
                         required=False)
     mode_parser = parser.add_subparsers(dest="mode", required=False)
 
     build_parser = mode_parser.add_parser('build')
     mode_parser.add_parser('prepare')
     mode_parser.add_parser('run')
+    clean_parser = mode_parser.add_parser('clean')
     mode_parser.add_parser('table')
 
     parser.add_argument('-d', dest='dataset', type=str, choices=DATASETS, required=False)
     parser.add_argument('-dr', dest='dataset_rate', help='Fraction of the dataset', type=float,
                         required=False)
     parser.add_argument('-dd', dest='data_distribution', help='Data distribution', type=str, required=False)
     parser.add_argument('-nb', dest='number_benign', type=int, required=False)
@@ -41,14 +42,18 @@
     parser.add_argument('--dev', dest='development', action='store_true', required=False)
     parser.add_argument('--no-docker', dest='docker', action='store_false', default=True)
 
     build_mode_parser = build_parser.add_subparsers(dest="build_mode")
     build_mode_parser.add_parser('download')
     build_mode_parser.add_parser('shape')
 
+    clean_mode_parser = clean_parser.add_subparsers(dest="clean_mode")
+    clean_mode_parser.add_parser('prepare')
+    clean_mode_parser.add_parser('build')
+
     return parser.parse_args(args)
 
 
 def download_data(fado_arguments):
     from fado.builder.data.download.nlafl_downloader import NLAFLDownloader
     from fado.builder.data.download.leaf_downloader import LEAFDownloader
 
@@ -253,50 +258,79 @@
 
 
 def verify_docker_install():
     # TODO:
     pass
 
 
+def clean_prepare():
+    subprocess.run(['docker', 'image', 'rm', f'ralexandre00/fado-router:{FADO_VERSION}'])
+    subprocess.run(['docker', 'image', 'rm', f'ralexandre00/fado-node:{FADO_VERSION}'])
+    subprocess.run(['docker', 'image', 'rm', f'ralexandre00/fado-node-requirements:{FADO_VERSION}'])
+
+
+def clean_build():
+    shutil.rmtree(FADO_DIR)
+
+
+def prepare_fado():
+    verify_docker_install()
+    logger.info("Pulling required docker images")
+    subprocess.run(['docker', 'pull', f'ralexandre00/fado-node-requirements:{FADO_VERSION}'])
+    subprocess.run(['docker', 'pull', f'ralexandre00/fado-router:{FADO_VERSION}'])
+    subprocess.run(['docker', 'pull', f'ralexandre00/fado-node:{FADO_VERSION}'])
+
+
 def cli():
     args = parse_args(sys.argv[1:])
 
     if args.yaml_file:
         config_file = args.yaml_file
     else:
         fado_config_env = os.getenv('FADO_CONFIG')
         config_file = fado_config_env if fado_config_env else FADO_DEFAULT_CONFIG_FILE_PATH
 
-    fado_arguments = FADOArguments(config_file)
-
     if args.mode == 'prepare':
-        verify_docker_install()
-        logger.info("Pulling required docker images -q")
-        subprocess.run(['docker', 'pull', f'ralexandre00/fado-node-requirements:{FADO_VERSION}'])
-        subprocess.run(['docker', 'pull', f'ralexandre00/fado-router:{FADO_VERSION}'])
-        subprocess.run(['docker', 'pull', f'ralexandre00/fado-node:{FADO_VERSION}'])
+        prepare_fado()
     if args.mode == 'build':
+        fado_arguments = FADOArguments(config_file)
         build_mode = args.build_mode
-        move_files_to_fado_home(config_file)
+        move_files_to_fado_home(fado_arguments, config_file)
 
         if build_mode == 'download':
             download_data(fado_arguments)
         elif build_mode == 'shape':
             shape_data(fado_arguments)
         else:
             download_data(fado_arguments)
             shape_data(fado_arguments)
 
     elif args.mode == 'run':
+        fado_arguments = FADOArguments(config_file)
         if 'vary' in fado_arguments:
             run_multiple(fado_arguments, args.development, args.docker)
             return
 
-        move_files_to_fado_home(config_file)
+        move_files_to_fado_home(fado_arguments, config_file)
         run(fado_arguments, args.development, args.docker)
     elif args.mode == 'table':
+        fado_arguments = FADOArguments(config_file)
         generate_table(fado_arguments.table_round)
         # clean()
+    elif args.mode == "clean":
+        clean_mode = args.clean_mode
+        if clean_mode == 'prepare':
+            clean_prepare()
+        elif clean_mode == 'shape':
+            clean_build()
+        else:
+            clean_prepare()
+            clean_build()
     else:
+        prepare_fado()
+        fado_arguments = FADOArguments(config_file)
+        if 'vary' in fado_arguments:
+            run_multiple(fado_arguments, args.development, args.docker)
+            return
         download_data(fado_arguments)
         shape_data(fado_arguments)
         run(fado_arguments, args.development, args.docker)
```

### Comparing `FAaDO-0.0.3/fado/constants/__init__.py` & `FAaDO-0.0.4/fado/constants/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import fado
 from fado.builder import crypto, default
 
 fado_module_dir = os.path.dirname(fado.__file__)
 crypto_module_dir = os.path.dirname(crypto.__file__)
 default_module_dir = os.path.dirname(default.__file__)
 
-FADO_VERSION = "0.0.3"
+FADO_VERSION = "0.0.4"
 
 FADO_DIR = os.getenv('FADO_HOME_FOLDER', os.path.join(os.path.expanduser("~"), '.fado'))
 FADO_SRC = os.path.join(fado_module_dir)
 
 CERTS_PATH = os.path.join(crypto_module_dir, 'certs')
 FADO_DEFAULT_CONFIG_FILE_PATH = os.path.join(default_module_dir, 'fado_config.yaml')
```

### Comparing `FAaDO-0.0.3/fado/runner/clients_run.py` & `FAaDO-0.0.4/fado/runner/clients_run.py`

 * *Files identical despite different names*

### Comparing `FAaDO-0.0.3/fado/runner/communication/base_com_manager.py` & `FAaDO-0.0.4/fado/runner/communication/base_com_manager.py`

 * *Files identical despite different names*

### Comparing `FAaDO-0.0.3/fado/runner/communication/config/config_clients_network.py` & `FAaDO-0.0.4/fado/runner/communication/config/config_clients_network.py`

 * *Files identical despite different names*

### Comparing `FAaDO-0.0.3/fado/runner/communication/config/config_server_network.py` & `FAaDO-0.0.4/fado/runner/communication/config/config_server_network.py`

 * *Files identical despite different names*

### Comparing `FAaDO-0.0.3/fado/runner/communication/message.py` & `FAaDO-0.0.4/fado/runner/communication/message.py`

 * *Files identical despite different names*

### Comparing `FAaDO-0.0.3/fado/runner/communication/sockets/client_com_manager.py` & `FAaDO-0.0.4/fado/runner/communication/sockets/client_com_manager.py`

 * *Files identical despite different names*

### Comparing `FAaDO-0.0.3/fado/runner/communication/sockets/server_com_manager.py` & `FAaDO-0.0.4/fado/runner/communication/sockets/server_com_manager.py`

 * *Files identical despite different names*

### Comparing `FAaDO-0.0.3/fado/runner/communication/sockets/server_pub_info_manager.py` & `FAaDO-0.0.4/fado/runner/communication/sockets/server_pub_info_manager.py`

 * *Files identical despite different names*

### Comparing `FAaDO-0.0.3/fado/runner/data/load/attacker_data_loader.py` & `FAaDO-0.0.4/fado/runner/data/load/attacker_data_loader.py`

 * *Files identical despite different names*

### Comparing `FAaDO-0.0.3/fado/runner/data/load/base_data_loader.py` & `FAaDO-0.0.4/fado/runner/data/load/base_data_loader.py`

 * *Files identical despite different names*

### Comparing `FAaDO-0.0.3/fado/runner/data/load/client_data_loader.py` & `FAaDO-0.0.4/fado/runner/data/load/client_data_loader.py`

 * *Files identical despite different names*

### Comparing `FAaDO-0.0.3/fado/runner/data/load/server_data_loader.py` & `FAaDO-0.0.4/fado/runner/data/load/server_data_loader.py`

 * *Files identical despite different names*

### Comparing `FAaDO-0.0.3/fado/runner/fl/aggregate/aggregator_manager.py` & `FAaDO-0.0.4/fado/runner/fl/aggregate/aggregator_manager.py`

 * *Files identical despite different names*

### Comparing `FAaDO-0.0.3/fado/runner/fl/aggregate/mean_aggregator.py` & `FAaDO-0.0.4/fado/runner/fl/aggregate/mean_aggregator.py`

 * *Files identical despite different names*

### Comparing `FAaDO-0.0.3/fado/runner/fl/fl_client.py` & `FAaDO-0.0.4/fado/runner/fl/fl_client.py`

 * *Files identical despite different names*

### Comparing `FAaDO-0.0.3/fado/runner/fl/fl_server.py` & `FAaDO-0.0.4/fado/runner/fl/fl_server.py`

 * *Files identical despite different names*

### Comparing `FAaDO-0.0.3/fado/runner/fl/select/participant_selector_manager.py` & `FAaDO-0.0.4/fado/runner/fl/select/participant_selector_manager.py`

 * *Files identical despite different names*

### Comparing `FAaDO-0.0.3/fado/runner/ml/model/built_in/mnist_conv_torch.py` & `FAaDO-0.0.4/fado/runner/ml/model/built_in/mnist_conv_torch.py`

 * *Files identical despite different names*

### Comparing `FAaDO-0.0.3/fado/runner/ml/model/built_in/nlafl_dbpedia_tf.py` & `FAaDO-0.0.4/fado/runner/ml/model/built_in/nlafl_dbpedia_tf.py`

 * *Files identical despite different names*

### Comparing `FAaDO-0.0.3/fado/runner/ml/model/built_in/nlafl_emnist_tf.py` & `FAaDO-0.0.4/fado/runner/ml/model/built_in/nlafl_emnist_tf.py`

 * *Files identical despite different names*

### Comparing `FAaDO-0.0.3/fado/runner/ml/model/built_in/nlafl_emnist_torch.py` & `FAaDO-0.0.4/fado/runner/ml/model/built_in/nlafl_emnist_torch.py`

 * *Files identical despite different names*

### Comparing `FAaDO-0.0.3/fado/runner/ml/model/built_in/nlafl_fashionmnist_tf.py` & `FAaDO-0.0.4/fado/runner/ml/model/built_in/nlafl_fashionmnist_tf.py`

 * *Files identical despite different names*

### Comparing `FAaDO-0.0.3/fado/runner/ml/model/module_manager.py` & `FAaDO-0.0.4/fado/runner/ml/model/module_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,11 +18,11 @@
                 return NlaflFashionmnistTf()
             elif args.model == 'nlafl_dbpedia_tf':
                 from fado.runner.ml.model.built_in.nlafl_dbpedia_tf import NlaflDbpediaTf
                 return NlaflDbpediaTf()
         elif args.model in ['mnist_conv_torch']:
             from fado.runner.ml.model.built_in.mnist_conv_torch import MnistConvTorch
             return MnistConvTorch()
-        elif 'py' in args.model:
+        elif '.py' in args.model:
             return args.get_class('model')()
         else:
             raise Exception(f"Model {args.model} not found")
```

### Comparing `FAaDO-0.0.3/fado/runner/output/results.py` & `FAaDO-0.0.4/fado/runner/output/results.py`

 * *Files identical despite different names*

### Comparing `FAaDO-0.0.3/fado/runner/output/table.py` & `FAaDO-0.0.4/fado/runner/output/table.py`

 * *Files identical despite different names*

### Comparing `FAaDO-0.0.3/fado/runner/router_run.py` & `FAaDO-0.0.4/fado/runner/router_run.py`

 * *Files identical despite different names*

### Comparing `FAaDO-0.0.3/fado/runner/server_run.py` & `FAaDO-0.0.4/fado/runner/server_run.py`

 * *Files identical despite different names*

### Comparing `FAaDO-0.0.3/fado/security/attack/client/nlafl_poison_attacker.py` & `FAaDO-0.0.4/fado/security/attack/client/nlafl_poison_attacker.py`

 * *Files identical despite different names*

### Comparing `FAaDO-0.0.3/fado/security/attack/client/server_attack_manager.py` & `FAaDO-0.0.4/fado/security/attack/client/server_attack_manager.py`

 * *Files identical despite different names*

### Comparing `FAaDO-0.0.3/fado/security/attack/network/network_attack_manager.py` & `FAaDO-0.0.4/fado/security/attack/network/network_attack_manager.py`

 * *Files identical despite different names*

### Comparing `FAaDO-0.0.3/fado/security/attack/network/nlafl_attacker.py` & `FAaDO-0.0.4/fado/security/attack/network/nlafl_attacker.py`

 * *Files identical despite different names*

### Comparing `FAaDO-0.0.3/fado/security/defend/server/clipping_defender.py` & `FAaDO-0.0.4/fado/security/defend/server/clipping_defender.py`

 * *Files identical despite different names*

### Comparing `FAaDO-0.0.3/fado/security/defend/server/server_defense_manager.py` & `FAaDO-0.0.4/fado/security/defend/server/server_defense_manager.py`

 * *Files identical despite different names*

### Comparing `FAaDO-0.0.3/setup.py` & `FAaDO-0.0.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 
 
 requirements = [
     "torch==1.13.1",
     "tensorflow==2.11.0",
     "PyYAML==6.0",
     "py7zr==0.20.4",
-    "numpy==1.21",
+    "numpy==1.24.2",
     "pandas==1.5.2"
 ]
 
 setup(
     name='FAaDO',
-    version='0.0.3',
+    version='0.0.4',
     license='MIT',
     maintainer="Rodrigo Simoes",
     maintainer_email='rsimoes@lasige.di.fc.ul.pt',
     packages=find_packages('.'),
     package_dir={'': '.'},
     url='https://github.com/rAlexandre00/FADO',
     keywords='Federated Attack and Defense Orchestrator',
```

