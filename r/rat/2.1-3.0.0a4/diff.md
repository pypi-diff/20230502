# Comparing `tmp/rat-2.1.tar.gz` & `tmp/rat-3.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rat-2.1.tar", last modified: Wed Oct 12 15:43:27 2022, max compression
+gzip compressed data, was "rat-3.0.0a4.tar", last modified: Tue May  2 17:36:27 2023, max compression
```

## Comparing `rat-2.1.tar` & `rat-3.0.0a4.tar`

### file list

```diff
@@ -1,51 +1,58 @@
-drwxrwxr-x   0 pdas47    (1002) pdas47    (1002)        0 2022-10-12 15:43:27.424335 rat-2.1/
--rw-rw-r--   0 pdas47    (1002) pdas47    (1002)    35148 2022-10-11 21:08:02.000000 rat-2.1/LICENSE
--rw-rw-r--   0 pdas47    (1002) pdas47    (1002)     7864 2022-10-12 15:43:27.423335 rat-2.1/PKG-INFO
--rw-rw-r--   0 pdas47    (1002) pdas47    (1002)     7317 2022-10-11 21:08:44.000000 rat-2.1/README.md
--rw-rw-r--   0 pdas47    (1002) pdas47    (1002)      626 2022-10-12 15:43:11.000000 rat-2.1/pyproject.toml
--rw-rw-r--   0 pdas47    (1002) pdas47    (1002)       38 2022-10-12 15:43:27.424335 rat-2.1/setup.cfg
--rw-rw-r--   0 pdas47    (1002) pdas47    (1002)      144 2022-10-12 15:43:16.000000 rat-2.1/setup.py
-drwxrwxr-x   0 pdas47    (1002) pdas47    (1002)        0 2022-10-12 15:43:27.414335 rat-2.1/src/
-drwxrwxr-x   0 pdas47    (1002) pdas47    (1002)        0 2022-10-12 15:43:27.416335 rat-2.1/src/rat/
--rw-rw-r--   0 pdas47    (1002) pdas47    (1002)        0 2022-10-11 18:01:38.000000 rat-2.1/src/rat/__init__.py
-drwxrwxr-x   0 pdas47    (1002) pdas47    (1002)        0 2022-10-12 15:43:27.419335 rat-2.1/src/rat/core/
--rw-rw-r--   0 pdas47    (1002) pdas47    (1002)    10536 2022-10-11 18:01:38.000000 rat-2.1/src/rat/core/generate_plots.py
--rw-rw-r--   0 pdas47    (1002) pdas47    (1002)     6434 2022-10-11 18:01:38.000000 rat-2.1/src/rat/core/run_altimetry.py
--rw-rw-r--   0 pdas47    (1002) pdas47    (1002)     2284 2022-10-11 18:01:38.000000 rat-2.1/src/rat/core/run_metsim.py
--rw-rw-r--   0 pdas47    (1002) pdas47    (1002)    10492 2022-10-11 18:01:38.000000 rat-2.1/src/rat/core/run_postprocessing.py
--rw-rw-r--   0 pdas47    (1002) pdas47    (1002)     5666 2022-10-11 18:01:38.000000 rat-2.1/src/rat/core/run_routing.py
--rw-rw-r--   0 pdas47    (1002) pdas47    (1002)     2384 2022-10-11 18:01:38.000000 rat-2.1/src/rat/core/run_sarea.py
--rw-rw-r--   0 pdas47    (1002) pdas47    (1002)     3937 2022-10-11 18:01:38.000000 rat-2.1/src/rat/core/run_vic.py
-drwxrwxr-x   0 pdas47    (1002) pdas47    (1002)        0 2022-10-12 15:43:27.420335 rat-2.1/src/rat/core/sarea/
--rw-rw-r--   0 pdas47    (1002) pdas47    (1002)    16235 2022-10-11 18:01:38.000000 rat-2.1/src/rat/core/sarea/TMS.py
--rw-rw-r--   0 pdas47    (1002) pdas47    (1002)    19114 2022-10-11 18:01:38.000000 rat-2.1/src/rat/core/sarea/sarea_cli_l8.py
--rw-rw-r--   0 pdas47    (1002) pdas47    (1002)    17417 2022-10-11 18:01:38.000000 rat-2.1/src/rat/core/sarea/sarea_cli_s2.py
--rw-rw-r--   0 pdas47    (1002) pdas47    (1002)     6091 2022-10-11 18:01:38.000000 rat-2.1/src/rat/core/sarea/sarea_cli_sar.py
-drwxrwxr-x   0 pdas47    (1002) pdas47    (1002)        0 2022-10-12 15:43:27.420335 rat-2.1/src/rat/data_processing/
--rw-rw-r--   0 pdas47    (1002) pdas47    (1002)        0 2022-10-11 18:01:38.000000 rat-2.1/src/rat/data_processing/__init__.py
--rw-rw-r--   0 pdas47    (1002) pdas47    (1002)    32640 2022-10-11 18:01:38.000000 rat-2.1/src/rat/data_processing/altimetry.py
--rw-rw-r--   0 pdas47    (1002) pdas47    (1002)     7440 2022-10-11 18:01:38.000000 rat-2.1/src/rat/data_processing/metsim_input_processing.py
--rw-rw-r--   0 pdas47    (1002) pdas47    (1002)    24408 2022-10-11 18:01:38.000000 rat-2.1/src/rat/data_processing/newdata.py
-drwxrwxr-x   0 pdas47    (1002) pdas47    (1002)        0 2022-10-12 15:43:27.421335 rat-2.1/src/rat/ee_utils/
--rw-rw-r--   0 pdas47    (1002) pdas47    (1002)        0 2022-10-11 18:01:38.000000 rat-2.1/src/rat/ee_utils/__init__.py
--rw-rw-r--   0 pdas47    (1002) pdas47    (1002)     3855 2022-10-11 18:01:38.000000 rat-2.1/src/rat/ee_utils/ee_aec_file_creator.py
--rw-rw-r--   0 pdas47    (1002) pdas47    (1002)      256 2022-10-11 18:01:38.000000 rat-2.1/src/rat/ee_utils/ee_config_template.py
--rw-rw-r--   0 pdas47    (1002) pdas47    (1002)     1103 2022-10-11 18:01:38.000000 rat-2.1/src/rat/ee_utils/ee_utils.py
--rw-rw-r--   0 pdas47    (1002) pdas47    (1002)    31680 2022-10-11 18:01:38.000000 rat-2.1/src/rat/rat.py
--rw-rw-r--   0 pdas47    (1002) pdas47    (1002)     6322 2022-10-11 18:01:38.000000 rat-2.1/src/rat/run_rat.py
-drwxrwxr-x   0 pdas47    (1002) pdas47    (1002)        0 2022-10-12 15:43:27.423335 rat-2.1/src/rat/utils/
--rw-rw-r--   0 pdas47    (1002) pdas47    (1002)        0 2022-10-11 18:01:38.000000 rat-2.1/src/rat/utils/__init__.py
--rw-rw-r--   0 pdas47    (1002) pdas47    (1002)     8112 2022-10-11 18:01:38.000000 rat-2.1/src/rat/utils/convert_for_website.py
--rw-rw-r--   0 pdas47    (1002) pdas47    (1002)     7389 2022-10-11 18:01:38.000000 rat-2.1/src/rat/utils/files_creator.py
--rw-rw-r--   0 pdas47    (1002) pdas47    (1002)     4634 2022-10-11 18:01:38.000000 rat-2.1/src/rat/utils/logging.py
--rw-rw-r--   0 pdas47    (1002) pdas47    (1002)     1849 2022-10-11 18:01:38.000000 rat-2.1/src/rat/utils/metsim_param_reader.py
--rw-rw-r--   0 pdas47    (1002) pdas47    (1002)     8403 2022-10-11 18:01:38.000000 rat-2.1/src/rat/utils/route_param_reader.py
--rw-rw-r--   0 pdas47    (1002) pdas47    (1002)     1062 2022-10-11 18:01:38.000000 rat-2.1/src/rat/utils/run_command.py
--rw-rw-r--   0 pdas47    (1002) pdas47    (1002)     1768 2022-10-11 18:01:38.000000 rat-2.1/src/rat/utils/science.py
--rw-rw-r--   0 pdas47    (1002) pdas47    (1002)     1692 2022-10-11 18:01:38.000000 rat-2.1/src/rat/utils/utils.py
--rw-rw-r--   0 pdas47    (1002) pdas47    (1002)    23838 2022-10-11 18:01:38.000000 rat-2.1/src/rat/utils/vic_param_reader.py
-drwxrwxr-x   0 pdas47    (1002) pdas47    (1002)        0 2022-10-12 15:43:27.417335 rat-2.1/src/rat.egg-info/
--rw-rw-r--   0 pdas47    (1002) pdas47    (1002)     7864 2022-10-12 15:43:27.000000 rat-2.1/src/rat.egg-info/PKG-INFO
--rw-rw-r--   0 pdas47    (1002) pdas47    (1002)     1151 2022-10-12 15:43:27.000000 rat-2.1/src/rat.egg-info/SOURCES.txt
--rw-rw-r--   0 pdas47    (1002) pdas47    (1002)        1 2022-10-12 15:43:27.000000 rat-2.1/src/rat.egg-info/dependency_links.txt
--rw-rw-r--   0 pdas47    (1002) pdas47    (1002)        4 2022-10-12 15:43:27.000000 rat-2.1/src/rat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:27.148266 rat-3.0.0a4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-02 17:36:15.000000 rat-3.0.0a4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    43730 2023-05-02 17:36:27.144266 rat-3.0.0a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-05-02 17:36:15.000000 rat-3.0.0a4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-02 17:36:15.000000 rat-3.0.0a4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 17:36:27.148266 rat-3.0.0a4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-02 17:36:15.000000 rat-3.0.0a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:27.132266 rat-3.0.0a4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:27.136266 rat-3.0.0a4/src/rat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:27.136266 rat-3.0.0a4/src/rat/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)    11137 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/cli/rat_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/cli/rat_init_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/cli/rat_test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:27.140266 rat-3.0.0a4/src/rat/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/core/run_altimetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/core/run_metsim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/core/run_postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5766 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/core/run_routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/core/run_sarea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/core/run_vic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:27.140266 rat-3.0.0a4/src/rat/core/sarea/
+-rw-r--r--   0 runner    (1001) docker     (123)    21334 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/core/sarea/TMS.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19904 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/core/sarea/sarea_cli_l8.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20478 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/core/sarea/sarea_cli_l9.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18180 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/core/sarea/sarea_cli_s2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/core/sarea/sarea_cli_sar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:27.144266 rat-3.0.0a4/src/rat/data_processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/data_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32463 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/data_processing/altimetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8457 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/data_processing/metsim_input_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28327 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/data_processing/newdata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:27.144266 rat-3.0.0a4/src/rat/ee_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/ee_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/ee_utils/ee_aec_file_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/ee_utils/ee_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/ee_utils/ee_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40632 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/rat_basin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9611 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/run_rat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:27.144266 rat-3.0.0a4/src/rat/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/utils/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/utils/convert_to_final_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/utils/files_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/utils/metsim_param_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8343 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/utils/route_param_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/utils/run_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/utils/science.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23852 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/utils/vic_param_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:27.136266 rat-3.0.0a4/src/rat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    43730 2023-05-02 17:36:27.000000 rat-3.0.0a4/src/rat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-02 17:36:27.000000 rat-3.0.0a4/src/rat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 17:36:27.000000 rat-3.0.0a4/src/rat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-02 17:36:27.000000 rat-3.0.0a4/src/rat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:27.144266 rat-3.0.0a4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-02 17:36:15.000000 rat-3.0.0a4/tests/test_imports.py
```

### Comparing `rat-2.1/LICENSE` & `rat-3.0.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `rat-2.1/pyproject.toml` & `rat-3.0.0a4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rat"
-version = "2.1"
+version = "3.0.0.alpha.4"
 authors = [
   { name="Pritam Das", email="pdas47@uw.edu" },
   { name="Sanchit Minocha", email="msanchit@uw.edu" },
 ]
 description = "Resevoir Monitoring using Satellite Remote Sensing"
 requires-python = ">=3.6"
 readme = "README.md"
+license = {file = "LICENSE"}
 classifiers = [
     "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
+    "License :: OSI Approved :: MIT License"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/UW-SASWE/RAT"
 "Bug Tracker" = "https://github.com/UW-SASWE/RAT/issues"
```

### Comparing `rat-2.1/src/rat/core/run_altimetry.py` & `rat-3.0.0a4/src/rat/core/run_altimetry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import configparser
 import os
 import pandas as pd
 import geopandas as gpd
-from utils.utils import create_directory
-from data_processing import altimetry as alt
+from rat.utils.utils import create_directory
+from rat.data_processing import altimetry as alt
 
 
 def altimeter_routine(reservoir_df, reservoir_column_dict, j3tracks, custom_reservoir_range_dict,
                                          user, password, lastcycle_no, basin_name, basin_data_dir, geoidpath, save_dirpath):
     resname = str(reservoir_df[reservoir_column_dict['unique_identifier']])
     latest_cycle = lastcycle_no         # for initializing latest cycle number
```

### Comparing `rat-2.1/src/rat/core/run_metsim.py` & `rat-3.0.0a4/src/rat/core/run_metsim.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,33 @@
+from http.server import executable
 from logging import getLogger
-import yaml
+import numpy as np
 import os
 import xarray as xr
-from utils.logging import LOG_NAME, NOTIFICATION
-from utils.run_command import run_command
-from utils.utils import create_directory
+from rat.utils.logging import LOG_NAME, NOTIFICATION
+from rat.utils.run_command import run_command
+from rat.utils.utils import create_directory
 
 log = getLogger(f"{LOG_NAME}.{__name__}")
 
 class MetSimRunner():
     def __init__(self, param_path, metsim_env, results_path, multiprocessing, conda_hook=None) -> None:
         self._param_path = param_path
         self._metsim_env = metsim_env
         self._conda_hook = conda_hook
         self.results_path = results_path
         self._mp = multiprocessing
 
     def run_metsim(self):
         if not self._conda_hook:
-            args = f'source activate {self._metsim_env} && ms -n {self._mp} {self._param_path}'
+            args = f'eval "$(conda shell.bash hook)" && conda activate {self._metsim_env} && ms -n {self._mp} {self._param_path}'
         else:
             args = f'source {self._conda_hook} && conda activate {self._metsim_env} && ms -n {self._mp} {self._param_path}'
         # print("will run: ", args)
-        ret_code = run_command(args, metsim=True, shell=True)
+        ret_code = run_command(args, metsim=True, shell=True, executable="/bin/bash")
     
     def convert_to_vic_forcings(self, forcings_dir):
         # The results have to be converted to VIC readable yearly netcdf files.
         ds = xr.open_dataset(self.results_path).load()
         
         years, dataset = zip(*ds.groupby('time.year'))
         paths = [os.path.join(forcings_dir, f'forcing_{y}.nc') for y in years]
@@ -41,13 +42,13 @@
                 existing.close()
 
                 log.debug(f"Writing file for year {year}: {p} -- Updating existing")
                 # xr.merge([existing, ds], compat='override', join='outer').to_netcdf(p)
                 # xr.concat([existing, ds], dim='time').to_netcdf(p)
                 last_existing_time = existing.time[-1]
                 log.debug("Existing data: %s", last_existing_time)
-                ds = ds.sel(time=slice(last_existing_time, ds.time[-1]))
-                ds = ds.isel(time=slice(1, None))
+                ds = ds.sel(time=slice(last_existing_time + np.timedelta64(6,'h'), ds.time[-1]))
+                #ds = ds.isel(time=slice(1, None))
                 xr.merge([existing, ds]).to_netcdf(p)
             else:
                 log.debug(f"Writing file for year {year}: {p} -- Updating new")
                 ds.to_netcdf(p)
```

### Comparing `rat-2.1/src/rat/core/run_postprocessing.py` & `rat-3.0.0a4/src/rat/core/run_postprocessing.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 import os
-import datetime
-import subprocess
 import pandas as pd
 import numpy as np
 import xarray as xr
 import geopandas as gpd
 import warnings
+import datetime
 
 warnings.filterwarnings("ignore")
 
 from logging import getLogger
-from utils.logging import LOG_NAME, NOTIFICATION
-from utils.utils import create_directory
-from utils.science import penman
+from rat.utils.logging import LOG_NAME, NOTIFICATION
+from rat.utils.science import penman
 
 log = getLogger(f"{LOG_NAME}.{__name__}")
 
 
 def calc_dels(aecpath, sareapath, savepath):
     aec = pd.read_csv(aecpath)
     df = pd.read_csv(sareapath, parse_dates=['date'])
@@ -102,38 +100,50 @@
         # print(f"[!] {len(points_within)} Grid cells inside reservoir found, averaging their values")
         data = reqvars.sel(lat=points_within.y, lon=points_within.x, method='nearest').to_dataframe().reset_index().groupby('time').mean()[1:]
 
         P = forcings.sel(lat=points_within.y, lon=points_within.x, method='nearest').resample({'time':'1D'}).mean().to_dataframe().groupby('time').mean()[1:]
 
     data['area'] = sarea_interpolated['area']
     data['P'] = P
-    print(data)
     data = data.dropna()
-    data['penman_E'] = data.apply(lambda row: penman(row['OUT_R_NET'], row['OUT_AIR_TEMP'], row['OUT_WIND'], row['OUT_VP'], row['P'], row['area']), axis=1)
-    data = data.reset_index()
-
-    # Save (Writing new file if not exist otherwise append)
-    if os.path.isfile(savepath):
-        existing_data = pd.read_csv(savepath, parse_dates=['time'])
-        new_data = data[['time', 'penman_E']].rename({'penman_E': 'OUT_EVAP'}, axis=1)
-        # Concat the two dataframes into a new dataframe holding all the data (memory intensive):
-        complement = pd.concat([existing_data, new_data], ignore_index=True)
-        # Remove all duplicates:
-        complement.drop_duplicates(subset=['time'],inplace=True, keep=False)
-        complement.to_csv(savepath, index=False)
+    if (data.empty):
+        print('After removal of NAN values, no data left to calculate evaporation.')
+        return None
     else:
-        data[['time', 'penman_E']].rename({'penman_E': 'OUT_EVAP'}, axis=1).to_csv(savepath, index=False)
+        data['penman_E'] = data.apply(lambda row: penman(row['OUT_R_NET'], row['OUT_AIR_TEMP'], row['OUT_WIND'], row['OUT_VP'], row['P'], row['area']), axis=1)
+        data = data.reset_index()
+
+        # Save (Writing new file if not exist otherwise append)
+        if os.path.isfile(savepath):
+            existing_data = pd.read_csv(savepath, parse_dates=['time'])
+            new_data = data[['time', 'penman_E']].rename({'penman_E': 'OUT_EVAP'}, axis=1)
+            # Concat the two dataframes into a new dataframe holding all the data (memory intensive):
+            complement = pd.concat([existing_data, new_data], ignore_index=True)
+            # Remove all duplicates:
+            complement.drop_duplicates(subset=['time'],inplace=True, keep='first')
+            complement.to_csv(savepath, index=False)
+        else:
+            data[['time', 'penman_E']].rename({'penman_E': 'OUT_EVAP'}, axis=1).to_csv(savepath, index=False)
 
 
 def calc_outflow(inflowpath, dspath, epath, area, savepath):
-    inflow = pd.read_csv(inflowpath, parse_dates=["date"])
-    E = pd.read_csv(epath, parse_dates=['time'])
+    if os.path.isfile(inflowpath):
+        inflow = pd.read_csv(inflowpath, parse_dates=["date"])
+    else:
+        print('Inflow file does not exist and Outflow cannot be calculated.')
+    if os.path.isfile(epath):
+        E = pd.read_csv(epath, parse_dates=['time'])
+    else:
+        print('Evaporation file does not exist and Outflow cannot be calculated.')
 
     if isinstance(dspath, str):
-        df = pd.read_csv(dspath, parse_dates=['date'])
+        if os.path.isfile(dspath):
+            df = pd.read_csv(dspath, parse_dates=['date'])
+        else:
+            print('Storage Change file does not exist and Outflow cannot be calculated.')
     else:
         df = dspath
     
     inflow = inflow[inflow['date']>=df['date'].iloc[0]]
     inflow = inflow[inflow['date']<=df['date'].iloc[-1]]
     inflow = inflow.set_index('date')
 
@@ -155,20 +165,24 @@
     df['outflow_vol'] = df['inflow_vol'] - (df['dS']*1e9)# - df['evap_vol']
     df['days_passed'] = (df['date'] - df['last_date']).dt.days
     df['outflow_rate'] = df['outflow_vol']/(df['days_passed']*24*60*60)   # cumecs
 
     df.to_csv(savepath, index=False)
 
 
