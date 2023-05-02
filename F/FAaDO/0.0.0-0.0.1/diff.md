# Comparing `tmp/FAaDO-0.0.0-py3-none-any.whl.zip` & `tmp/FAaDO-0.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 63349 bytes, number of entries: 99
+Zip file size: 62734 bytes, number of entries: 99
 -rw-rw-r--  2.0 unx        0 b- defN 23-Feb-22 17:07 docker/__init__.py
 -rw-rw-r--  2.0 unx      577 b- defN 23-Feb-24 20:54 fado/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Feb-17 16:37 fado/builder/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Feb-22 20:45 fado/builder/crypto/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Feb-17 16:40 fado/builder/data/__init__.py
 -rw-rw-r--  2.0 unx      762 b- defN 23-Feb-27 21:20 fado/builder/data/dataset.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Feb-20 16:37 fado/builder/data/download/__init__.py
@@ -20,18 +20,18 @@
 -rw-rw-r--  2.0 unx      839 b- defN 23-Mar-21 00:49 fado/builder/data/leaf/utils/util.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Feb-20 18:18 fado/builder/data/shape/__init__.py
 -rw-rw-r--  2.0 unx     4003 b- defN 23-Mar-21 00:49 fado/builder/data/shape/leaf_shaper.py
 -rw-rw-r--  2.0 unx    13753 b- defN 23-Mar-21 00:49 fado/builder/data/shape/nlafl_shaper.py
 -rw-rw-r--  2.0 unx      110 b- defN 23-Feb-22 20:36 fado/builder/data/shape/shaper.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Feb-22 20:47 fado/builder/default/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Feb-17 16:43 fado/cli/__init__.py
--rw-rw-r--  2.0 unx    12281 b- defN 23-May-02 14:06 fado/cli/fado_run.py
+-rw-rw-r--  2.0 unx    11452 b- defN 23-Mar-21 18:23 fado/cli/fado_run.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Feb-17 16:43 fado/cli/arguments/__init__.py
--rw-rw-r--  2.0 unx     2550 b- defN 23-May-02 13:31 fado/cli/arguments/arguments.py
--rw-rw-r--  2.0 unx     1769 b- defN 23-May-02 14:06 fado/constants/__init__.py
+-rw-rw-r--  2.0 unx     1845 b- defN 23-Mar-21 00:49 fado/cli/arguments/arguments.py
+-rw-rw-r--  2.0 unx     1689 b- defN 23-Mar-21 00:49 fado/constants/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Feb-17 16:37 fado/runner/__init__.py
 -rw-rw-r--  2.0 unx     2390 b- defN 23-Mar-21 23:47 fado/runner/clients_run.py
 -rw-rw-r--  2.0 unx     3784 b- defN 23-Apr-28 16:36 fado/runner/router_run.py
 -rw-rw-r--  2.0 unx     1883 b- defN 23-Mar-21 22:01 fado/runner/server_run.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Feb-17 16:41 fado/runner/communication/__init__.py
 -rw-rw-r--  2.0 unx      518 b- defN 23-Feb-18 14:22 fado/runner/communication/base_com_manager.py
 -rw-rw-r--  2.0 unx      475 b- defN 23-Feb-18 14:22 fado/runner/communication/fl_com_manager.py
@@ -54,25 +54,25 @@
 -rw-rw-r--  2.0 unx      842 b- defN 23-Feb-27 21:10 fado/runner/data/load/base_data_loader.py
 -rw-rw-r--  2.0 unx      782 b- defN 23-Mar-21 00:49 fado/runner/data/load/client_data_loader.py
 -rw-rw-r--  2.0 unx     1307 b- defN 23-Mar-21 00:49 fado/runner/data/load/server_data_loader.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Feb-17 16:51 fado/runner/fl/__init__.py
 -rw-rw-r--  2.0 unx     2414 b- defN 23-Mar-21 13:55 fado/runner/fl/fl_client.py
 -rw-rw-r--  2.0 unx     7013 b- defN 23-Mar-24 18:46 fado/runner/fl/fl_server.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Feb-17 16:38 fado/runner/fl/aggregate/__init__.py
--rw-rw-r--  2.0 unx      629 b- defN 23-May-02 13:42 fado/runner/fl/aggregate/aggregator_manager.py
+-rw-rw-r--  2.0 unx      527 b- defN 23-Feb-19 23:03 fado/runner/fl/aggregate/aggregator_manager.py
 -rw-rw-r--  2.0 unx      302 b- defN 23-Feb-19 23:05 fado/runner/fl/aggregate/base_aggregator.py
 -rw-rw-r--  2.0 unx      934 b- defN 23-Mar-21 01:56 fado/runner/fl/aggregate/mean_aggregator.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Feb-19 18:39 fado/runner/fl/select/__init__.py
 -rw-rw-r--  2.0 unx      196 b- defN 23-Feb-19 21:29 fado/runner/fl/select/base_participant_selector.py
