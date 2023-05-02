# Comparing `tmp/ecutilities-1.2.6.tar.gz` & `tmp/ecutilities-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecutilities-1.2.6.tar", last modified: Thu Mar 30 05:56:49 2023, max compression
+gzip compressed data, was "ecutilities-1.2.7.tar", last modified: Tue May  2 09:46:38 2023, max compression
```

## Comparing `ecutilities-1.2.6.tar` & `ecutilities-1.2.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 vtec      (1000) vtec      (1000)        0 2023-03-30 05:56:49.471691 ecutilities-1.2.6/
--rwxr-xr-x   0 vtec      (1000) vtec      (1000)     1077 2022-10-25 09:14:41.000000 ecutilities-1.2.6/LICENSE.txt
--rw-r--r--   0 vtec      (1000) vtec      (1000)       90 2022-10-28 16:19:44.000000 ecutilities-1.2.6/MANIFEST.in
--rw-r--r--   0 vtec      (1000) vtec      (1000)     1549 2023-03-30 05:56:49.471691 ecutilities-1.2.6/PKG-INFO
--rw-r--r--   0 vtec      (1000) vtec      (1000)      830 2023-01-30 15:03:53.000000 ecutilities-1.2.6/README.md
-drwxr-xr-x   0 vtec      (1000) vtec      (1000)        0 2023-03-30 05:56:49.461691 ecutilities-1.2.6/ecutilities/
--rw-r--r--   0 vtec      (1000) vtec      (1000)       22 2023-03-30 05:56:21.000000 ecutilities-1.2.6/ecutilities/__init__.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)     9638 2023-03-30 05:56:21.000000 ecutilities-1.2.6/ecutilities/_modidx.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)     6476 2023-03-30 05:56:21.000000 ecutilities-1.2.6/ecutilities/core.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)     4841 2023-03-30 05:56:21.000000 ecutilities-1.2.6/ecutilities/dev_utils.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)     2830 2023-03-30 05:56:21.000000 ecutilities-1.2.6/ecutilities/eda_stats_utils.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)     7902 2023-03-30 05:56:21.000000 ecutilities-1.2.6/ecutilities/image_utils.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)     5712 2023-03-30 05:56:21.000000 ecutilities-1.2.6/ecutilities/ipython.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)     7346 2023-03-30 05:56:21.000000 ecutilities-1.2.6/ecutilities/ml.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)     5670 2023-03-30 05:56:21.000000 ecutilities-1.2.6/ecutilities/plotting.py
-drwxr-xr-x   0 vtec      (1000) vtec      (1000)        0 2023-03-30 05:56:49.471691 ecutilities-1.2.6/ecutilities.egg-info/
--rw-r--r--   0 vtec      (1000) vtec      (1000)     1549 2023-03-30 05:56:49.000000 ecutilities-1.2.6/ecutilities.egg-info/PKG-INFO
--rw-r--r--   0 vtec      (1000) vtec      (1000)      516 2023-03-30 05:56:49.000000 ecutilities-1.2.6/ecutilities.egg-info/SOURCES.txt
--rw-r--r--   0 vtec      (1000) vtec      (1000)        1 2023-03-30 05:56:49.000000 ecutilities-1.2.6/ecutilities.egg-info/dependency_links.txt
--rw-r--r--   0 vtec      (1000) vtec      (1000)       44 2023-03-30 05:56:49.000000 ecutilities-1.2.6/ecutilities.egg-info/entry_points.txt
--rw-r--r--   0 vtec      (1000) vtec      (1000)        1 2023-01-27 05:44:01.000000 ecutilities-1.2.6/ecutilities.egg-info/not-zip-safe
--rw-r--r--   0 vtec      (1000) vtec      (1000)       80 2023-03-30 05:56:49.000000 ecutilities-1.2.6/ecutilities.egg-info/requires.txt
--rw-r--r--   0 vtec      (1000) vtec      (1000)       12 2023-03-30 05:56:49.000000 ecutilities-1.2.6/ecutilities.egg-info/top_level.txt
--rw-r--r--   0 vtec      (1000) vtec      (1000)      928 2023-03-17 04:45:13.000000 ecutilities-1.2.6/settings.ini
--rw-r--r--   0 vtec      (1000) vtec      (1000)       38 2023-03-30 05:56:49.471691 ecutilities-1.2.6/setup.cfg
--rw-r--r--   0 vtec      (1000) vtec      (1000)     2534 2022-10-28 06:03:02.000000 ecutilities-1.2.6/setup.py
+drwxr-xr-x   0 vtec      (1000) vtec      (1000)        0 2023-05-02 09:46:38.755649 ecutilities-1.2.7/
+-rwxr-xr-x   0 vtec      (1000) vtec      (1000)     1077 2022-10-25 09:14:41.000000 ecutilities-1.2.7/LICENSE.txt
+-rw-r--r--   0 vtec      (1000) vtec      (1000)       90 2022-10-28 16:19:44.000000 ecutilities-1.2.7/MANIFEST.in
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     1549 2023-05-02 09:46:38.755649 ecutilities-1.2.7/PKG-INFO
+-rw-r--r--   0 vtec      (1000) vtec      (1000)      830 2023-05-02 09:46:06.000000 ecutilities-1.2.7/README.md
+drwxr-xr-x   0 vtec      (1000) vtec      (1000)        0 2023-05-02 09:46:38.745649 ecutilities-1.2.7/ecutilities/
+-rw-r--r--   0 vtec      (1000) vtec      (1000)       22 2023-05-02 09:45:59.000000 ecutilities-1.2.7/ecutilities/__init__.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)    10826 2023-05-02 09:45:59.000000 ecutilities-1.2.7/ecutilities/_modidx.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)    11545 2023-05-02 09:45:59.000000 ecutilities-1.2.7/ecutilities/core.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     4841 2023-05-02 09:45:59.000000 ecutilities-1.2.7/ecutilities/dev_utils.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     2830 2023-05-02 09:45:59.000000 ecutilities-1.2.7/ecutilities/eda_stats_utils.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     7902 2023-05-02 09:45:59.000000 ecutilities-1.2.7/ecutilities/image_utils.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     5292 2023-05-02 09:45:59.000000 ecutilities-1.2.7/ecutilities/ipython.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     7346 2023-05-02 09:45:59.000000 ecutilities-1.2.7/ecutilities/ml.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     5670 2023-05-02 09:45:59.000000 ecutilities-1.2.7/ecutilities/plotting.py
+drwxr-xr-x   0 vtec      (1000) vtec      (1000)        0 2023-05-02 09:46:38.755649 ecutilities-1.2.7/ecutilities.egg-info/
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     1549 2023-05-02 09:46:38.000000 ecutilities-1.2.7/ecutilities.egg-info/PKG-INFO
+-rw-r--r--   0 vtec      (1000) vtec      (1000)      516 2023-05-02 09:46:38.000000 ecutilities-1.2.7/ecutilities.egg-info/SOURCES.txt
+-rw-r--r--   0 vtec      (1000) vtec      (1000)        1 2023-05-02 09:46:38.000000 ecutilities-1.2.7/ecutilities.egg-info/dependency_links.txt
+-rw-r--r--   0 vtec      (1000) vtec      (1000)       44 2023-05-02 09:46:38.000000 ecutilities-1.2.7/ecutilities.egg-info/entry_points.txt
+-rw-r--r--   0 vtec      (1000) vtec      (1000)        1 2023-01-27 05:44:01.000000 ecutilities-1.2.7/ecutilities.egg-info/not-zip-safe
+-rw-r--r--   0 vtec      (1000) vtec      (1000)       80 2023-05-02 09:46:38.000000 ecutilities-1.2.7/ecutilities.egg-info/requires.txt
+-rw-r--r--   0 vtec      (1000) vtec      (1000)       12 2023-05-02 09:46:38.000000 ecutilities-1.2.7/ecutilities.egg-info/top_level.txt
+-rw-r--r--   0 vtec      (1000) vtec      (1000)      928 2023-03-30 05:59:24.000000 ecutilities-1.2.7/settings.ini
+-rw-r--r--   0 vtec      (1000) vtec      (1000)       38 2023-05-02 09:46:38.755649 ecutilities-1.2.7/setup.cfg
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     2534 2022-10-28 06:03:02.000000 ecutilities-1.2.7/setup.py
```

### Comparing `ecutilities-1.2.6/LICENSE.txt` & `ecutilities-1.2.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ecutilities-1.2.6/PKG-INFO` & `ecutilities-1.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecutilities
-Version: 1.2.6
+Version: 1.2.7
 Summary: Set of utility functions used on regular basis
 Home-page: https://github.com/vtecftwy/ecutils
 Author: Etienne Charlier
 Author-email: github@procurasia.com
 License: MIT License
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ecutilities-1.2.6/README.md` & `ecutilities-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `ecutilities-1.2.6/ecutilities/_modidx.py` & `ecutilities-1.2.7/ecutilities/_modidx.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,43 @@
 # Autogenerated by nbdev
 
 d = { 'settings': { 'branch': 'master',
                 'doc_baseurl': '/ecutils',
                 'doc_host': 'https://vtecftwy.github.io',
                 'git_url': 'https://github.com/vtecftwy/ecutils',
                 'lib_path': 'ecutilities'},
-  'syms': { 'ecutilities.core': { 'ecutilities.core.IsLocalMachine': ('00_core.html#islocalmachine', 'ecutilities/core.py'),
-                                  'ecutilities.core.IsLocalMachine.__call__': ( '00_core.html#islocalmachine.__call__',
+  'syms': { 'ecutilities.core': { 'ecutilities.core.CurrentMachine': ('00_core.html#currentmachine', 'ecutilities/core.py'),
+                                  'ecutilities.core.CurrentMachine.__call__': ( '00_core.html#currentmachine.__call__',
                                                                                 'ecutilities/core.py'),
-                                  'ecutilities.core.IsLocalMachine.__new__': ('00_core.html#islocalmachine.__new__', 'ecutilities/core.py'),
-                                  'ecutilities.core.IsLocalMachine.home': ('00_core.html#islocalmachine.home', 'ecutilities/core.py'),
-                                  'ecutilities.core.IsLocalMachine.is_local': ( '00_core.html#islocalmachine.is_local',
+                                  'ecutilities.core.CurrentMachine.__init__': ( '00_core.html#currentmachine.__init__',
                                                                                 'ecutilities/core.py'),
-                                  'ecutilities.core.IsLocalMachine.os': ('00_core.html#islocalmachine.os', 'ecutilities/core.py'),
-                                  'ecutilities.core.IsLocalMachine.p2config': ( '00_core.html#islocalmachine.p2config',
+                                  'ecutilities.core.CurrentMachine.__new__': ('00_core.html#currentmachine.__new__', 'ecutilities/core.py'),
+                                  'ecutilities.core.CurrentMachine.deregister_as_local': ( '00_core.html#currentmachine.deregister_as_local',
+                                                                                           'ecutilities/core.py'),
+                                  'ecutilities.core.CurrentMachine.home': ('00_core.html#currentmachine.home', 'ecutilities/core.py'),
+                                  'ecutilities.core.CurrentMachine.is_local': ( '00_core.html#currentmachine.is_local',
                                                                                 'ecutilities/core.py'),
-                                  'ecutilities.core.IsLocalMachine.read_config': ( '00_core.html#islocalmachine.read_config',
+                                  'ecutilities.core.CurrentMachine.os': ('00_core.html#currentmachine.os', 'ecutilities/core.py'),
+                                  'ecutilities.core.CurrentMachine.p2config': ( '00_core.html#currentmachine.p2config',
+                                                                                'ecutilities/core.py'),
+                                  'ecutilities.core.CurrentMachine.read_config': ( '00_core.html#currentmachine.read_config',
                                                                                    'ecutilities/core.py'),
-                                  'ecutilities.core.IsLocalMachine.register_as_local': ( '00_core.html#islocalmachine.register_as_local',
+                                  'ecutilities.core.CurrentMachine.register_as_local': ( '00_core.html#currentmachine.register_as_local',
                                                                                          'ecutilities/core.py'),
+                                  'ecutilities.core.ProjectFileSystem': ('00_core.html#projectfilesystem', 'ecutilities/core.py'),
+                                  'ecutilities.core.ProjectFileSystem.create_project_file_system': ( '00_core.html#projectfilesystem.create_project_file_system',
+                                                                                                     'ecutilities/core.py'),
+                                  'ecutilities.core.ProjectFileSystem.data': ('00_core.html#projectfilesystem.data', 'ecutilities/core.py'),
+                                  'ecutilities.core.ProjectFileSystem.nbs': ('00_core.html#projectfilesystem.nbs', 'ecutilities/core.py'),
+                                  'ecutilities.core.ProjectFileSystem.project_root': ( '00_core.html#projectfilesystem.project_root',
+                                                                                       'ecutilities/core.py'),
                                   'ecutilities.core.files_in_tree': ('00_core.html#files_in_tree', 'ecutilities/core.py'),
                                   'ecutilities.core.get_config_value': ('00_core.html#get_config_value', 'ecutilities/core.py'),
                                   'ecutilities.core.is_type': ('00_core.html#is_type', 'ecutilities/core.py'),
-                                  'ecutilities.core.nbs_root_dir': ('00_core.html#nbs_root_dir', 'ecutilities/core.py'),
+                                  'ecutilities.core.path_to_parent_dir': ('00_core.html#path_to_parent_dir', 'ecutilities/core.py'),
                                   'ecutilities.core.safe_path': ('00_core.html#safe_path', 'ecutilities/core.py'),
                                   'ecutilities.core.validate_path': ('00_core.html#validate_path', 'ecutilities/core.py')},
             'ecutilities.dev_utils': { 'ecutilities.dev_utils.StackTrace': ('01_dev_utils.html#stacktrace', 'ecutilities/dev_utils.py'),
                                        'ecutilities.dev_utils.StackTrace.__call__': ( '01_dev_utils.html#stacktrace.__call__',
                                                                                       'ecutilities/dev_utils.py'),
                                        'ecutilities.dev_utils.StackTrace.__init__': ( '01_dev_utils.html#stacktrace.__init__',
                                                                                       'ecutilities/dev_utils.py'),
@@ -46,21 +57,19 @@
             'ecutilities.image_utils': { 'ecutilities.image_utils.add_missing_dates_to_exif': ( '01_image_utils.html#add_missing_dates_to_exif',
                                                                                                 'ecutilities/image_utils.py'),
                                          'ecutilities.image_utils.date_is_within_year': ( '01_image_utils.html#date_is_within_year',
                                                                                           'ecutilities/image_utils.py'),
                                          'ecutilities.image_utils.exif2dt': ('01_image_utils.html#exif2dt', 'ecutilities/image_utils.py'),
                                          'ecutilities.image_utils.get_date_from_file_name': ( '01_image_utils.html#get_date_from_file_name',
                                                                                               'ecutilities/image_utils.py')},
-            'ecutilities.ipython': { 'ecutilities.ipython.cloud_install_project_code': ( '01_ipython.html#cloud_install_project_code',
-                                                                                         'ecutilities/ipython.py'),
-                                     'ecutilities.ipython.df_all_cols_and_rows': ( '01_ipython.html#df_all_cols_and_rows',
-                                                                                   'ecutilities/ipython.py'),
-                                     'ecutilities.ipython.display_dfs': ('01_ipython.html#display_dfs', 'ecutilities/ipython.py'),
+            'ecutilities.ipython': { 'ecutilities.ipython.display_dfs': ('01_ipython.html#display_dfs', 'ecutilities/ipython.py'),
                                      'ecutilities.ipython.display_full_df': ('01_ipython.html#display_full_df', 'ecutilities/ipython.py'),
                                      'ecutilities.ipython.display_mds': ('01_ipython.html#display_mds', 'ecutilities/ipython.py'),
+                                     'ecutilities.ipython.install_code_on_cloud': ( '01_ipython.html#install_code_on_cloud',
+                                                                                    'ecutilities/ipython.py'),
                                      'ecutilities.ipython.nb_setup': ('01_ipython.html#nb_setup', 'ecutilities/ipython.py'),
                                      'ecutilities.ipython.pandas_nrows_ncols': ( '01_ipython.html#pandas_nrows_ncols',
                                                                                  'ecutilities/ipython.py'),
                                      'ecutilities.ipython.pandas_nrows_ncols.__enter__': ( '01_ipython.html#pandas_nrows_ncols.__enter__',
                                                                                            'ecutilities/ipython.py'),
                                      'ecutilities.ipython.pandas_nrows_ncols.__exit__': ( '01_ipython.html#pandas_nrows_ncols.__exit__',
                                                                                           'ecutilities/ipython.py'),
```

