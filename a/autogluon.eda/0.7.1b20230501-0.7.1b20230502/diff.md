# Comparing `tmp/autogluon.eda-0.7.1b20230501.tar.gz` & `tmp/autogluon.eda-0.7.1b20230502.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.eda-0.7.1b20230501.tar", last modified: Mon May  1 09:04:53 2023, max compression
+gzip compressed data, was "autogluon.eda-0.7.1b20230502.tar", last modified: Tue May  2 09:04:37 2023, max compression
```

## Comparing `autogluon.eda-0.7.1b20230501.tar` & `autogluon.eda-0.7.1b20230502.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:04:53.146127 autogluon.eda-0.7.1b20230501/
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-05-01 09:04:53.146127 autogluon.eda-0.7.1b20230501/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-01 09:04:53.146127 autogluon.eda-0.7.1b20230501/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-05-01 09:03:55.000000 autogluon.eda-0.7.1b20230501/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:04:53.138127 autogluon.eda-0.7.1b20230501/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:04:53.142127 autogluon.eda-0.7.1b20230501/src/autogluon/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-01 09:03:55.000000 autogluon.eda-0.7.1b20230501/src/autogluon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:04:53.142127 autogluon.eda-0.7.1b20230501/src/autogluon/eda/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-01 09:03:55.000000 autogluon.eda-0.7.1b20230501/src/autogluon/eda/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:04:53.142127 autogluon.eda-0.7.1b20230501/src/autogluon/eda/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-01 09:03:55.000000 autogluon.eda-0.7.1b20230501/src/autogluon/eda/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13434 2023-05-01 09:03:55.000000 autogluon.eda-0.7.1b20230501/src/autogluon/eda/analysis/anomaly.py
--rw-r--r--   0 runner    (1001) docker     (123)    11219 2023-05-01 09:03:55.000000 autogluon.eda-0.7.1b20230501/src/autogluon/eda/analysis/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    20850 2023-05-01 09:03:55.000000 autogluon.eda-0.7.1b20230501/src/autogluon/eda/analysis/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-05-01 09:03:55.000000 autogluon.eda-0.7.1b20230501/src/autogluon/eda/analysis/explain.py
--rw-r--r--   0 runner    (1001) docker     (123)    23667 2023-05-01 09:03:55.000000 autogluon.eda-0.7.1b20230501/src/autogluon/eda/analysis/interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-01 09:03:55.000000 autogluon.eda-0.7.1b20230501/src/autogluon/eda/analysis/missing.py
--rw-r--r--   0 runner    (1001) docker     (123)    10719 2023-05-01 09:03:55.000000 autogluon.eda-0.7.1b20230501/src/autogluon/eda/analysis/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    13198 2023-05-01 09:03:55.000000 autogluon.eda-0.7.1b20230501/src/autogluon/eda/analysis/shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-05-01 09:03:55.000000 autogluon.eda-0.7.1b20230501/src/autogluon/eda/analysis/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:04:53.142127 autogluon.eda-0.7.1b20230501/src/autogluon/eda/auto/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-01 09:03:55.000000 autogluon.eda-0.7.1b20230501/src/autogluon/eda/auto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    77515 2023-05-01 09:03:55.000000 autogluon.eda-0.7.1b20230501/src/autogluon/eda/auto/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-05-01 09:03:55.000000 autogluon.eda-0.7.1b20230501/src/autogluon/eda/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:04:53.142127 autogluon.eda-0.7.1b20230501/src/autogluon/eda/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 09:03:55.000000 autogluon.eda-0.7.1b20230501/src/autogluon/eda/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-01 09:03:55.000000 autogluon.eda-0.7.1b20230501/src/autogluon/eda/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-01 09:03:55.000000 autogluon.eda-0.7.1b20230501/src/autogluon/eda/utils/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-01 09:04:52.000000 autogluon.eda-0.7.1b20230501/src/autogluon/eda/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:04:53.146127 autogluon.eda-0.7.1b20230501/src/autogluon/eda/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-01 09:03:55.000000 autogluon.eda-0.7.1b20230501/src/autogluon/eda/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-05-01 09:03:55.000000 autogluon.eda-0.7.1b20230501/src/autogluon/eda/visualization/anomaly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-05-01 09:03:55.000000 autogluon.eda-0.7.1b20230501/src/autogluon/eda/visualization/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11954 2023-05-01 09:03:55.000000 autogluon.eda-0.7.1b20230501/src/autogluon/eda/visualization/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-05-01 09:03:55.000000 autogluon.eda-0.7.1b20230501/src/autogluon/eda/visualization/explain.py
--rw-r--r--   0 runner    (1001) docker     (123)    24169 2023-05-01 09:03:55.000000 autogluon.eda-0.7.1b20230501/src/autogluon/eda/visualization/interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-01 09:03:55.000000 autogluon.eda-0.7.1b20230501/src/autogluon/eda/visualization/jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-05-01 09:03:55.000000 autogluon.eda-0.7.1b20230501/src/autogluon/eda/visualization/layouts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-05-01 09:03:55.000000 autogluon.eda-0.7.1b20230501/src/autogluon/eda/visualization/missing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11369 2023-05-01 09:03:55.000000 autogluon.eda-0.7.1b20230501/src/autogluon/eda/visualization/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-01 09:03:55.000000 autogluon.eda-0.7.1b20230501/src/autogluon/eda/visualization/shift.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:04:53.142127 autogluon.eda-0.7.1b20230501/src/autogluon.eda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-05-01 09:04:53.000000 autogluon.eda-0.7.1b20230501/src/autogluon.eda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-05-01 09:04:53.000000 autogluon.eda-0.7.1b20230501/src/autogluon.eda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 09:04:53.000000 autogluon.eda-0.7.1b20230501/src/autogluon.eda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-01 09:04:53.000000 autogluon.eda-0.7.1b20230501/src/autogluon.eda.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-01 09:04:53.000000 autogluon.eda-0.7.1b20230501/src/autogluon.eda.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-01 09:04:53.000000 autogluon.eda-0.7.1b20230501/src/autogluon.eda.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 09:04:53.000000 autogluon.eda-0.7.1b20230501/src/autogluon.eda.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:04:37.882094 autogluon.eda-0.7.1b20230502/
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-05-02 09:04:37.882094 autogluon.eda-0.7.1b20230502/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-02 09:04:37.886094 autogluon.eda-0.7.1b20230502/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-05-02 09:03:38.000000 autogluon.eda-0.7.1b20230502/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:04:37.878094 autogluon.eda-0.7.1b20230502/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:04:37.878094 autogluon.eda-0.7.1b20230502/src/autogluon/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-02 09:03:38.000000 autogluon.eda-0.7.1b20230502/src/autogluon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:04:37.878094 autogluon.eda-0.7.1b20230502/src/autogluon/eda/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-02 09:03:38.000000 autogluon.eda-0.7.1b20230502/src/autogluon/eda/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:04:37.882094 autogluon.eda-0.7.1b20230502/src/autogluon/eda/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-02 09:03:38.000000 autogluon.eda-0.7.1b20230502/src/autogluon/eda/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13434 2023-05-02 09:03:38.000000 autogluon.eda-0.7.1b20230502/src/autogluon/eda/analysis/anomaly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11219 2023-05-02 09:03:38.000000 autogluon.eda-0.7.1b20230502/src/autogluon/eda/analysis/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20850 2023-05-02 09:03:38.000000 autogluon.eda-0.7.1b20230502/src/autogluon/eda/analysis/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-05-02 09:03:38.000000 autogluon.eda-0.7.1b20230502/src/autogluon/eda/analysis/explain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23667 2023-05-02 09:03:38.000000 autogluon.eda-0.7.1b20230502/src/autogluon/eda/analysis/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-02 09:03:38.000000 autogluon.eda-0.7.1b20230502/src/autogluon/eda/analysis/missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10719 2023-05-02 09:03:38.000000 autogluon.eda-0.7.1b20230502/src/autogluon/eda/analysis/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13198 2023-05-02 09:03:38.000000 autogluon.eda-0.7.1b20230502/src/autogluon/eda/analysis/shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-05-02 09:03:38.000000 autogluon.eda-0.7.1b20230502/src/autogluon/eda/analysis/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:04:37.882094 autogluon.eda-0.7.1b20230502/src/autogluon/eda/auto/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-02 09:03:38.000000 autogluon.eda-0.7.1b20230502/src/autogluon/eda/auto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77515 2023-05-02 09:03:38.000000 autogluon.eda-0.7.1b20230502/src/autogluon/eda/auto/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-05-02 09:03:38.000000 autogluon.eda-0.7.1b20230502/src/autogluon/eda/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:04:37.882094 autogluon.eda-0.7.1b20230502/src/autogluon/eda/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 09:03:38.000000 autogluon.eda-0.7.1b20230502/src/autogluon/eda/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-02 09:03:38.000000 autogluon.eda-0.7.1b20230502/src/autogluon/eda/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-02 09:03:38.000000 autogluon.eda-0.7.1b20230502/src/autogluon/eda/utils/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-02 09:04:37.000000 autogluon.eda-0.7.1b20230502/src/autogluon/eda/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:04:37.882094 autogluon.eda-0.7.1b20230502/src/autogluon/eda/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-02 09:03:38.000000 autogluon.eda-0.7.1b20230502/src/autogluon/eda/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-05-02 09:03:38.000000 autogluon.eda-0.7.1b20230502/src/autogluon/eda/visualization/anomaly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-05-02 09:03:38.000000 autogluon.eda-0.7.1b20230502/src/autogluon/eda/visualization/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11954 2023-05-02 09:03:38.000000 autogluon.eda-0.7.1b20230502/src/autogluon/eda/visualization/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-05-02 09:03:38.000000 autogluon.eda-0.7.1b20230502/src/autogluon/eda/visualization/explain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24169 2023-05-02 09:03:38.000000 autogluon.eda-0.7.1b20230502/src/autogluon/eda/visualization/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-02 09:03:38.000000 autogluon.eda-0.7.1b20230502/src/autogluon/eda/visualization/jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-05-02 09:03:38.000000 autogluon.eda-0.7.1b20230502/src/autogluon/eda/visualization/layouts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-05-02 09:03:38.000000 autogluon.eda-0.7.1b20230502/src/autogluon/eda/visualization/missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11369 2023-05-02 09:03:38.000000 autogluon.eda-0.7.1b20230502/src/autogluon/eda/visualization/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-02 09:03:38.000000 autogluon.eda-0.7.1b20230502/src/autogluon/eda/visualization/shift.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:04:37.878094 autogluon.eda-0.7.1b20230502/src/autogluon.eda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-05-02 09:04:37.000000 autogluon.eda-0.7.1b20230502/src/autogluon.eda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-05-02 09:04:37.000000 autogluon.eda-0.7.1b20230502/src/autogluon.eda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 09:04:37.000000 autogluon.eda-0.7.1b20230502/src/autogluon.eda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-02 09:04:37.000000 autogluon.eda-0.7.1b20230502/src/autogluon.eda.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-02 09:04:37.000000 autogluon.eda-0.7.1b20230502/src/autogluon.eda.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-02 09:04:37.000000 autogluon.eda-0.7.1b20230502/src/autogluon.eda.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 09:04:37.000000 autogluon.eda-0.7.1b20230502/src/autogluon.eda.egg-info/zip-safe
```

### Comparing `autogluon.eda-0.7.1b20230501/PKG-INFO` & `autogluon.eda-0.7.1b20230502/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.eda
-Version: 0.7.1b20230501
+Version: 0.7.1b20230502
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.eda-0.7.1b20230501/setup.cfg` & `autogluon.eda-0.7.1b20230502/setup.cfg`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.1b20230501/setup.py` & `autogluon.eda-0.7.1b20230502/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     'phik>=0.12.2,<0.13',
     'seaborn>=0.12.0,<0.13',
     'ipywidgets>=7.7.1,<9.0',  # min versions guidance: 7.7.1 collab/kaggle
     'shap>=0.41,<0.42',
     'yellowbrick>=1.5,<1.6',
     'pyod>=1.0,<1.1',
     'suod>=0.0.8,<0.1',
+    'ipython>7.16,<8.13',  # IPython 8.13+ supports Python 3.9 and above; Python 3.7 is supported with IPython >7.16
     f'autogluon.core=={version}',
     f'autogluon.common=={version}',
     f'autogluon.features=={version}',
     f'autogluon.tabular=={version}',
 ]
 
 extras_require = dict()
```