--rw-rw-r--  2.0 unx      655 b- defN 23-May-02 13:42 fado/runner/fl/select/participant_selector_manager.py
+-rw-rw-r--  2.0 unx      559 b- defN 23-Feb-19 23:03 fado/runner/fl/select/participant_selector_manager.py
 -rw-rw-r--  2.0 unx      296 b- defN 23-Feb-19 21:30 fado/runner/fl/select/random_participant_selector.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Feb-17 16:38 fado/runner/ml/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Feb-17 16:38 fado/runner/ml/model/__init__.py
 -rw-rw-r--  2.0 unx      325 b- defN 23-Mar-14 21:13 fado/runner/ml/model/fado_module.py
--rw-rw-r--  2.0 unx     1333 b- defN 23-May-02 13:08 fado/runner/ml/model/module_manager.py
+-rw-rw-r--  2.0 unx     1253 b- defN 23-Mar-21 01:08 fado/runner/ml/model/module_manager.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Feb-18 16:39 fado/runner/ml/model/built_in/__init__.py
 -rw-rw-r--  2.0 unx     5362 b- defN 23-Mar-21 02:44 fado/runner/ml/model/built_in/mnist_conv_torch.py
 -rw-rw-r--  2.0 unx     3267 b- defN 23-Mar-21 00:49 fado/runner/ml/model/built_in/nlafl_dbpedia_tf.py
 -rw-rw-r--  2.0 unx     3085 b- defN 23-Mar-21 00:49 fado/runner/ml/model/built_in/nlafl_emnist_tf.py
 -rw-rw-r--  2.0 unx     4090 b- defN 23-Mar-23 22:15 fado/runner/ml/model/built_in/nlafl_emnist_torch.py
 -rw-rw-r--  2.0 unx     3083 b- defN 23-Mar-21 00:49 fado/runner/ml/model/built_in/nlafl_fashionmnist_tf.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Feb-24 16:15 fado/runner/output/__init__.py
@@ -80,22 +80,22 @@
 -rw-rw-r--  2.0 unx     1160 b- defN 23-Mar-21 00:49 fado/runner/output/table.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Feb-17 16:39 fado/security/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Feb-17 16:39 fado/security/attack/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Mar-21 00:49 fado/security/attack/client/__init__.py
 -rw-rw-r--  2.0 unx      246 b- defN 23-Mar-21 00:49 fado/security/attack/client/attack_base.py
 -rw-rw-r--  2.0 unx     1089 b- defN 23-Mar-21 00:49 fado/security/attack/client/nlafl_poison_attacker.py
 -rw-rw-r--  2.0 unx      502 b- defN 23-Mar-21 00:49 fado/security/attack/client/random_attacker.py
--rw-rw-r--  2.0 unx      990 b- defN 23-May-02 13:09 fado/security/attack/client/server_attack_manager.py
+-rw-rw-r--  2.0 unx      750 b- defN 23-Mar-21 00:49 fado/security/attack/client/server_attack_manager.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Feb-27 13:32 fado/security/attack/network/__init__.py
 -rw-rw-r--  2.0 unx      596 b- defN 23-Mar-21 00:59 fado/security/attack/network/network_attack_manager.py
 -rw-rw-r--  2.0 unx     6868 b- defN 23-Apr-28 16:35 fado/security/attack/network/nlafl_attacker.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Feb-17 16:39 fado/security/defend/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Mar-21 00:49 fado/security/defend/server/__init__.py
 -rw-rw-r--  2.0 unx     1252 b- defN 23-Mar-21 00:49 fado/security/defend/server/clipping_defender.py
 -rw-rw-r--  2.0 unx      237 b- defN 23-Mar-21 00:49 fado/security/defend/server/server_defense_base.py
 -rw-rw-r--  2.0 unx      593 b- defN 23-Mar-21 00:49 fado/security/defend/server/server_defense_manager.py
--rw-rw-r--  2.0 unx      428 b- defN 23-May-02 14:30 FAaDO-0.0.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-02 14:30 FAaDO-0.0.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       47 b- defN 23-May-02 14:30 FAaDO-0.0.0.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       12 b- defN 23-May-02 14:30 FAaDO-0.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     9292 b- defN 23-May-02 14:30 FAaDO-0.0.0.dist-info/RECORD
-99 files, 149717 bytes uncompressed, 48143 bytes compressed:  67.8%
+-rw-rw-r--  2.0 unx      428 b- defN 23-Apr-28 16:40 FAaDO-0.0.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-28 16:40 FAaDO-0.0.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       47 b- defN 23-Apr-28 16:40 FAaDO-0.0.1.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       12 b- defN 23-Apr-28 16:40 FAaDO-0.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     9292 b- defN 23-Apr-28 16:40 FAaDO-0.0.1.dist-info/RECORD
+99 files, 147585 bytes uncompressed, 47528 bytes compressed:  67.8%
```

## zipnote {}

```diff
@@ -276,23 +276,23 @@
 
 Filename: fado/security/defend/server/server_defense_base.py
 Comment: 
 
 Filename: fado/security/defend/server/server_defense_manager.py
 Comment: 
 
