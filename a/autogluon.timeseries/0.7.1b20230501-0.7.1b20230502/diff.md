# Comparing `tmp/autogluon.timeseries-0.7.1b20230501.tar.gz` & `tmp/autogluon.timeseries-0.7.1b20230502.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.timeseries-0.7.1b20230501.tar", last modified: Mon May  1 09:04:40 2023, max compression
+gzip compressed data, was "autogluon.timeseries-0.7.1b20230502.tar", last modified: Tue May  2 09:04:24 2023, max compression
```

## Comparing `autogluon.timeseries-0.7.1b20230501.tar` & `autogluon.timeseries-0.7.1b20230502.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:04:40.349844 autogluon.timeseries-0.7.1b20230501/
--rw-r--r--   0 runner    (1001) docker     (123)    12593 2023-05-01 09:04:40.349844 autogluon.timeseries-0.7.1b20230501/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 09:04:40.349844 autogluon.timeseries-0.7.1b20230501/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-05-01 09:03:55.000000 autogluon.timeseries-0.7.1b20230501/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:04:40.341844 autogluon.timeseries-0.7.1b20230501/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:04:40.345844 autogluon.timeseries-0.7.1b20230501/src/autogluon/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-01 09:03:55.000000 autogluon.timeseries-0.7.1b20230501/src/autogluon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:04:40.345844 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-01 09:03:55.000000 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:04:40.345844 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/configs/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-01 09:03:55.000000 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-01 09:03:55.000000 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/configs/presets_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:04:40.345844 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-01 09:03:55.000000 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37170 2023-05-01 09:03:55.000000 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/dataset/ts_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-05-01 09:03:55.000000 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10081 2023-05-01 09:03:55.000000 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/learner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:04:40.345844 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/models/
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-01 09:03:55.000000 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:04:40.345844 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/models/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-01 09:03:55.000000 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/models/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19643 2023-05-01 09:03:55.000000 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-05-01 09:03:55.000000 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/models/abstract/model_trial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:04:40.345844 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/models/autogluon_tabular/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-01 09:03:55.000000 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/models/autogluon_tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-05-01 09:03:55.000000 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py
--rw-r--r--   0 runner    (1001) docker     (123)    17397 2023-05-01 09:03:55.000000 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/models/autogluon_tabular/tabular_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:04:40.345844 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/models/ensemble/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-01 09:03:55.000000 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/models/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-01 09:03:55.000000 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-05-01 09:03:55.000000 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:04:40.345844 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/models/gluonts/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-01 09:03:55.000000 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/models/gluonts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18951 2023-05-01 09:03:55.000000 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:04:40.349844 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/models/gluonts/mx/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-01 09:03:55.000000 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/models/gluonts/mx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-01 09:03:55.000000 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/models/gluonts/mx/callback.py
--rw-r--r--   0 runner    (1001) docker     (123)    22893 2023-05-01 09:03:55.000000 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/models/gluonts/mx/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:04:40.349844 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/models/gluonts/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-01 09:03:55.000000 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/models/gluonts/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14041 2023-05-01 09:03:55.000000 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/models/gluonts/torch/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:04:40.349844 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/models/local/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-01 09:03:55.000000 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/models/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-05-01 09:03:55.000000 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/models/local/abstract_local_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-05-01 09:03:55.000000 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/models/local/naive.py
--rw-r--r--   0 runner    (1001) docker     (123)    12222 2023-05-01 09:03:55.000000 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/models/local/statsforecast.py
--rw-r--r--   0 runner    (1001) docker     (123)    15697 2023-05-01 09:03:55.000000 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/models/local/statsmodels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:04:40.349844 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/models/multi_window/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-01 09:03:55.000000 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/models/multi_window/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9000 2023-05-01 09:03:55.000000 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/models/multi_window/multi_window_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-05-01 09:03:55.000000 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/models/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)    46535 2023-05-01 09:03:55.000000 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-05-01 09:03:55.000000 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:04:40.349844 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-01 09:03:55.000000 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41049 2023-05-01 09:03:55.000000 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/trainer/abstract_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-01 09:03:55.000000 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/trainer/auto_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:04:40.349844 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 09:03:55.000000 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-05-01 09:03:55.000000 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/utils/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-01 09:03:55.000000 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/utils/forecast.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-01 09:03:55.000000 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-01 09:03:55.000000 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/utils/seasonality.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-01 09:03:55.000000 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/utils/warning_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-01 09:04:40.000000 autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:04:40.345844 autogluon.timeseries-0.7.1b20230501/src/autogluon.timeseries.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12593 2023-05-01 09:04:40.000000 autogluon.timeseries-0.7.1b20230501/src/autogluon.timeseries.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-05-01 09:04:40.000000 autogluon.timeseries-0.7.1b20230501/src/autogluon.timeseries.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 09:04:40.000000 autogluon.timeseries-0.7.1b20230501/src/autogluon.timeseries.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-01 09:04:40.000000 autogluon.timeseries-0.7.1b20230501/src/autogluon.timeseries.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-01 09:04:40.000000 autogluon.timeseries-0.7.1b20230501/src/autogluon.timeseries.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-01 09:04:40.000000 autogluon.timeseries-0.7.1b20230501/src/autogluon.timeseries.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 09:04:40.000000 autogluon.timeseries-0.7.1b20230501/src/autogluon.timeseries.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:04:24.978148 autogluon.timeseries-0.7.1b20230502/
+-rw-r--r--   0 runner    (1001) docker     (123)    12593 2023-05-02 09:04:24.978148 autogluon.timeseries-0.7.1b20230502/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 09:04:24.978148 autogluon.timeseries-0.7.1b20230502/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-05-02 09:03:38.000000 autogluon.timeseries-0.7.1b20230502/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:04:24.950148 autogluon.timeseries-0.7.1b20230502/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:04:24.958148 autogluon.timeseries-0.7.1b20230502/src/autogluon/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-02 09:03:38.000000 autogluon.timeseries-0.7.1b20230502/src/autogluon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:04:24.966148 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-02 09:03:38.000000 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:04:24.966148 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-02 09:03:38.000000 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-02 09:03:38.000000 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/configs/presets_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:04:24.966148 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-02 09:03:38.000000 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37170 2023-05-02 09:03:38.000000 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/dataset/ts_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-05-02 09:03:38.000000 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10081 2023-05-02 09:03:38.000000 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/learner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:04:24.970148 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-02 09:03:38.000000 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:04:24.970148 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/models/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-02 09:03:38.000000 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/models/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19723 2023-05-02 09:03:38.000000 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-05-02 09:03:38.000000 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/models/abstract/model_trial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:04:24.970148 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/models/autogluon_tabular/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-02 09:03:38.000000 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/models/autogluon_tabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-05-02 09:03:38.000000 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17282 2023-05-02 09:03:38.000000 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/models/autogluon_tabular/tabular_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:04:24.974148 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/models/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-02 09:03:38.000000 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/models/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-02 09:03:38.000000 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-05-02 09:03:38.000000 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:04:24.974148 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/models/gluonts/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-02 09:03:38.000000 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/models/gluonts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18915 2023-05-02 09:03:38.000000 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:04:24.974148 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/models/gluonts/mx/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-02 09:03:38.000000 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/models/gluonts/mx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-02 09:03:38.000000 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/models/gluonts/mx/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22893 2023-05-02 09:03:38.000000 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/models/gluonts/mx/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:04:24.978148 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/models/gluonts/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-02 09:03:38.000000 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/models/gluonts/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13902 2023-05-02 09:03:38.000000 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/models/gluonts/torch/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:04:24.978148 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/models/local/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-02 09:03:38.000000 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/models/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6980 2023-05-02 09:03:38.000000 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/models/local/abstract_local_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-05-02 09:03:38.000000 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/models/local/naive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12222 2023-05-02 09:03:38.000000 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/models/local/statsforecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15697 2023-05-02 09:03:38.000000 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/models/local/statsmodels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:04:24.978148 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/models/multi_window/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-02 09:03:38.000000 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/models/multi_window/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9000 2023-05-02 09:03:38.000000 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/models/multi_window/multi_window_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9947 2023-05-02 09:03:38.000000 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/models/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46742 2023-05-02 09:03:38.000000 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-05-02 09:03:38.000000 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:04:24.978148 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-02 09:03:38.000000 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41049 2023-05-02 09:03:38.000000 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/trainer/abstract_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-02 09:03:38.000000 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/trainer/auto_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:04:24.978148 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 09:03:38.000000 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-05-02 09:03:38.000000 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/utils/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-02 09:03:38.000000 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/utils/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-02 09:03:38.000000 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-02 09:03:38.000000 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/utils/seasonality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-02 09:03:38.000000 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/utils/warning_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-02 09:04:24.000000 autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:04:24.962148 autogluon.timeseries-0.7.1b20230502/src/autogluon.timeseries.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12593 2023-05-02 09:04:24.000000 autogluon.timeseries-0.7.1b20230502/src/autogluon.timeseries.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-05-02 09:04:24.000000 autogluon.timeseries-0.7.1b20230502/src/autogluon.timeseries.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 09:04:24.000000 autogluon.timeseries-0.7.1b20230502/src/autogluon.timeseries.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-02 09:04:24.000000 autogluon.timeseries-0.7.1b20230502/src/autogluon.timeseries.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-02 09:04:24.000000 autogluon.timeseries-0.7.1b20230502/src/autogluon.timeseries.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-02 09:04:24.000000 autogluon.timeseries-0.7.1b20230502/src/autogluon.timeseries.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 09:04:24.000000 autogluon.timeseries-0.7.1b20230502/src/autogluon.timeseries.egg-info/zip-safe
```

### Comparing `autogluon.timeseries-0.7.1b20230501/PKG-INFO` & `autogluon.timeseries-0.7.1b20230502/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.timeseries
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