-def run_postprocessing(basin_name, basin_data_dir, reservoir_shpfile, reservoir_shpfile_column_dict, aec_dir_path, start_date, end_date,
+def run_postprocessing(basin_name, basin_data_dir, reservoir_shpfile, reservoir_shpfile_column_dict, aec_dir_path, start_date, end_date, rout_init_state_save_file, use_rout_state,
                             evap_datadir, dels_savedir, outflow_savedir, vic_status, routing_status, gee_status):
     # read file defining mapped resrvoirs
     # reservoirs_fn = os.path.join(project_dir, 'backend/data/ancillary/RAT-Reservoirs.geojson')
     reservoirs = gpd.read_file(reservoir_shpfile)
     start_date_str = start_date.strftime("%Y-%m-%d")
+    if(use_rout_state):
+        start_date_str_evap = (start_date-datetime.timedelta(days=100)).strftime("%Y-%m-%d")
+    else:
+        start_date_str_evap = start_date_str
     end_date_str = end_date.strftime("%Y-%m-%d")
     # Defining flags
     EVAP_STATUS = 0
     DELS_STATUS = 0
     OUTFLOW_STATUS = 0
 
     # SArea
@@ -176,72 +190,84 @@
 
     # DelS
     if(gee_status):
         log.debug("Calculating ∆S")
         aec_dir = aec_dir_path
 
         for reservoir_no,reservoir in reservoirs.iterrows():
-            # Reading reservoir information
-            reservoir_name = str(reservoir[reservoir_shpfile_column_dict['unique_identifier']])
-            sarea_path = os.path.join(sarea_raw_dir, reservoir_name + ".csv")
-            savepath = os.path.join(dels_savedir, reservoir_name + ".csv")
-            aecpath = os.path.join(aec_dir, reservoir_name + ".csv")
-
-            if os.path.isfile(sarea_path):
-                log.debug(f"Calculating ∆S for {reservoir_name}, saving at: {savepath}")
-                calc_dels(aecpath, sarea_path, savepath)
-            else:
-                log.debug(f"{sarea_path} not found; skipping ∆S calculation")
+            try:
+                # Reading reservoir information
+                reservoir_name = str(reservoir[reservoir_shpfile_column_dict['unique_identifier']])
+                sarea_path = os.path.join(sarea_raw_dir, reservoir_name + ".csv")
+                savepath = os.path.join(dels_savedir, reservoir_name + ".csv")
+                aecpath = os.path.join(aec_dir, reservoir_name + ".csv")
+
+                if os.path.isfile(sarea_path):
+                    log.debug(f"Calculating ∆S for {reservoir_name}, saving at: {savepath}")
+                    calc_dels(aecpath, sarea_path, savepath)
+                else:
+                    log.debug(f"{sarea_path} not found; skipping ∆S calculation")
+            except:
+                log.exception(f"∆S for {reservoir_name} could not be calculated.")
         DELS_STATUS=1
     else:
         log.debug("Cannot Calculate ∆S because GEE Run Failed.")
         
 
     # Evaporation
     if(vic_status and gee_status):
         log.debug("Retrieving Evaporation")
-        vic_results_path = os.path.join(basin_data_dir,'vic', "vic_outputs/nc_fluxes."+start_date_str+".nc")
+        if(use_rout_state):
+            vic_results_path = rout_init_state_save_file
+        else:
+            vic_results_path = os.path.join(basin_data_dir,'vic', "vic_outputs/nc_fluxes."+start_date_str+".nc")
         forcings_path = os.path.join(basin_data_dir,'vic', "vic_inputs/*.nc")
 
         for reservoir_no,reservoir in reservoirs.iterrows():
-            # Reading reservoir information
-            reservoir_name = str(reservoir[reservoir_shpfile_column_dict['unique_identifier']])
-            sarea_path = os.path.join(sarea_raw_dir, reservoir_name + ".csv")
-            e_path = os.path.join(evap_datadir, reservoir_name + ".csv")
-            
-            if os.path.isfile(sarea_path):
-                log.debug(f"Calculating Evaporation for {reservoir_name}")
-                # calc_E(e_path, respath, vic_results_path)
-                calc_E(reservoir, start_date_str, end_date_str, forcings_path, vic_results_path, sarea_path, e_path)
-            else:
-                log.debug(f"{sarea_path} not found; skipping evaporation calculation")
+            try:
+                # Reading reservoir information
+                reservoir_name = str(reservoir[reservoir_shpfile_column_dict['unique_identifier']])
+                sarea_path = os.path.join(sarea_raw_dir, reservoir_name + ".csv")
+                e_path = os.path.join(evap_datadir, reservoir_name + ".csv")
+                
+                if os.path.isfile(sarea_path):
+                    log.debug(f"Calculating Evaporation for {reservoir_name}")
+                    # calc_E(e_path, respath, vic_results_path)
+                    calc_E(reservoir, start_date_str_evap, end_date_str, forcings_path, vic_results_path, sarea_path, e_path)
+                else:
+                    log.debug(f"{sarea_path} not found; skipping evaporation calculation")
+            except:
+                log.exception(f"Evaporation for {reservoir_name} could not be calculated.")
         EVAP_STATUS = 1
     elif((not vic_status) and (not gee_status)):
         log.debug("Cannot Retrieve Evaporation because both VIC and GEE Run Failed.")
     elif(vic_status):
         log.debug("Cannot Retrieve Evaporation because VIC Run Failed.")
     else:
         log.debug("Cannot Retrieve Evaporation because GEE Run Failed.")
 
     # Outflow
     if((routing_status) and (EVAP_STATUS) and (DELS_STATUS)):
         log.debug("Calculating Outflow")
-        inflow_dir = os.path.join(basin_data_dir,'routing', "rout_inflow")
+        inflow_dir = os.path.join(basin_data_dir,'ro', "rout_inflow")
 
         for reservoir_no,reservoir in reservoirs.iterrows():
-            # Reading reservoir information
-            reservoir_name = str(reservoir[reservoir_shpfile_column_dict['unique_identifier']])
-            deltaS = os.path.join(dels_savedir, reservoir_name + ".csv")
-            inflowpath = os.path.join(inflow_dir, reservoir_name[:5] + ".csv")  ## Routing model keeps only first 5 letters of the reservoir name as file name
-            epath = os.path.join(evap_datadir, reservoir_name + ".csv")
-            a = float(reservoir[reservoir_shpfile_column_dict['area_column']])
-
-            savepath = os.path.join(outflow_savedir, reservoir_name + ".csv")
-            log.debug(f"Calculating Outflow for {reservoir_name} saving at: {savepath}")
-            calc_outflow(inflowpath, deltaS, epath, a, savepath)
+            try:
+                # Reading reservoir information
+                reservoir_name = str(reservoir[reservoir_shpfile_column_dict['unique_identifier']])
+                deltaS = os.path.join(dels_savedir, reservoir_name + ".csv")
+                inflowpath = os.path.join(inflow_dir, reservoir_name[:5] + ".csv")  ## Routing model keeps only first 5 letters of the reservoir name as file name
+                epath = os.path.join(evap_datadir, reservoir_name + ".csv")
+                a = float(reservoir[reservoir_shpfile_column_dict['area_column']])
+
+                savepath = os.path.join(outflow_savedir, reservoir_name + ".csv")
+                log.debug(f"Calculating Outflow for {reservoir_name} saving at: {savepath}")
+                calc_outflow(inflowpath, deltaS, epath, a, savepath)
+            except:
+                log.exception(f"Outflow for {reservoir_name} could not be calculated")
         OUTFLOW_STATUS = 1
     else:
         log.debug("Cannot Calculate Outflow because either evaporation, ∆S or Inflow is missing.")
     
     return (DELS_STATUS, EVAP_STATUS, OUTFLOW_STATUS)
 def main():
     pass
```

### Comparing `rat-2.1/src/rat/core/run_routing.py` & `rat-3.0.0a4/src/rat/core/run_routing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-import logging
+from http.server import executable
 import pandas as pd
 import rasterio as rio
 import os
 import datetime
-import subprocess
 
 from logging import getLogger
-from utils.logging import LOG_NAME, NOTIFICATION
-from utils.run_command import run_command
+from rat.utils.logging import LOG_NAME, NOTIFICATION
+from rat.utils.run_command import run_command
 
 log = getLogger(LOG_NAME)
 
 class RoutingRunner():
     # TODO Clean up UH files
     def __init__(self, project_dir, result_dir, inflow_dir, model_path, param_path, fdr_path, station_path_latlon, station_xy) -> None:
         self.project_dir = project_dir
@@ -81,15 +80,15 @@
         #   and their generated output files
         log.log(NOTIFICATION, "Running Routing model")
 
         # args = self.model_path, self.param_path]
         args = f'cd {self.project_dir} && {self.model_path} {self.param_path}'
         log.debug("Running: %s", " ".join(args))
         # ret_code = run_command(['cd',self.project_dir])
-        ret_code = run_command(args,shell=True)
+        ret_code = run_command(args,shell=True, executable="/bin/bash")
 
         # clean up
         log.debug("Cleaning up routing files")
         uh_s_fs = [os.path.join(self.project_dir, f) for f in os.listdir(self.project_dir) if f .endswith("uh_s")]
         for f in uh_s_fs:
             log.debug("Deleting %s", f)
             os.remove(f)
@@ -110,15 +109,16 @@
             ## Appending data if files exists otherwise creating new
             if os.path.isfile(outpath):
                 existing_data = pd.read_csv(outpath, parse_dates=['date'])
                 new_data = self._convert_streamflow(f)
                 # Concat the two dataframes into a new dataframe holding all the data (memory intensive):
                 complement = pd.concat([existing_data, new_data], ignore_index=True)
                 # Remove all duplicates:
-                complement.drop_duplicates(subset=['date'],inplace=True, keep=False)
+                complement.drop_duplicates(subset=['date'],inplace=True, keep='first')
+                complement.sort_values(by='date', inplace=True)
                 complement.to_csv(outpath, index=False)
             else:
                 self._convert_streamflow(f).to_csv(outpath, index=False)
 
 
     def _convert_streamflow(self, df_path) -> pd.DataFrame:
```

### Comparing `rat-2.1/src/rat/core/run_sarea.py` & `rat-3.0.0a4/src/rat/core/run_sarea.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import os
-import datetime
-import subprocess
 import geopandas as gpd
 
 from logging import getLogger
-from utils.logging import LOG_NAME, NOTIFICATION
+from rat.utils.logging import LOG_NAME, NOTIFICATION
 
-from core.sarea.sarea_cli_s2 import sarea_s2
-from core.sarea.sarea_cli_l8 import sarea_l8
-from core.sarea.sarea_cli_sar import sarea_s1
-from core.sarea.TMS import TMS
+from rat.core.sarea.sarea_cli_s2 import sarea_s2
+from rat.core.sarea.sarea_cli_l8 import sarea_l8
+from rat.core.sarea.sarea_cli_l9 import sarea_l9
+from rat.core.sarea.sarea_cli_sar import sarea_s1
+from rat.core.sarea.TMS import TMS
 
 log = getLogger(f"{LOG_NAME}.{__name__}")
 
 
 def run_sarea(start_date, end_date, datadir, reservoirs_shpfile, shpfile_column_dict):
     reservoirs_polygon = gpd.read_file(reservoirs_shpfile)
     
@@ -33,25 +32,24 @@
     sarea_s2(reservoir_name, reservoir_polygon, start_date, end_date, os.path.join(datadir, 's2'))
     s2_dfpath = os.path.join(datadir, 's2', reservoir_name+'.csv')
 
     # Landsat-8
     log.debug(f"Reservoir: {reservoir_name}; Downloading Landsat-8 data from {start_date} to {end_date}")
     sarea_l8(reservoir_name, reservoir_polygon, start_date, end_date, os.path.join(datadir, 'l8'))
     l8_dfpath = os.path.join(datadir, 'l8', reservoir_name+'.csv')
+    
+    # Landsat-9
+    log.debug(f"Reservoir: {reservoir_name}; Downloading Landsat-9 data from {start_date} to {end_date}")
+    sarea_l9(reservoir_name, reservoir_polygon, start_date, end_date, os.path.join(datadir, 'l9'))
+    l9_dfpath = os.path.join(datadir, 'l9', reservoir_name+'.csv')
 
     # Sentinel-1
     log.debug(f"Reservoir: {reservoir_name}; Downloading Sentinel-1 data from {start_date} to {end_date}")
     s1_dfpath = sarea_s1(reservoir_name, reservoir_polygon, start_date, end_date, os.path.join(datadir, 'sar'))
+    s1_dfpath = os.path.join(datadir, 'sar', reservoir_name+'_12d_sar.csv')
 
     tmsos = TMS(reservoir_name, reservoir_area)
-    result = tmsos.tms_os(l8_dfpath, s2_dfpath, s1_dfpath)
+    result = tmsos.tms_os(l9_dfpath=l9_dfpath, l8_dfpath=l8_dfpath, s2_dfpath=s2_dfpath, s1_dfpath=s1_dfpath)
 
     tmsos_savepath = os.path.join(datadir, reservoir_name+'.csv')
     log.debug(f"Saving surface area of {reservoir_name} at {tmsos_savepath}")
     result.reset_index().rename({'index': 'date', 'filled_area': 'area'}, axis=1).to_csv(tmsos_savepath, index=False)
-
-def main():
-    run_sarea("2021-01-01", "2022-05-02", datadir='backend/data/sarea_tmsos')
-
-
-if __name__ == '__main__':
-    main()
```

### Comparing `rat-2.1/src/rat/core/sarea/TMS.py` & `rat-3.0.0a4/src/rat/core/sarea/TMS.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,129 +1,190 @@
 import pandas as pd
 import numpy as np
 from scipy.interpolate import interp1d
-from scipy.stats import sigmaclip
+from scipy.stats import sigmaclip, zscore
 import warnings
+import os
 warnings.filterwarnings('ignore')
 
-from utils.utils import clip_ts
+from rat.utils.utils import clip_ts
 
 
 class TMS():
     def __init__(self, reservoir_name, area=None, AREA_DEVIATION_THRESHOLD_PCNT=5):
         """_summary_
-
         Args:
             reservoir_name (_type_): _description_
             area (_type_, optional): _description_
-            AREA_DEVIATION_THRESHOLD_PCNT (float, optional): _description_. Defaults to 5.
-
+            AREA_DEVIATION_THRESHOLD_PCNT (float, optional): _description_. Defaults to 25% for area<10 sq. km,  10% for area<100 sq. km, and 5% otherwise.
         Raises:
             Exception: _description_
-
         Returns:
             _type_: _description_
         """
         self.reservoir_name = reservoir_name
         self.area = area
+        if self.area < 100:
+            AREA_DEVIATION_THRESHOLD_PCNT=10
+        elif self.area < 10:
+            AREA_DEVIATION_THRESHOLD_PCNT=25
 
         self.AREA_DEVIATION_THRESHOLD = self.area * AREA_DEVIATION_THRESHOLD_PCNT/100
 
     def tms_os(self,
-            l8_dfpath: str, 
-            s2_dfpath: str, 
-            s1_dfpath: str, 
+            l8_dfpath: str = "", 
+            s2_dfpath: str = "", 
+            l9_dfpath: str = "", 
+            s1_dfpath: str = "", 
             CLOUD_THRESHOLD: float = 90.0,
             MIN_DATE: str = '2019-01-01'
         ):
+        ## TODO: add conditional, S1 required, any one of optical datasets required
         """Implements the TMS-OS methodology
-
         Args:
             l8_dfpath (string): Path of the surface area dataframe obtained using `sarea_cli_l8.py` - Landsat derived surface areas
             s2_dfpath (string): Path of the surface area dataframe obtained using `sarea_cli_s2.py` - Sentinel-2 derived surface areas
             s1_dfpath (string): Path of the surface area dataframe obtained using `sarea_cli_sar.py` - Sentinel-1  derived surface areas
             CLOUD_THRESHOLD (float): Threshold to use for cloud-masking in % (default: 90.0)
             MIN_DATE (str): Minimum date for which data to keep for all the datasets in YYYY-MM-DD or %Y-%m-%d format (default: 2019-01-01)
         """
         MIN_DATE = pd.to_datetime(MIN_DATE, format='%Y-%m-%d')
         S2_TEMPORAL_RESOLUTION = 5
         S1_TEMPORAL_RESOLUTION = 12
         L8_TEMPORAL_RESOLUTION = 16
+        L9_TEMPORAL_RESOLUTION = 16
 
-        # Read in Landsat-8
-        l8df = pd.read_csv(l8_dfpath, parse_dates=['mosaic_enddate']).rename({
-            'mosaic_enddate': 'date',
-            'water_area_cordeiro': 'water_area_uncorrected',
-            'non_water_area_cordeiro': 'non_water_area', 
-            'corrected_area_cordeiro': 'water_area_corrected'
-            }, axis=1).set_index('date')
-        l8df = l8df[['water_area_uncorrected', 'non_water_area', 'cloud_area', 'water_area_corrected']]
-        l8df['cloud_percent'] = l8df['cloud_area']*100/(l8df['water_area_uncorrected']+l8df['non_water_area']+l8df['cloud_area'])
-        l8df.replace(-1, np.nan, inplace=True)
-
-        # QUALITY_DESCRIPTION
-        #   0: Good, not interpolated either due to missing data or high clouds
-        #   1: Poor, interpolated either due to high clouds
-        #   2: Poor, interpolated either due to missing data
-        l8df.loc[:, "QUALITY_DESCRIPTION"] = 0
-        l8df.loc[l8df['cloud_percent']>=CLOUD_THRESHOLD, ("water_area_uncorrected", "non_water_area", "water_area_corrected")] = np.nan
-        l8df.loc[l8df['cloud_percent']>=CLOUD_THRESHOLD, "QUALITY_DESCRIPTION"] = 1
+        TO_MERGE = []
 
-        # in some cases l8df may have duplicated rows (with same values) that have to be removed
-        if l8df.index.duplicated().sum() > 0:
-            print("Duplicated labels, deleting")
-            l8df = l8df[~l8df.index.duplicated(keep='last')]
+        if os.path.isfile(l8_dfpath):
+            # Read in Landsat-8
+            l8df = pd.read_csv(l8_dfpath, parse_dates=['mosaic_enddate']).rename({
+                'mosaic_enddate': 'date',
+                'water_area_cordeiro': 'water_area_uncorrected',
+                'non_water_area_cordeiro': 'non_water_area', 
+                'corrected_area_cordeiro': 'water_area_corrected'
+                }, axis=1).set_index('date')
+            l8df = l8df[['water_area_uncorrected', 'non_water_area', 'cloud_area', 'water_area_corrected']]
+            l8df['cloud_percent'] = l8df['cloud_area']*100/(l8df['water_area_uncorrected']+l8df['non_water_area']+l8df['cloud_area'])
+            l8df.replace(-1, np.nan, inplace=True)
+
+            # QUALITY_DESCRIPTION
+            #   0: Good, not interpolated either due to missing data or high clouds
+            #   1: Poor, interpolated either due to high clouds
+            #   2: Poor, interpolated either due to missing data
+            l8df.loc[:, "QUALITY_DESCRIPTION"] = 0
+            l8df.loc[l8df['cloud_percent']>=CLOUD_THRESHOLD, ("water_area_uncorrected", "non_water_area", "water_area_corrected")] = np.nan
+            l8df.loc[l8df['cloud_percent']>=CLOUD_THRESHOLD, "QUALITY_DESCRIPTION"] = 1
+
+            # in some cases l8df may have duplicated rows (with same values) that have to be removed
+            if l8df.index.duplicated().sum() > 0:
+                print("Duplicated labels, deleting")
+                l8df = l8df[~l8df.index.duplicated(keep='last')]
+
+            # Fill in the gaps in l8df created due to high cloud cover with np.nan values
+            l8df_interpolated = l8df.reindex(pd.date_range(l8df.index[0], l8df.index[-1], freq=f'{L8_TEMPORAL_RESOLUTION}D'))
+            l8df_interpolated.loc[np.isnan(l8df_interpolated["QUALITY_DESCRIPTION"]), "QUALITY_DESCRIPTION"] = 2
+            l8df_interpolated.loc[np.isnan(l8df_interpolated['cloud_area']), 'cloud_area'] = max(l8df['cloud_area'])
+            l8df_interpolated.loc[np.isnan(l8df_interpolated['cloud_percent']), 'cloud_percent'] = 100
+            l8df_interpolated.loc[np.isnan(l8df_interpolated['non_water_area']), 'non_water_area'] = 0
+            l8df_interpolated.loc[np.isnan(l8df_interpolated['water_area_uncorrected']), 'water_area_uncorrected'] = 0
+
+            # Interpolate bad data
+            l8df_interpolated.loc[:, "water_area_corrected"] = l8df_interpolated.loc[:, "water_area_corrected"].interpolate(method="linear", limit_direction="forward")
+            l8df_interpolated['sat'] = 'l8'
+
+            TO_MERGE.append(l8df_interpolated)
+
+
+        # Read in Landsat-9
+        if os.path.isfile(l9_dfpath):
+            l9df = pd.read_csv(l9_dfpath, parse_dates=['mosaic_enddate']).rename({
+                'mosaic_enddate': 'date',
+                'water_area_cordeiro': 'water_area_uncorrected',
+                'non_water_area_cordeiro': 'non_water_area', 
+                'corrected_area_cordeiro': 'water_area_corrected'
+                }, axis=1).set_index('date')
+            l9df = l9df[['water_area_uncorrected', 'non_water_area', 'cloud_area', 'water_area_corrected']]
+            l9df['cloud_percent'] = l9df['cloud_area']*100/(l9df['water_area_uncorrected']+l9df['non_water_area']+l9df['cloud_area'])
+            l9df.replace(-1, np.nan, inplace=True)
+
+            # QUALITY_DESCRIPTION
+            #   0: Good, not interpolated either due to missing data or high clouds
+            #   1: Poor, interpolated either due to high clouds
+            #   2: Poor, interpolated either due to missing data
+            l9df.loc[:, "QUALITY_DESCRIPTION"] = 0
+            l9df.loc[l9df['cloud_percent']>=CLOUD_THRESHOLD, ("water_area_uncorrected", "non_water_area", "water_area_corrected")] = np.nan
+            l9df.loc[l9df['cloud_percent']>=CLOUD_THRESHOLD, "QUALITY_DESCRIPTION"] = 1
+
+            # in some cases l9df may have duplicated rows (with same values) that have to be removed
+            if l9df.index.duplicated().sum() > 0:
+                print("Duplicated labels, deleting")
+                l9df = l9df[~l9df.index.duplicated(keep='last')]
+
+            # Fill in the gaps in l9df created due to high cloud cover with np.nan values
+            l9df_interpolated = l9df.reindex(pd.date_range(l9df.index[0], l9df.index[-1], freq=f'{L9_TEMPORAL_RESOLUTION}D'))
+            l9df_interpolated.loc[np.isnan(l9df_interpolated["QUALITY_DESCRIPTION"]), "QUALITY_DESCRIPTION"] = 2
+            l9df_interpolated.loc[np.isnan(l9df_interpolated['cloud_area']), 'cloud_area'] = max(l9df['cloud_area'])
+            l9df_interpolated.loc[np.isnan(l9df_interpolated['cloud_percent']), 'cloud_percent'] = 100
+            l9df_interpolated.loc[np.isnan(l9df_interpolated['non_water_area']), 'non_water_area'] = 0
+            l9df_interpolated.loc[np.isnan(l9df_interpolated['water_area_uncorrected']), 'water_area_uncorrected'] = 0
+
+            # Interpolate bad data
+            l9df_interpolated.loc[:, "water_area_corrected"] = l8df_interpolated.loc[:, "water_area_corrected"].interpolate(method="linear", limit_direction="forward")
+            l9df_interpolated['sat'] = 'l9'
+            
+            TO_MERGE.append(l9df_interpolated)
+
+        if os.path.isfile(s2_dfpath):
+            # Read in Sentinel-2 data
+            s2df = pd.read_csv(s2_dfpath, parse_dates=['date']).set_index('date')
+            s2df = s2df[['water_area_uncorrected', 'non_water_area', 'cloud_area', 'water_area_corrected']]
+            s2df['cloud_percent'] = s2df['cloud_area']*100/(s2df['water_area_uncorrected']+s2df['non_water_area']+s2df['cloud_area'])
+            s2df.replace(-1, np.nan, inplace=True)
+            s2df.loc[s2df['cloud_percent']>=CLOUD_THRESHOLD, ("water_area_uncorrected", "non_water_area", "water_area_corrected")] = np.nan
+
+            # QUALITY_DESCRIPTION
+            #   0: Good, not interpolated either due to missing data or high clouds
+            #   1: Poor, interpolated either due to high clouds
+            #   2: Poor, interpolated either due to missing data
+            s2df.loc[:, "QUALITY_DESCRIPTION"] = 0
+            s2df.loc[s2df['cloud_percent']>=CLOUD_THRESHOLD, "QUALITY_DESCRIPTION"] = 1
+
+            # in some cases s2df may have duplicated rows (with same values) that have to be removed
+            if s2df.index.duplicated().sum() > 0:
+                print("Duplicated labels, deleting")
+                s2df = s2df[~s2df.index.duplicated(keep='last')]
+
+            # Fill in the gaps in s2df created due to high cloud cover with np.nan values
+            s2df_interpolated = s2df.reindex(pd.date_range(s2df.index[0], s2df.index[-1], freq=f'{S2_TEMPORAL_RESOLUTION}D'))
+            s2df_interpolated.loc[np.isnan(s2df_interpolated["QUALITY_DESCRIPTION"]), "QUALITY_DESCRIPTION"] = 2
+            s2df_interpolated.loc[np.isnan(s2df_interpolated['cloud_area']), 'cloud_area'] = max(s2df['cloud_area'])
+            s2df_interpolated.loc[np.isnan(s2df_interpolated['cloud_percent']), 'cloud_percent'] = 100
+            s2df_interpolated.loc[np.isnan(s2df_interpolated['non_water_area']), 'non_water_area'] = 0
+            s2df_interpolated.loc[np.isnan(s2df_interpolated['water_area_uncorrected']), 'water_area_uncorrected'] = 0
+
+            # Interpolate bad data
+            s2df_interpolated.loc[:, "water_area_corrected"] = s2df_interpolated.loc[:, "water_area_corrected"].interpolate(method="linear", limit_direction="forward")
+            s2df_interpolated['sat'] = 's2'
 
-        # Fill in the gaps in l8df created due to high cloud cover with np.nan values
-        l8df_interpolated = l8df.reindex(pd.date_range(l8df.index[0], l8df.index[-1], freq=f'{L8_TEMPORAL_RESOLUTION}D'))
-        l8df_interpolated.loc[np.isnan(l8df_interpolated["QUALITY_DESCRIPTION"]), "QUALITY_DESCRIPTION"] = 2
-        l8df_interpolated.loc[np.isnan(l8df_interpolated['cloud_area']), 'cloud_area'] = max(l8df['cloud_area'])
-        l8df_interpolated.loc[np.isnan(l8df_interpolated['cloud_percent']), 'cloud_percent'] = 100
-        l8df_interpolated.loc[np.isnan(l8df_interpolated['non_water_area']), 'non_water_area'] = 0
-        l8df_interpolated.loc[np.isnan(l8df_interpolated['water_area_uncorrected']), 'water_area_uncorrected'] = 0
-
-        # Interpolate bad data
-        l8df_interpolated.loc[:, "water_area_corrected"] = l8df_interpolated.loc[:, "water_area_corrected"].interpolate(method="linear", limit_direction="forward")
-
-
-        # Read in Sentinel-2 data
-        s2df = pd.read_csv(s2_dfpath, parse_dates=['date']).set_index('date')
-        s2df = s2df[['water_area_uncorrected', 'non_water_area', 'cloud_area', 'water_area_corrected']]
-        s2df['cloud_percent'] = s2df['cloud_area']*100/(s2df['water_area_uncorrected']+s2df['non_water_area']+s2df['cloud_area'])
-        s2df.replace(-1, np.nan, inplace=True)
-        s2df.loc[s2df['cloud_percent']>=CLOUD_THRESHOLD, ("water_area_uncorrected", "non_water_area", "water_area_corrected")] = np.nan
-
-        # QUALITY_DESCRIPTION
-        #   0: Good, not interpolated either due to missing data or high clouds
-        #   1: Poor, interpolated either due to high clouds
-        #   2: Poor, interpolated either due to missing data
-        s2df.loc[:, "QUALITY_DESCRIPTION"] = 0
-        s2df.loc[s2df['cloud_percent']>=CLOUD_THRESHOLD, "QUALITY_DESCRIPTION"] = 1
-
-        # in some cases s2df may have duplicated rows (with same values) that have to be removed
-        if s2df.index.duplicated().sum() > 0:
-            print("Duplicated labels, deleting")
-            s2df = s2df[~s2df.index.duplicated(keep='last')]
-
-        # Fill in the gaps in s2df created due to high cloud cover with np.nan values
-        s2df_interpolated = s2df.reindex(pd.date_range(s2df.index[0], s2df.index[-1], freq=f'{S2_TEMPORAL_RESOLUTION}D'))
-        s2df_interpolated.loc[np.isnan(s2df_interpolated["QUALITY_DESCRIPTION"]), "QUALITY_DESCRIPTION"] = 2
-        s2df_interpolated.loc[np.isnan(s2df_interpolated['cloud_area']), 'cloud_area'] = max(s2df['cloud_area'])
-        s2df_interpolated.loc[np.isnan(s2df_interpolated['cloud_percent']), 'cloud_percent'] = 100
-        s2df_interpolated.loc[np.isnan(s2df_interpolated['non_water_area']), 'non_water_area'] = 0
-        s2df_interpolated.loc[np.isnan(s2df_interpolated['water_area_uncorrected']), 'water_area_uncorrected'] = 0
-
-        # Interpolate bad data
-        s2df_interpolated.loc[:, "water_area_corrected"] = s2df_interpolated.loc[:, "water_area_corrected"].interpolate(method="linear", limit_direction="forward")
+            TO_MERGE.append(s2df_interpolated)
 
         # Read in Sentinel-1 data
         sar = pd.read_csv(s1_dfpath, parse_dates=['time']).rename({'time': 'date'}, axis=1)
         sar['date'] = sar['date'].apply(lambda d: np.datetime64(d.strftime('%Y-%m-%d')))
         sar.set_index('date', inplace=True)
         sar.sort_index(inplace=True)
+
+        # apply weekly area change filter
+        sar = sar_data_statistical_fix(sar, self.area, 15)
+
+        std = zscore(sar['sarea'])
+        SAR_ZSCORE_LIM = 3
+        sar.loc[(std > SAR_ZSCORE_LIM) | (std < -SAR_ZSCORE_LIM), 'sarea'] = np.nan
+        sar['sarea'] = sar['sarea'].interpolate()
         sar = sar.loc[MIN_DATE:, :]
 
         # in some cases s2df may have duplicated rows (with same values) that have to be removed
         if sar.index.duplicated().sum() > 0:
             print("Duplicated labels, deleting")
             sar = sar[~sar.index.duplicated(keep='last')]
 
@@ -135,30 +196,62 @@
         in_unix_time = lambda x: (x - pd.Timestamp("1970-01-01"))//pd.Timedelta('1s')
 
         extrapolated_value = interp1d(in_unix_time(sar.index[-7:]), sar['sarea'][-7:], kind='linear', fill_value="extrapolate")(in_unix_time(extrapolated_date))
 
         sar.loc[extrapolated_date, "sarea"] = extrapolated_value
 
         # combine opticals into one dataframes
-        l8df_interpolated['sat'] = 'l8'
-        s2df_interpolated['sat'] = 's2'
-        optical = pd.concat([l8df_interpolated, s2df_interpolated]).sort_index()
+        
+        optical = pd.concat(TO_MERGE).sort_index()
         optical = optical.loc[~optical.index.duplicated(keep='last')] # when both s2 and l8 are present, keep s2
         optical.rename({'water_area_corrected': 'area'}, axis=1, inplace=True)
         sar = sar.rename({'sarea': 'area'}, axis=1)
 
         # Apply the trend based corrections
         result = trend_based_correction(optical.copy(), sar.copy(), self.AREA_DEVIATION_THRESHOLD)
 
         return result
 
+def area_change(df, date, n=14):
+    """calculate the change in area in last n days"""
+    start = date - pd.Timedelta(days=n)
+    end = date
+
+    # if start date is before the first date in the df, return nan
+    if start < df.index[0]:
+        return np.nan
+
+    start_area = df.loc[start:end, "sarea"].iloc[0]
+    end_area = df.loc[date, "sarea"]
+    try:  # if end_area is a series which may happen in a SAR area dataframe (TODO: fix the cause of this issue, same area is returned twice), take the first value
+        end_area = end_area.iloc[0]
+    except AttributeError as AE:
+        pass
+    except Exception as E:
+        raise E
+
+    return end_area - start_area
+    
+
+def sar_data_statistical_fix(sar_df, nominal_area, threshold_percentage=15):
+    """fix the sar data using statistical method"""
+    threshold = (threshold_percentage / 100) * nominal_area
+
+    sar_df_copy = sar_df.copy()
+    sar_df_copy['date'] = sar_df_copy.index.to_series()
+
+    sar_df_copy['area_change'] = sar_df_copy['date'].apply(lambda x: area_change(sar_df_copy, x))
+
+    sar_df_copy.loc[(sar_df_copy['area_change'] < -threshold)|(sar_df_copy['area_change'] > threshold), 'sarea'] = np.nan
+    sar_df_copy['sarea'] = sar_df_copy['sarea'].interpolate(method='time')
+
+    return sar_df_copy.drop('area_change', axis=1).drop('date', axis=1)
 
 def deviation_from_sar(optical_areas, sar_areas, DEVIATION_THRESHOLD = 20, LOW_STD_LIM=2, HIGH_STD_LIM=2):
     """Filter out points based on deviations from SAR reported areas after correcting for bias in SAR water areas. Remove NaNs beforehand.
-
     Args:
         optical_areas (pd.Series): Time-series of areas obtained using an optical sensor (S2, L8, etc) on which the filtering will be applied. Must have `pd.DatetimeIndex` and corresponding areas in a column named `area`.
         sar_areas (pd.Series): Time-series of S1 surface areas. Must have `pd.DatetimeIndex` and corresponding areas in a column named `area`.
         DEVIATION_THRESHOLD (number): (Default: 20 [sq. km.]) Theshold of deviation from bias corrected SAR reported 
         LOW_STD_LIM (number): (Default: 2) Lower limit of standard deviations to use for clipping the deviations, required for calculating the bias.
         HIGH_STD_LIM (number): (Default: 2) Upper limit of standard deviations to use for clipping the deviations, required for calculating the bias.
     """
@@ -218,17 +311,18 @@
 
     inner_area.loc[:, 'deviation'] = np.abs(inner_area['trend']-inner_area['sar_trend'])
 
     inner_area.loc[:, 'erroneous'] = inner_area['deviation'] > DEVIATION_THRESHOLD
 
     inner_area.loc[:, 'corrected_trend'] = inner_area['trend']
     inner_area.loc[inner_area['erroneous'], 'corrected_trend'] = inner_area['sar_trend']
-
-    areas = backcalculate(inner_area[AREA_COL_NAME], inner_area['corrected_trend'], inner_area['erroneous'])
-    inner_area[AREA_COL_NAME] = areas
+    print(inner_area)
+    if(not inner_area['erroneous'].empty):
+        areas = backcalculate(inner_area[AREA_COL_NAME], inner_area['corrected_trend'], inner_area['erroneous'])
+        inner_area[AREA_COL_NAME] = areas
 
     return inner_area
 
 def sign_based_correction(area, AREA_COL_NAME='corrected_areas_1', TREND_COL_NAME='corrected_trend_1'):
     inner_area = area.copy()
     inner_area['sign_based_correction_reqd'] = (inner_area['trend']<0)&(inner_area['sar_trend']>0)|(inner_area['trend']>0)&(inner_area['sar_trend']<0)
     inner_area.loc[:, 'corrected_trend'] = inner_area[TREND_COL_NAME]
@@ -236,20 +330,18 @@
 
     inner_area['area'] = backcalculate(inner_area[AREA_COL_NAME], inner_area['corrected_trend'], inner_area['sign_based_correction_reqd'])
 
     return inner_area
 
 def filled_by_trend(filtered_area, sar_trend, days_passed) -> pd.Series:
     """Fills in `np.nan` values of optically obtained surface area time series using SAR based time-series.
-
     Args:
         filtered_area (pd.Series): Optical sensor based surface areas containing `np.nan` values that will be filled in.
         sar_trend (pd.Series): SAR based surface area trends.
         days_passed (pd.Series): Days sicne last observation of optical sensor observed surface areas.
-
     Returns:
         pd.Series: Filled nan values
     """
     filled = [filtered_area.iloc[0]]
     for i in range(1, len(filtered_area)):
         if np.isnan(filtered_area.iloc[i]):
             a = filled[-1] + sar_trend.iloc[i] * days_passed.iloc[i]
@@ -258,15 +350,14 @@
             filled.append(filtered_area.iloc[i])
     
     return pd.Series(filled, dtype=float, name='filled_area', index=filtered_area.index)
 
 # Trend based correction function
 def trend_based_correction(area, sar, AREA_DEVIATION_THRESHOLD=25, TREND_DEVIATION_THRESHOLD = 10):
     """Apply trend based correction on a time-series
-
     Args:
         area (pd.DataFrame): Pandas dataframe containing date as pd.DatetimeIndex and areas in column named `area`
         sar (pd.DataFrame): Pandas dataframe containing surface area time-series obtained from Sentinel-1 (SAR). Same format as `area`
         AREA_DEVIATION_THRESHOLD (number): (Default: 25) Threshold value of deviation of optically derived areas from SAR derived areas fro filtering.
         TREND_DEVIATION_THRESHOLD (number): (Default: 10) Threshold value of deviation in trend above which the observation is marked as erroneous and the correction step is applied
     """
 
@@ -274,15 +365,15 @@
     area.rename({'area': 'unfiltered_area'}, axis=1, inplace=True)
     # area.rename({'filtered_area': 'area'}, axis=1, inplace=True)
     
     area_filtered = area.dropna(subset=['filtered_area'])
 
     area_filtered.loc[:, 'days_passed'] = area_filtered.index.to_series().diff().dt.days
     area_filtered.loc[:, 'trend'] = area_filtered['filtered_area'].diff()/area_filtered['days_passed']
-
+    
     sar, area_filtered = clip_ts(sar, area_filtered, which='left')
     # sometimes the sar time-series has duplicate values which have to be removed
     sar = sar[~sar.index.duplicated(keep='first')]   # https://stackoverflow.com/a/34297689/4091712
     trend_generator = lambda arg: sar_trend(arg.index[0], arg.index[-1], sar)
 
     area_filtered.loc[:, 'sar_trend'] = area_filtered['filtered_area'].rolling(2, min_periods=0).apply(trend_generator)
```

### Comparing `rat-2.1/src/rat/core/sarea/sarea_cli_l8.py` & `rat-3.0.0a4/src/rat/core/sarea/sarea_cli_l8.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,24 @@
 # import geemap as gee
 import ee
 from datetime import datetime, timedelta, timezone
 import pandas as pd
 import time
 import os
 from random import randint
-import argparse
 from itertools import zip_longest
-import pprint
-from ee_utils.ee_utils import poly2feature
+from rat.ee_utils.ee_utils import poly2feature
 
-from utils.logging import LOG_NAME, NOTIFICATION
+from rat.ee_utils.ee_utils import poly2feature
+from rat.utils.logging import LOG_NAME, NOTIFICATION
+from rat.utils.utils import days_between
 from logging import getLogger
 
 log = getLogger(f"{LOG_NAME}.{__name__}")
 
-#### initialize the connection to the server ####
-from ee_utils.ee_config import service_account,key_file
-
-ee_credentials = ee.ServiceAccountCredentials(service_account, key_file)
-ee.Initialize(ee_credentials)
-#### Connection established ####
-
 def grouper(iterable, n, *, incomplete='fill', fillvalue=None):
     "Collect data into non-overlapping fixed-length chunks or blocks"
     # grouper('ABCDEFG', 3, fillvalue='x') --> ABC DEF Gxx
     # grouper('ABCDEFG', 3, incomplete='strict') --> ABC DEF ValueError
     # grouper('ABCDEFG', 3, incomplete='ignore') --> ABC DEF
     args = [iter(iterable)] * n
     if incomplete == 'fill':
@@ -324,143 +317,153 @@
 def run_process_long(res_name, res_polygon, start, end, datadir):
     fo = start
     enddate = end
 
     # Extracting reservoir geometry 
     global aoi
     aoi = poly2feature(res_polygon,BUFFER_DIST).geometry()
+    ## Checking if time interval is small then the image collection should not be empty in GEE
+    if (days_between(start,end) < 30):     # less than a month difference
+        number_of_images = l8.filterBounds(aoi).filterDate(start, end).size().getInfo()
+    else:
+        number_of_images = 1     # more than a month difference simply run, so no need to calculate number_of_images
     
-    fo = get_first_obs(start, end).format('YYYY-MM-dd').getInfo()
-    first_obs = datetime.strptime(fo, '%Y-%m-%d')
+    if(number_of_images):
+        fo = get_first_obs(start, end).format('YYYY-MM-dd').getInfo()
+        first_obs = datetime.strptime(fo, '%Y-%m-%d')
 
-    scratchdir = os.path.join(datadir, "_scratch")
+        scratchdir = os.path.join(datadir, "_scratch")
 
-    # flag = True
-    num_runs = 0
+        # flag = True
+        num_runs = 0
 
-    # If data already exists, only get new data starting from the last one
-    savepath = os.path.join(datadir, f"{res_name}.csv")
-    
-    if os.path.isfile(savepath):
-        temp_df = pd.read_csv(savepath, parse_dates=['mosaic_enddate']).set_index('mosaic_enddate')
-
-        last_date = temp_df.index[-1].to_pydatetime()
-        fo = (last_date - timedelta(days=TEMPORAL_RESOLUTION*2)).strftime("%Y-%m-%d")
-        to_combine = [savepath]
-        print(f"Existing file found - Last observation ({TEMPORAL_RESOLUTION*2} day lag): {last_date}")
-
-        # If 16 days have not passed since last observation, skip the processing
-        days_passed = (datetime.strptime(end, "%Y-%m-%d") - last_date).days
-        print(f"No. of days passed since: {days_passed}")
-        if days_passed < TEMPORAL_RESOLUTION:
-            print(f"No new observation expected. Quitting early")
-            return None
-    else:
-        to_combine = []
-    
-    savedir = os.path.join(scratchdir, f"{res_name}_l8_cordeiro_zhao_gao_{fo}_{enddate}")
-    if not os.path.isdir(savedir):
-        os.makedirs(savedir)
-    
-    print(f"Extracting SA for the period {fo} -> {enddate}")
-
-    dates = pd.date_range(fo, enddate, freq=f'{TEMPORAL_RESOLUTION}D')
-    grouped_dates = grouper(dates, RESULTS_PER_ITER)
-
-    # # redo the calculations part and see where it is complaining about too many aggregations
-    # subset_dates = next(grouped_dates)
-    # dates = ee.List([ee.Date(d) for d in subset_dates if d is not None])
-
-    # print(subset_dates)
-    # res = generate_timeseries(dates).filterMetadata('s2_images', 'greater_than', 0)
-    # pprint.pprint(res.aggregate_array('s2_images').getInfo())
-
-    # uncorrected_columns_to_extract = ['from_date', 'to_date', 'water_area_cordeiro', 'non_water_area_cordeiro', 'water_area_NDWI', 'non_water_area_NDWI', 'cloud_area', 's2_images']
-    # uncorrected_final_data_ee = res.reduceColumns(ee.Reducer.toList(len(uncorrected_columns_to_extract)), uncorrected_columns_to_extract).get('list')
-    # uncorrected_final_data = uncorrected_final_data_ee.getInfo()
-    
-
-    for subset_dates in grouped_dates:
-        try:
-            print(subset_dates)
-            dates = ee.List([ee.Date(d) for d in subset_dates if d is not None])
-            
-            res = generate_timeseries(dates).filterMetadata('l8_images', 'greater_than', 0)
-            # pprint.pprint(res.getInfo())
-
-            uncorrected_columns_to_extract = ['from_date', 'to_date', 'water_area_cordeiro', 'non_water_area_cordeiro', 'cloud_area', 'l8_images']
-            uncorrected_final_data_ee = res.reduceColumns(ee.Reducer.toList(len(uncorrected_columns_to_extract)), uncorrected_columns_to_extract).get('list')
-            uncorrected_final_data = uncorrected_final_data_ee.getInfo()
-            print("Uncorrected", uncorrected_final_data)
-
-            res_corrected_cordeiro = res.map(lambda im: postprocess_wrapper(im, 'water_map_cordeiro', im.get('water_area_cordeiro')))
-            corrected_columns_to_extract = ['to_date', 'corrected_area']
-            corrected_final_data_cordeiro_ee = res_corrected_cordeiro \
-                                                .filterMetadata('corrected_area', 'not_equals', None) \
-                                                .reduceColumns(
-                                                    ee.Reducer.toList(
-                                                        len(corrected_columns_to_extract)), 
-                                                        corrected_columns_to_extract
-                                                        ).get('list')
-            corrected_final_data_cordeiro = corrected_final_data_cordeiro_ee.getInfo()
-            print("Corrected - Cordeiro", corrected_final_data_cordeiro)
-
-            # res_corrected_NDWI = res.map(lambda im: postprocess_wrapper(im, 'water_map_NDWI', im.get('water_area_NDWI')))
-            # corrected_final_data_NDWI_ee = res_corrected_NDWI \
-            #                                     .filterMetadata('corrected_area', 'not_equals', None) \
-            #                                     .reduceColumns(
-            #                                         ee.Reducer.toList(
-            #                                             len(corrected_columns_to_extract)), 
-            #                                             corrected_columns_to_extract
-            #                                             ).get('list')
-            
-            # corrected_final_data_NDWI = corrected_final_data_NDWI_ee.getInfo()
-            
-            # print(uncorrected_final_data, corrected_final_data_cordeiro)
-            if len(uncorrected_final_data) == 0:
+        # If data already exists, only get new data starting from the last one
+        savepath = os.path.join(datadir, f"{res_name}.csv")
+        
+        if os.path.isfile(savepath):
+            temp_df = pd.read_csv(savepath, parse_dates=['mosaic_enddate']).set_index('mosaic_enddate')
+
+            last_date = temp_df.index[-1].to_pydatetime()
+            fo = (last_date - timedelta(days=TEMPORAL_RESOLUTION*2)).strftime("%Y-%m-%d")
+            to_combine = [savepath]
+            print(f"Existing file found - Last observation ({TEMPORAL_RESOLUTION*2} day lag): {last_date}")
+
+            # If 16 days have not passed since last observation, skip the processing
+            days_passed = (datetime.strptime(end, "%Y-%m-%d") - last_date).days
+            print(f"No. of days passed since: {days_passed}")
+            if days_passed < TEMPORAL_RESOLUTION:
+                print(f"No new observation expected. Quitting early")
+                return None
+        else:
+            to_combine = []
+        
+        savedir = os.path.join(scratchdir, f"{res_name}_l8_cordeiro_zhao_gao_{fo}_{enddate}")
+        if not os.path.isdir(savedir):
+            os.makedirs(savedir)
+        
+        print(f"Extracting SA for the period {fo} -> {enddate}")
+
+        dates = pd.date_range(fo, enddate, freq=f'{TEMPORAL_RESOLUTION}D')
+        grouped_dates = grouper(dates, RESULTS_PER_ITER)
+
+        # # redo the calculations part and see where it is complaining about too many aggregations
+        # subset_dates = next(grouped_dates)
+        # dates = ee.List([ee.Date(d) for d in subset_dates if d is not None])
+
+        # print(subset_dates)
+        # res = generate_timeseries(dates).filterMetadata('s2_images', 'greater_than', 0)
+        # pprint.pprint(res.aggregate_array('s2_images').getInfo())
+
+        # uncorrected_columns_to_extract = ['from_date', 'to_date', 'water_area_cordeiro', 'non_water_area_cordeiro', 'water_area_NDWI', 'non_water_area_NDWI', 'cloud_area', 's2_images']
+        # uncorrected_final_data_ee = res.reduceColumns(ee.Reducer.toList(len(uncorrected_columns_to_extract)), uncorrected_columns_to_extract).get('list')
+        # uncorrected_final_data = uncorrected_final_data_ee.getInfo()
+        
+        for subset_dates in grouped_dates:
+            try:
+                print(subset_dates)
+                dates = ee.List([ee.Date(d) for d in subset_dates if d is not None])
+                
+                res = generate_timeseries(dates).filterMetadata('l8_images', 'greater_than', 0)
+                # pprint.pprint(res.getInfo())
+
+                uncorrected_columns_to_extract = ['from_date', 'to_date', 'water_area_cordeiro', 'non_water_area_cordeiro', 'cloud_area', 'l8_images']
+                uncorrected_final_data_ee = res.reduceColumns(ee.Reducer.toList(len(uncorrected_columns_to_extract)), uncorrected_columns_to_extract).get('list')
+                uncorrected_final_data = uncorrected_final_data_ee.getInfo()
+                print("Uncorrected", uncorrected_final_data)
+
+                res_corrected_cordeiro = res.map(lambda im: postprocess_wrapper(im, 'water_map_cordeiro', im.get('water_area_cordeiro')))
+                corrected_columns_to_extract = ['to_date', 'corrected_area']
+                corrected_final_data_cordeiro_ee = res_corrected_cordeiro \
+                                                    .filterMetadata('corrected_area', 'not_equals', None) \
+                                                    .reduceColumns(
+                                                        ee.Reducer.toList(
+                                                            len(corrected_columns_to_extract)), 
+                                                            corrected_columns_to_extract
+                                                            ).get('list')
+                corrected_final_data_cordeiro = corrected_final_data_cordeiro_ee.getInfo()
+                print("Corrected - Cordeiro", corrected_final_data_cordeiro)
+
+                # res_corrected_NDWI = res.map(lambda im: postprocess_wrapper(im, 'water_map_NDWI', im.get('water_area_NDWI')))
+                # corrected_final_data_NDWI_ee = res_corrected_NDWI \
+                #                                     .filterMetadata('corrected_area', 'not_equals', None) \
+                #                                     .reduceColumns(
+                #                                         ee.Reducer.toList(
+                #                                             len(corrected_columns_to_extract)), 
+                #                                             corrected_columns_to_extract
+                #                                             ).get('list')
+                
+                # corrected_final_data_NDWI = corrected_final_data_NDWI_ee.getInfo()
+                
+                # print(uncorrected_final_data, corrected_final_data_cordeiro)
+                if len(uncorrected_final_data) == 0:
+                    continue
+                uncorrected_df = pd.DataFrame(uncorrected_final_data, columns=uncorrected_columns_to_extract)
+                corrected_cordeiro_df = pd.DataFrame(corrected_final_data_cordeiro, columns=corrected_columns_to_extract).rename({'corrected_area': 'corrected_area_cordeiro'}, axis=1)
+                # corrected_NDWI_df = pd.DataFrame(corrected_final_data_NDWI, columns=corrected_columns_to_extract).rename({'corrected_area': 'corrected_area_NDWI'}, axis=1)
+                # corrected_df = pd.merge(corrected_cordeiro_df, corrected_NDWI_df, 'left', 'to_date')
+                df = pd.merge(uncorrected_df, corrected_cordeiro_df, 'left', 'to_date')
+
+                df['from_date'] = pd.to_datetime(df['from_date'], format="%Y-%m-%d")
+                df['to_date'] = pd.to_datetime(df['to_date'], format="%Y-%m-%d")
+                df['mosaic_enddate'] = df['to_date'] - pd.Timedelta(1, unit='day')
+                df = df.set_index('mosaic_enddate')
+                print(df.head(2))
+
+                fname = os.path.join(savedir, f"{df.index[0].strftime('%Y%m%d')}_{df.index[-1].strftime('%Y%m%d')}_{res_name}.csv")
+                df.to_csv(fname)
+
+                s_time = randint(20, 30)
+                print(f"Sleeping for {s_time} seconds")
+                time.sleep(randint(20, 30))
+
+                if (datetime.strptime(enddate, "%Y-%m-%d")-df.index[-1]).days < TEMPORAL_RESOLUTION:
+                    print(f"Quitting: Reached enddate {enddate}")
+                    break
+                elif df.index[-1].strftime('%Y-%m-%d') == fo:
+                    print(f"Reached last available observation - {fo}")
+                    break
+                elif num_runs > 1000:
+                    print("Quitting: Reached 1000 iterations")
+                    break
+            except Exception as e:
+                log.error(e)
                 continue
-            uncorrected_df = pd.DataFrame(uncorrected_final_data, columns=uncorrected_columns_to_extract)
-            corrected_cordeiro_df = pd.DataFrame(corrected_final_data_cordeiro, columns=corrected_columns_to_extract).rename({'corrected_area': 'corrected_area_cordeiro'}, axis=1)
-            # corrected_NDWI_df = pd.DataFrame(corrected_final_data_NDWI, columns=corrected_columns_to_extract).rename({'corrected_area': 'corrected_area_NDWI'}, axis=1)
-            # corrected_df = pd.merge(corrected_cordeiro_df, corrected_NDWI_df, 'left', 'to_date')
-            df = pd.merge(uncorrected_df, corrected_cordeiro_df, 'left', 'to_date')
-
-            df['from_date'] = pd.to_datetime(df['from_date'], format="%Y-%m-%d")
-            df['to_date'] = pd.to_datetime(df['to_date'], format="%Y-%m-%d")
-            df['mosaic_enddate'] = df['to_date'] - pd.Timedelta(1, unit='day')
-            df = df.set_index('mosaic_enddate')
-            print(df.head(2))
-
-            fname = os.path.join(savedir, f"{df.index[0].strftime('%Y%m%d')}_{df.index[-1].strftime('%Y%m%d')}_{res_name}.csv")
-            df.to_csv(fname)
-
-            s_time = randint(20, 30)
-            print(f"Sleeping for {s_time} seconds")
-            time.sleep(randint(20, 30))
-
-            if (datetime.strptime(enddate, "%Y-%m-%d")-df.index[-1]).days < TEMPORAL_RESOLUTION:
-                print(f"Quitting: Reached enddate {enddate}")
-                break
-            elif df.index[-1].strftime('%Y-%m-%d') == fo:
-                print(f"Reached last available observation - {fo}")
-                break
-            elif num_runs > 1000:
-                print("Quitting: Reached 1000 iterations")
-                break
-        except Exception as e:
-            log.error(e)
-            continue
-
-
-    # Combine the files into one database
-    to_combine.extend([os.path.join(savedir, f) for f in os.listdir(savedir) if f.endswith(".csv")])
+        
 
-    files = [pd.read_csv(f, parse_dates=["mosaic_enddate"]).set_index("mosaic_enddate") for f in to_combine]
-    data = pd.concat(files).drop_duplicates().sort_values("mosaic_enddate")
 
-    data.to_csv(savepath)
+        # Combine the files into one database
+        to_combine.extend([os.path.join(savedir, f) for f in os.listdir(savedir) if f.endswith(".csv")])
 
-    return savepath
+        files = [pd.read_csv(f, parse_dates=["mosaic_enddate"]).set_index("mosaic_enddate") for f in to_combine]
+        data = pd.concat(files).drop_duplicates().sort_values("mosaic_enddate")
+
+        data.to_csv(savepath)
+
+        return savepath
+    
+    else:
+        print(f"No observation observed between {start} and {end}. Quitting!")
+        return None
 
 # User-facing wrapper function
 def sarea_l8(res_name,res_polygon, start, end, datadir):
     return run_process_long(res_name,res_polygon, start, end, datadir)
```

### Comparing `rat-2.1/src/rat/core/sarea/sarea_cli_s2.py` & `rat-3.0.0a4/src/rat/core/sarea/sarea_cli_s2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,25 @@
 
-# import geemap as gee
-from asyncio.log import logger
 import ee
 from datetime import datetime, timedelta, timezone
 import pandas as pd
 import numpy as np
 import time
 import os
 from random import randint
-import argparse
 from itertools import zip_longest
-import pprint
-from ee_utils.ee_utils import poly2feature
+from rat.ee_utils.ee_utils import poly2feature
 
-from utils.logging import LOG_NAME, NOTIFICATION
+from rat.ee_utils.ee_utils import poly2feature
+from rat.utils.logging import LOG_NAME, NOTIFICATION
+from rat.utils.utils import days_between
 from logging import getLogger
 
 log = getLogger(f"{LOG_NAME}.{__name__}")
 
-#### initialize the connection to the server ####
-from ee_utils.ee_config import service_account,key_file
-
-ee_credentials = ee.ServiceAccountCredentials(service_account, key_file)
-ee.Initialize(ee_credentials)
-#### Connection established ####
-
-
 def grouper(iterable, n, *, incomplete='fill', fillvalue=None):
     "Collect data into non-overlapping fixed-length chunks or blocks"
     # grouper('ABCDEFG', 3, fillvalue='x') --> ABC DEF Gxx
     # grouper('ABCDEFG', 3, incomplete='strict') --> ABC DEF ValueError
     # grouper('ABCDEFG', 3, incomplete='ignore') --> ABC DEF
     args = [iter(iterable)] * n
     if incomplete == 'fill':
@@ -337,152 +327,161 @@
 def run_process_long(res_name,res_polygon, start, end, datadir):
     fo = start
     enddate = end
 
     # Extracting reservoir geometry 
     global aoi
     aoi = poly2feature(res_polygon,BUFFER_DIST).geometry()
-    
-    fo = get_first_obs(start, end).format('YYYY-MM-dd').getInfo()
-    first_obs = datetime.strptime(fo, '%Y-%m-%d')
-
-    scratchdir = os.path.join(datadir, "_scratch")
-
-    # flag = True
-    num_runs = 0
-
-    # If data already exists, only get new data starting from the last one
-    savepath = os.path.join(datadir, f"{res_name}.csv")
-    
-    if os.path.isfile(savepath):
-        temp_df = pd.read_csv(savepath, parse_dates=['date']).set_index('date')
-
-        last_date = temp_df.index[-1].to_pydatetime()
-        fo = (last_date - timedelta(days=TEMPORAL_RESOLUTION*2)).strftime("%Y-%m-%d")
-        to_combine = [savepath]
-        print(f"Existing file found - Last observation ({TEMPORAL_RESOLUTION*2} day lag): {last_date}")
-
-        # If 16 days have not passed since last observation, skip the processing
-        days_passed = (datetime.strptime(end, "%Y-%m-%d") - last_date).days
-        print(f"No. of days passed since: {days_passed}")
-        if days_passed < TEMPORAL_RESOLUTION:
-            print(f"No new observation expected. Quitting early")
-            return None
+     ## Checking if time interval is small then the image collection should not be empty in GEE
+    if (days_between(start,end) < 30):     # less than a month difference
+        number_of_images = s2.filterBounds(aoi).filterDate(start, end).size().getInfo()
     else:
-        to_combine = []
+        number_of_images = 1     # more than a month difference simply run, so no need to calculate number_of_images
     
-    savedir = os.path.join(scratchdir, f"{res_name}_s2_cordeiro_zhao_gao_{fo}_{enddate}")
-    if not os.path.isdir(savedir):
-        os.makedirs(savedir)
-    
-    print(f"Extracting SA for the period {fo} -> {enddate}")
-
-    dates = pd.date_range(fo, enddate, freq=f'{TEMPORAL_RESOLUTION}D')
-    grouped_dates = grouper(dates, RESULTS_PER_ITER)
-
-    # # redo the calculations part and see where it is complaining about too many aggregations
-    # subset_dates = next(grouped_dates)
-    # dates = ee.List([ee.Date(d) for d in subset_dates if d is not None])
-
-    # print(subset_dates)
-    # res = generate_timeseries(dates).filterMetadata('s2_images', 'greater_than', 0)
-    # pprint.pprint(res.aggregate_array('s2_images').getInfo())
-
-    # uncorrected_columns_to_extract = ['from_date', 'to_date', 'water_area_cordeiro', 'non_water_area_cordeiro', 'water_area_NDWI', 'non_water_area_NDWI', 'cloud_area', 's2_images']
-    # uncorrected_final_data_ee = res.reduceColumns(ee.Reducer.toList(len(uncorrected_columns_to_extract)), uncorrected_columns_to_extract).get('list')
-    # uncorrected_final_data = uncorrected_final_data_ee.getInfo()
-    
-
-
-    for subset_dates in grouped_dates:
-        try:
-            print(subset_dates)
-            dates = ee.List([ee.Date(d) for d in subset_dates if d is not None])
-            
-            ts_imcoll = generate_timeseries(dates)
-            postprocessed_ts_imcoll = ts_imcoll.map(postprocess_wrapper)
-
-            # Download the data locally
-            ts_imcoll_L = ts_imcoll.getInfo()
-            postprocessed_ts_imcoll_L = postprocessed_ts_imcoll.getInfo()
-
-            # Parse the data to create dataframe
-            PROCESSING_STATUSES = []
-            POSTPROCESSING_STATUSES = []
-            cloud_areas = []
-            cloud_percents = []
-            from_dates = []
-            to_dates = []
-            obs_dates = []
-            non_water_areas = []
-            water_areas = []
-            water_areas_zhaogao = []
-            for f, f_postprocessed in zip(ts_imcoll_L['features'], postprocessed_ts_imcoll_L['features']):
-                PROCESSING_STATUS = f['properties']['PROCESSING_SUCCESSFUL']
-                PROCESSING_STATUSES.append(PROCESSING_STATUS)
-                POSTPROCESSING_STATUS = f_postprocessed['properties']['POSTPROCESSING_SUCCESSFUL']
-                POSTPROCESSING_STATUSES.append(POSTPROCESSING_STATUS)
-                obs_dates.append(pd.to_datetime(f['properties']['system:time_start']))
-                from_dates.append(pd.to_datetime(f['properties']['from_date']))
-                to_dates.append(pd.to_datetime(f['properties']['to_date']))
-                if PROCESSING_STATUS:
-                    water_areas.append(f['properties']['water_area_clustering'])
-                    non_water_areas.append(f['properties']['non_water_area_clustering'])
-                    cloud_areas.append(f['properties']['cloud_area'])
-                    cloud_percents.append(f['properties']['cloud_percent'])
-                else:
-                    water_areas.append(np.nan)
-                    non_water_areas.append(np.nan)
-                    cloud_areas.append(np.nan)
-                    cloud_percents.append(np.nan)
-                if POSTPROCESSING_STATUS:
-                    water_areas_zhaogao.append(f_postprocessed['properties']['corrected_area'])
-                else:
-                    water_areas_zhaogao.append(np.nan)
-            
-            df = pd.DataFrame({
-                'date': obs_dates,
-                'PROCESSING_STATUS': PROCESSING_STATUSES,
-                'POSTPROCESSING_STATUS': POSTPROCESSING_STATUSES,
-                'from_date': from_dates,
-                'to_date': to_dates,
-                'cloud_area': cloud_areas,
-                'cloud_percent': cloud_percents,
-                'water_area_uncorrected': water_areas,
-                'non_water_area': non_water_areas,
-                'water_area_corrected': water_areas_zhaogao
-            }).set_index('date')
-
-            fname = os.path.join(savedir, f"{df.index[0].strftime('%Y%m%d')}_{df.index[-1].strftime('%Y%m%d')}_{res_name}.csv")
-            df.to_csv(fname)
-            print(df.tail())
-
-            s_time = randint(5, 10)
-            print(f"Sleeping for {s_time} seconds")
-            time.sleep(s_time)
-
-            if (datetime.strptime(enddate, "%Y-%m-%d")-df.index[-1]).days < TEMPORAL_RESOLUTION:
-                print(f"Quitting: Reached enddate {enddate}")
-                break
-            elif df.index[-1].strftime('%Y-%m-%d') == fo:
-                print(f"Reached last available observation - {fo}")
-                break
-            elif num_runs > 1000:
-                print("Quitting: Reached 1000 iterations")
-                break
-        except Exception as e:
-            log.error(e)
-            continue
+    if(number_of_images):
+        fo = get_first_obs(start, end).format('YYYY-MM-dd').getInfo()
+        first_obs = datetime.strptime(fo, '%Y-%m-%d')
+
+        scratchdir = os.path.join(datadir, "_scratch")
+
+        # flag = True
+        num_runs = 0
+
+        # If data already exists, only get new data starting from the last one
+        savepath = os.path.join(datadir, f"{res_name}.csv")
+        
+        if os.path.isfile(savepath):
+            temp_df = pd.read_csv(savepath, parse_dates=['date']).set_index('date')
+
+            last_date = temp_df.index[-1].to_pydatetime()
+            fo = (last_date - timedelta(days=TEMPORAL_RESOLUTION*2)).strftime("%Y-%m-%d")
+            to_combine = [savepath]
+            print(f"Existing file found - Last observation ({TEMPORAL_RESOLUTION*2} day lag): {last_date}")
+
+            # If 16 days have not passed since last observation, skip the processing
+            days_passed = (datetime.strptime(end, "%Y-%m-%d") - last_date).days
+            print(f"No. of days passed since: {days_passed}")
+            if days_passed < TEMPORAL_RESOLUTION:
+                print(f"No new observation expected. Quitting early")
+                return None
+        else:
+            to_combine = []
+        
+        savedir = os.path.join(scratchdir, f"{res_name}_s2_cordeiro_zhao_gao_{fo}_{enddate}")
+        if not os.path.isdir(savedir):
+            os.makedirs(savedir)
+        
+        print(f"Extracting SA for the period {fo} -> {enddate}")
+
+        dates = pd.date_range(fo, enddate, freq=f'{TEMPORAL_RESOLUTION}D')
+        grouped_dates = grouper(dates, RESULTS_PER_ITER)
+
+        # # redo the calculations part and see where it is complaining about too many aggregations
+        # subset_dates = next(grouped_dates)
+        # dates = ee.List([ee.Date(d) for d in subset_dates if d is not None])
+
+        # print(subset_dates)
+        # res = generate_timeseries(dates).filterMetadata('s2_images', 'greater_than', 0)
+        # pprint.pprint(res.aggregate_array('s2_images').getInfo())
+
+        # uncorrected_columns_to_extract = ['from_date', 'to_date', 'water_area_cordeiro', 'non_water_area_cordeiro', 'water_area_NDWI', 'non_water_area_NDWI', 'cloud_area', 's2_images']
+        # uncorrected_final_data_ee = res.reduceColumns(ee.Reducer.toList(len(uncorrected_columns_to_extract)), uncorrected_columns_to_extract).get('list')
+        # uncorrected_final_data = uncorrected_final_data_ee.getInfo()
+        
+
+
+        for subset_dates in grouped_dates:
+            try:
+                print(subset_dates)
+                dates = ee.List([ee.Date(d) for d in subset_dates if d is not None])
+                
+                ts_imcoll = generate_timeseries(dates)
+                postprocessed_ts_imcoll = ts_imcoll.map(postprocess_wrapper)
+
+                # Download the data locally
+                ts_imcoll_L = ts_imcoll.getInfo()
+                postprocessed_ts_imcoll_L = postprocessed_ts_imcoll.getInfo()
+
+                # Parse the data to create dataframe
+                PROCESSING_STATUSES = []
+                POSTPROCESSING_STATUSES = []
+                cloud_areas = []
+                cloud_percents = []
+                from_dates = []
+                to_dates = []
+                obs_dates = []
+                non_water_areas = []
+                water_areas = []
+                water_areas_zhaogao = []
+                for f, f_postprocessed in zip(ts_imcoll_L['features'], postprocessed_ts_imcoll_L['features']):
+                    PROCESSING_STATUS = f['properties']['PROCESSING_SUCCESSFUL']
+                    PROCESSING_STATUSES.append(PROCESSING_STATUS)
+                    POSTPROCESSING_STATUS = f_postprocessed['properties']['POSTPROCESSING_SUCCESSFUL']
+                    POSTPROCESSING_STATUSES.append(POSTPROCESSING_STATUS)
+                    obs_dates.append(pd.to_datetime(f['properties']['system:time_start']))
+                    from_dates.append(pd.to_datetime(f['properties']['from_date']))
+                    to_dates.append(pd.to_datetime(f['properties']['to_date']))
+                    if PROCESSING_STATUS:
+                        water_areas.append(f['properties']['water_area_clustering'])
+                        non_water_areas.append(f['properties']['non_water_area_clustering'])
+                        cloud_areas.append(f['properties']['cloud_area'])
+                        cloud_percents.append(f['properties']['cloud_percent'])
+                    else:
+                        water_areas.append(np.nan)
+                        non_water_areas.append(np.nan)
+                        cloud_areas.append(np.nan)
+                        cloud_percents.append(np.nan)
+                    if POSTPROCESSING_STATUS:
+                        water_areas_zhaogao.append(f_postprocessed['properties']['corrected_area'])
+                    else:
+                        water_areas_zhaogao.append(np.nan)
+                
+                df = pd.DataFrame({
+                    'date': obs_dates,
+                    'PROCESSING_STATUS': PROCESSING_STATUSES,
+                    'POSTPROCESSING_STATUS': POSTPROCESSING_STATUSES,
+                    'from_date': from_dates,
+                    'to_date': to_dates,
+                    'cloud_area': cloud_areas,
+                    'cloud_percent': cloud_percents,
+                    'water_area_uncorrected': water_areas,
+                    'non_water_area': non_water_areas,
+                    'water_area_corrected': water_areas_zhaogao
+                }).set_index('date')
+
+                fname = os.path.join(savedir, f"{df.index[0].strftime('%Y%m%d')}_{df.index[-1].strftime('%Y%m%d')}_{res_name}.csv")
+                df.to_csv(fname)
+                print(df.tail())
+
+                s_time = randint(5, 10)
+                print(f"Sleeping for {s_time} seconds")
+                time.sleep(s_time)
+
+                if (datetime.strptime(enddate, "%Y-%m-%d")-df.index[-1]).days < TEMPORAL_RESOLUTION:
+                    print(f"Quitting: Reached enddate {enddate}")
+                    break
+                elif df.index[-1].strftime('%Y-%m-%d') == fo:
+                    print(f"Reached last available observation - {fo}")
+                    break
+                elif num_runs > 1000:
+                    print("Quitting: Reached 1000 iterations")
+                    break
+            except Exception as e:
+                log.error(e)
+                continue
 
-    # Combine the files into one database
-    to_combine.extend([os.path.join(savedir, f) for f in os.listdir(savedir) if f.endswith(".csv")])
+        # Combine the files into one database
+        to_combine.extend([os.path.join(savedir, f) for f in os.listdir(savedir) if f.endswith(".csv")])
 
-    files = [pd.read_csv(f, parse_dates=["date"]).set_index("date") for f in to_combine]
-    data = pd.concat(files).drop_duplicates().sort_values("date")
+        files = [pd.read_csv(f, parse_dates=["date"]).set_index("date") for f in to_combine]
+        data = pd.concat(files).drop_duplicates().sort_values("date")
 
-    data.to_csv(savepath)
+        data.to_csv(savepath)
+    else:
+        print(f"No observation observed between {start} and {end}. Quitting!")
+        return None
 
     return savepath
 
 # User-facing wrapper function
 def sarea_s2(res_name, res_polygon, start, end, datadir):
     return run_process_long(res_name,res_polygon, start, end, datadir)
```

### Comparing `rat-2.1/src/rat/core/sarea/sarea_cli_sar.py` & `rat-3.0.0a4/src/rat/core/sarea/sarea_cli_sar.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,16 @@
-from core.sarea.sarea_cli_s2 import TEMPORAL_RESOLUTION
 import ee
 import numpy as np
 import pandas as pd
-import argparse
 import os
 from datetime import datetime, timedelta
 
-from ee_utils.ee_utils import poly2feature
-
-#### initialize the connection to the server ####
-from ee_utils.ee_config import service_account,key_file
-
-ee_credentials = ee.ServiceAccountCredentials(service_account, key_file)
-ee.Initialize(ee_credentials)
-#### Connection established ####
+from rat.core.sarea.sarea_cli_s2 import TEMPORAL_RESOLUTION
+from rat.ee_utils.ee_utils import poly2feature
+from rat.utils.utils import days_between
 
 s1 = ee.ImageCollection("COPERNICUS/S1_GRD")
 
 # definitions
 ANGLE_THRESHOLD_1 = ee.Number(45.4);
 ANGLE_THRESHOLD_2 = ee.Number(31.66)
 REVISIT_TIME = ee.Number(12)
@@ -108,15 +101,15 @@
         'sarea': wc
     })
     df['time'] = df['time'].apply(lambda t: np.datetime64(t, 'ms'))
     
     return df
 
 def retrieve_sar(start_date, end_date, res='ys'):