-Filename: FAaDO-0.0.0.dist-info/METADATA
+Filename: FAaDO-0.0.1.dist-info/METADATA
 Comment: 
 
-Filename: FAaDO-0.0.0.dist-info/WHEEL
+Filename: FAaDO-0.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: FAaDO-0.0.0.dist-info/entry_points.txt
+Filename: FAaDO-0.0.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: FAaDO-0.0.0.dist-info/top_level.txt
+Filename: FAaDO-0.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: FAaDO-0.0.0.dist-info/RECORD
+Filename: FAaDO-0.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fado/cli/fado_run.py

```diff
@@ -1,18 +1,16 @@
 import argparse
-import importlib
 import itertools
 import logging
 import os
 import shutil
 import socket
 import subprocess
 import sys
 import time
-from distutils.dir_util import copy_tree
 from threading import Thread
 
 from fado.constants import *
 from fado.cli.arguments.arguments import FADOArguments
 from fado.runner import server_run, clients_run
 from fado.runner.output.table import generate_table
 
@@ -24,15 +22,14 @@
     parser = argparse.ArgumentParser()
 
     parser.add_argument('-f', dest='yaml_file', type=str, help='Specify a custom yaml configuration file',
                         required=False)
     mode_parser = parser.add_subparsers(dest="mode", required=False)
 
     build_parser = mode_parser.add_parser('build')
-    mode_parser.add_parser('prepare')
     mode_parser.add_parser('run')
     mode_parser.add_parser('table')
 
     parser.add_argument('-d', dest='dataset', type=str, choices=DATASETS, required=False)
     parser.add_argument('-dr', dest='dataset_rate', help='Fraction of the dataset', type=float,
                         required=False)
     parser.add_argument('-dd', dest='data_distribution', help='Data distribution', type=str, required=False)
@@ -59,15 +56,16 @@
 
     if dataset in LEAF_DATASETS:
         logger.info("Executing LEAF...")
         LEAFDownloader().download()
     elif dataset in NLAFL_DATASETS:
         NLAFLDownloader().download()
     else:
-        fado_arguments.get_class('downloader')().download()
+        logger.info("Executing Torch vision Downloader...")
+        # TODO: TorchVisionDownloader().download()
 
 
 def shape_data(fado_arguments):
     from fado.builder.data.shape.nlafl_shaper import NLAFLShaper
     from fado.builder.data.shape.leaf_shaper import LEAFShaper
 
     dataset = fado_arguments.dataset
@@ -77,15 +75,16 @@
 
     if dataset in LEAF_DATASETS:
         logger.info("Executing LEAF...")
         LEAFShaper().shape()
     elif dataset in NLAFL_DATASETS:
         NLAFLShaper().shape()
     else:
-        fado_arguments.get_class('shaper')().shape()
+        logger.info("Executing Torch vision Shaper ...")
+        # TODO: TorchVisionShaper.shape()
 
 
 def create_networks():
     subprocess.run(['docker', 'network', 'create', 'clients-network'])
     subprocess.run(['docker', 'network', 'create', 'server-network'])
 
 
@@ -93,21 +92,20 @@
     if not docker:
         clients_run.main()
         return
 
     # Start clients container
     subprocess.run(['docker', 'run', '-d', '-w', '/app', '--name', 'fado-clients', '--cap-add=NET_ADMIN',
                     '--network', 'clients-network'] + add_flags +
-                   [f'ralexandre00/fado-node:{FADO_VERSION}', 'bash', '-c', 'tail -f /dev/null'])
+                   ['ralexandre00/fado-node:latest', 'bash', '-c', 'tail -f /dev/null'])
 
     # Send fado_config and data to container
     subprocess.run(['docker', 'cp', f'{FADO_CONFIG_OUT}', 'fado-clients:/app/config/fado_config.yaml'])
     client_data_path = os.path.join(ALL_DATA_FOLDER, fado_args.dataset, 'train')
     subprocess.run(['docker', 'cp', client_data_path, 'fado-clients:/app/data'])
-    subprocess.run(['docker', 'cp', IMPORT_OUT, 'fado-clients:/app/import'])
 
     if dev_mode:
         # Install current fado
         subprocess.run(['docker', 'cp', f'{FADO_SRC}', 'fado-clients:/app/fado'])
         subprocess.run(['docker', 'exec', 'fado-clients', '/bin/bash', './run_dev.sh'], stdout=subprocess.DEVNULL)
 
     # Start clients
@@ -121,23 +119,22 @@
         server_run.main()
         return
 
     # Start server container
     subprocess.run(['docker', 'run', '-d', '-w', '/app', '--name', 'fado-server', '--cap-add=NET_ADMIN',
                     '-v', f'{LOGS_DIRECTORY}:/app/logs', '-v', f'{RESULTS_DIRECTORY}:/app/results',
                     '--network', 'server-network'] + add_flags +
-                   [f'ralexandre00/fado-node:{FADO_VERSION}', 'bash', '-c', 'tail -f /dev/null'])
+                   ['ralexandre00/fado-node:latest', 'bash', '-c', 'tail -f /dev/null'])
 
     # Send fado_config and data to container
     subprocess.run(['docker', 'cp', f'{FADO_CONFIG_OUT}', 'fado-server:/app/config/fado_config.yaml'])
     data_path = os.path.join(ALL_DATA_FOLDER, fado_args.dataset)
     subprocess.run(['docker', 'cp', os.path.join(data_path, 'train'), 'fado-server:/app/data'])
     subprocess.run(['docker', 'cp', os.path.join(data_path, 'test'), 'fado-server:/app/data'])
     subprocess.run(['docker', 'cp', os.path.join(data_path, 'target_test'), 'fado-server:/app/data'])
-    subprocess.run(['docker', 'cp', IMPORT_OUT, 'fado-server:/app/import'])
 
     if dev_mode:
         # Install current fado
         subprocess.run(['docker', 'cp', f'{FADO_SRC}', 'fado-server:/app/fado'])
         subprocess.run(['docker', 'exec', 'fado-server', '/bin/bash', './run_dev.sh'], stdout=subprocess.DEVNULL)
 
     # Start clients
@@ -151,24 +148,23 @@
     if not docker:
         # Do nothing
         return
 
     # Start server container
     subprocess.run(['docker', 'run', '-d', '-w', '/app', '--name', 'fado-router', '--cap-add=NET_ADMIN',
                     '--network', 'server-network'] + add_flags +
-                   [f'ralexandre00/fado-router:{FADO_VERSION}', 'bash', '-c', 'tail -f /dev/null'])
+                   ['ralexandre00/fado-router:latest', 'bash', '-c', 'tail -f /dev/null'])
     subprocess.run(['docker', 'network', 'connect', 'clients-network', 'fado-router'])
 
     # Send fado_config and data to container
     subprocess.run(['docker', 'cp', f'{FADO_CONFIG_OUT}', 'fado-router:/app/config/fado_config.yaml'])
     data_path = os.path.join(ALL_DATA_FOLDER, fado_args.dataset)
     subprocess.run(['docker', 'cp', os.path.join(data_path, 'target_test_attacker'), 'fado-router:/app/data'])
     # Here to copy any data required to build the model
     subprocess.run(['docker', 'cp', os.path.join(data_path, 'train'), 'fado-router:/app/data'])
-    subprocess.run(['docker', 'cp', IMPORT_OUT, 'fado-router:/app/import'])
 
     if dev_mode:
         # Install current fado
         subprocess.run(['docker', 'cp', f'{FADO_SRC}', 'fado-router:/app/fado'])
         subprocess.run(['docker', 'exec', 'fado-router', '/bin/bash', './run_dev.sh'], stdout=subprocess.DEVNULL)
 
     # Start router
@@ -214,69 +210,57 @@
     finally:
         if docker:
             stop_server()
             stop_router()
             stop_clients()
 
 
-def move_files_to_fado_home(fado_arguments, config_file):
+def move_files_to_fado_home(config_file):
     os.makedirs(CONFIG_OUT, exist_ok=True)
     os.makedirs(LOGS_DIRECTORY, exist_ok=True)
-    os.makedirs(IMPORT_OUT, exist_ok=True)
     shutil.copyfile(config_file, FADO_CONFIG_OUT)
-    python_import_folder = os.path.join(fado_arguments.config_path, fado_arguments.python_import_folder)
-    copy_tree(python_import_folder, IMPORT_OUT)
 
 
 def run_multiple(fado_arguments, development, docker):
     # Create a dictionary with all possible combinations of configs to vary
     vary_list = list(itertools.product(*fado_arguments.vary.values()))
     temp_output = os.path.join(TEMP_DIRECTORY, 'fado_config.yaml')
     os.makedirs(TEMP_DIRECTORY, exist_ok=True)
 
     # For each combination execute fado run
     for experiment in vary_list:
-        # Set varying parameters
         for i, vary_key in enumerate(fado_arguments.vary.keys()):
             fado_arguments.set_argument(vary_key, experiment[i])
 
         # Save current experiment fado_config file in temp folder
         fado_arguments.save_to_file(temp_output)
         logger.info(f"Running experiment {experiment}")
 
         fado_arguments_experiment = FADOArguments(temp_output)
 
-        move_files_to_fado_home(fado_arguments_experiment, temp_output)
+        move_files_to_fado_home(temp_output)
         download_data(fado_arguments_experiment)
         shape_data(fado_arguments_experiment)
         run(fado_arguments_experiment, development, docker)
     os.remove(temp_output)
 
 
-def verify_docker_install():
-    # TODO:
-    pass
-
-
 def cli():
     args = parse_args(sys.argv[1:])
 
     if args.yaml_file:
         config_file = args.yaml_file
     else:
         fado_config_env = os.getenv('FADO_CONFIG')
         config_file = fado_config_env if fado_config_env else FADO_DEFAULT_CONFIG_FILE_PATH
 
     fado_arguments = FADOArguments(config_file)
 
-    if args.mode == 'prepare':
-        verify_docker_install()
-        logger.info("Pulling required docker images -q")
-        subprocess.run(['docker', 'pull', f'ralexandre00/fado-node-requirements:{FADO_VERSION}'])
-        subprocess.run(['docker', 'pull', f'ralexandre00/fado-router:{FADO_VERSION}'])
+    # docker pull ralexandre00/fado-node-requirements
+
     if args.mode == 'build':
         build_mode = args.build_mode
         move_files_to_fado_home(config_file)
 
         if build_mode == 'download':
             download_data(fado_arguments)
         elif build_mode == 'shape':
```