### Comparing `autogluon.timeseries-0.7.1b20230501/setup.py` & `autogluon.timeseries-0.7.1b20230502/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/__init__.py` & `autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/configs/presets_configs.py` & `autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/configs/presets_configs.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/dataset/ts_dataframe.py` & `autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/dataset/ts_dataframe.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/evaluator.py` & `autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/evaluator.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/learner.py` & `autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/learner.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/models/__init__.py` & `autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/models/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py` & `autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import os
+import re
 import time
 from typing import Any, Dict, List, Optional, Union
 
 import autogluon.core as ag
 from autogluon.common.loaders import load_pkl
 from autogluon.common.savers import save_pkl
 from autogluon.core.hpo.exceptions import EmptySearchSpace
@@ -82,14 +83,15 @@
         name: Optional[str] = None,
         metadata: Optional[CovariateMetadata] = None,
         eval_metric: Optional[str] = None,
         eval_metric_seasonal_period: Optional[int] = None,
         hyperparameters: Dict[str, Union[int, float, str, ag.Space]] = None,
         **kwargs,
     ):
+        name = name or re.sub(r"Model$", "", self.__class__.__name__)
         super().__init__(
             path=path,
             name=name,
             problem_type=None,
             eval_metric=None,
             hyperparameters=hyperparameters,
         )