-    date_ranges = list(pd.date_range(start_date, end_date, freq=res).strftime("%Y-%m-%d").tolist()) + [end_date]
+    date_ranges = list((pd.date_range(start_date, end_date, freq=res).union([pd.to_datetime(start_date), pd.to_datetime(end_date)])).strftime("%Y-%m-%d").tolist()) 
     print(date_ranges)
     dfs = []
     # for begin, end in zip(date_ranges[:-1], date_ranges.shift(1)[:-1]):
     for begin, end in zip(date_ranges[:-1], date_ranges[1:]):
         # begin_str, end_str = begin.strftime('%Y-%m-%d'), end.strftime('%Y-%m-%d')
         print(f"Processing: {begin} - {end} ")
         dfs.append(ee_get_data(begin, end))
@@ -132,34 +125,50 @@
 def sarea_s1(reservoir, reservoir_polygon ,start_date, end_date, datadir):
     
     # Extracting reservoir geometry 
     global ROI 
     ROI = poly2feature(reservoir_polygon,BUFFER_DIST).geometry()
     TEMPORAL_RESOLUTION = 12
 
-    savepath = os.path.join(datadir, f"{reservoir}_12d_sar.csv")
-    if os.path.isfile(savepath):
-        existing_df = pd.read_csv(savepath, parse_dates=['time']).set_index('time')
-
-        last_date = existing_df.index[-1].to_pydatetime()
-        start_date = (last_date - timedelta(days=TEMPORAL_RESOLUTION*2)).strftime("%Y-%m-%d")
-        to_combine = [existing_df.reset_index()]
-        print(f"Existing file found - Last observation ({TEMPORAL_RESOLUTION*2} day lag): {last_date}")
-
-        # If <TEMPORAL RESOLUTION> days have not passed since last observation, skip the processing
-        days_passed = (datetime.strptime(end_date, "%Y-%m-%d") - last_date).days
-        print(f"No. of days passed since: {days_passed}")
-        if days_passed < TEMPORAL_RESOLUTION:
-            print(f"No new observation expected. Quitting early")
-            return savepath
+    ## Checking if time interval is small then the image collection should not be empty in GEE
+    if (days_between(start_date,end_date) < 30):     # less than a month difference
+        number_of_images = s1.filterDate(start_date,end_date) \
+            .filterBounds(ROI) \
+            .filter(ee.Filter.listContains('transmitterReceiverPolarisation', 'VV')) \
+            .filter(ee.Filter.eq('instrumentMode', 'IW')).size().getInfo()
     else:
-        to_combine = []
+        number_of_images = 1     # more than a month difference simply run, so no need to calculate number_of_images
+    
+    if(number_of_images):
+        savepath = os.path.join(datadir, f"{reservoir}_12d_sar.csv")
+        if os.path.isfile(savepath):
+            existing_df = pd.read_csv(savepath, parse_dates=['time']).set_index('time')
+
+            last_date = existing_df.index[-1].to_pydatetime()
+            start_date = (last_date - timedelta(days=TEMPORAL_RESOLUTION*2)).strftime("%Y-%m-%d")
+            to_combine = [existing_df.reset_index()]
+            print(f"Existing file found - Last observation ({TEMPORAL_RESOLUTION*2} day lag): {last_date}")
+
+            # If <TEMPORAL RESOLUTION> days have not passed since last observation, skip the processing
+            days_passed = (datetime.strptime(end_date, "%Y-%m-%d") - last_date).days
+            print(f"No. of days passed since: {days_passed}")
+            if days_passed < TEMPORAL_RESOLUTION:
+                print(f"No new observation expected. Quitting early")
+                return savepath
+        else:
+            to_combine = []
+
+        results = retrieve_sar(start_date, end_date, res='6MS')
+        to_combine.append(results)
+        data = pd.concat(to_combine).drop_duplicates().sort_values("time")
+        
+        if not os.path.isdir(datadir):
+            os.makedirs(datadir)
+        data.to_csv(savepath, index=False)
+
+        return savepath
 
-    results = retrieve_sar(start_date, end_date, res='6MS')
-    to_combine.append(results)
-    data = pd.concat(to_combine).drop_duplicates().sort_values("time")
-    
-    if not os.path.isdir(datadir):
-        os.makedirs(datadir)
-    data.to_csv(savepath, index=False)
+    else:
+        print(f"No observation observed between {start_date} and {end_date}. Quitting!")
+        return None
 
     return savepath
```

### Comparing `rat-2.1/src/rat/data_processing/altimetry.py` & `rat-3.0.0a4/src/rat/data_processing/altimetry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 import geopandas as gpd
-from osgeo import gdal, ogr
-import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
-from scipy.fft import fft
-from shapely.geometry.linestring import LineString
 import netCDF4 