## fado/cli/arguments/arguments.py

```diff
@@ -1,60 +1,46 @@
-import importlib
-import logging
-import os
 import random
-import sys
-from pathlib import Path
 
 import yaml
 
-from fado.constants import IMPORT_OUT
-
-logger = logging.getLogger('fado')
-logger = logging.LoggerAdapter(logger, {'node_id': 'arguments'})
 
 class FADOArguments:
     """ A class for reading arguments from a yaml file """
 
     def __init__(self, config_path=None):
         """
             Parameters:
                 config_path(str): path of yaml configuration file
         """
         if config_path is not None:
             with open(config_path, 'r') as file:
                 args = yaml.load(file, Loader=yaml.FullLoader)
 
-            config_path = Path(config_path).parent.absolute().__str__()
-            setattr(self, 'config_path', config_path)
-            self._set_arguments(args, config_path)
+            self._set_arguments(args)
             self._process_arguments()
 
     def __new__(cls, config_path=None):
         if not hasattr(cls, 'instance'):
             cls.instance = super(FADOArguments, cls).__new__(cls)
         return cls.instance
 
     def _process_arguments(self):
         """ Uses the arguments read to do needed computations"""
         if 'random_seed' in self:
             random.seed(self.random_seed)
             # TODO: check if TF or Torch is in use and set seed
-        if 'python_import_folder' in self:
-            sys.path.append(os.path.join(IMPORT_OUT))
-            sys.path.append('/app/import')
 
-    def _set_arguments(self, key_pairs, config_path):
+    def _set_arguments(self, key_pairs):
         """ Sets the arguments
             Parameters:
                 key_pairs(dict): key, value pairs with sections(dicts) that contain n (property_name, property_value)
         """
         for section_name, section in key_pairs.items():
             if type(section) == dict:
-                self._set_arguments(section, config_path)
+                self._set_arguments(section)
             elif type(section) == list:
                 if 'vary' not in self:
                     self.vary = {}
                 self.vary[section_name] = section
             else:
                 setattr(self, section_name, section)
 
@@ -66,12 +52,7 @@
 
     def __contains__(self, key):
         return hasattr(self, key)
 
     def save_to_file(self, file_path):
         with open(file_path, 'w') as file:
             yaml.dump(self.__dict__, file)
-
-    def get_class(self, key):
-        module_name = os.path.join(self.get_argument(key))[:-3]
-        module = importlib.import_module(module_name)
-        return module.get_class()
```