```

### Comparing `autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/models/abstract/model_trial.py` & `autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/models/abstract/model_trial.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py` & `autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/models/autogluon_tabular/tabular_model.py` & `autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/models/autogluon_tabular/tabular_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import logging
-import re
 import time
 import warnings
 from typing import Any, Callable, Dict, List, Optional, Tuple
 
 import numpy as np
 import pandas as pd
 
@@ -65,15 +64,14 @@
         prediction_length: int = 1,
         path: Optional[str] = None,
         name: Optional[str] = None,
         eval_metric: str = None,
         hyperparameters: Dict[str, Any] = None,
         **kwargs,  # noqa
     ):
-        name = name or re.sub(r"Model$", "", self.__class__.__name__)  # TODO: look name up from presets
         super().__init__(
             path=path,
             freq=freq,
             prediction_length=prediction_length,
             name=name,
             eval_metric=eval_metric,
             hyperparameters=hyperparameters,
```

### Comparing `autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py` & `autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py` & `autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py` & `autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import logging
-import re
 from pathlib import Path
 from typing import Any, Callable, Dict, Iterator, List, Optional, Type
 
 import gluonts
 import gluonts.core.settings
 import numpy as np
 import pandas as pd
@@ -145,15 +144,14 @@
         prediction_length: int = 1,
         path: Optional[str] = None,
         name: Optional[str] = None,
         eval_metric: str = None,
         hyperparameters: Dict[str, Any] = None,
         **kwargs,  # noqa
     ):