-from utils.utils import round_up
+from rat.utils.utils import round_up
 
 
 def get_j3_tracks(reservoir, reservoir_column_dict, tracks_df, custom_reservoir_range_dict):
     """Returns a list of Jason-3 ground tracks and the min-max latitudes of intersection
 
     Args:
         reservoir (geopandas dataframe): Geodataframe object of reservoir having only one row
@@ -64,28 +60,26 @@
 import os, sys
 import os.path
 import numpy as np
 import pandas as pd
 from netCDF4 import Dataset
 from datetime import datetime
 from ftplib import FTP
-from tqdm import tqdm
 import glob
 import time
 from numpy import empty
 from numpy import loadtxt
 import math
 import statistics
 from scipy import io
 from scipy import stats
 from scipy import interpolate
 from scipy.cluster.vq import kmeans2
 import matplotlib.pyplot as plt
 from sklearn.cluster import KMeans
-from tqdm import tqdm
 
 import configparser
 from datetime import timedelta, datetime
 
 
 def _get_suffix():
     return datetime.today().strftime("%Y%m%d_%H_%M_%S")
```

### Comparing `rat-2.1/src/rat/data_processing/metsim_input_processing.py` & `rat-3.0.0a4/src/rat/data_processing/metsim_input_processing.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,38 @@
 import xarray as xr
 import datetime
 import os
 from logging import getLogger
-from tqdm import tqdm
-import configparser
 import numpy as np
 import rasterio as rio
 import numpy as np
 import xarray as xr
 import os
-from tqdm import tqdm
-import itertools
 import pandas as pd
 
-from utils.logging import LOG_NAME, NOTIFICATION
+from rat.utils.logging import LOG_NAME, NOTIFICATION
 
 log = getLogger(LOG_NAME)
 
 class CombinedNC:
-    def __init__(self, start, end, datadir, basingridpath, outputdir):
+    def __init__(self, start, end, datadir, basingridpath, outputdir, use_previous):
         """
         Parameters:
             start: Start date in YYYY-MM-DD format
             :
             :
             datadir: Directory path of ascii format files
         """
         log.debug("Started combining forcing data for MetSim processing")
         self._start = start
         self._end = end
         self._total_days = (self._end - self._start).days
         self._datadir = datadir
         self._outputpath = outputdir
+        self._use_previous = use_previous
 
         self._rast = rio.open(basingridpath)
         self._ar = self._rast.read(1, masked=True)
         self._gridvalue = self._ar.flatten()
 
         self._longitudes1d, self._latitudes1d = self._get_lat_long_1d()
         self._latitudes, self._longitudes = self._get_lat_long_meshgrid()
@@ -63,15 +60,14 @@
         longitudes, latitudes = xy[1].flatten(), xy[0].flatten()
         # Need to flip latutudes on horizontal axis
         latitudes = np.flip(latitudes, 0)
         
         return latitudes, longitudes
 
     def _read(self):
-        # with tqdm(total=len(self.dates)) as pbar:
         for day, date in enumerate(self.dates):
             fileDate = date
             reqDate = fileDate.strftime("%Y-%m-%d")
             log.debug("Combining data: %s", reqDate)
             # pbar.set_description(reqDate)
             
             precipfilepath = os.path.join(self._datadir, f'precipitation/{reqDate}_IMERG.asc')
@@ -97,14 +93,26 @@
             # self.dates.append(fileDate)
             self.precips[day, :, :] = precipitation
             self.tmaxes[day, :, :] = tmax
             self.tmins[day, :, :] = tmin
             self.winds[day, :, :] = wind
             # pbar.update(1)
 
+    def _impute_basin_missing_data(self, combined_data):
+        combine_nomiss_data = combined_data.where(combined_data['extent']==1,-9999)
+        try:
+            combine_nomiss_data = combine_nomiss_data.interpolate_na(dim="time", method="linear", fill_value="extrapolate")
+        except:
+            try:
+                combine_nomiss_data = combine_nomiss_data.interpolate_na(dim="lon", method="linear", fill_value="extrapolate")
+            except:
+                print("No inter or extra polation can be done.")
+        combine_nomiss_data = combine_nomiss_data.where(combine_nomiss_data!=-9999,combined_data)
+        return combine_nomiss_data
+
     def _write(self):
         precip_da = xr.DataArray(
             data = self.precips,
             coords=[self.dates, np.flip(self._latitudes1d), self._longitudes1d],
             dims=['time', 'lat', 'lon']
         )
 
@@ -138,28 +146,34 @@
                 tmax = tmax_da,
                 tmin = tmin_da,
                 wind = wind_da,
                 extent = extent_da
             )
         )
 
-        if os.path.isfile(self._outputpath):
-            log.debug(f"Found existing file at {self._outputpath} -- Updating in-place")
-            # Assuming the existing file structure is same as the one generated now. Basically
-            #   assuming that the previous file was also created by MetSimRunner
-            existing = xr.open_dataset(self._outputpath).load()
-            existing.close()
-            last_existing_time = existing.time[-1]
-            log.debug("Existing data: %s", last_existing_time)
-            ds = ds.sel(time=slice(last_existing_time + np.timedelta64(1,'D') , ds.time[-1]))
-            # ds = ds.isel(time=slice(1, None))
-            xr.merge([existing, ds]).to_netcdf(self._outputpath)
+        if self._use_previous:
+            if os.path.isfile(self._outputpath):
+                log.debug(f"Found existing file at {self._outputpath} -- Updating in-place")
+                # Assuming the existing file structure is same as the one generated now. Basically
+                #   assuming that the previous file was also created by MetSimRunner
+                existing = xr.open_dataset(self._outputpath).load()
+                existing.close()
+                last_existing_time = existing.time[-1]
+                log.debug("Existing data: %s", last_existing_time)
+                existing_to_append = existing.sel(time=slice(ds.time[0] - np.timedelta64(120,'D') , last_existing_time))
+                ds = ds.sel(time=slice(last_existing_time + np.timedelta64(1,'D') , ds.time[-1]))
+                # ds = ds.isel(time=slice(1, None))
+                write_ds = xr.merge([existing_to_append, ds])
+                ds = self._impute_basin_missing_data(write_ds)
+            else:
+                raise Exception('Previous combined dataset not found. Please run RAT without state files first.')
         else:
             log.debug(f"Creating new file at {self._outputpath}")
-            ds.to_netcdf(self._outputpath)
+            ds = self._impute_basin_missing_data(ds)
+        ds.to_netcdf(self._outputpath)
         # log.debug(f"Saving {len(paths)} files at {self._outputdir}")
         # xr.save_mfdataset(datasets, paths)
 
 def generate_state_and_inputs(forcings_startdate, forcings_enddate, combined_datapath, out_dir):
     # Generate state. Assuming `nc_fmt_data` contains all the data, presumably containing enough data
     # to create state file (upto 90 days prior data from forcings_startdate)
     combined_data = xr.open_dataset(combined_datapath)
```

### Comparing `rat-2.1/src/rat/data_processing/newdata.py` & `rat-3.0.0a4/src/rat/data_processing/newdata.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 import subprocess
-import yaml
 import requests
 from datetime import datetime, timedelta
-from tqdm import tqdm
 import os
+import time
 import shutil
 import tempfile
 import rioxarray as rxr
 import xarray as xr
 from logging import getLogger
 import pandas as pd
+from concurrent.futures import ProcessPoolExecutor, as_completed
+from pathlib import Path
+from dask.distributed import Semaphore
+import dask
 
-from utils.logging import LOG_NAME, NOTIFICATION
-from utils.utils import create_directory
+from rat.utils.logging import LOG_NAME, NOTIFICATION
+from rat.utils.utils import create_directory
 import configparser
 
 log = getLogger(LOG_NAME)
 
 def run_command(cmd,shell_bool=False):
     """Safely runs a command, and returns the returncode silently in case of no error. Otherwise,
     raises an Exception
@@ -84,15 +87,14 @@
             '--password',
             f'{secrets["imerg"]["pwd"]}',
             link,
             '--no-proxy'
         ]
     return cmd
 
-
 def download_precip(date, version, outputpath, secrets, interpolate=True):
     """
     Parameters:
         date: datetime object that defines the date for which data is required
         version: which version of data to download - IMERG-LATE or IMERG-EARLY
         outputpath: path where the data should be downloaded
     =======
@@ -160,97 +162,153 @@
 def download_tmax(year, outputpath):
     """
     Parameters:
         year: year for which data is to be downloaded, as a string
         outputpath: path where the data has to be saved
     """
     ## New data will keep on coming in the year going on i.e. recent year
-    tod = datetime.now()
-    days_ago_20 = tod - timedelta(days=20)
-    today_year = str(tod.year)
-    recent_year_20day_ago = str(days_ago_20.year) 
-    if ((not(os.path.exists(outputpath))) or (year == recent_year_20day_ago) or (year == today_year)):
+    tod = datetime.now()  #today date
+    days_ago_20 = tod - timedelta(days=20)  # date 20 days back
+    today_year = str(tod.year)    # today year 
+    recent_year_20day_ago = str(days_ago_20.year)  # year for 20 days back 
+    if (not(os.path.exists(outputpath))):
         cmd = [
             'wget', 
             '-O', 
             f'{outputpath}', 
             f'ftp://ftp.cdc.noaa.gov/Datasets/cpc_global_temp/tmax.{year}.nc'
         ]
         log.debug("Downloading tmax: %s", year)
         return run_command(cmd)
     else:
         log.info("File already exists tmax: %s", year)
+        date_of_file_modification = time.ctime(os.path.getmtime(outputpath))
+        log.info(f"Last modified date:{date_of_file_modification}")
+        if ((year == recent_year_20day_ago) or (year == today_year)):
+            if(datetime.strptime(date_of_file_modification, "%c").date()==tod.date()):
+                log.info("No data since last modified date. No need to download.")
+            else:
+                cmd = [
+                    'wget', 
+                    '-O', 
+                    f'{outputpath}', 
+                    f'ftp://ftp.cdc.noaa.gov/Datasets/cpc_global_temp/tmax.{year}.nc'
+                ]
+                log.debug("Last modified date is not today. So, updating tmax: %s", year)
+                return run_command(cmd)
+                
 
 def download_tmin(year, outputpath):
     """
     Parameters:
         year: year for which data is to be downloaded, as a string
         outputpath: path where the data has to be saved
     """
     ## New data will keep on coming in the year going on i.e. recent year
-    tod = datetime.now()
-    days_ago_20 = tod - timedelta(days=20)
-    today_year = str(tod.year)
-    recent_year_20day_ago = str(days_ago_20.year)  
-    if ((not(os.path.exists(outputpath))) or (year == recent_year_20day_ago) or (year == today_year)):
+    tod = datetime.now()  #today date
+    days_ago_20 = tod - timedelta(days=20)  # date 20 days back
+    today_year = str(tod.year)    # today year 
+    recent_year_20day_ago = str(days_ago_20.year)  # year for 20 days back 
+    if (not(os.path.exists(outputpath))):
         cmd = [
             'wget', 
             '-O', 
             f'{outputpath}', 
             f'ftp://ftp.cdc.noaa.gov/Datasets/cpc_global_temp/tmin.{year}.nc'
         ]
         log.debug("Downloading tmin: %s", year)
         return run_command(cmd)
     else:
         log.info("File already exists tmin: %s", year)
+        date_of_file_modification = time.ctime(os.path.getmtime(outputpath))
+        log.info(f"Last modified date:{date_of_file_modification}")
+        if ((year == recent_year_20day_ago) or (year == today_year)):
+            if(datetime.strptime(date_of_file_modification, "%c").date()==tod.date()):
+                log.info("No data since last modified date. No need to download.")
+            else:
+                cmd = [
+                    'wget', 
+                    '-O', 
+                    f'{outputpath}', 
+                    f'ftp://ftp.cdc.noaa.gov/Datasets/cpc_global_temp/tmin.{year}.nc'
+                ]
+                log.debug("Last modified date is not today. So, updating tmin: %s", year)
+                return run_command(cmd)
 
 def download_uwnd(year, outputpath):
     """
     Parameters:
         year: year for which data is to be downloaded, as a string
         outputpath: path where the data has to be saved
     """
     ## New data will keep on coming in the year going on i.e. recent year
-    tod = datetime.now()
-    days_ago_20 = tod - timedelta(days=20)
-    today_year = str(tod.year)
-    recent_year_20day_ago = str(days_ago_20.year) 
-    if ((not(os.path.exists(outputpath))) or (year == recent_year_20day_ago) or (year == today_year)):
+    tod = datetime.now()  #today date
+    days_ago_20 = tod - timedelta(days=20)  # date 20 days back
+    today_year = str(tod.year)    # today year 
+    recent_year_20day_ago = str(days_ago_20.year)  # year for 20 days back 
+    if (not(os.path.exists(outputpath))):
         cmd = [
             'wget', 
             '-O', 
             f'{outputpath}', 
             f'ftp://ftp2.psl.noaa.gov/Datasets/ncep.reanalysis/surface_gauss/uwnd.10m.gauss.{year}.nc'
         ]
         log.debug("Downloading uwnd: %s", year)
         return run_command(cmd)
     else:
         log.info("File already exists uwnd: %s", year)
+        date_of_file_modification = time.ctime(os.path.getmtime(outputpath))
+        log.info(f"Last modified date:{date_of_file_modification}")
+        if ((year == recent_year_20day_ago) or (year == today_year)):
+            if(datetime.strptime(date_of_file_modification, "%c").date()==tod.date()):
+                log.info("No data since last modified date. No need to download.")
+            else:
+                cmd = [
+                    'wget', 
+                    '-O', 
+                    f'{outputpath}', 
+                    f'ftp://ftp2.psl.noaa.gov/Datasets/ncep.reanalysis/surface_gauss/uwnd.10m.gauss.{year}.nc'
+                ]
+                log.debug("Last modified date is not today. So, updating uwnd: %s", year)
+                return run_command(cmd)
 
 def download_vwnd(year, outputpath):
     """
     Parameters:
         year: year for which data is to be downloaded, as a string
         outputpath: path where the data has to be saved
     """
     ## New data will keep on coming in the year going on i.e. recent year
-    tod = datetime.now()
-    days_ago_20 = tod - timedelta(days=20)
-    today_year = str(tod.year)
-    recent_year_20day_ago = str(days_ago_20.year) 
-    if ((not(os.path.exists(outputpath))) or (year == recent_year_20day_ago) or (year == today_year)):
+    tod = datetime.now()  #today date
+    days_ago_20 = tod - timedelta(days=20)  # date 20 days back
+    today_year = str(tod.year)    # today year 
+    recent_year_20day_ago = str(days_ago_20.year)  # year for 20 days back 
+    if (not(os.path.exists(outputpath))):
         cmd = [
             'wget', 
             '-O', 
             f'{outputpath}', 
             f'ftp://ftp2.psl.noaa.gov/Datasets/ncep.reanalysis/surface_gauss/vwnd.10m.gauss.{year}.nc']
         log.debug("Downloading vwnd: %s", year)
         return run_command(cmd)
     else:
         log.info("File already exists vwnd: %s", year)
+        date_of_file_modification = time.ctime(os.path.getmtime(outputpath))
+        log.info(f"Last modified date:{date_of_file_modification}")
+        if ((year == recent_year_20day_ago) or (year == today_year)):
+            if(datetime.strptime(date_of_file_modification, "%c").date()==tod.date()):
+                log.info("No data since last modified date. No need to download.")
+            else:
+                cmd = [
+                    'wget', 
+                    '-O', 
+                    f'{outputpath}', 
+                    f'ftp://ftp2.psl.noaa.gov/Datasets/ncep.reanalysis/surface_gauss/vwnd.10m.gauss.{year}.nc']
+                log.debug("Last modified date is not today. So, updating vwnd: %s", year)
+                return run_command(cmd)
 
 def download_data(begin, end, datadir, secrets):
     """Downloads the data between dates defined by begin and end
 
     Parameters:
         begin: Data will start downloading from this date, including this date
         end: Data will be downloaded until this date, including this date
@@ -259,44 +317,43 @@
 
     # Obtain list of dates to be downloaded
     # required_dates = [begin+timedelta(days=n) for n in range((end-begin).days)]
     required_dates = pd.date_range(begin, end)
     required_years = list(set([d.strftime("%Y") for d in required_dates]))
     # Download Precipitation
     log.debug("Downloading Precipitation")
-    # with tqdm(required_dates) as pbar:
+
+    sem = Semaphore(max_leases=4, name="IMERG-Downloader")
+    def download_precip_with_semaphore(date, version, outputpath, secrets, sem):
+        with sem:
+            result = download_precip(date, version, outputpath, secrets)
+            return result
+    
+    futures = []
     for date in required_dates:
-        # determine what kind of data is required
         data_version = _determine_precip_version(date)
         outputpath = os.path.join(datadir, "precipitation", f"{date.strftime('%Y-%m-%d')}_IMERG.tif")
-        # pbar.set_description(f"{date.strftime('%Y-%m-%d')} ({data_version})")
-        download_precip(date, data_version, outputpath, secrets)
-        # pbar.update(1)
-    
+        if not os.path.isfile(outputpath):
+            future = dask.delayed(download_precip_with_semaphore)(date, data_version, outputpath, secrets, sem)
+            futures.append(future)
+
+    results = dask.compute(*futures) # downloading precipitation files first
+    futures = []
+
     # Download other forcing data
     log.debug("Downloading TMax, TMin, UWnd, and VWnd")
-    # with tqdm(required_years, total=len(required_years)*4) as pbar:
     for year in required_years:
-        # pbar.set_description(f"{year} (TMax)")
-        download_tmax(year, os.path.join(datadir, "tmax", year+'.nc'))
-        # pbar.update(1)
-
-        # pbar.set_description(f"{year} (TMin)")
-        download_tmin(year, os.path.join(datadir, "tmin", year+'.nc'))
-        # pbar.update(1)
-
-        # pbar.set_description(f"{year} (UWnd)")
-        download_uwnd(year, os.path.join(datadir, "uwnd", year+'.nc'))
-        # pbar.update(1)
-
-        # pbar.set_description(f"{year} (VWnd)")
-        download_vwnd(year, os.path.join(datadir, "vwnd", year+'.nc'))
-        # pbar.update(1)
+        futures.append(dask.delayed(download_tmax)(year, os.path.join(datadir, "tmax", year+'.nc')))
+        futures.append(dask.delayed(download_tmin)(year, os.path.join(datadir, "tmin", year+'.nc')))
+        futures.append(dask.delayed(download_uwnd)(year, os.path.join(datadir, "uwnd", year+'.nc')))
+        futures.append(dask.delayed(download_vwnd)(year, os.path.join(datadir, "vwnd", year+'.nc')))
+    
+    results = dask.compute(*futures)
 
-def process_precip(basin_bounds,srcpath, dstpath, temp_datadir=None):
+def process_precip(basin_bounds, srcpath, dstpath, secrets=None, temp_datadir=None, itry=0):
     """For any IMERG Precipitation file located at `srcpath` is clipped, scaled and converted to
     ASCII grid file and saved at `dstpath`. All of this is done in a temporarily created directory
     which can be controlled by the `datadir` path
     """
     if temp_datadir is not None and not os.path.isdir(temp_datadir):
         raise Exception(f"ERROR: {temp_datadir} directory doesn't exist")
     
@@ -319,15 +376,32 @@
                 str(basin_bounds[3]),
                 '-of',
                 'GTiff',
                 '-overwrite', 
                 f'{srcpath}',
                 clipped_temp_file
             ]