### Comparing `ecutilities-1.2.6/ecutilities/dev_utils.py` & `ecutilities-1.2.7/ecutilities/dev_utils.py`

 * *Files identical despite different names*

### Comparing `ecutilities-1.2.6/ecutilities/eda_stats_utils.py` & `ecutilities-1.2.7/ecutilities/eda_stats_utils.py`

 * *Files identical despite different names*

### Comparing `ecutilities-1.2.6/ecutilities/image_utils.py` & `ecutilities-1.2.7/ecutilities/image_utils.py`

 * *Files identical despite different names*

### Comparing `ecutilities-1.2.6/ecutilities/ipython.py` & `ecutilities-1.2.7/ecutilities/ipython.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,108 +3,117 @@
 # %% ../nbs-dev/0_01_ipython.ipynb 2
 from __future__ import annotations
 from fastcore.test import test_fail
 from functools import wraps
 from IPython.core.getipython import get_ipython
 from IPython.display import display, Markdown, display_markdown
 from pathlib import Path
-from typing import Any, Callable, Optional
-from .core import validate_path, is_type, IsLocalMachine
+from typing import Any, List, Callable, Optional
+from .core import safe_path, path_to_parent_dir, is_type, CurrentMachine
 
-import configparser
 import numpy as np
-import os
 import pandas as pd