## fado/constants/__init__.py

```diff
@@ -3,30 +3,27 @@
 import fado
 from fado.builder import crypto, default
 
 fado_module_dir = os.path.dirname(fado.__file__)
 crypto_module_dir = os.path.dirname(crypto.__file__)
 default_module_dir = os.path.dirname(default.__file__)
 
-FADO_VERSION = "0.0.2"
-
 FADO_DIR = os.getenv('FADO_HOME_FOLDER', os.path.join(os.path.expanduser("~"), '.fado'))
 FADO_SRC = os.path.join(fado_module_dir)
 
 CERTS_PATH = os.path.join(crypto_module_dir, 'certs')
 FADO_DEFAULT_CONFIG_FILE_PATH = os.path.join(default_module_dir, 'fado_config.yaml')
 
 CONFIG_HASH = os.path.join(FADO_DIR, '.config_hash')
 LOGS_DIRECTORY = os.path.join(FADO_DIR, 'logs')
 RESULTS_DIRECTORY = os.path.join(FADO_DIR, 'results')
 TENSORBOARD_DIRECTORY = os.path.join(FADO_DIR, 'runs')
 ATTACK_DIRECTORY = os.path.join(FADO_DIR, 'attack')
 DEFENSE_DIRECTORY = os.path.join(FADO_DIR, 'defense')
 CONFIG_OUT = os.path.join(FADO_DIR, 'config')
-IMPORT_OUT = os.path.join(FADO_DIR, 'import')
 FADO_CONFIG_OUT = os.path.join(CONFIG_OUT, 'fado_config.yaml')
 BENIGN_CONFIG_OUT = os.path.join(CONFIG_OUT, 'benign_ranks.csv')
 MAL_CONFIG_OUT = os.path.join(CONFIG_OUT, 'malicious_ranks.csv')
 CERTS_OUT = os.path.join(FADO_DIR, 'certs')
 DOCKER_COMPOSE_OUT = os.path.join(FADO_DIR, 'docker-compose.yml')
 TEMP_DIRECTORY = os.path.join(FADO_DIR, 'temp')
 
@@ -34,12 +31,12 @@
 
 IMAGES_PATH = os.path.join(FADO_DIR, 'docker')
 FEDML_IMAGE = os.path.join(IMAGES_PATH, 'client')
 ROUTER_IMAGE = os.path.join(IMAGES_PATH, 'router')
 
 LEAF_DATASETS = ['femnist', 'emnist', 'shakespeare', 'sent140']
 NLAFL_DATASETS = ['nlafl_emnist', 'nlafl_fashionmnist', 'nlafl_dbpedia']
-DATASETS = ['custom', 'cifar10', 'cifar100', 'mnist'] + LEAF_DATASETS + NLAFL_DATASETS
+DATASETS = ['cifar10', 'cifar100', 'mnist'] + LEAF_DATASETS + NLAFL_DATASETS
 
 SERVER_IP = '10.0.0.2'
 SERVER_PORT = 51000
 SERVER_PUB_PORT = 51001
```