-            run_command(cmd)
+            try:
+                run_command(cmd)
+            except subprocess.CalledProcessError as e:
+                src_fn = Path(srcpath)
+                date = pd.to_datetime(src_fn.stem.split('_')[0])
+                log.error(f"subprocess.CalledProcessError in {date}: ", e)
+                
+                # delete old precipitation file and redownload. retry once
+                if itry <= 1:
+                    src_fn = Path(srcpath)
+                    src_fn.unlink(missing_ok=True)
+
+                    version = _determine_precip_version(date)
+
+                    download_precip(date, version, srcpath, secrets)
+                    run_command(cmd)
+                else:
+                    raise e
 
             # Scale down (EARLY)
             scaled_temp_file = os.path.join(tempdir, 'scaled.tif')
             cmd = [
                 "gdal_calc.py", 
                 "-A", 
                 clipped_temp_file, 
@@ -351,15 +425,15 @@
 
             # Move to destination
             shutil.move(aai_temp_file, dstpath)
     else:
         print(f"Processing Precipitation file exist: {srcpath}")
 
 
-def process_nc(basin_bounds,date, srcpath, dstpath, temp_datadir=None):
+def process_nc(basin_bounds,date, srcpath, dstpath, temp_datadir=None, itry=0):
     """For TMax, TMin, UWnd and VWnd, the processing steps are same, and can be performed using
     this function.
 
     Parameters:
         date: Datetime object of the date of data
         srcpath: path of the nc file
         dstpath: path where the final ascii file will be saved
@@ -393,16 +467,16 @@
             "90",
             "-of",
             "GTiff",
             "-overwrite", 
             converted_tif_temp_file, 
             warped_temp_file]
             # runs and return non-zero code, so don't use run_command
-            cmd = " ".join(cmd)
-            subprocess.run(cmd,shell=True,stdout=subprocess.DEVNULL)
+            cmd = " ".join(cmd) 
+            subprocess.run(cmd, shell=True,stdout=subprocess.DEVNULL)
             
             
             # Change resolution
             scaled_temp_file = os.path.join(tempdir, "scaled.tif")
             cmd = [
                 "gdalwarp",
                 "-dstnodata", 
@@ -417,126 +491,121 @@
                 str(basin_bounds[3]),
                 '-of',
                 'GTiff',
                 '-overwrite',  
                 warped_temp_file, 
                 scaled_temp_file]
 
-                
             run_command(cmd)
 
             # Convert GeoTiff to AAI
             aai_temp_file = os.path.join(tempdir, "final_aai.tif")
             cmd = ["gdal_translate", "-of", "aaigrid", scaled_temp_file, aai_temp_file]
             run_command(cmd)
 
             # Move file to destination
             shutil.move(aai_temp_file, dstpath)
     else:
         print(f"Processing NC file exists: {srcpath} for date {date.strftime('%Y-%m-%d')}")
 
-
-def process_data(basin_bounds,raw_datadir, processed_datadir, begin, end, temp_datadir):
+def process_data(basin_bounds,raw_datadir, processed_datadir, begin, end, secrets, temp_datadir):
     if not os.path.isdir(temp_datadir):
         os.makedirs(temp_datadir)
 
     #### Process precipitation ####
     log.debug("Processing Precipitation")
     raw_datadir_precip = os.path.join(raw_datadir, "precipitation")
     processed_datadir_precip = os.path.join(processed_datadir, "precipitation")
 
-
     # with tqdm(os.listdir(raw_datadir_precip)) as pbar:
     ds = pd.date_range(begin, end)
+
+    futures = []
+    
     for srcname in os.listdir(raw_datadir_precip):
         if datetime.strptime(srcname.split(os.sep)[-1].split("_")[0], "%Y-%m-%d") in ds:
             srcpath = os.path.join(raw_datadir_precip, srcname)
             dstpath = os.path.join(processed_datadir_precip, srcname.replace("tif", "asc"))
 
             # pbar.set_description(f"Precipitation: {srcname.split('_')[0]}")
-            process_precip(basin_bounds,srcpath, dstpath, temp_datadir)
-            # pbar.update(1)
+            future = dask.delayed(process_precip)(basin_bounds, srcpath, dstpath, secrets, temp_datadir)
+            futures.append(future)
 
     #### Process NC files ####
     # required_dates = [begin+timedelta(days=n) for n in range((end-begin).days)]
     required_dates = pd.date_range(begin, end)
     #### Process TMAX ####
     log.debug("Processing TMAX")
     raw_datadir_tmax = os.path.join(raw_datadir, "tmax")
     processed_datadir_tmax = os.path.join(processed_datadir, "tmax")
 
-    # with tqdm(required_dates) as pbar:
     for date in required_dates:
         srcpath = os.path.join(raw_datadir_tmax, date.strftime('%Y')+'.nc')
         dstpath = os.path.join(processed_datadir_tmax, f"{date.strftime('%Y-%m-%d')}_TMAX.asc")
 
-        # pbar.set_description(f"TMAX: {date.strftime('%Y-%m-%d')}")
-        process_nc(basin_bounds,date, srcpath, dstpath, temp_datadir)
-        # pbar.update(1)
+        future = dask.delayed(process_nc)(basin_bounds,date, srcpath, dstpath, temp_datadir)
+        futures.append(future)
     
     #### Process TMin ####
     log.debug("Processing TMIN")
     raw_datadir_tmin = os.path.join(raw_datadir, "tmin")
     processed_datadir_tmin = os.path.join(processed_datadir, "tmin")
 
-    # with tqdm(required_dates) as pbar:
     for date in required_dates:
         srcpath = os.path.join(raw_datadir_tmin, date.strftime('%Y')+'.nc')
         dstpath = os.path.join(processed_datadir_tmin, f"{date.strftime('%Y-%m-%d')}_TMIN.asc")
 
-        # pbar.set_description(f"TMIN: {date.strftime('%Y-%m-%d')}")
-        process_nc(basin_bounds,date, srcpath, dstpath, temp_datadir)
-        # pbar.update(1)
+        future = dask.delayed(process_nc)(basin_bounds,date, srcpath, dstpath, temp_datadir)
+        futures.append(future)
+    
+    results = dask.compute(*futures)
 
     #### Process UWND ####
     log.debug("Processing UWND")
     raw_datadir_uwnd = os.path.join(raw_datadir, "uwnd")
     daily_datadir_uwnd = os.path.join(raw_datadir, "uwnd_daily")
     processed_datadir_uwnd = os.path.join(processed_datadir, "uwnd")
 
     uwnd_files = [os.path.join(raw_datadir_uwnd, f) for f in os.listdir(raw_datadir_uwnd)]
 
     for uwnd_f in uwnd_files:
         xr.open_dataset(uwnd_f).resample(time='1D').mean().to_netcdf(os.path.join(daily_datadir_uwnd, uwnd_f.split(os.sep)[-1]))
         # xr.open_dataset(vwnd_f).resample(time='1D').mean().to_netcdf(os.path.join(vwnd_outdir, vwnd_f.split(os.sep)[-1]))
 
-    # with tqdm(required_dates) as pbar:
     for date in required_dates:
         srcpath = os.path.join(daily_datadir_uwnd, date.strftime('%Y')+'.nc')
         dstpath = os.path.join(processed_datadir_uwnd, f"{date.strftime('%Y-%m-%d')}_UWND.asc")
 
-        # pbar.set_description(f"UWND: {date.strftime('%Y-%m-%d')}")
-        process_nc(basin_bounds,date, srcpath, dstpath, temp_datadir)
-        # pbar.update(1)
+        future = dask.delayed(process_nc)(basin_bounds,date, srcpath, dstpath, temp_datadir)
+        futures.append(future)
 
     #### Process VWND ####
     log.debug("Processing VWND")
     raw_datadir_vwnd = os.path.join(raw_datadir, "vwnd")
     daily_datadir_vwnd = os.path.join(raw_datadir, "vwnd_daily")
     processed_datadir_vwnd = os.path.join(processed_datadir, "vwnd")
 
     vwnd_files = [os.path.join(raw_datadir_vwnd, f) for f in os.listdir(raw_datadir_vwnd)]
 
     for vwnd_f in vwnd_files:
         xr.open_dataset(vwnd_f).resample(time='1D').mean().to_netcdf(os.path.join(daily_datadir_vwnd, vwnd_f.split(os.sep)[-1]))
 
-    # with tqdm(required_dates) as pbar:
     for date in required_dates:
         srcpath = os.path.join(daily_datadir_vwnd, date.strftime('%Y')+'.nc')
         dstpath = os.path.join(processed_datadir_vwnd, f"{date.strftime('%Y-%m-%d')}_VWND.asc")
 
-        # pbar.set_description(f"VWND: {date.strftime('%Y-%m-%d')}")
-        process_nc(basin_bounds,date, srcpath, dstpath, temp_datadir)
-        # pbar.update(1)
+        future = dask.delayed(process_nc)(basin_bounds,date, srcpath, dstpath, temp_datadir)
+        futures.append(future)
+    results = dask.compute(*futures)
 
 
 def get_newdata(basin_name,basin_bounds,data_dir, basin_data_dir,startdate, enddate, secrets_file, download=True, process=True):
-    raw_datadir = os.path.join(data_dir, "raw",'')
-    processed_datadir = os.path.join(basin_data_dir, "processed",'')
-    temp_datadir = os.path.join(basin_data_dir, "temp",'')
+    raw_datadir = os.path.join(data_dir,"raw",'')
+    processed_datadir = os.path.join(basin_data_dir,"pre_processing","processed",'')
+    temp_datadir = os.path.join(basin_data_dir,"pre_processing","temp",'')
     
     ####Creating the required directories####
 
     dir_paths=[raw_datadir,processed_datadir]
     #Creating data directory if does not exist
     create_directory(basin_data_dir)
 
@@ -572,8 +641,8 @@
 
     #### DATA DOWNLOADING ####
     if download:
         download_data(startdate, enddate, raw_datadir, secrets)
 
     #### DATA PROCESSING ####
     if process:
-        process_data(basin_bounds,raw_datadir, processed_datadir, startdate, enddate, temp_datadir)
+        process_data(basin_bounds,raw_datadir, processed_datadir, startdate, enddate, secrets, temp_datadir)
```

### Comparing `rat-2.1/src/rat/ee_utils/ee_aec_file_creator.py` & `rat-3.0.0a4/src/rat/ee_utils/ee_aec_file_creator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,14 @@
 import ee
 import os
 import geopandas as gpd
 import pandas as pd
 import numpy as np
 from itertools import zip_longest,chain
-from ee_utils.ee_utils import poly2feature
-
-#### initialize the connection to the server ####
-from ee_utils.ee_config import service_account,key_file
-
-ee_credentials = ee.ServiceAccountCredentials(service_account, key_file)
-ee.Initialize(ee_credentials)
-#### Connection established ####
+from rat.ee_utils.ee_utils import poly2feature
 
 BUFFER_DIST = 500
 DEM = ee.Image('USGS/SRTMGL1_003')
 
 def grouper(iterable, n, *, incomplete='fill', fillvalue=None):
     "Collect data into non-overlapping fixed-length chunks or blocks"
     # grouper('ABCDEFG', 3, fillvalue='x') --> ABC DEF Gxx
```

### Comparing `rat-2.1/src/rat/rat.py` & `rat-3.0.0a4/src/rat/rat_basin.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,136 +1,273 @@
-import subprocess
-import yaml
-from datetime import datetime, timedelta
-from tqdm import tqdm
+from datetime import datetime
 import os
-import shutil
-import tempfile
-import xarray as xr
-import rioxarray as rxr
-import rasterio
 from logging import getLogger
-import pandas as pd
-import configparser
 import datetime
 import geopandas as gpd
-from shapely.geometry import Polygon,mapping
 import numpy as np
-import math
-import glob
+import xarray as xr
 
-from utils.utils import create_directory
-from utils.logging import init_logger,close_logger,NOTIFICATION
-from utils.files_creator import create_basingridfile, create_basin_domain_nc_file ,create_vic_domain_param_file, create_basin_grid_flow_asc
-from utils.files_creator import create_basin_station_latlon_csv, create_basin_reservoir_shpfile
+from rat.utils.utils import create_directory
+from rat.utils.logging import init_logger,close_logger,NOTIFICATION
+from rat.utils.files_creator import create_basingridfile, create_basin_domain_nc_file ,create_vic_domain_param_file, create_basin_grid_flow_asc
+from rat.utils.files_creator import create_basin_station_latlon_csv, create_basin_reservoir_shpfile
+from rat.utils.clean import Clean
 
-from data_processing.newdata import get_newdata
+from rat.data_processing.newdata import get_newdata
 
-from data_processing.metsim_input_processing import CombinedNC,generate_state_and_inputs
-from utils.metsim_param_reader import MSParameterFile
-from core.run_metsim import MetSimRunner
+from rat.data_processing.metsim_input_processing import CombinedNC,generate_state_and_inputs
+from rat.utils.metsim_param_reader import MSParameterFile
+from rat.core.run_metsim import MetSimRunner
 
-from utils.vic_param_reader import VICParameterFile
-from core.run_vic import VICRunner
+from rat.utils.vic_param_reader import VICParameterFile
+from rat.core.run_vic import VICRunner
 
-from utils.route_param_reader import RouteParameterFile
-from core.run_routing import RoutingRunner
+from rat.utils.route_param_reader import RouteParameterFile
+from rat.core.run_routing import RoutingRunner
 
-from core.run_sarea import run_sarea
-from core.run_altimetry import altimeter_routine, run_altimetry
+from rat.core.run_altimetry import run_altimetry
 
-from ee_utils.ee_aec_file_creator import aec_file_creator
-from core.run_postprocessing import run_postprocessing
+from rat.core.run_postprocessing import run_postprocessing
 
-from utils.convert_for_website import convert_sarea, convert_inflow, convert_dels, convert_evaporation, convert_outflow, convert_altimeter
-from core.generate_plots import generate_plots
+from rat.utils.convert_to_final_outputs import convert_sarea, convert_inflow, convert_dels, convert_evaporation, convert_outflow, convert_altimeter
 
+# Step-(-1): Reading Configuration settings to run RAT
+# Step-0: Creating required directory structure for RAT
 # Step-1: Downloading and Pre-processing of meteorolgical data
 # Step-2: Pre-processing of data and preparation of MetSim Input
 # Step-3: Preparation of MetSim Parameter Files
 # Step-4: Running MetSim & preparation of VIC input
 # Step-5: Preparation of VIC Parameter Files
 # Step-6: Running of VIC and preparation of Routing input
 # Step-7: Preparation of Routing Parameter Files
 # Step-8: Runnning Routing and generating Inflow
 # Step-9: Preparation of parameter files for Surface Area Calculation
 # Step-10: TMS-OS Surface Area Calculation from GEE 
 # Step-11: Elevation extraction from Altimeter
 # Step-12: Generating Area Elevation Curves for reservoirs
 # Step-13: Calculation of Outflow, Evaporation and Storage change
+# Step-14: Conversion of output data to final format as time series
 
-def rat(config, rat_logger, steps=[2,3,5,7,9,12,13,4,6,8,10,11]):
+#TODO: Converting steps to separate modules to make RAT more robust and generalized
+#module-1 step-1,2 data_preparation_vic
+#module-2 step-3to8 inflow_vic
+#module-3 step- NA evaporation
+#module-4 step-10to12 storage_change
+#module-5 step-13 outflow (mass-balance)
+#RAT using all modules and step-14 to produce final outputs
 
-    rat_logger = getLogger('run_rat')
-    ##--------------------- Reading and initialising global parameters ----------------------##
-    # Defining resolution to run RAT
-    xres=0.0625
-    yres=0.0625 
-
-    # Obtaining basin related information from RAT_Runner.yml
-    basins_shapefile_path = config['GLOBAL']['basin_shpfile'] # Shapefile containg information of basin(s)- geometry and attributes
-    basins_shapefile = gpd.read_file(basins_shapefile_path)  # Reading basins_shapefile_path to get basin polygons and their attributes
-    basins_shapefile_column_dict = config['GLOBAL']['basin_shpfile_column_dict'] # Dictionary of column names in basins_shapefile, Must contain 'id' field
-    major_basin_name = config['BASIN']['major_basin_name']  # Major basin name used to cluster multiple basins data in data-directory
-    basin_name = config['BASIN']['basin_name']              # Basin name used to save basin related data
-    basin_id = config['BASIN']['basin_id']                  # Unique identifier for each basin used to map basin polygon in basins_shapefile
-    basin_data = basins_shapefile[basins_shapefile[basins_shapefile_column_dict['id']]==basin_id] # Getting the particular basin related information corresponding to basin_id
-    basin_bounds = basin_data.bounds                          # Obtaining bounds of the particular basin
-    basin_bounds = np.array(basin_bounds)[0]
-    basin_geometry = basin_data.geometry                      # Obtaining geometry of the particular basin
-
-    # Defining paths for RAT processing
-    project_dir = config['GLOBAL']['project_dir']    # Directory of RAT 
-    data_dir = config['GLOBAL']['data_dir']          # Data-Directory of RAT
-    major_basin_data_dir = create_directory(os.path.join(data_dir,major_basin_name), True) # Major Basin data-directory within the data-directory of RAT
-    basin_data_dir = create_directory(os.path.join(major_basin_data_dir,'basins',basin_name), True)  # Basin data-directory within the major basin's data-directory 
-    log_dir = create_directory(os.path.join(major_basin_data_dir,'logs',basin_name,''), True)  # Log directory within the major basin's data-directory
-
-    # Change datetimes format
-    #config['BASIN']['begin'] = datetime.datetime.combine(config['BASIN']['begin'], datetime.time.min)
-    config['BASIN']['start'] = datetime.datetime.combine(config['BASIN']['start'], datetime.time.min)
-    config['BASIN']['end'] = datetime.datetime.combine(config['BASIN']['end'], datetime.time.min)
+def rat_basin(config, rat_logger):
+    """Runs RAT as per configuration defined in `config_fn` for one single basin.
 
-    if(not config['BASIN']['first_run']):
-        config['BASIN']['vic_init_state_date'] = datetime.datetime.combine(config['BASIN']['vic_init_state_date'], datetime.time.min)
+    parameters:
+        config_fn (str): Path to the configuration file for one basin and not for multiple basins. To run rat for multiple basins use run_rat()
     
-    # Changing start date if running RAT for first time for the particular basin to give VIC and MetSim to have their spin off periods
-    if(config['BASIN']['first_run']):
-        user_given_start = config['BASIN']['start']
-        config['BASIN']['start'] = user_given_start-datetime.timedelta(days=800)  # Running RAT for extra 800 days before the user-given start date for VIC to give reliable results starting from user-given start date
-        data_download_start = config['BASIN']['start']-datetime.timedelta(days=90)    # Downloading 90 days of extra meteorological data for MetSim to prepare it's initial state
-        vic_init_state_date = None    # No initial state of VIC is present as running RAT for first time in this basin
+    returns:
+        no_errors (int): Number of errors/exceptions occurred while running rat
+        latest_altimetry_cycle (int): Latest altimetry jason3 cycle number if rat runs step 11
+    """
+    rat_logger = getLogger('run_rat')
+
+    # Tracking number of errors to output
+    no_errors = 0
+
+    # Tracking latest altimetry cycle number if step 11 is run, otherwise return None
+    latest_altimetry_cycle = None
+
+    ######### Step -1 Mandatory Step
+    try:
+        rat_logger.info("Reading Configuration settings to run RAT")
+        ##--------------------- Reading and initialising global parameters ----------------------##
+
+        # Reading steps to be executed in RAT otherwise seting default value
+        if config['GLOBAL'].get('steps'):
+            steps = config['GLOBAL']['steps']
+        else:
+            steps = [1,2,3,4,5,6,7,8,9,10,11,12,13,14]
+
+        # Defining resolution to run RAT
+        xres = 0.0625
+        yres = 0.0625 
+
+        # Obtaining basin related information from RAT_Runner.yml
+        basins_shapefile_path = config['GLOBAL']['basin_shpfile'] # Shapefile containg information of basin(s)- geometry and attributes
+        basins_shapefile = gpd.read_file(basins_shapefile_path)  # Reading basins_shapefile_path to get basin polygons and their attributes
+        basins_shapefile_column_dict = config['GLOBAL']['basin_shpfile_column_dict'] # Dictionary of column names in basins_shapefile, Must contain 'id' field
+        region_name = config['BASIN']['region_name']  # Major basin name used to cluster multiple basins data in data-directory
+        basin_name = config['BASIN']['basin_name']              # Basin name used to save basin related data
+        basin_id = config['BASIN']['basin_id']                  # Unique identifier for each basin used to map basin polygon in basins_shapefile
+        basin_data = basins_shapefile[basins_shapefile[basins_shapefile_column_dict['id']]==basin_id] # Getting the particular basin related information corresponding to basin_id
+        basin_bounds = basin_data.bounds                          # Obtaining bounds of the particular basin
+        basin_bounds = np.array(basin_bounds)[0]
+        basin_geometry = basin_data.geometry                      # Obtaining geometry of the particular basin
+
+        # Defining paths for RAT processing
+        project_dir = config['GLOBAL']['project_dir']    # Directory of RAT 
+        data_dir = config['GLOBAL']['data_dir']          # Data-Directory of RAT
+        region_data_dir = create_directory(os.path.join(data_dir,region_name), True) # Major Basin data-directory within the data-directory of RAT
+        basin_data_dir = create_directory(os.path.join(region_data_dir,'basins',basin_name), True)  # Basin data-directory within the major basin's data-directory 
+        log_dir = create_directory(os.path.join(region_data_dir,'logs',basin_name,''), True)  # Log directory within the major basin's data-directory
+
+        # Change datetimes format
+        #config['BASIN']['begin'] = datetime.datetime.combine(config['BASIN']['begin'], datetime.time.min)
+        config['BASIN']['start'] = datetime.datetime.combine(config['BASIN']['start'], datetime.time.min)
+        config['BASIN']['end'] = datetime.datetime.combine(config['BASIN']['end'], datetime.time.min)
+        rout_init_state_save_date = config['BASIN']['end']
+
+        if(not config['BASIN']['spin_up']):
+            if(config['BASIN'].get('vic_init_state_date')):
+                config['BASIN']['vic_init_state_date'] = datetime.datetime.combine(config['BASIN']['vic_init_state_date'], datetime.time.min)
+        
+        # Changing start date if running RAT for first time for the particular basin to give VIC and MetSim to have their spin off periods
+        if(config['BASIN']['spin_up']):
+            user_given_start = config['BASIN']['start']
+            config['BASIN']['start'] = user_given_start-datetime.timedelta(days=800)  # Running RAT for extra 800 days before the user-given start date for VIC to give reliable results starting from user-given start date
+            data_download_start = config['BASIN']['start']-datetime.timedelta(days=90)    # Downloading 90 days of extra meteorological data for MetSim to prepare it's initial state
+            vic_init_state_date = None    # No initial state of VIC is present as running RAT for first time in this basin
+            use_state = False            # Routing state file won't be used
+        elif(config['BASIN'].get('vic_init_state_date')):
+            data_download_start = config['BASIN']['start']    # Downloading data from the same date as we want to run RAT from
+            vic_init_state_date = config['BASIN']['vic_init_state_date'] # Date of which initial state of VIC for the particular basin exists
+            use_state = True           # Routing state file will be used
+        else:
+            data_download_start = config['BASIN']['start']-datetime.timedelta(days=90)    # Downloading 90 days of extra meteorological data for MetSim to prepare it's initial state
+            vic_init_state_date = None    # No initial state of VIC is present as running RAT for first time in this basin
+            use_state = False            # Routing state file won't be used
+
+        # Defining logger
+        log = init_logger(
+            log_dir= log_dir,
+            verbose= False,
+            # notify= True,
+            notify= False,
+            log_level= 'DEBUG'
+        )
+
+        # Cleaning class object for removing/deleting unwanted data
+        cleaner = Clean(basin_data_dir)
+
+        # Clearing out previous rat outputs so that the new data does not gets appended.
+        if(config['CLEAN_UP']['clean_previous_outputs']):
+            rat_logger.info("Clearing up memory space: Removal of previous rat outputs, routing inflow, extracted altimetry data and gee extracted surface area time series")
+            cleaner.clean_previous_outputs()
+
+        # Initializing Status for different models & tasks (1 for successful run & 0 for failed run)
+        NEW_DATA_STATUS = 1
+        METSIM_STATUS = 1
+        VIC_STATUS = 1
+        ROUTING_STATUS = 1
+        GEE_STATUS = 1
+        ALTIMETER_STATUS = 1
+        DELS_STATUS = 0
+        EVAP_STATUS = 0
+        OUTFLOW_STATUS = 0
+    except:
+        no_errors = -1
+        rat_logger.exception("Error in Configuration parameters defined to run RAT.")
+        return (no_errors, latest_altimetry_cycle)
     else:
-        data_download_start = config['BASIN']['start']    # Downloading data from the same date as we want to run RAT from
-        vic_init_state_date = config['BASIN']['vic_init_state_date'] # Date of which initial state of VIC for the particular basin exists
-    
-    # Defining logger
-    log = init_logger(
-        log_dir= log_dir,
-        verbose= False,
-        # notify= True,
-        notify= False,
-        log_level= 'DEBUG'
-    )
-
-    # Initializing Status for different models & tasks (1 for successful run & 0 for failed run)
-    NEW_DATA_STATUS = 1
-    METSIM_STATUS = 1
-    VIC_STATUS = 1
-    ROUTING_STATUS = 1
-    GEE_STATUS = 1
-    ALTIMETER_STATUS = 1
-    DELS_STATUS = 0
-    EVAP_STATUS = 0
-    OUTFLOW_STATUS = 0
+        rat_logger.info("Read Configuration settings to run RAT.")
+        ##--------------------- Read and initialised global parameters ----------------------##
 
-    ##--------------------- Read and initialised global parameters ----------------------##
+    rat_logger.info(f"Running RAT from {config['BASIN']['start'] } to {config['BASIN']['end']}")
+
+    ######### Step-0 Mandatory Step
+    try:
+        rat_logger.info("Creating required directory structure for RAT")
+        
+        ##--------------------- Defining global paths and variables ----------------------##
+
+        #----------- Paths Necessary for running of METSIM  -----------#
+        # Path of directory which will contain the combined data in nc format.
+        combined_datapath = create_directory(os.path.join(basin_data_dir,'pre_processing','nc', ''), True)
+        combined_datapath = os.path.join(combined_datapath, 'combined_data.nc')
+        # Path where the processed downloaded data is present
+        processed_datadir = os.path.join(basin_data_dir,'pre_processing','processed')
+        # basingrid_file path to clip the global downloaded data
+        basingridfile_path= create_directory(os.path.join(basin_data_dir, 'basin_grid_data',''), True)
+        basingridfile_path= os.path.join(basingridfile_path, basin_name+'_grid_mask.tif')
+        #Creating metsim input directory for basin if not exist
+        metsim_inputs_dir = create_directory(os.path.join(basin_data_dir, 'metsim', 'metsim_inputs', ''),True)
+        #Defining paths for metsim input data, metsim state and metsim domain
+        ms_state = os.path.join(metsim_inputs_dir, 'state.nc')
+        ms_input_data = os.path.join(metsim_inputs_dir,'metsim_input.nc')
+        domain_nc_path = os.path.join(metsim_inputs_dir,'domain.nc')
+        #Creating metsim output directory for basin if not exist
+        metsim_output_path = create_directory(os.path.join(basin_data_dir, 'metsim', 'metsim_outputs',''), True)
+        #Creating vic input directory for basin if not exist
+        vic_input_path = create_directory(os.path.join(basin_data_dir, 'vic', 'vic_inputs',''), True)
+        #----------- Paths Necessary for running of METSIM  -----------#
+
+        #----------- Paths Necessary for running of VIC  -----------#
+        vic_input_forcing_path = os.path.join(vic_input_path,'forcing_')
+        vic_output_path = create_directory(os.path.join(basin_data_dir,'vic','vic_outputs',''), True)
+        rout_input_path = create_directory(os.path.join(basin_data_dir,'ro','in',''), True)
+        rout_input_state_folder = create_directory(os.path.join(basin_data_dir,'ro','rout_state_file',''), True)
+        rout_input_state_file = os.path.join(rout_input_state_folder,'ro_init_state_file_'+config['BASIN']['start'].strftime("%Y-%m-%d")+'.nc')
+        rout_init_state_save_file = os.path.join(rout_input_state_folder,'ro_init_state_file_'+rout_init_state_save_date.strftime("%Y-%m-%d")+'.nc')
+        #----------- Paths Necessary for running of VIC  -----------#
+
+        #----------- Paths Necessary for running of Routing  -----------#
+        # Routing_input files prefix path
+        rout_input_path_prefix = os.path.join(rout_input_path,'fluxes_')
+        # Creating routing parameter directory
+        rout_param_dir = create_directory(os.path.join(basin_data_dir,'ro','pars',''), True)
+        # Defining path and name for basin flow direction file
+        basin_flow_dir_file = os.path.join(rout_param_dir,'fl.asc')
+        # Defining Basin station latlon file path
+        if (config['ROUTING']['station_global_data']):
+            basin_station_latlon_file = os.path.join(rout_param_dir,'basin_station_latlon.csv')
+        else:
+            basin_station_latlon_file = config['ROUTING']['station_latlon_path']
+        # Creating routing inflow directory
+        rout_inflow_dir = create_directory(os.path.join(basin_data_dir,'ro', 'rout_inflow',''), True)
+        #----------- Paths Necessary for running of Routing  -----------#
+
+        #----------- Paths Necessary for running of Surface Area Calculation and Altimetry-----------#
+        # Defining routing station file
+        if(config['ROUTING PARAMETERS'].get('station_file')):
+            basin_station_xy_path = config['ROUTING PARAMETERS'].get('station_file')
+        else:
+            basin_station_xy_path = os.path.join(basin_data_dir,'ro', 'pars','sta_xy.txt')
+        # Defining path for basin reservoir shapefile
+        basin_reservoir_shpfile_path = create_directory(os.path.join(basin_data_dir,'gee','gee_basin_params',''), True)
+        basin_reservoir_shpfile_path = os.path.join(basin_reservoir_shpfile_path,'basin_reservoirs.shp')
+        # Reading dictionary of column values for reservoir shapefile path
+        reservoirs_gdf_column_dict = config['GEE']['reservoir_vector_file_columns_dict']
+        # Adding key-value pair to Basin Reservoir Shapefile's column dictionary ### 
+        if (config['ROUTING']['station_global_data']):
+            reservoirs_gdf_column_dict['unique_identifier'] = 'uniq_id'
+        else:
+            reservoirs_gdf_column_dict['unique_identifier'] = reservoirs_gdf_column_dict['dam_name_column']
+        # Defining paths to save surface area from gee and heights from altimetry
+        sarea_savepath = create_directory(os.path.join(basin_data_dir,'gee','gee_sarea_tmsos',''), True)
+        altimetry_savepath = os.path.join(basin_data_dir,'altimetry','altimetry_timeseries')
+        #----------- Paths Necessary for running of Surface Area Calculation and Altimetry-----------#
+
+        #----------- Paths Necessary for running of Post-Processing-----------#
+        # Defining path for the Area Elevation curve
+        if (config['POST_PROCESSING'].get('aec_dir')):
+            aec_dir_path = config['POST_PROCESSING'].get('aec_dir')
+        else:
+            aec_dir_path = create_directory(os.path.join(basin_data_dir,'post_processing','post_processing_gee_aec',''), True)
+        ## Paths for storing post-processed data and in webformat data
+        evap_savedir = create_directory(os.path.join(basin_data_dir,'rat_outputs', "Evaporation"), True)
+        dels_savedir = create_directory(os.path.join(basin_data_dir,'rat_outputs', "dels"), True)
+        outflow_savedir = create_directory(os.path.join(basin_data_dir,'rat_outputs', "rat_outflow"),True)
+        final_output_path = create_directory(os.path.join(basin_data_dir,'final_outputs',''),True)
+        ## End of defining paths for storing post-processed data and webformat data
+        #----------- Paths Necessary for running of Post-Processing-----------#
+    except:
+        no_errors = -1
+        rat_logger.exception("Error in creating required directory structure for RAT")
+        return (no_errors, latest_altimetry_cycle)
+    else:
+        rat_logger.info("Finished creating required directory structure for RAT")
+        ##--------------------- Definied global paths and variables ----------------------##
 
-    rat_logger.info(f"Running RAT from {config['BASIN']['start']} to {config['BASIN']['end']}")
-    
     ######### Step-1
     if(1 in steps):
         try:
             rat_logger.info("Starting Step-1: Downloading and Pre-processing of meteorological data")
             ##----------------------- Downloading meteorological data ------------------------##
             ##--------- Download Data Begin ----------#
             get_newdata(
@@ -143,89 +280,74 @@
                 secrets_file= config['CONFIDENTIAL']['secrets'],
                 download= True,
                 process= True
             )
             ##---------- Download Data End -----------# 
             NEW_DATA_STATUS = 1   #Data downloaded successfully
         except:
+            no_errors = no_errors+1
             rat_logger.exception("Error Executing Step-1: Downloading and Pre-processing of meteorological data")
         else:
             rat_logger.info("Finished Step-1: Downloading and Pre-processing of meteorological data")
             ##----------------------- Downloaded meteorological data ------------------------##
 
 
     ######### Step-2
     if(2 in steps):
         try:
             rat_logger.info("Starting Step-2: Pre-processing of data and preparation of MetSim Input")
             ##----------------------- Pre-processing step for METSIM ------------------------##
-            #----------- Paths Necessary for creating METSIM Input Data  -----------#
-            # Path of directory which will contain the combined data in nc format.
-            combined_datapath = create_directory(os.path.join(basin_data_dir, 'nc', ''), True)
-            combined_datapath = os.path.join(combined_datapath, 'combined_data.nc')
-
-            # Path where the processed downloaded data is present
-            processed_datadir = os.path.join(basin_data_dir, 'processed')
-
-            # basingrid_file path to clip the global downloaded data
-            basingridfile_path= create_directory(os.path.join(basin_data_dir, 'basin_grid_data',''), True)
-            basingridfile_path= os.path.join(basingridfile_path, basin_name+'_grid_mask.tif')
-
+            #----------- Files Necessary for creating METSIM Input Data  -----------#
             # Creating basinggrid_file if not exists
             if not os.path.exists(basingridfile_path):
                 create_basingridfile(basin_bounds,basin_geometry,basingridfile_path,xres,yres)
-            #----------- Created Paths Necessary for creating METSIM Input Data  -----------#
+            #----------- Created Files Necessary for creating METSIM Input Data  -----------#
 
             #----------- Process Data Begin to combine all var data -----------#
             CombinedNC(
                 start= data_download_start,
                 end= config['BASIN']['end'],
                 datadir= processed_datadir,
                 basingridpath= basingridfile_path,
-                outputdir= combined_datapath
+                outputdir= combined_datapath,
+                use_previous= use_state,
             )
             #----------- Process Data End and combined data created -----------#
 
             #------ MetSim Input Data Preparation Begin ------#
             # Prepare data to metsim input format
-            metsim_inputs_dir = create_directory(os.path.join(basin_data_dir, 'metsim', 'metsim_inputs', ''),True)
-
             ms_state, ms_input_data = generate_state_and_inputs(
                 forcings_startdate= config['BASIN']['start'],
                 forcings_enddate= config['BASIN']['end'],
                 combined_datapath= combined_datapath, 
                 out_dir= metsim_inputs_dir
             )
             #------- MetSim Input Data Preparation End -------#
-
-            #---------- Creating metsim output directory for basin if not exist---------#
-            metsim_output_path = create_directory(os.path.join(basin_data_dir, 'metsim', 'metsim_outputs',''), True)
-            #----------metsim output directory created for basin if not exist---------#
-
-            #---------- Creating vic input directory for basin if not exist---------#
-            vic_input_path = create_directory(os.path.join(basin_data_dir, 'vic', 'vic_inputs',''), True)
-            #----------vic input directory created for basin if not exist---------#
         except:
+            no_errors = no_errors+1
             rat_logger.exception("Error Executing Step-2: Pre-processing of data and preparation of MetSim Input")
         else:
             rat_logger.info("Finished Step-2: Pre-processing of data and preparation of MetSim Input")
             ##----------------------- Pre-processing step finished for METSIM ------------------------##
 
     ######### Step-3
     if(3 in steps):
         try:
             rat_logger.info("Starting Step-3: Preparation of MetSim Parameter Files")
             ##----------------------- Preparing parameter files for METSIM ------------------------##
             ## ---------- Creating domain.nc file for basin if not exist---------#
-            domain_nc_path = os.path.join(metsim_inputs_dir,'domain.nc')
-            if not os.path.exists(domain_nc_path):
-                elevation_tif_filepath = config['GLOBAL']['elevation_tif_file']
-                create_basin_domain_nc_file(elevation_tif_filepath,basingridfile_path,domain_nc_path)
+            if(config['GLOBAL'].get('elevation_tif_file')):
+                if not os.path.exists(domain_nc_path):
+                    elevation_tif_filepath = config['GLOBAL']['elevation_tif_file']
+                    create_basin_domain_nc_file(elevation_tif_filepath,basingridfile_path,domain_nc_path)
+            else:
+                domain_nc_path = config['METSIM']['metsim_domain_file']
             #----------domain.nc file created for basin if not exist ---------#
         except:
+            no_errors = no_errors+1
             rat_logger.exception("Error Executing Step-3: Preparation of MetSim Parameter Files")
         else:
             rat_logger.info("Finished Step-3: Preparation of MetSim Parameter Files")
             ##----------------------- Prepared parameter files for METSIM ------------------------##
 
     ######### Step-4
     if(4 in steps):
@@ -252,14 +374,15 @@
                     log.log(NOTIFICATION, f'Starting metsim from {config["BASIN"]["start"].strftime("%Y-%m-%d")} to {config["BASIN"]["end"].strftime("%Y-%m-%d")}')
                     ms.run_metsim()
                     ms.convert_to_vic_forcings(vic_input_path)
                 METSIM_STATUS=1    #Metsim run successfully
             else:
                 rat_logger.info("New Data Download Failed. Skipping Step-4: Running MetSim & preparation of VIC input")
         except:
+            no_errors = no_errors+1
             rat_logger.exception("Error Executing Step-4: Running MetSim & preparation of VIC input")
         else:
             rat_logger.info("Finished Step-4: Running MetSim & preparation of VIC input")
             ##--------------- Metsim End & Pre-processing for VIC done--------------##
 
 
      ######### Step-5
@@ -279,21 +402,16 @@
                     global_vic_domain_file = os.path.join(config['VIC']['vic_global_param_dir'],config['VIC']['vic_basin_continent_domain_filename'])
 
                     create_vic_domain_param_file(global_vic_param_file,global_vic_domain_file,basingridfile_path,vic_param_dir)
                 
                 # Setting vic soil_param_file and domain file paths in config, will be used in vic_params produced by VICParameterFile
                 config['VIC']['vic_soil_param_file']=os.path.join(vic_param_dir,'vic_soil_param.nc')
                 config['VIC']['vic_domain_file']=os.path.join(vic_param_dir,'vic_domain.nc')
-
-            vic_input_forcing_path = os.path.join(vic_input_path,'forcing_')
-            vic_output_path = create_directory(os.path.join(basin_data_dir,'vic','vic_outputs',''), True)
-            rout_input_path = create_directory(os.path.join(basin_data_dir,'routing','rout_inputs',''), True)
-            rout_input_state_file = create_directory(os.path.join(basin_data_dir,'routing','rout_state_file',''), True)
-            rout_input_state_file = os.path.join(rout_input_state_file,'combined_input_state_file.nc')
         except:
+            no_errors = no_errors+1
             rat_logger.exception("Error Executing Step-5: Preparation of VIC Parameter Files")
         else:
             rat_logger.info("Finished Step-5: Preparation of VIC Parameter Files")
             ##--------------- Preparation of Vic Parameter Files end--------------##
     
     ######### Step-6
     if(6 in steps):
@@ -313,79 +431,78 @@
                     vic = VICRunner(
                         vic_env= config['VIC']['vic_env'],
                         param_file= p.vic_param_path,
                         vic_result_file= p.vic_result_file,
                         rout_input_dir= rout_input_path
                     )
                     vic.run_vic(np=config['GLOBAL']['multiprocessing'])
-                    vic.generate_routing_input_state(ndays=365, rout_input_state_file=rout_input_state_file)
-                    if(config['BASIN']['first_run']):
-                        vic.disagg_results(rout_input_state_file=p.vic_result_file)       # If first run, use vic result file
+                    vic.generate_routing_input_state(ndays=365, rout_input_state_file=rout_input_state_file, 
+                                                                                        save_path=rout_init_state_save_file, use_rout_state=use_state) # Start date of routing state file will be returned
+                    if(config['BASIN']['spin_up']):
+                        vic.disagg_results(rout_input_state_file=p.vic_result_file)       # If spin_up, use vic result file
+                    elif(config['BASIN'].get('vic_init_state_date')):                      # If vic_state file exists
+                        vic.disagg_results(rout_input_state_file=rout_init_state_save_file)    # If not spin_up, use rout_init_state_save file just creates as it contains the recent vic outputs.
                     else:
-                        vic.disagg_results(rout_input_state_file=rout_input_state_file)    # If not first run, use rout input state file
+                        vic.disagg_results(rout_input_state_file=p.vic_result_file)       # If spin_up is false and vic state file does not exist, use vic result file
                     vic_startdate = p.vic_startdate
                     vic_enddate = p.vic_enddate
                 VIC_STATUS=1         #Vic run successfully
             else:
                 rat_logger.info("MetSim Run Failed. Skipping Step-6: Running of VIC and preparation of Routing input")
         except:
+            no_errors = no_errors+1
             rat_logger.exception("Error Executing Step-6: Running of VIC and preparation of Routing input")
         else:
             rat_logger.info("Finished Step-6: Running of VIC and preparation of Routing input")
             ##---------------- VIC End & Results pre-processed for Routing-----------------##
 
 
     ######### Step-7
     if(7 in steps):
         try:    
             rat_logger.info("Starting Step-7: Preparation of Routing Parameter Files")
             ##--------------- Preparation of Routing Parameter Files begin--------------##
-            # Routing_input files prefix path
-            rout_input_path_prefix = os.path.join(rout_input_path,'fluxes_')
-
-            # Creating routing parameter directory
-            rout_param_dir = create_directory(os.path.join(basin_data_dir,'routing','rout_basin_params',''), True)
-
             ### Basin Grid Flow Firection File
-            # Defining path and name for basin flow direction file
-            basin_flow_dir_file = os.path.join(rout_param_dir,'basin_flow_dir')
             # Creating basin grid flow diretion file if not present
             if (config['ROUTING'].get('global_flow_dir_tif_file')):
-                if not os.path.exists(basin_flow_dir_file+'.asc'):
-                    create_basin_grid_flow_asc(config['ROUTING']['global_flow_dir_tif_file'], basingridfile_path, basin_flow_dir_file,
+                if not os.path.exists(basin_flow_dir_file):
+                    create_basin_grid_flow_asc(config['ROUTING']['global_flow_dir_tif_file'], basingridfile_path, basin_flow_dir_file[:-4],
                                                                     config['ROUTING'].get('replace_flow_directions'))
-            basin_flow_dir_file = basin_flow_dir_file+'.asc'
-
             ### Basin Station File
-            basin_station_latlon_file = os.path.join(rout_param_dir,'basin_station_latlon.csv')
             if (config['ROUTING']['station_global_data']):
                 if not os.path.exists(basin_station_latlon_file):
-                    create_basin_station_latlon_csv(basin_name, config['ROUTING']['stations_vector_file'], basin_data, 
+                    create_basin_station_latlon_csv(region_name,basin_name, config['ROUTING']['stations_vector_file'], basin_data, 
                                                         config['ROUTING']['stations_vector_file_columns_dict'], basin_station_latlon_file)
-            else:
-                basin_station_latlon_file = config['ROUTING']['station_latlon_path']
-
-            # Creating routing inflow directory
-            rout_inflow_dir = create_directory(os.path.join(basin_data_dir,'routing', 'rout_inflow',''), True)
         except:
+            no_errors = no_errors+1
             rat_logger.exception("Error Executing Step-7: Preparation of Routing Parameter Files")
         else:    
             rat_logger.info("Finished Step-7: Preparation of Routing Parameter Files")
             ##--------------- Preparation of Routing Parameter Files end--------------##
 
     ######### Step-8
     if(8 in steps):
         try:
             if(VIC_STATUS):
                 rat_logger.info("Starting Step-8: Runnning Routing and generating Inflow")
+                ### Extracting routing start date ###
+                if(config['BASIN']['spin_up']):
+                    rout_input_state_start_date = config['BASIN']['start']
+                elif(config['BASIN'].get('vic_init_state_date')): 
+                    rout_state_data = xr.open_dataset(rout_init_state_save_file).load()
+                    rout_input_state_start_date = rout_state_data.time[0].values.astype('datetime64[us]').astype(datetime.datetime)
+                    rout_state_data.close()
+                else:
+                    rout_input_state_start_date = config['BASIN']['start']
+                ### Extracted routing start date ###
                 #------------- Routing Begins and Pre processing for Mass Balance --------------#
                 with RouteParameterFile(
                     config = config,
                     basin_name = basin_name,
-                    start = config['BASIN']['start'],
+                    start = rout_input_state_start_date,
                     end = config['BASIN']['end'],
                     basin_flow_direction_file = basin_flow_dir_file,
                     clean=False,
                     rout_input_path_prefix = rout_input_path_prefix
                     ) as r:
                     route = RoutingRunner(    
                         project_dir = config['GLOBAL']['project_dir'], 
@@ -401,154 +518,173 @@
                     route.run_routing()
                     route.generate_inflow()
                     basin_station_xy_path = route.station_path_xy
                 ROUTING_STATUS=1
             else:
                 rat_logger.info("VIC Run Failed. Skipping Step-8: Runnning Routing and generating Inflow")
         except:
+            no_errors = no_errors+1
             rat_logger.exception("Error Executing Step-8: Runnning Routing and generating Inflow")
         else:
             rat_logger.info("Finished Step-8: Runnning Routing and generating Inflow")
             #------------- Routing Ends and Inflow pre-processed for Mass Balance --------------#
 
     ######### Step-9
     if(9 in steps):
         try:
             rat_logger.info("Starting Step-9: Preparation of parameter files for Surface Area Calculation")
             #------------- Selection of Reservoirs within the basin begins--------------#
             ###### Preparing basin's reservoir shapefile and it's associated column dictionary for calculating surface area #####
             ### Creating Basin Reservoir Shapefile, if not exists ###
-            reservoirs_gdf_column_dict = config['GEE']['reservoir_vector_file_columns_dict']
-
-            basin_reservoir_shpfile_path = create_directory(os.path.join(basin_data_dir,'gee','gee_basin_params',''), True)
-            basin_reservoir_shpfile_path = os.path.join(basin_reservoir_shpfile_path,'basin_reservoirs.shp')
             if not os.path.exists(basin_reservoir_shpfile_path):
-                create_basin_reservoir_shpfile(config['GEE']['reservoir_vector_file'], reservoirs_gdf_column_dict, basin_station_xy_path,
+                if os.path.exists(basin_station_xy_path):
+                    create_basin_reservoir_shpfile(config['GEE']['reservoir_vector_file'], reservoirs_gdf_column_dict, basin_station_xy_path,
                                                                                 config['ROUTING']['station_global_data'], basin_reservoir_shpfile_path)
-            ### Creating Basin Reservoir Shapefile's column dictionary ### 
-            if (config['ROUTING']['station_global_data']):
-                reservoirs_gdf_column_dict['unique_identifier'] = 'uniq_id'
-            else:
-                reservoirs_gdf_column_dict['unique_identifier'] = reservoirs_gdf_column_dict['dam_name_column']
-            ### Defining paths to save surface area from gee and heights from altimetry
-            sarea_savepath = create_directory(os.path.join(basin_data_dir,'gee','gee_sarea_tmsos',''), True)
-            altimetry_savepath = os.path.join(basin_data_dir,'altimetry','altimetry_timeseries')
-            
             ###### Prepared basin's reservoir shapefile and it's associated column dictionary #####
         except:
+            no_errors = no_errors+1
             rat_logger.exception("Error Executing Step-9: Preparation of parameter files for Surface Area Calculation")
         else:
             rat_logger.info("Finished Step-9: Preparation of parameter files for Surface Area Calculation")
             #------------- Selection of Reservoirs within the basin ends--------------#
 
     ######### Step-10
     if(10 in steps):
         try:
+            from rat.core.run_sarea import run_sarea
             rat_logger.info("Starting Step-10: TMS-OS Surface Area Calculation from GEE")
             ##----------- Remote Sensing to estimate surface area begins -----------##
+            if (not os.path.exists(basin_reservoir_shpfile_path)):
+                if (not config['ROUTING']['station_global_data']):
+                    basin_reservoir_shpfile_path = config['GEE']['reservoir_vector_file']
+                else: 
+                    raise Exception('There was an error in creating reservoir shapefile using spatial join for this basin from the global reservoir vector file.')
             # Get Sarea
             run_sarea(config['BASIN']['start'].strftime("%Y-%m-%d"), config['BASIN']['end'].strftime("%Y-%m-%d"), sarea_savepath, 
                                                                                     basin_reservoir_shpfile_path, reservoirs_gdf_column_dict)
             GEE_STATUS = 1
         except:
+            no_errors = no_errors+1
             rat_logger.exception("Error Executing Step-10: TMS-OS Surface Area Calculation from GEE")
         else:
             rat_logger.info("Finished Step-10: TMS-OS Surface Area Calculation from GEE")                                                                        
             ##----------- Remote Sensing to estimate surface area ends -----------##
     
     ######### Step-11
     if(11 in steps):
         try:
             rat_logger.info("Starting Step-11: Elevation extraction from Altimeter")
-            ##----------- Altimeter height ectraction begins -----------##
+            ##----------- Altimeter height extraction begins -----------##
             # Altimeter
             latest_altimetry_cycle = run_altimetry(config, 'ALTIMETER', basin_reservoir_shpfile_path, reservoirs_gdf_column_dict, 
                                                                                     basin_name, basin_data_dir, altimetry_savepath)
             ALTIMETER_STATUS = 1
         except:
+            no_errors = no_errors+1
             rat_logger.exception("Error Executing Step-11: Elevation extraction from Altimeter")
         else:
             rat_logger.info("Finished Step-11: Elevation extraction from Altimeter")                                                                        
-            ##----------- Altimeter height ectraction ends -----------##
+            ##----------- Altimeter height extraction ends -----------##
 
     ######### Step-12
     if(12 in steps):
         try:
+            from rat.ee_utils.ee_aec_file_creator import aec_file_creator
             rat_logger.info("Starting Step-12: Generating Area Elevation Curves for reservoirs")
             ##--------------------------------Area Elevation Curves Extraction begins ------------------- ##
             ## Creating AEC files if not present for post-processing dels calculation
-            if (config['POST_PROCESSING'].get('aec_dir')):
-                aec_dir_path = config['POST_PROCESSING'].get('aec_dir')
-            else:
-                aec_dir_path = create_directory(os.path.join(basin_data_dir,'post_processing','post_processing_gee_aec',''), True)
             aec_file_creator(basin_reservoir_shpfile_path,reservoirs_gdf_column_dict,aec_dir_path)
-
-            ## Paths for storing post-processed data and in webformat data
-            evap_savedir = create_directory(os.path.join(basin_data_dir,'rat_outputs', "Evaporation"), True)
-            dels_savedir = create_directory(os.path.join(basin_data_dir,'rat_outputs', "dels"), True)
-            outflow_savedir = create_directory(os.path.join(basin_data_dir,'rat_outputs', "rat_outflow"),True)
-            web_dir_path = create_directory(os.path.join(basin_data_dir,'web_format_data',''),True)
-            ## End of defining paths for storing post-processed data and webformat data
         except:
             rat_logger.exception("Finished Step-12: Generating Area Elevation Curves for reservoirs")
         else:
             rat_logger.info("Finished Step-12: Generating Area Elevation Curves for reservoirs")
             ##--------------------------------Area Elevation Curves Extraction ends ------------------- ##
 
     ######### Step-13
     if(13 in steps):
         try:
             rat_logger.info("Starting Step-13: Calculation of Outflow, Evaporation and Storage change")
             
-            ##---------- Mass-balance Approach begins and then post-processing ----------##
+            ##---------- Mass-balance Approach begins and then post-processing ----------## 
             DELS_STATUS, EVAP_STATUS, OUTFLOW_STATUS = run_postprocessing(basin_name, basin_data_dir, basin_reservoir_shpfile_path, reservoirs_gdf_column_dict,
-                                aec_dir_path, config['BASIN']['start'], config['BASIN']['end'], evap_savedir, dels_savedir, outflow_savedir, VIC_STATUS, ROUTING_STATUS, GEE_STATUS)
+                                aec_dir_path, config['BASIN']['start'], config['BASIN']['end'], rout_init_state_save_file, use_state, evap_savedir, dels_savedir, outflow_savedir, VIC_STATUS, ROUTING_STATUS, GEE_STATUS)
 
-            # Convert to format that is expected by the website and save in web_dir
+        except:
+            no_errors = no_errors+1
+            rat_logger.exception("Error Executing Step-13: Calculation of Outflow, Evaporation and Storage change")
+        else:
+            rat_logger.info("Finished Step-13: Calculation of Outflow, Evaporation and Storage change")
+            ##---------- Mass-balance Approach ends and then post-processed outputs to obtain timeseries  -----------------##
+    
+    ######### Step-14
+    if(14 in steps):
+        try:
+            rat_logger.info("Starting Step-14: Creating final outputs in a timeseries format and cleaning up.")
+
+            ##---------- Convert all time-series to final output csv format and clean up----------## 
             ## Surface Area
             if(GEE_STATUS):
-                convert_sarea(sarea_savepath,web_dir_path)
+                convert_sarea(sarea_savepath,final_output_path)
                 rat_logger.info("Converted Surface Area to the Output Format.")
             else:
                 rat_logger.info("Could not convert Surface Area to the Output Format as GEE run failed.")
             
             ## Inflow
             if(ROUTING_STATUS):
-                convert_inflow(rout_inflow_dir, basin_reservoir_shpfile_path, reservoirs_gdf_column_dict, web_dir_path)
+                convert_inflow(rout_inflow_dir, basin_reservoir_shpfile_path, reservoirs_gdf_column_dict, final_output_path)
                 rat_logger.info("Converted Inflow to the Output Format.")
             else:
                 rat_logger.info("Could not convert Inflow to the Output Format as Routing run failed.")
             
             ## Dels 
             if(DELS_STATUS):
-                convert_dels(dels_savedir, web_dir_path)
+                convert_dels(dels_savedir, final_output_path)
                 rat_logger.info("Converted ∆S to the Output Format.")
             else:
                 rat_logger.info("Could not convert ∆S to the Output Format as GEE run failed.")
             
             ## Evaporation
             if(EVAP_STATUS):
-                convert_evaporation(evap_savedir, web_dir_path)
+                convert_evaporation(evap_savedir, final_output_path)
                 rat_logger.info("Converted Evaporation to the Output Format.")
             else:
                 rat_logger.info("Could not convert Evaporation to the Output Format as either GEE or VIC run failed.")
 
             ## Outflow
             if(OUTFLOW_STATUS):
-                convert_outflow(outflow_savedir, web_dir_path)
+                convert_outflow(outflow_savedir, final_output_path)
                 rat_logger.info("Converted Outflow to the Output Format.")
             else:
                 rat_logger.info("Could not convert Outflow to the Output Format as either GEE or Routing run failed resulting in failure of calculation of either Inflow, ∆S or Evaporation.")
             
             ## Altimeter
             if(ALTIMETER_STATUS):
-                convert_altimeter(altimetry_savepath, web_dir_path)
+                convert_altimeter(altimetry_savepath, final_output_path)
                 rat_logger.info("Converted Extracted Height from Altimeter to the Output Format.")
             else:
                 rat_logger.info("Could not convert Extracted Height from Altimeter to the Output Format as Altimeter Run failed.")
+            
+            # Clearing out memory space as per user input 
+            if(config['CLEAN_UP'].get('clean_metsim')):
+                rat_logger.info("Clearing up memory space: Removal of metsim output files")
+                cleaner.clean_metsim()
+            if(config['CLEAN_UP'].get('clean_vic')):
+                rat_logger.info("Clearing up memory space: Removal of vic input, output files and previous init_state_files")
+                cleaner.clean_vic()
+            if(config['CLEAN_UP'].get('clean_routing')):
+                rat_logger.info("Clearing up memory space: Removal of routing input and output files")
+                cleaner.clean_routing()
+            if(config['CLEAN_UP'].get('clean_gee')):
+                rat_logger.info("Clearing up memory space: Removal of unwanted gee extracted small chunk files")
+                cleaner.clean_gee()
+            if(config['CLEAN_UP'].get('clean_altimetry')):
+                rat_logger.info("Clearing up memory space: Removal of raw altimetry downloaded data files.")
+                cleaner.clean_altimetry()
         except:
-            rat_logger.exception("Error Executing Step-13: Calculation of Outflow, Evaporation and Storage change")
+            no_errors = no_errors+1
+            rat_logger.exception("Error Executing Step-14: Creating final outputs in a timeseries format and cleaning up.")
         else:
-            rat_logger.info("Finished Step-13: Calculation of Outflow, Evaporation and Storage change")
-            ##---------- Mass-balance Approach ends and then post-processed outputs to obtain timeseries  -----------------##
+            rat_logger.info("Finished Step-14: Creating final outputs in a timeseries format and cleaning up.")
+            ##----------Converted all time-series to final output csv format and cleaned up----------## 
 
-    close_logger()
+    close_logger()
+    return (no_errors, latest_altimetry_cycle)
```

### Comparing `rat-2.1/src/rat/utils/convert_for_website.py` & `rat-3.0.0a4/src/rat/utils/convert_to_final_outputs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import os
-import datetime
 import pandas as pd
 import geopandas as gpd
 import numpy as np
-from utils.utils import create_directory
+from rat.utils.utils import create_directory
 
 def convert_sarea(sarea_dir, website_v_dir):
     # Surface Area
     sarea_paths = [os.path.join(sarea_dir, f) for f in os.listdir(sarea_dir) if f.endswith(".csv")]
-    sarea_web_dir = create_directory(os.path.join(website_v_dir,'sarea' ),True)
+    sarea_web_dir = create_directory(os.path.join(website_v_dir,'sarea_tmsos' ),True)
     for sarea_path in sarea_paths:
         res_name = os.path.splitext(os.path.split(sarea_path)[-1])[0]
 
         
-        savepath = os.path.join(sarea_web_dir, f"{res_name}.txt")
+        savepath = os.path.join(sarea_web_dir, f"{res_name}.csv")
 
         df = pd.read_csv(sarea_path, parse_dates=['date'])
         df = df[['date', 'area']]
         df['area'] = np.round(df['area'], 3)
         df.rename({'area':'area (km2)'}, axis=1, inplace=True)
         print(f"Converting [Surface Area]: {res_name}")
         df.to_csv(savepath, index=False)
@@ -32,15 +31,15 @@
     inflow_web_dir = create_directory(os.path.join(website_v_dir,'inflow' ),True)
 
     for inflow_path in inflow_paths:
         res_name = os.path.splitext(os.path.split(inflow_path)[-1])[0]
 
         if res_name in reservoirs['Inflow_filename'].tolist():
             savename = reservoirs[reservoirs['Inflow_filename'] == res_name][reservoir_shpfile_column_dict['unique_identifier']].values[0]
-            savepath = os.path.join(inflow_web_dir ,f"{savename}.txt")
+            savepath = os.path.join(inflow_web_dir ,f"{savename}.csv")
 
             df = pd.read_csv(inflow_path, parse_dates=['date'])
             df['inflow (m3/d)'] = df['streamflow'] * (24*60*60)        # indicate units, convert from m3/s to m3/d
             df = df[['date', 'inflow (m3/d)']]
 
             print(f"Converting [Inflow]: {res_name}")
             df.to_csv(savepath, index=False)
@@ -53,15 +52,15 @@
     dels_paths = [os.path.join(dels_dir, f) for f in os.listdir(dels_dir) if f.endswith(".csv")]
     dels_web_dir = create_directory(os.path.join(website_v_dir,'dels' ),True)
 
     for dels_path in dels_paths:
         res_name = os.path.splitext(os.path.split(dels_path)[-1])[0]
         savename = res_name
 
-        savepath = os.path.join(dels_web_dir , f"{savename}.txt")
+        savepath = os.path.join(dels_web_dir , f"{savename}.csv")
 
         df = pd.read_csv(dels_path, parse_dates=['date'])[['date', 'dS', 'days_passed']]
         df['dS (m3)'] = df['dS'] * 1e9                                     # indicate units, convert from BCM to m3
         df = df[['date', 'dS (m3)']]
 
         print(f"Converting [∆S]: {res_name}, {savepath}")
         df.to_csv(savepath, index=False)
@@ -71,15 +70,15 @@
     evap_paths = [os.path.join(evap_dir, f) for f in os.listdir(evap_dir) if f.endswith(".csv")]
     evap_web_dir = create_directory(os.path.join(website_v_dir,'evaporation' ),True)
 
     for evap_path in evap_paths:
         res_name = os.path.splitext(os.path.split(evap_path)[-1])[0]
         savename = res_name
 
-        savepath = os.path.join(evap_web_dir , f"{savename}.txt")
+        savepath = os.path.join(evap_web_dir , f"{savename}.csv")
 
         df = pd.read_csv(evap_path)
         df = df[['time', 'OUT_EVAP']]
         df.rename({'time':'date', 'OUT_EVAP':'evaporation (mm)'}, axis=1, inplace=True)
 
         print(f"Converting [Evaporation]: {res_name}, {savepath}")
         df.to_csv(savepath, index=False)
@@ -90,15 +89,15 @@
     outflow_web_dir = create_directory(os.path.join(website_v_dir,'outflow' ),True)
 
     for outflow_path in outflow_paths:
         res_name = os.path.splitext(os.path.split(outflow_path)[-1])[0]
 
         savename = res_name
 
-        savepath = os.path.join(outflow_web_dir, f"{savename}.txt")
+        savepath = os.path.join(outflow_web_dir, f"{savename}.csv")
 
         df = pd.read_csv(outflow_path, parse_dates=['date'])[['date', 'outflow_rate']]
         df.loc[df['outflow_rate']<0, 'outflow_rate'] = 0
         df['outflow (m3/d)'] = df['outflow_rate'] * (24*60*60)        # indicate units, convert from m3/s to m3/d
         df = df[['date', 'outflow (m3/d)']]
 
         print(f"Converting [Outflow]: {res_name}, {savepath}")
@@ -109,15 +108,15 @@
     if os.path.exists(altimeter_ts_dir):
         altimeter_tses = [os.path.join(altimeter_ts_dir, f) for f in os.listdir(altimeter_ts_dir) if f.endswith(".csv")]
         altimeter_web_dir = create_directory(os.path.join(website_v_dir,'altimeter' ),True)
 
         for altimeter_ts_path in altimeter_tses:
             res_name = os.path.splitext(os.path.split(altimeter_ts_path)[-1])[0]
             savename = res_name
-            savepath = os.path.join(altimeter_web_dir , f"{savename}.txt")
+            savepath = os.path.join(altimeter_web_dir , f"{savename}.csv")
 
             df = pd.read_csv(altimeter_ts_path, parse_dates=['date'])
             df = df[['date', 'H [m w.r.t. EGM2008 Geoid]']]
             df['date'] = df['date'].dt.strftime("%Y-%m-%d")
             df['H [m w.r.t. EGM2008 Geoid]'] = np.round(df['H [m w.r.t. EGM2008 Geoid]'], 2)
             df.rename({'H [m w.r.t. EGM2008 Geoid]':'height (m)'}, axis=1, inplace=True)
```

### Comparing `rat-2.1/src/rat/utils/files_creator.py` & `rat-3.0.0a4/src/rat/utils/files_creator.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import xarray as xr
 import rioxarray as rxr
 import rasterio
 from shapely.geometry import mapping
 import geopandas as gpd
 import pandas as pd
 
-from utils.utils import round_pixels,round_up
-from utils.run_command import run_command
+from rat.utils.utils import round_pixels,round_up
+from rat.utils.run_command import run_command
 
 
 def create_basingridfile(basin_bounds,basin_geometry,basingridfile_path,xres,yres):    
     xmin,ymin,xmax,ymax=basin_bounds
     nx=round_pixels((xmax-xmin)/xres)
     ny=round_pixels((ymax-ymin)/yres)
     Z=np.ones((ny,nx))
@@ -90,28 +90,30 @@
         '-of', 
         'aaigrid', 
         savepath+'.tif', 
         savepath+'.asc'
     ]
     cmd_out_code = run_command(cmd)
 
-def create_basin_station_latlon_csv(basin_name, global_station_file, basin_gpd_df, column_dict, savepath, geojson_file=True):
+def create_basin_station_latlon_csv(region_name, basin_name, global_station_file, basin_gpd_df, column_dict, savepath, geojson_file=True):
     basins_station=gpd.read_file(global_station_file)
     basin_data_crs_changed = basin_gpd_df.to_crs(basins_station.crs)
     basins_station_spatialjoin = gpd.sjoin(basins_station, basin_data_crs_changed, "inner")[[
                         column_dict['id_column'],
                         column_dict['name_column'],
                         column_dict['lon_column'],
                         column_dict['lat_column'],
                         'geometry']]
     if(geojson_file):
+        basins_station_spatialjoin['regionname'] = str(region_name)
         basins_station_spatialjoin['basinname'] = str(basin_name)
         basins_station_spatialjoin['filename'] = basins_station_spatialjoin[column_dict['id_column']].astype(str)+'_'+ \
                                         basins_station_spatialjoin[column_dict['name_column']].str.replace(' ','_')
-        basins_station_spatialjoin.to_file(savepath[:-4]+'.geojson', driver= "GeoJSON")
+        geojson_save_path = os.path.join(os.path.dirname(savepath),basin_name+'_station.geojson')
+        basins_station_spatialjoin.to_file(geojson_save_path, driver= "GeoJSON")
 
     basins_station_lat_lon = basins_station_spatialjoin[[
                             column_dict['id_column'],
                             column_dict['name_column'],
                             column_dict['lon_column'],
                             column_dict['lat_column']]]
     basins_station_lat_lon['name'] = basins_station_lat_lon[column_dict['id_column']].astype(str
@@ -132,9 +134,11 @@
         stations_df = stations_df.rename(columns={'name':'uniq_id'})                                            
         reservoirs_gdf = reservoirs.merge(stations_df['uniq_id'], how='inner', on='uniq_id')
     else:
         stations_df = stations_df.rename(columns={'name':reservoirs_gdf_column_dict['dam_name_column']})
         reservoirs_gdf = reservoirs.merge(stations_df[reservoirs_gdf_column_dict['dam_name_column']], 
                                         how='inner', on=reservoirs_gdf_column_dict['dam_name_column'])
     
-    reservoirs_gdf.to_file(savepath)
+    if(reservoirs_gdf.empty):
+        raise Exception('Reservoir names in reservoir shapefile are not matching with the station names in the station file used for routing.')
+    reservoirs_gdf.to_file(savepath, index=False)
```

### Comparing `rat-2.1/src/rat/utils/logging.py` & `rat-3.0.0a4/src/rat/utils/logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import os
 import sys
 from time import gmtime, strftime
 import datetime
 import logging
 import subprocess
-from utils.utils import create_directory
+from rat.utils.utils import create_directory
 
 # -------------------------------------------------------------------- #
 LOG_NAME = 'rat-logger'
 FORMATTER = logging.Formatter('%(levelname)s:%(funcName)s>> %(message)s')
 
 NOTIFICATION = 25    # Setting level above INFO, below WARNING
 logging.addLevelName(NOTIFICATION, "NOTIFICATION")
```

### Comparing `rat-2.1/src/rat/utils/metsim_param_reader.py` & `rat-3.0.0a4/src/rat/utils/metsim_param_reader.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-from mimetypes import init
 import yaml
 import datetime
 from logging import getLogger
 import os
 
-from utils.logging import LOG_NAME, NOTIFICATION
-from utils.utils import create_directory
+from rat.utils.logging import LOG_NAME, NOTIFICATION
+from rat.utils.utils import create_directory
 
 log = getLogger(LOG_NAME)
 
 
 class MSParameterFile:
     def __init__(self, start, end, init_param, out_dir, forcings=None, state=None, domain=None, workspace=None, runname=None):
         self.params = yaml.safe_load(open(init_param, 'r'))   # Initialize from a parameter file
```

### Comparing `rat-2.1/src/rat/utils/route_param_reader.py` & `rat-3.0.0a4/src/rat/utils/route_param_reader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import datetime
 from logging import getLogger
 import yaml
 import shutil
 
-from utils.utils import create_directory
-from utils.logging import LOG_NAME, NOTIFICATION
+from rat.utils.utils import create_directory
+from rat.utils.logging import LOG_NAME, NOTIFICATION
 
 log = getLogger(LOG_NAME)
 
 class RouteParameterFile:
     def __init__(self, config, basin_name, start, end, basin_flow_direction_file=None, clean=False, runname=None, rout_input_path_prefix=None,
                                 config_section='ROUTING', intermediate_files=False):
         self.params = {
@@ -67,44 +67,44 @@
 
         # setup workspace
         if (config[self.config_section].get('route_workspace')):
             self.workspace = create_directory(os.path.join(config[self.config_section]['route_workspace'],
                                                                  f'run_{self.runname}'))
         else:
             if(self.intermediate_files):
-                self.workspace = create_directory(os.path.join(config['GLOBAL']['data_dir'],config['BASIN']['major_basin_name'],'basins',
-                                                                self.basin_name,'routing','rout_workspace',f'run_{self.runname}'))
+                self.workspace = create_directory(os.path.join(config['GLOBAL']['data_dir'],config['BASIN']['region_name'],'basins',
+                                                                self.basin_name,'ro','rout_workspace',f'run_{self.runname}'))
         
         ## Route parameter file, this is where the parameter file will be saved
         if (self.intermediate_files):
             self.route_param_path = os.path.relpath(os.path.join(self.workspace, 'route_param.txt'),self.project_dir)
         else:
             # Replacing the init_route_param_file
             if(config[self.config_section].get('route_param_file')):
                 self.route_param_path = os.path.relpath(config[self.config_section].get('route_param_file'),self.project_dir)
             # Or storing it in route basin params dir and replace it from next cycle
             else:
-                self.route_param_path = create_directory(os.path.join(config['GLOBAL']['data_dir'],config['BASIN']['major_basin_name'],
+                self.route_param_path = create_directory(os.path.join(config['GLOBAL']['data_dir'],config['BASIN']['region_name'],
                                                             'basins',self.basin_name,'rout_basin_params'),True)
                 self.route_param_path = os.path.relpath(os.path.join(self.route_param_path,'route_param.txt'),self.project_dir)
         
         ## flow direction file
         self.params['flow_direction_file'] = self.basin_flow_direction_file
 
         ## output dir
-        self.params['output_dir'] = create_directory(os.path.join(config['GLOBAL']['data_dir'],config['BASIN']['major_basin_name'],
-                                                            'basins',self.basin_name,'routing','rout_outputs'),True)
+        self.params['output_dir'] = create_directory(os.path.join(config['GLOBAL']['data_dir'],config['BASIN']['region_name'],
+                                                            'basins',self.basin_name,'ro','ou'),True)
         
         ## stations
         if (self.intermediate_files):
-            self.params['station'] = os.path.join(self.workspace, 'stations_xy.txt')
+            self.params['station'] = os.path.join(self.workspace, 'sta_xy.txt')
         else:
-            self.params['station'] = create_directory(os.path.join(config['GLOBAL']['data_dir'],config['BASIN']['major_basin_name'],
-                                                        'basins',self.basin_name,'routing','rout_basin_params'),True)
-            self.params['station'] = os.path.join(self.params['station'],'stations_xy.txt')
+            self.params['station'] = create_directory(os.path.join(config['GLOBAL']['data_dir'],config['BASIN']['region_name'],
+                                                        'basins',self.basin_name,'ro','pars'),True)
+            self.params['station'] = os.path.join(self.params['station'],'sta_xy.txt')
 
         # Routing Input file prefix path   
         self.params['input_files_prefix'] = self.rout_input_path_prefix
         
         # load from config
         for key in config[f'{self.config_section} PARAMETERS']:
             val = config[f'{self.config_section} PARAMETERS'][key]
```

### Comparing `rat-2.1/src/rat/utils/run_command.py` & `rat-3.0.0a4/src/rat/utils/run_command.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import subprocess
 from logging import getLogger
-import os
-from utils.logging import LOG_NAME
+from rat.utils.logging import LOG_NAME
 
 def run_command(args, metsim=False, **kwargs):
     """Safely runs a command, logs and returns the returncode silently in case of no error. 
     Otherwise, raises an Exception
     """
     log = getLogger(LOG_NAME)
     if isinstance(args, list):
@@ -24,11 +23,8 @@
         log.debug("Finished running command successfully: EXIT CODE %s", exitcode)
     elif (exitcode == 1 and metsim==True):
         log.debug("Finished running metsim successfully: EXIT CODE %s", exitcode)
     else:
         log.error("ERROR Occurred with exit code: %s", exitcode)
         raise Exception
     
-    return exitcode
-
-
-
+    return exitcode
```

### Comparing `rat-2.1/src/rat/utils/science.py` & `rat-3.0.0a4/src/rat/utils/science.py`

 * *Files identical despite different names*

### Comparing `rat-2.1/src/rat/utils/utils.py` & `rat-3.0.0a4/src/rat/utils/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 import os
 import math
+from datetime import datetime
+
+def days_between(d1, d2):
+    d1 = datetime.strptime(d1, "%Y-%m-%d")
+    d2 = datetime.strptime(d2, "%Y-%m-%d")
+    return abs((d2 - d1).days)
 
 def round_pixels(x):
     if((x*10)%10<5):
         x=int(x)
     else:
         x=int(x)+1
     return(x)
@@ -35,14 +41,17 @@
                                or 'both'
 
     Returns:
         lists: returns the time-series as an unpacked list in the same order that they were passed
     """
     mint = max([min(ts.index) for ts in tss])
     maxt = min([max(ts.index) for ts in tss])
+    
+    if mint > maxt:
+        raise Exception('No overlapping time period between the time series.')
 
     if which == 'both':
         clipped_tss = [ts.loc[(ts.index>=mint)&(ts.index<=maxt)] for ts in tss]
     elif which == 'left':
         clipped_tss = [ts.loc[ts.index>=mint] for ts in tss]
     elif which == 'right':
         clipped_tss = [ts.loc[ts.index<=maxt] for ts in tss]
```

### Comparing `rat-2.1/src/rat/utils/vic_param_reader.py` & `rat-3.0.0a4/src/rat/utils/vic_param_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import datetime
 import os
 from logging import getLogger
 
 import yaml
 
-from utils.logging import LOG_NAME, NOTIFICATION
-from utils.utils import create_directory
+from rat.utils.logging import LOG_NAME, NOTIFICATION
+from rat.utils.utils import create_directory
 
 log = getLogger(LOG_NAME)
 
 class VICParameterFile:
     def __init__(self, config, basin_name, startdate=None, enddate=None, vic_output_path=None, vic_section='VIC',
                                      forcing_prefix=None, runname=None, init_state_date=None, save_init_state=True,
                                       intermediate_files= False):
@@ -104,24 +104,26 @@
         self.init_state_date = init_state_date if init_state_date else None
 
         self.vic_output_path = vic_output_path
         self.intermediate_files = intermediate_files
         self.straight_from_metsim = False
         self.save_init_state = save_init_state
         #VIC State Save Date
-        self.vic_init_state_save_date = config['BASIN']['end']+datetime.timedelta(days=1)
+        self.vic_init_state_save_date = config['BASIN']['end']
 
         if runname is None:
             self.runname = datetime.datetime.now().strftime("%Y%m%d_%H%M%S")
         else:
             self.runname = str(runname)
-        if self.workspace:
-            self.workspace = create_directory(os.path.join(self.workspace, f'run_{self.runname}'),True)
-        else :
-            self.workspace = create_directory(os.path.join(config['GLOBAL']['data_dir'],config['BASIN']['major_basin_name'],'basins',basin_name,'vic','vic_workspace',f'run_{self.runname}'),True)
+        
+        if (self.intermediate_files):
+            if self.workspace:
+                self.workspace = create_directory(os.path.join(self.workspace, f'run_{self.runname}'),True)
+            else :
+                self.workspace = create_directory(os.path.join(config['GLOBAL']['data_dir'],config['BASIN']['region_name'],'basins',basin_name,'vic','vic_workspace',f'run_{self.runname}'),True)
 
         if self.init_param_file:
             self._load_from_vic_param()
         
         if forcing_prefix:
             self.straight_from_metsim = True
             self.forcing_prefix = forcing_prefix
@@ -216,18 +218,18 @@
             
         else:
             # Replacing the init_param_file if given
             if self.init_param_file:
                 self.vic_param_path = self.init_param_file   # Paramter file will be replaced
             # Or storing it in vic basin params dir and replace it from next cycle
             else:
-                self.vic_param_path = create_directory(os.path.join(config['GLOBAL']['data_dir'],config['BASIN']['major_basin_name'],
+                self.vic_param_path = create_directory(os.path.join(config['GLOBAL']['data_dir'],config['BASIN']['region_name'],
                                                             'basins',self.basin_name,'vic','vic_basin_params'),True)
                 self.vic_param_path = os.path.join(self.vic_param_path,'vic_param.txt')
-            self.params['results']['LOG_DIR'] = create_directory(os.path.join(config['GLOBAL']['data_dir'],config['BASIN']['major_basin_name'],
+            self.params['results']['LOG_DIR'] = create_directory(os.path.join(config['GLOBAL']['data_dir'],config['BASIN']['region_name'],
                                                              'vic_logs',self.basin_name,''),True) 
         log.debug("VIC Logs Directory: %s ", self.params['results']['LOG_DIR'])
         # if not self.params['results']['LOG_DIR'].endswith(os.sep):
         #     self.params['results']['LOG_DIR'] = self.params['results']['LOG_DIR'] + f'{os.sep}'
 
             
 
@@ -297,27 +299,27 @@
         
         # If vic_output_path is passed as constructor parameter, override it
         if self.vic_output_path:
             self.params['results']['RESULT_DIR'] = self.vic_output_path
         
         # Saving initital state file for vic's next run  if save_init_state is True else deleting STATENAME from state_file_params
         if (self.save_init_state):
-            create_directory(os.path.join(config['GLOBAL']['data_dir'],config['BASIN']['major_basin_name'],'basins',self.basin_name,'vic','vic_init_states'),False)
-            self.params['state_file_params']['STATENAME'] = os.path.join(config['GLOBAL']['data_dir'],config['BASIN']['major_basin_name'],'basins',self.basin_name,'vic','vic_init_states','state_')
+            create_directory(os.path.join(config['GLOBAL']['data_dir'],config['BASIN']['region_name'],'basins',self.basin_name,'vic','vic_init_states'),False)
+            self.params['state_file_params']['STATENAME'] = os.path.join(config['GLOBAL']['data_dir'],config['BASIN']['region_name'],'basins',self.basin_name,'vic','vic_init_states','state_')
             self.params['state_file_params']['STATEYEAR'] = self.vic_init_state_save_date.strftime('%Y')
             self.params['state_file_params']['STATEMONTH'] = self.vic_init_state_save_date.strftime('%m')
             self.params['state_file_params']['STATEDAY'] = self.vic_init_state_save_date.strftime('%d')
         else:
             del self.params['state_file_params']['STATENAME']
 
         # Using initital state file for this run if init_state_date is not None else deleting INIT_STATE from state_file_params
         if (self.init_state_date):
             init_state_date_str = str(self.init_state_date.strftime('%Y'))+str(self.init_state_date.strftime('%m'))+\
                                   str(self.init_state_date.strftime('%d'))
-            self.params['state_file_params']['INIT_STATE'] = os.path.join(config['GLOBAL']['data_dir'],config['BASIN']['major_basin_name'],
+            self.params['state_file_params']['INIT_STATE'] = os.path.join(config['GLOBAL']['data_dir'],config['BASIN']['region_name'],
                                                             'basins',self.basin_name,'vic','vic_init_states',
                                                             'state_.'+init_state_date_str+'_00000.nc')
         else:
             del self.params['state_file_params']['INIT_STATE']
 
     def _out_format_params(self): # return a VIC compatible string of paramters
         header = '\n'.join([
```

### Comparing `rat-2.1/src/rat.egg-info/SOURCES.txt` & `rat-3.0.0a4/src/rat.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,45 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 src/rat/__init__.py
-src/rat/rat.py
+src/rat/rat_basin.py
 src/rat/run_rat.py
 src/rat.egg-info/PKG-INFO
 src/rat.egg-info/SOURCES.txt
 src/rat.egg-info/dependency_links.txt
 src/rat.egg-info/top_level.txt
-src/rat/core/generate_plots.py
+src/rat/cli/rat_cli.py
+src/rat/cli/rat_init_config.py
+src/rat/cli/rat_test_config.py
 src/rat/core/run_altimetry.py
 src/rat/core/run_metsim.py
 src/rat/core/run_postprocessing.py
 src/rat/core/run_routing.py
 src/rat/core/run_sarea.py
 src/rat/core/run_vic.py
 src/rat/core/sarea/TMS.py
 src/rat/core/sarea/sarea_cli_l8.py
+src/rat/core/sarea/sarea_cli_l9.py
 src/rat/core/sarea/sarea_cli_s2.py
 src/rat/core/sarea/sarea_cli_sar.py
 src/rat/data_processing/__init__.py
 src/rat/data_processing/altimetry.py
 src/rat/data_processing/metsim_input_processing.py
 src/rat/data_processing/newdata.py
 src/rat/ee_utils/__init__.py
 src/rat/ee_utils/ee_aec_file_creator.py
-src/rat/ee_utils/ee_config_template.py
+src/rat/ee_utils/ee_config.py
 src/rat/ee_utils/ee_utils.py
 src/rat/utils/__init__.py
-src/rat/utils/convert_for_website.py
+src/rat/utils/clean.py
+src/rat/utils/convert_to_final_outputs.py
 src/rat/utils/files_creator.py
 src/rat/utils/logging.py
 src/rat/utils/metsim_param_reader.py
 src/rat/utils/route_param_reader.py
 src/rat/utils/run_command.py
 src/rat/utils/science.py
 src/rat/utils/utils.py
-src/rat/utils/vic_param_reader.py
+src/rat/utils/vic_param_reader.py
+tests/test_imports.py
```