+import sys
 import subprocess
 import warnings
 
 # %% auto 0
-__all__ = ['run_cli', 'nb_setup', 'cloud_install_project_code', 'display_mds', 'display_dfs', 'pandas_nrows_ncols',
-           'df_all_cols_and_rows', 'display_full_df']
+__all__ = ['run_cli', 'nb_setup', 'install_code_on_cloud', 'display_mds', 'display_dfs', 'pandas_nrows_ncols', 'display_full_df']
 
 # %% ../nbs-dev/0_01_ipython.ipynb 5
 def run_cli(cmd:str = 'ls -l'   # command to execute in the cli
            ):
     """Runs a cli command from jupyter notebook and print the shell output message
     
     Uses subprocess.run with passed command to run the cli command"""
     p = subprocess.run(cmd, stdout=subprocess.PIPE, shell=True)
     print(str(p.stdout, 'utf-8'))
 
 # %% ../nbs-dev/0_01_ipython.ipynb 8
-def nb_setup(autoreload:bool = True,   # True to set autoreload in this notebook
-             paths:list(Path) = None   # Paths to add to the path environment variable
-            ):
-    """Use in first cell of notebook to set autoreload, and paths"""
-#   Add paths. Default is 'src' if it exists
-    if paths is None:
-        p = Path('../src').resolve().absolute()
-        if p.is_dir():
-            paths = [str(p)]
-        else:
-            paths=[]
+def nb_setup(
+    autoreload:bool = True,       # True to set autoreload in this notebook
+    paths:List[str|Path] = None   # Paths to add to the path environment variable
+    ):
+    """Use in first cell of notebook to set autoreload, and add system paths
+    
+    Always add a path to 'src' in the project root, if the directory exists
+    """
+    #  Handle paths
+    #  Add src if it exists
+    nbs_root = path_to_parent_dir('nbs')
+    p2src = (nbs_root / '../src').resolve().absolute()
+    if p2src.is_dir():
+        p = str(p2src.absolute())
+        if p not in sys.path:
+            sys.path.insert(0, p)
+            print(f"Added path: {p2src.absolute()}")
+    # Add passed paths
     if paths:
         for p in paths:
-            sys.path.insert(1, str(p))
-        print(f"Added following paths: {','.join(paths)}")
+            if isinstance(p, Path): p = str(p.resolve().absolute())
+            if p not in sys.path:
+                sys.path.insert(1, p)
+                print(f"Added path: {p}")
 
 #   Setup auto reload
     if autoreload:
         ipshell = get_ipython()
         ipshell.run_line_magic('load_ext',  'autoreload')
         ipshell.run_line_magic('autoreload', '2')
         print('Set autoreload mode')
 
-# %% ../nbs-dev/0_01_ipython.ipynb 12
-def cloud_install_project_code(
-    package_name:str # project package name, e.g. metagentools or git+https://github.com/repo.git@main
+# %% ../nbs-dev/0_01_ipython.ipynb 18
+def install_code_on_cloud(
+    package_name:str, # project package name, e.g. metagentools or git+https://github.com/repo.git@main
+    quiet:bool=False # install quietly with Trud
 ):
-    """When nb is running in the cloud, pip install the project code package"""
+    """pip install the project code package, when nb is running in the cloud."""
     
-    # test whether it runs on colab
-    try:
-        from google.colab import drive
-        RUN_LOCALLY = False
-        print('The notebook is running on colab')
-
-    except ModuleNotFoundError:
-        # not running on colab, testing is it runs on on a local machine
-        RUN_LOCALLY = IsLocalMachine().is_local
-        
-        if RUN_LOCALLY:
-            print('The notebook is running locally, will not automatically install project code')
-        else:
-            print('The notebook is running on a cloud VM or the machine was not registered as local')
+    machine = CurrentMachine()
+
+    if machine.is_colab:
+        CLOUD = True
+        print('The notebook is running on colab.', end=' ')
+        print(f'Will install {package_name}')
+    elif machine.is_kaggle:
+        CLOUD = True
+        print('The notebook is running on kaggle.', end=' ')
+        print(f'Will install {package_name}')
+    elif machine.is_local:
+        CLOUD = False
+        print('The notebook is running locally, will not automatically install project code')
+    else:
+        CLOUD = True
+        print('The notebook is running on a cloud VM or the machine was not registered as local')
+        print(f'Will install {package_name}')
 
-    if not RUN_LOCALLY:
+    if CLOUD:
         print(f'Installing project code {package_name}')
-        cmd = f"pip install -U {package_name}"
+        cmd = f"pip install -{'qq' if quiet else ''}U {package_name}"
         run_cli(cmd)
         print((f"{package_name} is installed."))
-        
-    return RUN_LOCALLY
 
-# %% ../nbs-dev/0_01_ipython.ipynb 16
+# %% ../nbs-dev/0_01_ipython.ipynb 23
 def display_mds(
     *strings:str|tuple[str] # any number of strings with text in markdown format
 ):
     """Display one or several strings formatted in markdown format"""
     for string in strings:
         display_markdown(Markdown(data=string))
 
-# %% ../nbs-dev/0_01_ipython.ipynb 20
+# %% ../nbs-dev/0_01_ipython.ipynb 27
 def display_dfs(*dfs:pd.DataFrame       # any number of Pandas DataFrames
                ):
     """Display one or several `pd.DataFrame` in a single cell output"""
     for df in dfs:
         display(df)
 
-# %% ../nbs-dev/0_01_ipython.ipynb 23
+# %% ../nbs-dev/0_01_ipython.ipynb 30
 class pandas_nrows_ncols:
-    """Context manager set max number of rows and cols to apply to any output within the context"""
+    """Context manager that sets the max number of rows and cols to apply to any output within the context"""
     def __init__(
         self, 
         nrows:int|None=None, # max number of rows to show; show all rows if `None`
         ncols:int|None=None, # max number of columns to show; show all columns if `None`
     ):
         self.nrows = nrows
         self.ncols = ncols
@@ -116,36 +125,15 @@
         pd.options.display.max_columns = self.ncols
         return self.max_rows, self.max_cols
 
     def __exit__(self, exc_type, exc_value, exc_tb):
         pd.options.display.max_rows = self.max_rows
         pd.options.display.max_columns = self.max_cols
 
-# %% ../nbs-dev/0_01_ipython.ipynb 36
-def df_all_cols_and_rows(
-    f:Callable,   # function to apply the decorator ti
-)-> Callable:     # decorated function
-    """decorator function forcing all rows and columns of `DataFrames` to be displayed in the wrapped function"""
-    
-    msg = 'This decorator is deprecated. Will be removed soon. Use context manager `pandas_nrows_ncols` instead.'
-    warnings.warn(msg, category=DeprecationWarning)
-    
-    @wraps(f)
-    def wrapper(*args, **kwargs):
-        max_rows = pd.options.display.max_rows
-        max_cols = pd.options.display.max_columns
-        pd.options.display.max_rows = None
-        pd.options.display.max_columns = None
-        f(*args, **kwargs)
-        pd.options.display.max_rows = max_rows
-        pd.options.display.max_columns = max_cols
-    
-    return wrapper
-
-# %% ../nbs-dev/0_01_ipython.ipynb 40
+# %% ../nbs-dev/0_01_ipython.ipynb 44
 def display_full_df(
     df:pd.DataFrame|pd.Series,  # `DataFrame` or `Series` to display
 ):
     """Display a pandas `DataFrame` or `Series` showing all rows and columns"""
     if is_type(df, pd.DataFrame, raise_error=False) or is_type(df, pd.Series, raise_error=False):
         with pandas_nrows_ncols():
             display(df)
```

### Comparing `ecutilities-1.2.6/ecutilities/ml.py` & `ecutilities-1.2.7/ecutilities/ml.py`

 * *Files identical despite different names*

### Comparing `ecutilities-1.2.6/ecutilities/plotting.py` & `ecutilities-1.2.7/ecutilities/plotting.py`

 * *Files identical despite different names*

### Comparing `ecutilities-1.2.6/ecutilities.egg-info/PKG-INFO` & `ecutilities-1.2.7/ecutilities.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecutilities
-Version: 1.2.6
+Version: 1.2.7
 Summary: Set of utility functions used on regular basis
 Home-page: https://github.com/vtecftwy/ecutils
 Author: Etienne Charlier
 Author-email: github@procurasia.com
 License: MIT License
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ecutilities-1.2.6/ecutilities.egg-info/SOURCES.txt` & `ecutilities-1.2.7/ecutilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ecutilities-1.2.6/settings.ini` & `ecutilities-1.2.7/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = ecutils
 lib_name = ecutilities
-version = 1.2.6
+version = 1.2.7
 min_python = 3.8
 license = MIT
 doc_path = _docs
 lib_path = ecutilities
 nbs_path = nbs-dev
 recursive = True
 tst_flags = notest
```

### Comparing `ecutilities-1.2.6/setup.py` & `ecutilities-1.2.7/setup.py`

 * *Files identical despite different names*