## fado/runner/fl/aggregate/aggregator_manager.py

```diff
@@ -8,12 +8,10 @@
 class AggregatorManager:
 
     @classmethod
     def get_aggregator(cls, global_module) -> Aggregator:
         args = FADOArguments()
         if args.aggregator == 'mean':
             return MeanAggregator(global_module)
-        elif '.py' in args.aggregator:
-            return args.get_class('aggregator')(global_module)
         else:
             raise Exception("Specified aggregator does not exist")
         pass
```

## fado/runner/fl/select/participant_selector_manager.py

```diff
@@ -6,11 +6,10 @@
 class ParticipantSelectorManager:
 
     @classmethod
     def get_selector(cls) -> ParticipantSelector:
         args = FADOArguments()
         if args.participant_selector == 'random':
             return RandomParticipantSelector()
-        elif '.py' in args.participant_selector:
-            return args.get_class('participant_selector')()
         else:
             raise Exception("Specified participant selector does not exist")
+        pass
```

## fado/runner/ml/model/module_manager.py

```diff
@@ -15,14 +15,12 @@
                 return NlaflEmnistTf()
             elif args.model == 'nlafl_fashionmnist_tf':
                 from fado.runner.ml.model.built_in.nlafl_fashionmnist_tf import NlaflFashionmnistTf
                 return NlaflFashionmnistTf()
             elif args.model == 'nlafl_dbpedia_tf':
                 from fado.runner.ml.model.built_in.nlafl_dbpedia_tf import NlaflDbpediaTf
                 return NlaflDbpediaTf()
-        elif args.model in ['mnist_conv_torch']:
+        if args.model in ['mnist_conv_torch']:
             from fado.runner.ml.model.built_in.mnist_conv_torch import MnistConvTorch
             return MnistConvTorch()
-        elif 'py' in args.model:
-            return args.get_class('model')()
         else:
             raise Exception(f"Model {args.model} not found")
```

## fado/security/attack/client/server_attack_manager.py

```diff
@@ -1,28 +1,22 @@
-import logging
 from typing import Type
 
 from fado.cli.arguments.arguments import FADOArguments
 from fado.security.attack.client.attack_base import Attack
 from fado.security.attack.client.random_attacker import RandomAttacker
 from fado.security.attack.client.nlafl_poison_attacker import NLAFLPoisonAttacker
 
-logger = logging.getLogger("fado")
-logger = logging.LoggerAdapter(logger, {'node_id': 'none'})
-
 
 class ClientAttackManager:
 
     @classmethod
     def get_attacker(cls, client_id) -> Attack:
         args = FADOArguments()
 
         model_attack_name = args.model_attack_name if 'model_attack_name' in args else None
-
+        
         if model_attack_name == 'random':
             return RandomAttacker()
         elif model_attack_name == 'nlafl_poison':
             return NLAFLPoisonAttacker(client_id=client_id)
-        elif 'py' in model_attack_name:
-            return args.get_class('model_attack_name')()
         else:
-            raise Exception(f"Model {model_attack_name} not found")
+            return Attack()
```