### Comparing `autogluon.eda-0.7.1b20230501/src/autogluon/eda/analysis/__init__.py` & `autogluon.eda-0.7.1b20230502/src/autogluon/eda/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.1b20230501/src/autogluon/eda/analysis/anomaly.py` & `autogluon.eda-0.7.1b20230502/src/autogluon/eda/analysis/anomaly.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.1b20230501/src/autogluon/eda/analysis/base.py` & `autogluon.eda-0.7.1b20230502/src/autogluon/eda/analysis/base.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.1b20230501/src/autogluon/eda/analysis/dataset.py` & `autogluon.eda-0.7.1b20230502/src/autogluon/eda/analysis/dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.1b20230501/src/autogluon/eda/analysis/explain.py` & `autogluon.eda-0.7.1b20230502/src/autogluon/eda/analysis/explain.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.1b20230501/src/autogluon/eda/analysis/interaction.py` & `autogluon.eda-0.7.1b20230502/src/autogluon/eda/analysis/interaction.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.1b20230501/src/autogluon/eda/analysis/missing.py` & `autogluon.eda-0.7.1b20230502/src/autogluon/eda/analysis/missing.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.1b20230501/src/autogluon/eda/analysis/model.py` & `autogluon.eda-0.7.1b20230502/src/autogluon/eda/analysis/model.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.1b20230501/src/autogluon/eda/analysis/shift.py` & `autogluon.eda-0.7.1b20230502/src/autogluon/eda/analysis/shift.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.1b20230501/src/autogluon/eda/analysis/transform.py` & `autogluon.eda-0.7.1b20230502/src/autogluon/eda/analysis/transform.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.1b20230501/src/autogluon/eda/auto/simple.py` & `autogluon.eda-0.7.1b20230502/src/autogluon/eda/auto/simple.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.1b20230501/src/autogluon/eda/state.py` & `autogluon.eda-0.7.1b20230502/src/autogluon/eda/state.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.1b20230501/src/autogluon/eda/utils/common.py` & `autogluon.eda-0.7.1b20230502/src/autogluon/eda/utils/common.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.1b20230501/src/autogluon/eda/utils/defaults.py` & `autogluon.eda-0.7.1b20230502/src/autogluon/eda/utils/defaults.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.1b20230501/src/autogluon/eda/visualization/__init__.py` & `autogluon.eda-0.7.1b20230502/src/autogluon/eda/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.1b20230501/src/autogluon/eda/visualization/anomaly.py` & `autogluon.eda-0.7.1b20230502/src/autogluon/eda/visualization/anomaly.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.1b20230501/src/autogluon/eda/visualization/base.py` & `autogluon.eda-0.7.1b20230502/src/autogluon/eda/visualization/base.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.1b20230501/src/autogluon/eda/visualization/dataset.py` & `autogluon.eda-0.7.1b20230502/src/autogluon/eda/visualization/dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.1b20230501/src/autogluon/eda/visualization/explain.py` & `autogluon.eda-0.7.1b20230502/src/autogluon/eda/visualization/explain.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.1b20230501/src/autogluon/eda/visualization/interaction.py` & `autogluon.eda-0.7.1b20230502/src/autogluon/eda/visualization/interaction.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.1b20230501/src/autogluon/eda/visualization/jupyter.py` & `autogluon.eda-0.7.1b20230502/src/autogluon/eda/visualization/jupyter.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.1b20230501/src/autogluon/eda/visualization/layouts.py` & `autogluon.eda-0.7.1b20230502/src/autogluon/eda/visualization/layouts.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.1b20230501/src/autogluon/eda/visualization/missing.py` & `autogluon.eda-0.7.1b20230502/src/autogluon/eda/visualization/missing.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.1b20230501/src/autogluon/eda/visualization/model.py` & `autogluon.eda-0.7.1b20230502/src/autogluon/eda/visualization/model.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.1b20230501/src/autogluon/eda/visualization/shift.py` & `autogluon.eda-0.7.1b20230502/src/autogluon/eda/visualization/shift.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.1b20230501/src/autogluon.eda.egg-info/PKG-INFO` & `autogluon.eda-0.7.1b20230502/src/autogluon.eda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.eda
-Version: 0.7.1b20230501
+Version: 0.7.1b20230502
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.eda-0.7.1b20230501/src/autogluon.eda.egg-info/SOURCES.txt` & `autogluon.eda-0.7.1b20230502/src/autogluon.eda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