-        name = name or re.sub(r"Model$", "", self.__class__.__name__)  # TODO: look name up from presets
         super().__init__(
             path=path,
             freq=freq,
             prediction_length=prediction_length,
             name=name,
             eval_metric=eval_metric,
             hyperparameters=hyperparameters,
@@ -226,14 +224,15 @@
         if "callbacks" in kwargs:
             self.callbacks += kwargs["callbacks"]
 
     def _get_model_params(self) -> dict:
         """Gets params that are passed to the inner model."""
         args = super()._get_model_params().copy()
         args.setdefault("batch_size", 64)
+        args.setdefault("context_length", max(10, 2 * self.prediction_length))
         args.update(
             dict(
                 freq=self.freq,
                 prediction_length=self.prediction_length,
                 quantiles=self.quantile_levels,
                 callbacks=self.callbacks,
             )
```

### Comparing `autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/models/gluonts/mx/__init__.py` & `autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/models/gluonts/mx/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/models/gluonts/mx/callback.py` & `autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/models/gluonts/mx/callback.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/models/gluonts/mx/models.py` & `autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/models/gluonts/mx/models.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/models/gluonts/torch/models.py` & `autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/models/gluonts/torch/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,35 +46,32 @@
 
     def _get_hpo_backend(self):
         return CUSTOM_BACKEND
 
     def _get_estimator_init_args(self) -> Dict[str, Any]:
         """Get GluonTS specific constructor arguments for estimator objects, an alias to
         `self._get_model_params` for better readability."""
-        init_kwargs = self._get_model_params()
-
-        # GluonTS does not handle context_length=1 well, and sets the context to only prediction_length
-        # we set it to a minimum of 10 here.
-        init_kwargs["context_length"] = max(10, init_kwargs.get("context_length", self.prediction_length))
+        init_kwargs = super()._get_estimator_init_args()
+        # Map MXNet kwarg names to PyTorch Lightning kwarg names
         init_kwargs.setdefault("lr", init_kwargs.get("learning_rate", 1e-3))
-
+        init_kwargs.setdefault("max_epochs", init_kwargs.get("epochs"))
         return init_kwargs
 
     def _get_estimator(self) -> GluonTSPyTorchLightningEstimator:
         """Return the GluonTS Estimator object for the model"""
 
         # As GluonTSPyTorchLightningEstimator objects do not implement `from_hyperparameters` convenience
         # constructors, we re-implement the logic here.
         # we translate the "epochs" parameter to "max_epochs" for consistency in the AbstractGluonTSModel
         # interface
 
         init_args = self._get_estimator_init_args()
 
         trainer_kwargs = {}
-        epochs = init_args.get("max_epochs", init_args.get("epochs"))
+        epochs = init_args.get("max_epochs")
         callbacks = init_args.get("callbacks", [])
 
         # TODO: Provide trainer_kwargs outside the function (e.g., to specify # of GPUs)?
         if epochs is not None:
             trainer_kwargs.update({"max_epochs": epochs})
         trainer_kwargs.update({"callbacks": callbacks, "enable_progress_bar": False})
         trainer_kwargs["default_root_dir"] = self.path
@@ -294,15 +291,15 @@
 
     gluonts_estimator_class: Type[GluonTSPyTorchLightningEstimator] = TemporalFusionTransformerEstimator
     supports_known_covariates = True
     supports_past_covariates = True
 
     def _get_estimator_init_args(self) -> Dict[str, Any]:
         init_kwargs = super()._get_estimator_init_args()
-        init_kwargs.setdefault("context_length", max(64, self.prediction_length))
+        init_kwargs["context_length"] = max(64, init_kwargs["context_length"])
         if self.num_feat_dynamic_real > 0:
             init_kwargs["dynamic_dims"] = [self.num_feat_dynamic_real]
         if self.num_past_feat_dynamic_real > 0:
             init_kwargs["past_dynamic_dims"] = [self.num_past_feat_dynamic_real]
         if self.num_feat_static_real > 0:
             init_kwargs["static_dims"] = [self.num_feat_static_real]
         if len(self.feat_static_cat_cardinality):
```

### Comparing `autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/models/local/abstract_local_model.py` & `autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/models/local/abstract_local_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import hashlib
 import logging
-import re
 from multiprocessing import cpu_count
 from typing import Any, Dict, List, Optional, Union
 
 import pandas as pd
 from joblib import Parallel, delayed
 
 from autogluon.timeseries.dataset.ts_dataframe import ITEMID, TIMESTAMP, TimeSeriesDataFrame
@@ -41,15 +40,14 @@
         prediction_length: int = 1,
         path: Optional[str] = None,
         name: Optional[str] = None,
         eval_metric: str = None,
         hyperparameters: Dict[str, Any] = None,
         **kwargs,  # noqa
     ):
-        name = name or re.sub(r"Model$", "", self.__class__.__name__)
         super().__init__(
             path=path,
             freq=freq,
             prediction_length=prediction_length,
             name=name,
             eval_metric=eval_metric,
             hyperparameters=hyperparameters,
```

### Comparing `autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/models/local/naive.py` & `autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/models/local/naive.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/models/local/statsforecast.py` & `autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/models/local/statsforecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/models/local/statsmodels.py` & `autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/models/local/statsmodels.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/models/multi_window/multi_window_model.py` & `autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/models/multi_window/multi_window_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/models/presets.py` & `autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/models/presets.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import copy
 import logging
-from typing import Any, Dict, List, Optional, Union
+import re
+from typing import Any, Dict, List, Optional, Type, Union
 
 import autogluon.core as ag
 import autogluon.timeseries as agts
 
 from . import (
     ARIMAModel,
     AutoARIMAModel,
@@ -81,19 +82,23 @@
     DeepARMXNet=50,
     SimpleFeedForwardMXNet=30,
     TemporalFusionTransformerMXNet=50,
     MQCNNMXNet=10,
     MQRNNMXNet=10,
 )
 DEFAULT_CUSTOM_MODEL_PRIORITY = 0
-MINIMUM_CONTEXT_LENGTH = 10
 
+VALID_AG_ARGS_KEYS = {
+    "name",
+    "name_prefix",
+    "name_suffix",
+}
 
-def get_default_hps(key, prediction_length):
-    context_length = max(prediction_length * 2, MINIMUM_CONTEXT_LENGTH)
+
+def get_default_hps(key):
     default_model_hps = {
         "local_only": {
             "Naive": {},
             "SeasonalNaive": {},
             "ARIMA": {},
             "ETS": {},
             "Theta": {},
@@ -102,63 +107,55 @@
             "Naive": {},
             "SeasonalNaive": {},
             "ARIMA": {},
             "ETS": {},
             "AutoETS": {},
             "Theta": {},
             "AutoGluonTabular": {},
-            "DeepAR": {
-                "context_length": context_length,
-            },
+            "DeepAR": {},
         },
         "high_quality": {
             "Naive": {},
             "SeasonalNaive": {},
             "ARIMA": {},
             "ETS": {},
             "AutoETS": {},
             "AutoARIMA": {},
             "Theta": {},
             "AutoGluonTabular": {},
-            "DeepAR": {
-                "context_length": context_length,
-            },
-            "SimpleFeedForward": {
-                "context_length": context_length,
-            },
+            "DeepAR": {},
+            "SimpleFeedForward": {},
             "TemporalFusionTransformer": {},
         },
         "best_quality": {
             "Naive": {},
             "SeasonalNaive": {},
             "ARIMA": {},
             "ETS": {},
             "AutoETS": {},
             "AutoARIMA": {},
             "DynamicOptimizedTheta": {},
             "Theta": {},
             "AutoGluonTabular": {},
             "DeepAR": {
-                "context_length": context_length,
                 "num_layers": ag.Int(1, 3, default=2),
                 "hidden_size": ag.Int(40, 80, default=40),
             },
             "SimpleFeedForward": {
-                "context_length": context_length,
                 "hidden_dimensions": ag.Categorical([40], [40, 40], [120]),
             },
             "TemporalFusionTransformer": {},
         },
     }
 
     # update with MXNet if installed
     if agts.MXNET_INSTALLED:
         mxnet_default_updates = {
             "best_quality": {
-                "TransformerMXNet": {"context_length": context_length},
+                "TransformerMXNet": {},
             },
         }
         for k in default_model_hps:
             default_model_hps[k] = dict(**default_model_hps[k], **mxnet_default_updates.get(k, {}))
 
     # For backwards compatibility
     default_model_hps["default"] = default_model_hps["medium_quality"]
@@ -182,25 +179,19 @@
     """
     Create a list of models according to hyperparameters. If hyperparamaters=None,
     will create models according to presets.
     """
     models = []
     if hyperparameters is None:
         hp_string = "default_hpo" if hyperparameter_tune else "default"
-        hyperparameters = copy.deepcopy(get_default_hps(hp_string, prediction_length))
+        hyperparameters = copy.deepcopy(get_default_hps(hp_string))
     elif isinstance(hyperparameters, str):
-        hyperparameters = copy.deepcopy(get_default_hps(hyperparameters, prediction_length))
+        hyperparameters = copy.deepcopy(get_default_hps(hyperparameters))
     elif isinstance(hyperparameters, dict):
-        default_hps = copy.deepcopy(get_default_hps("default", prediction_length))
-        updated_hyperparameters = {}
-        # Only train models from `hyperparameters`, overload default HPs if provided
-        for model, hps in hyperparameters.items():
-            updated_hyperparameters[model] = default_hps.get(model, {})
-            updated_hyperparameters[model].update(hps)
-        hyperparameters = copy.deepcopy(updated_hyperparameters)
+        hyperparameters = copy.deepcopy(hyperparameters)
     else:
         raise ValueError(
             f"hyperparameters must be a dict, a string or None (received {type(hyperparameters)}). "
             f"Please see the documentation for TimeSeriesPredictor.fit"
         )
 
     if hyperparameter_tune:
@@ -210,73 +201,106 @@
 
     invalid_model_names = set(invalid_model_names)
     all_assigned_names = set(invalid_model_names)
 
     model_priority_list = sorted(hyperparameters.keys(), key=lambda x: DEFAULT_MODEL_PRIORITY.get(x, 0), reverse=True)
 
     for model in model_priority_list:
-        model_hps = hyperparameters[model]
         if isinstance(model, str):
             if model not in MODEL_TYPES:
                 raise ValueError(f"Model {model} is not supported yet.")
             model_type = MODEL_TYPES[model]
         elif isinstance(model, AbstractTimeSeriesModelFactory):
             model_type = model
         elif not issubclass(model, AbstractTimeSeriesModel):
             logger.warning(f"Customized model {model} does not inherit from {AbstractTimeSeriesModel}")
             model_type = model
         else:
             logger.log(20, f"Custom Model Type Detected: {model}")
             model_type = model
 
-        model_type_kwargs = dict(
-            path=path,
-            freq=freq,
-            prediction_length=prediction_length,
-            eval_metric=eval_metric,
-            eval_metric_seasonal_period=eval_metric_seasonal_period,
-            hyperparameters=model_hps,
-            **kwargs,
-        )
+        model_hps_list = hyperparameters[model]
+        if not isinstance(model_hps_list, list):
+            model_hps_list = [model_hps_list]
+
+        for model_hps in model_hps_list:
+            ag_args = model_hps.pop(ag.constants.AG_ARGS, {})
+            for key in ag_args:
+                if key not in VALID_AG_ARGS_KEYS:
+                    raise ValueError(
+                        f"Model {model_type} received unknown ag_args key: {key} (valid keys {VALID_AG_ARGS_KEYS})"
+                    )
+            model_name_base = get_model_name(ag_args, model_type)
+
+            model_type_kwargs = dict(
+                name=model_name_base,
+                path=path,
+                freq=freq,
+                prediction_length=prediction_length,
+                eval_metric=eval_metric,
+                eval_metric_seasonal_period=eval_metric_seasonal_period,
+                hyperparameters=model_hps,
+                **kwargs,
+            )
+
+            # add models while preventing name collisions
+            model = model_type(**model_type_kwargs)
 
-        # add models while preventing name collisions
-        model = model_type(**model_type_kwargs)
-        name_stem = model.name
-
-        model_type_kwargs.pop("name", None)
-        increment = 1
-        while model.name in all_assigned_names:
-            increment += 1
-            model = model_type(name=f"{name_stem}_{increment}", **model_type_kwargs)
+            model_type_kwargs.pop("name", None)
+            increment = 1
+            while model.name in all_assigned_names:
+                increment += 1
+                model = model_type(name=f"{model_name_base}_{increment}", **model_type_kwargs)
 
-        if multi_window:
-            model = MultiWindowBacktestingModel(model_base=model, name=model.name, **model_type_kwargs)
+            if multi_window:
+                model = MultiWindowBacktestingModel(model_base=model, name=model.name, **model_type_kwargs)
 
-        all_assigned_names.add(model.name)
-        models.append(model)
+            all_assigned_names.add(model.name)
+            models.append(model)
 
     return models
 
 
+def get_model_name(ag_args: Dict[str, Any], model_type: Type[AbstractTimeSeriesModel]) -> str:
+    name = ag_args.get("name")
+    if name is None:
+        name_stem = re.sub(r"Model$", "", model_type.__name__)
+        name_prefix = ag_args.get("name_prefix", "")
+        name_suffix = ag_args.get("name_suffix", "")
+        name = name_prefix + name_stem + name_suffix
+    return name
+
+
 def contains_searchspace(model_hyperparameters: Dict[str, Any]) -> bool:
     for hp_value in model_hyperparameters.values():
         if isinstance(hp_value, ag.space.Space):
             return True
     return False
 
 
 def verify_contains_at_least_one_searchspace(hyperparameters: Dict[str, Dict[str, Any]]):
-    if not any(contains_searchspace(model_hps) for model_hps in hyperparameters.values()):
-        raise ValueError(
-            f"Hyperparameter tuning specified, but no model contains a hyperparameter search space. "
-            f"Please disable hyperparameter tuning with `hyperparameter_tune_kwargs=None` or provide a search space "
-            f"for at least one model."
-        )
+    for model, model_hps_list in hyperparameters.items():
+        if not isinstance(model_hps_list, list):
+            model_hps_list = [model_hps_list]
+
+        for model_hps in model_hps_list:
+            if contains_searchspace(model_hps):
+                return
+
+    raise ValueError(
+        f"Hyperparameter tuning specified, but no model contains a hyperparameter search space. "
+        f"Please disable hyperparameter tuning with `hyperparameter_tune_kwargs=None` or provide a search space "
+        f"for at least one model."
+    )
 
 
 def verify_contains_no_searchspaces(hyperparameters: Dict[str, Dict[str, Any]]):
-    for model, model_hps in hyperparameters.items():
-        if contains_searchspace(model_hps):
-            raise ValueError(
-                f"Hyperparameter tuning not specified, so hyperparameters must have fixed values. "
-                f"However, for model {model} hyperparameters {model_hps} contain a search space."
-            )
+    for model, model_hps_list in hyperparameters.items():
+        if not isinstance(model_hps_list, list):
+            model_hps_list = [model_hps_list]
+
+        for model_hps in model_hps_list:
+            if contains_searchspace(model_hps):
+                raise ValueError(
+                    f"Hyperparameter tuning not specified, so hyperparameters must have fixed values. "
+                    f"However, for model {model} hyperparameters {model_hps} contain a search space."
+                )
```

### Comparing `autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/predictor.py` & `autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/predictor.py`

 * *Files 2% similar despite different names*

```diff
@@ -374,29 +374,33 @@
         hyperparameters : str or dict, default = "medium_quality"
             Determines what models are trained and what hyperparameters are used by each model.
 
             If str is passed, will use a preset hyperparameter configuration defined in`
             `autogluon/timeseries/trainer/models/presets.py``.
 
             If dict is provided, the keys are strings or Types that indicate which models to train. Each value is
-            itself a dict containing hyperparameters for each of the trained models. Any omitted hyperparameters not
-            specified here will be set to default. For example::
+            itself a dict containing hyperparameters for each of the trained models, or a list of such dicts. Any
+            omitted hyperparameters not specified here will be set to default. For example::
 
                 predictor.fit(
                     ...
                     hyperparameters={
                         "DeepAR": {},
-                        "ETS": {"seasonal_period": 7},
+                        "ETS": [
+                            {"seasonal": "add"},
+                            {"seasonal": None},
+                        ],
                     }
                 )
 
-            The above example will only train two models:
+            The above example will train three models:
 
-            * ``DeepAR`` (with default hyperparameters)
-            * ``ETS`` (with the given `seasonal_period`; all other parameters set to their defaults)
+            * ``DeepAR`` with default hyperparameters
+            * ``ETS`` with additive seasonality (all other parameters set to their defaults)
+            * ``ETS`` with seasonality disabled (all other parameters set to their defaults)
 
             Full list of available models and their hyperparameters is provided in :ref:`forecasting_zoo`.
 
             The hyperparameters for each model can be fixed values (as shown above), or search spaces over which
             hyperparameter optimization is performed. A search space should only be provided when
             ``hyperparameter_tune_kwargs`` is given (i.e., hyperparameter-tuning is utilized). For example::
```

### Comparing `autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/splitter.py` & `autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/splitter.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/trainer/abstract_trainer.py` & `autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/trainer/abstract_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/trainer/auto_trainer.py` & `autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/trainer/auto_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/utils/features.py` & `autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/utils/features.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/utils/forecast.py` & `autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/utils/forecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/utils/seasonality.py` & `autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/utils/seasonality.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230501/src/autogluon/timeseries/utils/warning_filters.py` & `autogluon.timeseries-0.7.1b20230502/src/autogluon/timeseries/utils/warning_filters.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230501/src/autogluon.timeseries.egg-info/PKG-INFO` & `autogluon.timeseries-0.7.1b20230502/src/autogluon.timeseries.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.timeseries
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

### Comparing `autogluon.timeseries-0.7.1b20230501/src/autogluon.timeseries.egg-info/SOURCES.txt` & `autogluon.timeseries-0.7.1b20230502/src/autogluon.timeseries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