## Comparing `FAaDO-0.0.0.dist-info/RECORD` & `FAaDO-0.0.1.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 fado/builder/data/leaf/utils/util.py,sha256=f3e06hf2Zgu6iQOhz4Ww03S_EoIVYph5OiivVqvg3Dk,839
 fado/builder/data/shape/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fado/builder/data/shape/leaf_shaper.py,sha256=8F1zpFArOgTBq9k4GEQ8DnCWz_CA7I-91tM5ZDu90Hc,4003
 fado/builder/data/shape/nlafl_shaper.py,sha256=11gq7XcUjLjUN8ntLYBLJKqaZKK8RETBl0OetuRQEuw,13753
 fado/builder/data/shape/shaper.py,sha256=3AVETZM2_wfQ_L7PGI_55DiWHdDxQkYgQbwX8N6cuUg,110
 fado/builder/default/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fado/cli/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-fado/cli/fado_run.py,sha256=aKxotdl6OeVYNpf-xg3VZKkMM5zpnw5ku3ewRr8nBHY,12281
+fado/cli/fado_run.py,sha256=D_HvJ8Qu3jTV6XzyeGbWyDThktQz6pqn7gItNkAfUdc,11452
 fado/cli/arguments/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-fado/cli/arguments/arguments.py,sha256=Ni5xEFdaCcH3Wv4vTtjxjBTxBiaHKLU6pPfOlbkc-js,2550
-fado/constants/__init__.py,sha256=lnJwxq1Rwk2ceiFi42CvDN-8Q68rw9335LD7R275eKY,1769
+fado/cli/arguments/arguments.py,sha256=aKe4WLScVfW7HLIJ3It7q7OSFG-B0E0ExfCj32BCL74,1845
+fado/constants/__init__.py,sha256=IkvoWlslxQkd_YEwradndww1DL6dn7pEY35xcDBOAak,1689
 fado/runner/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fado/runner/clients_run.py,sha256=snFTC14Vs-Z8ahVDjjzPDO4Dt9QFAEwUzdF_0Y3qGcc,2390
 fado/runner/router_run.py,sha256=y_LZB80Eg59TnyaE2DLbo-sIFtBRXzOIeDf6-bHmO7E,3784
 fado/runner/server_run.py,sha256=bm_FnaYJwOckv_myzX9uDjDACF1zd2z2smDdcJWMZbM,1883
 fado/runner/communication/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fado/runner/communication/base_com_manager.py,sha256=cDmBzyLtKiX4bjE_vI_c0H5CFjS72EUg0fZDFliIuJc,518
 fado/runner/communication/fl_com_manager.py,sha256=PggM9QCYKR2Ssf4aatM7FOmJUWKdj3QWy6xevqRl0gI,475
@@ -53,25 +53,25 @@
 fado/runner/data/load/base_data_loader.py,sha256=0ZENP_12jeqbsh3fwVDIl6skYVPY_1Yv1eMNkwbYFg0,842
 fado/runner/data/load/client_data_loader.py,sha256=8-fUORtT0IyWa5y9cZ8t8I0W3eaYvFBdXqsJK5iymnw,782
 fado/runner/data/load/server_data_loader.py,sha256=dPqDDAgejcg2m78lpXsuzL4hjW9g1T8XEgRI4QMNxsQ,1307
 fado/runner/fl/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fado/runner/fl/fl_client.py,sha256=Wu-nrPMI-vMUnQ-cUbrh7lz2oBtoaY3zTKgBWheqmCo,2414
 fado/runner/fl/fl_server.py,sha256=IsiJ6Ml8iclDC_qhm2O-AdD355kSoCske521xrlNQ20,7013
 fado/runner/fl/aggregate/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-fado/runner/fl/aggregate/aggregator_manager.py,sha256=yOfPjMwlZsJMkzKDqCk0T-nLO2-4QGuXVOROT7mtMTE,629
+fado/runner/fl/aggregate/aggregator_manager.py,sha256=2oEycRhHtyPJ_XDnHY10r1AmxcAJG3xfCfCJvq-ekqs,527
 fado/runner/fl/aggregate/base_aggregator.py,sha256=b3FBUjJciRgbR8RSPFKDhTKnehOKIq0gq5XGUDk6FGY,302
 fado/runner/fl/aggregate/mean_aggregator.py,sha256=-jfHDc-MFlLvBdhZJD8cNwXxWClGBnYP5w3lm-vGzDc,934
 fado/runner/fl/select/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fado/runner/fl/select/base_participant_selector.py,sha256=Suq_vKMELzQpewaqm5aym9UVZ1mKU07SU0fDJMFou2Q,196
-fado/runner/fl/select/participant_selector_manager.py,sha256=N43fxg6nr5GBl622rJ_8xe-cxtWJP8QD0SqQzp3Mee0,655
+fado/runner/fl/select/participant_selector_manager.py,sha256=YMiJSTnFu8PoKKbG2eT-afSlyUwFft4yUTcKlJkIFv0,559
 fado/runner/fl/select/random_participant_selector.py,sha256=kX_UnHSZ_Xtu-Qw3zevm9hPxLvCBhkmhOK4ycQZzDHo,296
 fado/runner/ml/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fado/runner/ml/model/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fado/runner/ml/model/fado_module.py,sha256=9QutAlujajouTPavDrkadw7UwIk7pe-5786QnBrsYGw,325
-fado/runner/ml/model/module_manager.py,sha256=lslEEjVvWHn_veZKjPIHSBY3_9gZcT5JryenwRF5Kc8,1333
+fado/runner/ml/model/module_manager.py,sha256=OiuBiFC0LNH1xYyTTXT5_8wgNDzmbb3Zq2LTlv47BLs,1253
 fado/runner/ml/model/built_in/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fado/runner/ml/model/built_in/mnist_conv_torch.py,sha256=JtMlXlcJwgl6XZ6NdQXA50dTJWBe6S-6_bEk78O1SXQ,5362
 fado/runner/ml/model/built_in/nlafl_dbpedia_tf.py,sha256=cDuVkKPSFZhZRByxB27Hl1Cy4618s7N7pfPJ_ZpgqPA,3267
 fado/runner/ml/model/built_in/nlafl_emnist_tf.py,sha256=gfMAJQXwbJ_r1kvyKwU1QO-oDVsbFvOzAs11Kk5hunc,3085
 fado/runner/ml/model/built_in/nlafl_emnist_torch.py,sha256=HIYN9R_MD16cOb4AlhnHCW8QrLhEVVCfPDmZILs-kFQ,4090
 fado/runner/ml/model/built_in/nlafl_fashionmnist_tf.py,sha256=F8H1TJKNTHrhff0ayFc6pWZGCwgJHa2WZ-KGjshL7GQ,3083
 fado/runner/output/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -79,21 +79,21 @@
 fado/runner/output/table.py,sha256=ceWCaJjz0e9RUPM319uMe_kpfGcTf4USyg4eCVslxRk,1160
 fado/security/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fado/security/attack/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fado/security/attack/client/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fado/security/attack/client/attack_base.py,sha256=vdb_6rFZLE3qlUjqDFFdLe1sIhgIoG-D40BxMG9CE-k,246
 fado/security/attack/client/nlafl_poison_attacker.py,sha256=hcfhYJ2s6YSybRa7pg2g_5vZXTrdRLJD2wRvz_fwqok,1089
 fado/security/attack/client/random_attacker.py,sha256=ElM3t1SmaSqvrVINB3DePbauAUVJtPcGIAVJYNvWQTQ,502
-fado/security/attack/client/server_attack_manager.py,sha256=6lXVqZcFns-CG86qakyx3znAvgpRjFgt0LbIMEW8y70,990
+fado/security/attack/client/server_attack_manager.py,sha256=ohvPlRgpXReGKjyz1xRRDem9gnyuB7TaZ0AkDuKh2Gw,750
 fado/security/attack/network/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fado/security/attack/network/network_attack_manager.py,sha256=g3QMZanQtkLaJvClNWWx9yvFTYFYs8sJE3nCDY6R8f0,596
 fado/security/attack/network/nlafl_attacker.py,sha256=8SPp89j810JgMOL2yE4dVjRD69v6wxZ3TnXpNodXLrE,6868
 fado/security/defend/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fado/security/defend/server/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fado/security/defend/server/clipping_defender.py,sha256=m53Bikw_RNN3SbbmU5pKLErldjWHo8aEPnvIQC77s-E,1252
 fado/security/defend/server/server_defense_base.py,sha256=u4q4f5Ui9nhuplpCOjAFczMe0eD5g_DiPozCW6aTiG0,237
 fado/security/defend/server/server_defense_manager.py,sha256=BMwRFoFqp0jj3Jaarn9NS7eMOEjfT30nkMuBxfvDMzA,593
-FAaDO-0.0.0.dist-info/METADATA,sha256=rdituY8EGeaun-rcxT-5L1rN-Q75a_jBDVvfuNjyxqw,428
-FAaDO-0.0.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-FAaDO-0.0.0.dist-info/entry_points.txt,sha256=kg8vWFB7vm1lFSnJPE32ifCR33x0_F-xGxXOZ9bkhnM,47
-FAaDO-0.0.0.dist-info/top_level.txt,sha256=6ExdU3XhrMitkINHWvNndTM5Yd7d8sDJJw3WCPK-008,12
-FAaDO-0.0.0.dist-info/RECORD,,
+FAaDO-0.0.1.dist-info/METADATA,sha256=bTPBWot7YohDhk3XhmYPzHOOriOeEYyDcRJ-L8vs5io,428
+FAaDO-0.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+FAaDO-0.0.1.dist-info/entry_points.txt,sha256=kg8vWFB7vm1lFSnJPE32ifCR33x0_F-xGxXOZ9bkhnM,47
+FAaDO-0.0.1.dist-info/top_level.txt,sha256=6ExdU3XhrMitkINHWvNndTM5Yd7d8sDJJw3WCPK-008,12
+FAaDO-0.0.1.dist-info/RECORD,,
```

