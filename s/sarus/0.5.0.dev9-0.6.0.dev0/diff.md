# Comparing `tmp/sarus-0.5.0.dev9.tar.gz` & `tmp/sarus-0.6.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sarus-0.5.0.dev9.tar", last modified: Wed Apr  5 07:24:32 2023, max compression
+gzip compressed data, was "dist/sarus-0.6.0.dev0.tar", last modified: Tue May  2 06:50:18 2023, max compression
```

## Comparing `sarus-0.5.0.dev9.tar` & `sarus-0.6.0.dev0.tar`

### file list

```diff
@@ -1,99 +1,101 @@
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-05 07:24:32.328827 sarus-0.5.0.dev9/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       25 2022-09-14 12:56:20.000000 sarus-0.5.0.dev9/MANIFEST.in
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1563 2023-04-05 07:24:32.328827 sarus-0.5.0.dev9/PKG-INFO
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      663 2021-08-24 10:18:30.000000 sarus-0.5.0.dev9/README.rst
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      100 2021-09-06 19:14:48.000000 sarus-0.5.0.dev9/pyproject.toml
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-05 07:24:32.316826 sarus-0.5.0.dev9/sarus/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      549 2023-04-05 07:24:09.000000 sarus-0.5.0.dev9/sarus/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    13051 2023-04-04 14:59:28.000000 sarus-0.5.0.dev9/sarus/config.yaml
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-05 07:24:32.320826 sarus-0.5.0.dev9/sarus/context/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2022-09-14 12:56:20.000000 sarus-0.5.0.dev9/sarus/context/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3069 2023-04-04 14:59:28.000000 sarus-0.5.0.dev9/sarus/context/local_sdk.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      302 2022-09-14 12:56:20.000000 sarus-0.5.0.dev9/sarus/context/typing.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    14472 2023-04-04 17:16:43.000000 sarus-0.5.0.dev9/sarus/dataspec_wrapper.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      743 2023-04-04 14:59:28.000000 sarus-0.5.0.dev9/sarus/debug.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-05 07:24:32.320826 sarus-0.5.0.dev9/sarus/imblearn/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      265 2022-11-29 13:03:29.000000 sarus-0.5.0.dev9/sarus/imblearn/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      578 2022-11-29 13:03:29.000000 sarus-0.5.0.dev9/sarus/imblearn/over_sampling.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      558 2022-11-29 13:03:29.000000 sarus-0.5.0.dev9/sarus/imblearn/pipeline.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      556 2022-11-29 13:03:29.000000 sarus-0.5.0.dev9/sarus/imblearn/under_sampling.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-05 07:24:32.320826 sarus-0.5.0.dev9/sarus/legacy/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       42 2022-11-29 13:03:29.000000 sarus-0.5.0.dev9/sarus/legacy/__init__.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-05 07:24:32.320826 sarus-0.5.0.dev9/sarus/legacy/pandas/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      100 2023-01-27 14:38:46.000000 sarus-0.5.0.dev9/sarus/legacy/pandas/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    16606 2023-01-27 14:38:46.000000 sarus-0.5.0.dev9/sarus/legacy/pandas/dataframe.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-05 07:24:32.320826 sarus-0.5.0.dev9/sarus/legacy/tensorflow/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      132 2022-09-14 12:56:20.000000 sarus-0.5.0.dev9/sarus/legacy/tensorflow/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    13194 2022-12-01 13:21:20.000000 sarus-0.5.0.dev9/sarus/legacy/tensorflow/dataset.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    42361 2022-11-29 13:03:29.000000 sarus-0.5.0.dev9/sarus/legacy/tensorflow/model.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-05 07:24:32.324827 sarus-0.5.0.dev9/sarus/manager/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2022-09-14 12:56:20.000000 sarus-0.5.0.dev9/sarus/manager/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2994 2023-04-04 14:59:28.000000 sarus-0.5.0.dev9/sarus/manager/arrow_computation.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2738 2023-04-04 14:59:28.000000 sarus-0.5.0.dev9/sarus/manager/cache_scalar_computation.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2486 2023-04-04 14:59:28.000000 sarus-0.5.0.dev9/sarus/manager/caching_computation.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     6003 2023-04-04 14:59:28.000000 sarus-0.5.0.dev9/sarus/manager/dataspec_api.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-05 07:24:32.324827 sarus-0.5.0.dev9/sarus/manager/ops/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2022-09-14 12:56:20.000000 sarus-0.5.0.dev9/sarus/manager/ops/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      921 2023-04-04 14:59:28.000000 sarus-0.5.0.dev9/sarus/manager/ops/api.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    15974 2023-04-04 17:16:43.000000 sarus-0.5.0.dev9/sarus/manager/sdk_manager.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2564 2023-04-04 17:16:43.000000 sarus-0.5.0.dev9/sarus/manager/typing.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2792 2023-04-04 14:59:28.000000 sarus-0.5.0.dev9/sarus/manager/value_computation.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-05 07:24:32.324827 sarus-0.5.0.dev9/sarus/numpy/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      337 2022-09-14 12:56:20.000000 sarus-0.5.0.dev9/sarus/numpy/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       81 2022-09-14 12:56:20.000000 sarus-0.5.0.dev9/sarus/numpy/random.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      963 2022-09-14 12:56:20.000000 sarus-0.5.0.dev9/sarus/numpy/scalars.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-05 07:24:32.324827 sarus-0.5.0.dev9/sarus/pandas/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      197 2022-11-29 13:03:29.000000 sarus-0.5.0.dev9/sarus/pandas/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      822 2022-11-29 13:03:29.000000 sarus-0.5.0.dev9/sarus/pandas/core.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4918 2023-04-04 14:59:28.000000 sarus-0.5.0.dev9/sarus/pandas/dataframe.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      206 2022-11-29 13:03:29.000000 sarus-0.5.0.dev9/sarus/pandas/io.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-05 07:24:32.324827 sarus-0.5.0.dev9/sarus/pandas_profiling/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       81 2022-09-14 12:56:20.000000 sarus-0.5.0.dev9/sarus/pandas_profiling/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      841 2022-09-14 12:56:20.000000 sarus-0.5.0.dev9/sarus/pandas_profiling/profile_report.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-05 07:24:32.324827 sarus-0.5.0.dev9/sarus/plotly/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      108 2022-09-14 12:56:20.000000 sarus-0.5.0.dev9/sarus/plotly/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      138 2022-09-14 12:56:20.000000 sarus-0.5.0.dev9/sarus/plotly/express.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    55278 2023-04-04 17:16:43.000000 sarus-0.5.0.dev9/sarus/sarus.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-05 07:24:32.324827 sarus-0.5.0.dev9/sarus/scripts/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-04-04 14:59:28.000000 sarus-0.5.0.dev9/sarus/scripts/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4618 2023-04-04 14:59:28.000000 sarus-0.5.0.dev9/sarus/scripts/generate_op_list.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-05 07:24:32.328827 sarus-0.5.0.dev9/sarus/sklearn/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      680 2023-04-04 14:59:28.000000 sarus-0.5.0.dev9/sarus/sklearn/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     6821 2022-11-25 16:40:07.000000 sarus-0.5.0.dev9/sarus/sklearn/cluster.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      766 2022-11-29 13:03:29.000000 sarus-0.5.0.dev9/sarus/sklearn/compose.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      833 2022-09-14 12:56:20.000000 sarus-0.5.0.dev9/sarus/sklearn/decomposition.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    11790 2022-11-25 16:40:07.000000 sarus-0.5.0.dev9/sarus/sklearn/ensemble.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      566 2022-11-29 13:03:29.000000 sarus-0.5.0.dev9/sarus/sklearn/impute.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      177 2022-09-14 12:56:20.000000 sarus-0.5.0.dev9/sarus/sklearn/inspection.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      668 2023-04-04 14:59:28.000000 sarus-0.5.0.dev9/sarus/sklearn/linear_model.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      174 2022-09-14 12:56:20.000000 sarus-0.5.0.dev9/sarus/sklearn/metrics.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1161 2022-11-29 13:03:29.000000 sarus-0.5.0.dev9/sarus/sklearn/model_selection.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      558 2022-11-29 13:03:29.000000 sarus-0.5.0.dev9/sarus/sklearn/pipeline.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1618 2022-11-29 13:03:29.000000 sarus-0.5.0.dev9/sarus/sklearn/preprocessing.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      613 2022-09-14 12:56:20.000000 sarus-0.5.0.dev9/sarus/sklearn/svm.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-05 07:24:32.328827 sarus-0.5.0.dev9/sarus/skopt/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      223 2022-11-29 13:03:29.000000 sarus-0.5.0.dev9/sarus/skopt/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      929 2022-11-29 13:03:29.000000 sarus-0.5.0.dev9/sarus/skopt/searchcv.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-05 07:24:32.328827 sarus-0.5.0.dev9/sarus/std/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      154 2022-11-29 13:03:29.000000 sarus-0.5.0.dev9/sarus/std/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1074 2022-11-29 13:03:29.000000 sarus-0.5.0.dev9/sarus/std/types.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-05 07:24:32.328827 sarus-0.5.0.dev9/sarus/storage/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-01-27 14:38:46.000000 sarus-0.5.0.dev9/sarus/storage/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4552 2023-01-27 14:38:46.000000 sarus-0.5.0.dev9/sarus/storage/legacy_local.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-05 07:24:32.328827 sarus-0.5.0.dev9/sarus/tensorflow/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2022-09-14 12:56:20.000000 sarus-0.5.0.dev9/sarus/tensorflow/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1676 2023-04-04 14:59:28.000000 sarus-0.5.0.dev9/sarus/typing.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    10996 2023-04-04 14:59:28.000000 sarus-0.5.0.dev9/sarus/utils.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1461 2023-04-04 14:59:28.000000 sarus-0.5.0.dev9/sarus/wrapper_factory.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-05 07:24:32.328827 sarus-0.5.0.dev9/sarus/xgboost/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      213 2022-09-14 12:56:20.000000 sarus-0.5.0.dev9/sarus/xgboost/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      774 2022-09-14 12:56:20.000000 sarus-0.5.0.dev9/sarus/xgboost/xgboost.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-05 07:24:32.320826 sarus-0.5.0.dev9/sarus.egg-info/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1563 2023-04-05 07:24:32.000000 sarus-0.5.0.dev9/sarus.egg-info/PKG-INFO
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2000 2023-04-05 07:24:32.000000 sarus-0.5.0.dev9/sarus.egg-info/SOURCES.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2023-04-05 07:24:32.000000 sarus-0.5.0.dev9/sarus.egg-info/dependency_links.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2021-08-30 08:41:07.000000 sarus-0.5.0.dev9/sarus.egg-info/not-zip-safe
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      345 2023-04-05 07:24:32.000000 sarus-0.5.0.dev9/sarus.egg-info/requires.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        6 2023-04-05 07:24:32.000000 sarus-0.5.0.dev9/sarus.egg-info/top_level.txt
--rwxrwxr-x   0 vincent   (1000) vincent   (1000)     1302 2023-04-05 07:24:32.332826 sarus-0.5.0.dev9/setup.cfg
--rwxrwxr-x   0 vincent   (1000) vincent   (1000)      111 2023-04-05 07:23:51.000000 sarus-0.5.0.dev9/setup.py
+drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/
+-rw-rw-r--   0 vl        (1001) vl        (1002)      100 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/pyproject.toml
+-rwxrwxr-x   0 vl        (1001) vl        (1002)      111 2023-05-02 06:50:02.000000 sarus-0.6.0.dev0/setup.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)      663 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/README.rst
+-rw-rw-r--   0 vl        (1001) vl        (1002)       25 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/MANIFEST.in
+drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/
+-rw-rw-r--   0 vl        (1001) vl        (1002)      743 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/debug.py
+drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/xgboost/
+-rw-rw-r--   0 vl        (1001) vl        (1002)      213 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/xgboost/__init__.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)      755 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/xgboost/xgboost.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)    10518 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/utils.py
+drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/pandas/
+-rw-rw-r--   0 vl        (1001) vl        (1002)      197 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/pandas/__init__.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)     4918 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/pandas/dataframe.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)      822 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/pandas/core.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)      206 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/pandas/io.py
+drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/std/
+-rw-rw-r--   0 vl        (1001) vl        (1002)      154 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/std/__init__.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)     1074 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/std/types.py
+drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/pandas_profiling/
+-rw-rw-r--   0 vl        (1001) vl        (1002)       81 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/pandas_profiling/__init__.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)      841 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/pandas_profiling/profile_report.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)      549 2023-05-02 06:50:02.000000 sarus-0.6.0.dev0/sarus/__init__.py
+drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/legacy/
+drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/legacy/pandas/
+-rw-rw-r--   0 vl        (1001) vl        (1002)      100 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/legacy/pandas/__init__.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)    16606 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/legacy/pandas/dataframe.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)       42 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/legacy/__init__.py
+drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/legacy/tensorflow/
+-rw-rw-r--   0 vl        (1001) vl        (1002)      132 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/legacy/tensorflow/__init__.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)    42361 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/legacy/tensorflow/model.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)    13194 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/legacy/tensorflow/dataset.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)    13051 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/config.yaml
+-rw-rw-r--   0 vl        (1001) vl        (1002)     1708 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/typing.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)    55988 2023-05-02 06:50:02.000000 sarus-0.6.0.dev0/sarus/sarus.py
+drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/plotly/
+-rw-rw-r--   0 vl        (1001) vl        (1002)      108 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/plotly/__init__.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)      138 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/plotly/express.py
+drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/tensorflow/
+-rw-rw-r--   0 vl        (1001) vl        (1002)        0 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/tensorflow/__init__.py
+drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/context/
+-rw-rw-r--   0 vl        (1001) vl        (1002)        0 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/context/__init__.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)      302 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/context/typing.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)     3069 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/context/local_sdk.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)     1461 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/wrapper_factory.py
+drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/sklearn/
+-rw-rw-r--   0 vl        (1001) vl        (1002)      766 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/sklearn/compose.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)      680 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/sklearn/__init__.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)      566 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/sklearn/impute.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)      174 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/sklearn/metrics.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)      594 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/sklearn/svm.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)      668 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/sklearn/linear_model.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)     1569 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/sklearn/preprocessing.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)      814 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/sklearn/decomposition.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)      558 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/sklearn/pipeline.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)     6604 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/sklearn/cluster.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)      177 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/sklearn/inspection.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)     1112 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/sklearn/model_selection.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)    11437 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/sklearn/ensemble.py
+drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/scripts/
+-rw-rw-r--   0 vl        (1001) vl        (1002)     4618 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/scripts/generate_op_list.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)        0 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/scripts/__init__.py
+drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/numpy/
+-rw-rw-r--   0 vl        (1001) vl        (1002)      337 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/numpy/__init__.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)       81 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/numpy/random.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)      963 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/numpy/scalars.py
+drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/storage/
+-rw-rw-r--   0 vl        (1001) vl        (1002)        0 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/storage/__init__.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)     4552 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/storage/legacy_local.py
+drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/imblearn/
+-rw-rw-r--   0 vl        (1001) vl        (1002)      265 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/imblearn/__init__.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)      556 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/imblearn/under_sampling.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)      558 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/imblearn/pipeline.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)      578 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/imblearn/over_sampling.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)    14156 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/dataspec_wrapper.py
+drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/manager/
+-rw-rw-r--   0 vl        (1001) vl        (1002)    19293 2023-05-02 06:50:02.000000 sarus-0.6.0.dev0/sarus/manager/sdk_manager.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)     1949 2023-05-02 06:50:02.000000 sarus-0.6.0.dev0/sarus/manager/arrow_remote.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)     1595 2023-05-02 06:50:02.000000 sarus-0.6.0.dev0/sarus/manager/value_remote.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)        0 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/manager/__init__.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)     2556 2023-05-02 06:50:02.000000 sarus-0.6.0.dev0/sarus/manager/typing.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)     6201 2023-05-02 06:50:02.000000 sarus-0.6.0.dev0/sarus/manager/dataspec_api.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)     5360 2023-05-02 06:50:02.000000 sarus-0.6.0.dev0/sarus/manager/arrow_local.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)     3733 2023-05-02 06:50:02.000000 sarus-0.6.0.dev0/sarus/manager/cache_scalar_local.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)     4599 2023-05-02 06:50:02.000000 sarus-0.6.0.dev0/sarus/manager/value_local.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)     3352 2023-05-02 06:50:02.000000 sarus-0.6.0.dev0/sarus/manager/parquet_local.py
+drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/manager/ops/
+-rw-rw-r--   0 vl        (1001) vl        (1002)        0 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/manager/ops/__init__.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)      921 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/manager/ops/api.py
+drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/skopt/
+-rw-rw-r--   0 vl        (1001) vl        (1002)      223 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/skopt/__init__.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)      929 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/skopt/searchcv.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)     1830 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/PKG-INFO
+drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus.egg-info/
+-rw-rw-r--   0 vl        (1001) vl        (1002)        6 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus.egg-info/top_level.txt
+-rw-rw-r--   0 vl        (1001) vl        (1002)        1 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus.egg-info/dependency_links.txt
+-rw-rw-r--   0 vl        (1001) vl        (1002)     2036 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus.egg-info/SOURCES.txt
+-rw-rw-r--   0 vl        (1001) vl        (1002)        1 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus.egg-info/not-zip-safe
+-rw-rw-r--   0 vl        (1001) vl        (1002)     1830 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus.egg-info/PKG-INFO
+-rw-rw-r--   0 vl        (1001) vl        (1002)      344 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus.egg-info/requires.txt
+-rwxrwxr-x   0 vl        (1001) vl        (1002)     1301 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `sarus-0.5.0.dev9/PKG-INFO` & `sarus-0.6.0.dev0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,48 @@
 Metadata-Version: 2.1
 Name: sarus
-Version: 0.5.0.dev9
+Version: 0.6.0.dev0
 Summary: Python client for the Sarus Gateway
 Home-page: https://sarus.tech
 Author: Sarus Technologies
 Author-email: contact@sarus.tech
 License: Apache License 2.0
+Description: 
+        Sarus
+        
+        ===
+        
+        Python client for the Sarus Gateway. It provides simple connectors to leverage confidential data while ensuring data privacy. Users can explore & train AI models on sensitive data, via synthetic data browsing, remote training and differential privacy.
+        
+        Installation
+        ------------
+        
+        PIP
+        ^^^
+        
+        To install locally the latest available version :
+        
+        ``pip install sarus``
+        
+        Usage
+        -----
+        
+        Client
+        ^^^^^^
+        
+        Use this class to connect to **Sarus Gateway**.
+        
+        .. code-block:: python
+        
+           from sarus import Client
+        
+           client = Client(url="http://admin.sarus.tech:5000")
+           available = client.available_datasets()
+           print(f'Datasets available on the server: {available}')
+        
 Keywords: differential privacy,AI,Data privacy
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -21,42 +54,7 @@
 Provides-Extra: imblearn
 Provides-Extra: tensorflow
 Provides-Extra: pandas_profiling
 Provides-Extra: plotly
 Provides-Extra: xgboost
 Provides-Extra: skopt
 Provides-Extra: tests
-
-
-Sarus
-
-===
-
-Python client for the Sarus Gateway. It provides simple connectors to leverage confidential data while ensuring data privacy. Users can explore & train AI models on sensitive data, via synthetic data browsing, remote training and differential privacy.
-
-Installation
-------------
-
-PIP
-^^^
-
-To install locally the latest available version :
-
-``pip install sarus``
-
-Usage
------
-
-Client
-^^^^^^
-
-Use this class to connect to **Sarus Gateway**.
-
-.. code-block:: python
-
-   from sarus import Client
-
-   client = Client(url="http://admin.sarus.tech:5000")
-   available = client.available_datasets()
-   print(f'Datasets available on the server: {available}')
-
-
```

### Comparing `sarus-0.5.0.dev9/README.rst` & `sarus-0.6.0.dev0/README.rst`

 * *Files identical despite different names*

### Comparing `sarus-0.5.0.dev9/sarus/__init__.py` & `sarus-0.6.0.dev0/sarus/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         std,
         xgboost,
     )
 
     from .sarus import Client, Dataset
     from .utils import eval, eval_policy, floating, integer, length
 
-VERSION = "0.5.0.dev9"
+VERSION = "0.6.0.dev0"
 
 __all__ = [
     "Dataset",
     "Client",
     "length",
     "eval",
     "eval_policy",
```

### Comparing `sarus-0.5.0.dev9/sarus/config.yaml` & `sarus-0.6.0.dev0/sarus/config.yaml`

 * *Files identical despite different names*

### Comparing `sarus-0.5.0.dev9/sarus/context/local_sdk.py` & `sarus-0.6.0.dev0/sarus/context/local_sdk.py`

 * *Files identical despite different names*

### Comparing `sarus-0.5.0.dev9/sarus/dataspec_wrapper.py` & `sarus-0.6.0.dev0/sarus/dataspec_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -335,21 +335,20 @@
         alt_dataspec, alt_policy = self.alternative_dataspec(target_epsilon)
 
         if (
             target_epsilon is not None
             and alt_policy == DataspecPrivacyPolicy.SYNTHETIC
             and verbose >= 1
         ):
-            warning_message = (
+            logger.warning(
                 "Warning: target_epsilon could not be consumed. "
                 "This might be due to privacy budget "
                 "constraints or some operations not "
                 "compilable with Differential Privacy."
             )
-            print(warning_message)
 
         if alt_dataspec.prototype() == sp.Dataset:
             dataset = cast(st.Dataset, alt_dataspec)
             mapping = {key: val for val, key in MetaWrapper._wrapper_classes}
             python_class = mapping[type(self)]
             if python_class == str(pd.DataFrame):
                 value = dataset.to_pandas()
@@ -358,21 +357,15 @@
             else:
                 raise TypeError(f"Dataset not viewable as {python_class}")
         else:
             scalar = cast(st.Scalar, alt_dataspec)
             value = cast(st.Scalar, scalar.value())
 
         if verbose >= 1:
-            messages = {
-                DataspecPrivacyPolicy.WHITE_LISTED: "Whitelisted",
-                DataspecPrivacyPolicy.DP: "Differentially-private evaluation",
-                DataspecPrivacyPolicy.SYNTHETIC: "Evaluated from synthetic data only",
-            }
-            message = messages[alt_policy]
-
+            message = alt_policy.value
             if alt_policy == DataspecPrivacyPolicy.DP:
                 epsilon = self.manager().consumed_epsilon(alt_dataspec)
                 message = f"{message} (epsilon={epsilon:.2f})"
 
             print(message)
 
         return value
```

### Comparing `sarus-0.5.0.dev9/sarus/debug.py` & `sarus-0.6.0.dev0/sarus/debug.py`

 * *Files identical despite different names*

### Comparing `sarus-0.5.0.dev9/sarus/imblearn/over_sampling.py` & `sarus-0.6.0.dev0/sarus/imblearn/over_sampling.py`

 * *Files identical despite different names*

### Comparing `sarus-0.5.0.dev9/sarus/imblearn/pipeline.py` & `sarus-0.6.0.dev0/sarus/imblearn/pipeline.py`

 * *Files identical despite different names*

### Comparing `sarus-0.5.0.dev9/sarus/imblearn/under_sampling.py` & `sarus-0.6.0.dev0/sarus/imblearn/under_sampling.py`

 * *Files identical despite different names*

### Comparing `sarus-0.5.0.dev9/sarus/legacy/pandas/dataframe.py` & `sarus-0.6.0.dev0/sarus/legacy/pandas/dataframe.py`

 * *Files identical despite different names*

### Comparing `sarus-0.5.0.dev9/sarus/legacy/tensorflow/dataset.py` & `sarus-0.6.0.dev0/sarus/legacy/tensorflow/dataset.py`

 * *Files identical despite different names*

### Comparing `sarus-0.5.0.dev9/sarus/legacy/tensorflow/model.py` & `sarus-0.6.0.dev0/sarus/legacy/tensorflow/model.py`

 * *Files identical despite different names*

### Comparing `sarus-0.5.0.dev9/sarus/manager/arrow_computation.py` & `sarus-0.6.0.dev0/sarus/manager/arrow_remote.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,83 +1,54 @@
-import traceback
 import typing as t
 
 import pyarrow as pa
-import pyarrow.parquet as pq
-import sarus_data_spec.status as stt
+
 from sarus_data_spec import typing as st
 from sarus_data_spec.constants import ARROW_TASK
-from sarus_data_spec.manager.asyncio.api.api_computation import ApiComputation
-from sarus_data_spec.manager.asyncio.base import ErrorCatchingAsyncIterator
-from sarus_data_spec.manager.asyncio.utils import async_iter
-
-from .caching_computation import ToParquetComputationFromServer
-from .dataspec_api import dataset_result, launch_dataspec
-from .typing import SDKManager
+from sarus_data_spec.manager.computations.remote.base import RemoteComputation
+from sarus_data_spec.manager.computations.base import (
+    ErrorCatchingAsyncIterator,
+)
+import sarus_data_spec.status as stt
+from .dataspec_api import dataset_result, launch_dataspec, dataspec_status
 
 
 class ToArrowComputationOnServer(
-    ApiComputation[t.AsyncIterator[pa.RecordBatch]]
+    RemoteComputation[t.AsyncIterator[pa.RecordBatch]]
 ):
     """ToArrowComputation on the Sarus server through the REST API."""
 
     task_name = ARROW_TASK
 
-    def __init__(
-        self,
-        manager: SDKManager,
-        parquet_computation: ToParquetComputationFromServer,
-    ):
-        self._manager: SDKManager = manager
-        self.parquet_computation = parquet_computation
-
     def launch_task(self, dataspec: st.DataSpec) -> None:
         """Launch the computation of a Dataset on the server."""
         status = self.status(dataspec)
         if status is None:
-            launch_dataspec(self._manager.client(), dataspec.uuid())
-            stt.pending(
-                dataspec=dataspec, manager=self.manager(), task=self.task_name
-            )
+            launch_dataspec(self.computing_manager().client(), dataspec.uuid())
 
-    async def read_ready_result(
+    async def result_from_stage_properties(
         self,
         dataspec: st.DataSpec,
         properties: t.Mapping[str, str],
         **kwargs: t.Any,
     ) -> t.AsyncIterator[pa.RecordBatch]:
         """Return the task result, launch the computation if needed."""
         batch_size = kwargs["batch_size"]
+        ait = dataset_result(
+            self.computing_manager().client(), dataspec.uuid(), batch_size
+        )
+        return ErrorCatchingAsyncIterator(ait, dataspec, self)
 
-        if self._manager.is_cached(dataspec):
-            cache_path = await self.parquet_computation.task_result(dataspec)
-            try:
-                ait = async_iter(
-                    pq.read_table(source=cache_path).to_batches(
-                        max_chunksize=batch_size
-                    )
-                )
-            except Exception:
-                stt.error(
-                    dataspec=dataspec,
-                    manager=self.manager(),
-                    task=self.task_name,
-                    properties={
-                        "message": traceback.format_exc(),
-                        "relaunch": str(True),
-                    },
-                )
-                stt.error(
-                    dataspec=dataspec,
-                    manager=self.manager(),
-                    task=self.parquet_computation.task_name,
-                    properties={
-                        "message": traceback.format_exc(),
-                        "relaunch": str(True),
-                    },
-                )
-                raise stt.DataSpecErrorStatus((True, traceback.format_exc()))
+    def status(self, dataspec: st.DataSpec) -> t.Optional[st.Status]:
+        """In this case, the computation retrieves the status from the server
+        via an API call, a local status is created but not stored in order
+        to use it just for the polling"""
+
+        status_proto = dataspec_status(
+            client=self.computing_manager().client(),
+            uuid=dataspec.uuid(),
+            task_names=[self.task_name],
+        )
+        if status_proto is None:
+            return None
         else:
-            ait = dataset_result(
-                self._manager.client(), dataspec.uuid(), batch_size
-            )
-        return ErrorCatchingAsyncIterator(ait, dataspec, self)
+            return stt.Status(protobuf=status_proto, store=False)
```

### Comparing `sarus-0.5.0.dev9/sarus/manager/cache_scalar_computation.py` & `sarus-0.6.0.dev0/sarus/manager/parquet_local.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,82 +1,97 @@
 import logging
-import pickle as pkl
+import os
 import traceback
+import typing as t
+
+import pyarrow as pa
+import pyarrow.parquet as pq
 
-import sarus_data_spec.protobuf as sp
 from sarus_data_spec import typing as st
-from sarus_data_spec.constants import (
-    CACHE_PATH,
-    CACHE_PROTO,
-    CACHE_TYPE,
-    ScalarCaching,
-)
-from sarus_data_spec.manager.asyncio.worker.cache_scalar_computation import (
-    CacheScalarComputation,
-)
+from sarus_data_spec.constants import CACHE_PATH, TO_PARQUET_TASK
+from sarus_data_spec.dataset import Dataset
+from sarus_data_spec.manager.base import Base
+from sarus.manager.arrow_remote import ToArrowComputationOnServer
 from sarus_data_spec.status import DataSpecErrorStatus, error, ready
-
-from .dataspec_api import scalar_result
+from sarus_data_spec.manager.computations.local.base import LocalComputation
 
 logger = logging.getLogger(__name__)
 
+BATCH_SIZE = 10000
 
-class CacheScalarComputationFromServer(CacheScalarComputation):
+
+class ToParquetComputation(LocalComputation[str]):
     """Class responsible for handling the caching
-    in of a scalar computed on the server."""
+    in parquet of a dataset. It wraps a ToArrowComputation
+    to get the iterator."""
 
-    async def prepare(self, dataspec: st.DataSpec) -> None:
+    task_name = TO_PARQUET_TASK
 
-        logger.debug(f"STARTING CACHE_SCALAR {dataspec.uuid()}")
+    def __init__(
+        self, computing_manager: Base, arrow_remote: ToArrowComputationOnServer
+    ) -> None:
+        super().__init__(computing_manager)
+        self.remote_arrow = arrow_remote
+
+    async def prepare(self, dataspec: st.DataSpec) -> None:
+        logger.debug(f'STARTING LOCAL TO_PARQUET {dataspec.uuid()}')
         try:
-            # This task is normally prepared only when the scalar result is
-            # ready on the server
-            # This line is the only one that changes from the Worker
-            # CacheScalarComputation
-            value = scalar_result(self._manager.client(), dataspec.uuid())
-            if isinstance(value, st.HasProtobuf):
-                properties = {
-                    CACHE_PROTO: sp.to_base64(value.protobuf()),
-                    CACHE_TYPE: sp.type_name(value.prototype()),
-                }
+            if self.computing_manager().is_computation_remote(dataspec):
+                iterator = await self.remote_arrow.task_result(
+                    dataspec, batch_size=BATCH_SIZE
+                )
             else:
-                properties = {
-                    CACHE_TYPE: ScalarCaching.PICKLE.value,
-                    CACHE_PATH: self.cache_path(dataspec),
-                }
-                with open(self.cache_path(dataspec), "wb") as f:
-                    pkl.dump(value, f)
-
+                iterator = await self.computing_manager().async_to_arrow_op(
+                    dataset=t.cast(Dataset, dataspec), batch_size=BATCH_SIZE
+                )
+
+            batches = [batch async for batch in iterator]
+            pq.write_table(
+                table=pa.Table.from_batches(batches),
+                where=self.cache_path(dataspec=dataspec),
+                version='2.6',
+            )
         except DataSpecErrorStatus as exception:
             error(
                 dataspec=dataspec,
-                manager=self.manager(),
+                manager=self.computing_manager(),
                 task=self.task_name,
                 properties={
                     "message": traceback.format_exc(),
-                    "relaunch": str(exception.relaunch),
+                    'relaunch': str(exception.relaunch),
                 },
             )
-            raise DataSpecErrorStatus(
-                (exception.relaunch, traceback.format_exc())
-            )
-
+            raise
         except Exception:
             error(
                 dataspec=dataspec,
-                manager=self.manager(),
+                manager=self.computing_manager(),
                 task=self.task_name,
                 properties={
                     "message": traceback.format_exc(),
-                    "relaunch": str(False),
+                    'relaunch': str(False),
                 },
             )
-
             raise DataSpecErrorStatus((False, traceback.format_exc()))
         else:
-            logger.debug(f"FINISHED CACHE_SCALAR {dataspec.uuid()}")
+            logger.debug(f'FINISHED LOCAL TO_PARQUET {dataspec.uuid()}')
             ready(
                 dataspec=dataspec,
-                manager=self.manager(),
-                task=self.task_name,
-                properties=properties,
+                manager=self.computing_manager(),
+                task=TO_PARQUET_TASK,
+                properties={CACHE_PATH: self.cache_path(dataspec)},
             )
+
+    async def result_from_stage_properties(
+        self,
+        dataspec: st.DataSpec,
+        properties: t.Mapping[str, str],
+        **kwargs: t.Any,
+    ) -> str:
+        """Returns the cache_path"""
+        return properties[CACHE_PATH]
+
+    def cache_path(self, dataspec: st.DataSpec) -> str:
+        """Returns the path where to cache the dataset"""
+        return os.path.join(
+            dataspec.manager().parquet_dir(), f"{dataspec.uuid()}.parquet"
+        )
```

### Comparing `sarus-0.5.0.dev9/sarus/manager/dataspec_api.py` & `sarus-0.6.0.dev0/sarus/manager/dataspec_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 import io
 import pickle as pkl
 import typing as t
+import json
 from http import HTTPStatus
 
 import pyarrow as pa
 import pyarrow.parquet as pq
 import sarus_data_spec.protobuf as sp
 import sarus_data_spec.typing as st
 from requests import Response
 from sarus_data_spec.constants import (
     BEST_ALTERNATIVE,
     CONSTRAINT_KIND,
     PRIVACY_LIMIT,
 )
-from sarus_data_spec.manager.asyncio.utils import async_iter
-from sarus_data_spec.protobuf.utilities import dict_deserialize, dict_serialize
+from sarus_data_spec.manager.async_utils import async_iter
 from sarus_data_spec.dataspec_validator.typing import DataspecPrivacyPolicy
+from sarus_data_spec.protobuf.utilities import dict_deserialize, dict_serialize
 
 from sarus.typing import Client
 
 
 def raise_response(resp: Response) -> None:
     """Raise exception with message encapsulated in the response JSON data."""
+    if resp.status_code >= HTTPStatus.INTERNAL_SERVER_ERROR:
+        resp.raise_for_status()
     if resp.status_code >= HTTPStatus.BAD_REQUEST:
-        message = resp.json().get("message")
+        try:
+            message = resp.json().get("message")
+        except json.JSONDecodeError as e:
+            resp.raise_for_status()
         if message is not None:
             raise ValueError(f"Server - {message}")
     resp.raise_for_status()
 
 
 def get_dataspec(
     client: Client, uuid: str
```

### Comparing `sarus-0.5.0.dev9/sarus/manager/ops/api.py` & `sarus-0.6.0.dev0/sarus/manager/ops/api.py`

 * *Files identical despite different names*

### Comparing `sarus-0.5.0.dev9/sarus/manager/sdk_manager.py` & `sarus-0.6.0.dev0/sarus/manager/sdk_manager.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,32 +6,43 @@
 import pyarrow as pa
 import requests
 import sarus_data_spec.protobuf as sp
 import sarus_data_spec.status as stt
 import sarus_data_spec.storage.typing as storage_typing
 import sarus_data_spec.typing as st
 from sarus_data_spec.attribute import attach_properties
-from sarus_data_spec.constants import ARROW_TASK, SCALAR_TASK
-from sarus_data_spec.manager.asyncio.delegating import DelegatingManager
+from sarus_data_spec.constants import (
+    ARROW_TASK,
+    SCALAR_TASK,
+    BIG_DATA_TASK,
+    IS_BIG_DATA,
+)
 from sarus_data_spec.manager.base import Base
+from sarus_data_spec.manager.computations.base import BaseComputation
+from sarus_data_spec.manager.computations.local.schema import SchemaComputation
 from sarus_data_spec.dataspec_validator.privacy_limit import DeltaEpsilonLimit
 from sarus_data_spec.dataspec_validator.typing import DataspecPrivacyPolicy
-from sarus_data_spec.status import Status
-
+from .arrow_local import ToArrowComputation
+from .value_local import ValueComputation
+from .cache_scalar_local import CacheScalarComputation
+from .parquet_local import ToParquetComputation
 import sarus.manager.dataspec_api as api
 import sarus.manager.ops.api as api_ops
+from sarus_data_spec.manager.ops.source.routing import SourceScalar
 from sarus.typing import ADMIN_DS, MOCK, PYTHON_TYPE, Client
+from sarus_data_spec.manager.ops.processor.routing import (
+    TransformedDataset,
+    TransformedScalar,
+)
 
-from .arrow_computation import ToArrowComputationOnServer
-from .cache_scalar_computation import CacheScalarComputationFromServer
-from .caching_computation import ToParquetComputationFromServer
-from .value_computation import ValueComputationOnServer
+from .arrow_remote import ToArrowComputationOnServer
+from .value_remote import ValueComputationOnServer
 
 
-class SDKManager(DelegatingManager):
+class SDKManager(Base):
     """The Manager of the SDK running on the client side.
 
     This Manager has two additional functionalities compared to the
     DelegatingManager manager.
 
     First, it manages the relationship with the remote server using the API
     endpoints.
@@ -51,47 +62,50 @@
 
     def __init__(
         self,
         storage: storage_typing.Storage,
         protobuf: sp.Manager,
         client: Client,
     ) -> None:
-        properties = {
-            "type": "remote_manager",
-            "remote_url": client.url(),
-        }
-        remote_manager = Base(
-            storage=storage,
-            protobuf=sp.Manager(properties=properties),
-        )
+        super().__init__(storage, protobuf)
 
-        super().__init__(storage, protobuf, remote_manager)
+        self.schema_computation = SchemaComputation(self)
+        self.to_parquet_computation = ToParquetComputation(
+            self, arrow_remote=ToArrowComputationOnServer(self)
+        )
+        self.to_arrow_computation = ToArrowComputation(
+            self,
+            parquet_computation=self.to_parquet_computation,
+            arrow_remote=self.to_parquet_computation.remote_arrow,
+        )
+        self.cache_scalar_computation = CacheScalarComputation(
+            self, ValueComputationOnServer(self)
+        )
+        self.value_computation = ValueComputation(
+            self,
+            cache_scalar_computation=self.cache_scalar_computation,
+            remote_scalar=self.cache_scalar_computation.remote_scalar,
+        )
 
         self._client = client
         self._mock_size = 1000
         self._parquet_dir = os.path.join(tempfile.mkdtemp(), "sarus_dataspec")
         os.makedirs(self._parquet_dir, exist_ok=True)
 
-        self.remote_to_arrow_computation = ToArrowComputationOnServer(
-            self, ToParquetComputationFromServer(self)
-        )
-        self.remote_value_computation = ValueComputationOnServer(
-            self, CacheScalarComputationFromServer(self)
-        )
-
     def set_admin_ds(
         self, source_ds: st.DataSpec, admin_ds: t.Dict[str, t.Any]
     ) -> None:
         """Attach the admin_ds to a source dataspec in a status."""
         assert source_ds.is_source()
-        stt.ready(
-            source_ds,
-            task=ADMIN_DS,
-            properties={ADMIN_DS: json.dumps(admin_ds)},
-        )
+        if source_ds.status([ADMIN_DS]) is None:
+            stt.ready(
+                source_ds,
+                task=ADMIN_DS,
+                properties={ADMIN_DS: json.dumps(admin_ds)},
+            )
 
     def default_delta(self, dataspec: st.DataSpec) -> t.Optional[float]:
         """Get the default delta of a dataspec."""
         sources_ds = dataspec.sources(sp.type_name(sp.Dataset))
         source = sources_ds.pop()
         status = source.status(task_names=[ADMIN_DS])
         if status is None:
@@ -114,15 +128,15 @@
         """Return the sarus.Client object used to make API calls."""
         return self._client
 
     def is_cached(self, dataspec: st.DataSpec) -> bool:
         """Return True if the dataspec is cached locally."""
         return True
 
-    def is_delegated(self, dataspec: st.DataSpec) -> bool:
+    def is_computation_remote(self, dataspec: st.DataSpec) -> bool:
         """Return True if the dataspec is remotely computed."""
         # `select_sql` transforms are delegated, whether mock or not
         if dataspec.is_transformed():
             transform = dataspec.transform()
             if transform.protobuf().spec.HasField("select_sql"):
                 computation_graph = self.computation_graph(dataspec)
                 referrables = (
@@ -131,14 +145,40 @@
                     + list(computation_graph["attributes"])
                 )
                 api.push_dataspec_graph(self._client, referrables)
 
         ds, _ = api.get_dataspec(self.client(), dataspec.uuid())
         return ds is not None
 
+    def is_big_data(self, dataset: st.Dataset) -> bool:
+        """Method to compute is_big data if the status
+        is not in the storage and the dataset is source
+        we retrieve it via an api call"""
+
+        last_status = self.status(dataset, task_name=BIG_DATA_TASK)
+        if last_status:
+            stage = last_status.task(task=BIG_DATA_TASK)
+            is_big = stage.properties().get(IS_BIG_DATA)
+            return is_big == str(True)
+
+        if dataset.is_source():
+            status_proto = api.dataspec_status(
+                self.client(), dataset.uuid(), task_names=[BIG_DATA_TASK]
+            )
+            stt.ready(
+                dataset,
+                manager=self,
+                task=BIG_DATA_TASK,
+                properties=status_proto.task_stages[BIG_DATA_TASK].properties,
+            )
+            return status_proto.task_stages[BIG_DATA_TASK].properties[
+                IS_BIG_DATA
+            ] == str(True)
+        return super().is_big_data(dataset)
+
     def push(self, dataspec: st.DataSpec) -> None:
         """Push a Dataspec's computation graph on the server."""
         computation_graph = self.computation_graph(dataspec)
         referrables = (
             list(computation_graph["dataspecs"])
             + list(computation_graph["transforms"])
             + list(computation_graph["attributes"])
@@ -164,28 +204,14 @@
         alt_dataspec = self.storage().referrable(alt_dataspec_uuid)
         return alt_dataspec, privacy_policy
 
     def launch(self, dataspec: st.DataSpec) -> None:
         """Launch a Dataspec's computation on the server."""
         api.launch_dataspec(self.client(), dataspec.uuid())
 
-    def _delegate_manager_status(
-        self, dataspec: st.DataSpec, task_name: str
-    ) -> t.Optional[st.Status]:
-        """Fetch a dataspec's status from the server."""
-        status_proto = api.dataspec_status(
-            client=self.client(),
-            uuid=dataspec.uuid(),
-            task_names=[task_name],
-        )
-        if status_proto is None:
-            return None
-        else:
-            return Status(protobuf=status_proto, store=True)
-
     def python_type(self, dataspec: st.DataSpec) -> str:
         """Return the Python class name of a DataSpec.
 
         This is used to instantiate the correct DataSpecWrapper class.
         """
         python_type_att = dataspec.attribute(name=PYTHON_TYPE)
         if python_type_att is not None:
@@ -410,14 +436,78 @@
         label = f"{label_type}: {symbol}{msg}"
 
         return (
             f'"{dataspec.uuid()}"[label="{label}", '
             f'fillcolor="{fillcolor}", color="{color}", shape={shape}]'
         )
 
+    async def async_schema_op(self, dataset: st.Dataset) -> st.Schema:
+        if dataset.is_transformed():
+            return await TransformedDataset(dataset).schema()
+        else:
+            raise ValueError('Dataset should be transformed.')
+
+    async def async_to_arrow_op(
+        self, dataset: st.Dataset, batch_size: int
+    ) -> t.AsyncIterator[pa.RecordBatch]:
+        """Route a Dataset to its Op implementation.
+
+        When the computation is not delegated the manager should also be
+        able to compute the value.
+        """
+        if dataset.is_transformed():
+            iterator = await TransformedDataset(dataset).to_arrow(
+                batch_size=batch_size
+            )
+            return iterator
+
+        else:
+            raise ValueError('Dataset should be transformed.')
+
+    async def async_value_op(self, scalar: st.Scalar) -> t.Any:
+        """Route a Scalar to its Op implementation.
+
+        This method is shared between API and Worker because when the data is
+        not cached the API manager should also be able to compute the value.
+        """
+        if scalar.is_transformed():
+            return await TransformedScalar(scalar).value()
+        else:
+            return await SourceScalar(scalar).value()
+
+    def copy_status_from_server(
+        self, dataspec: st.DataSpec, task_names: t.List[str]
+    ) -> None:
+        status = api.dataspec_status(
+            self.client(), dataspec.uuid(), task_names=task_names
+        )
+        for task_name in task_names:
+            stt.ready(
+                dataspec,
+                manager=self,
+                task=task_name,
+                properties=status.task_stages[task_name].properties,
+            )
+
+    def dataspec_computation(
+        self,
+        dataspec: st.DataSpec,
+    ) -> BaseComputation:
+        """Return the computation for a DataSpec."""
+        proto = dataspec.prototype()
+        if proto == sp.Dataset:
+            return self.to_arrow_computation
+        return self.value_computation
+
+    def computation_timeout(self, dataspec: st.DataSpec) -> int:
+        return 600
+
+    def computation_max_delay(self, dataspec: st.DataSpec) -> int:
+        return 10
+
 
 def manager(
     storage: storage_typing.Storage, client, **kwargs: t.Any
 ) -> SDKManager:
     """Create the SDK manager."""
     properties = {"type": "sdk_manager"}
     properties.update(kwargs)
```

### Comparing `sarus-0.5.0.dev9/sarus/manager/typing.py` & `sarus-0.6.0.dev0/sarus/manager/typing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import typing as t
 
 import sarus_data_spec.typing as st
-from sarus_data_spec.manager.asyncio.base import Computation
+from sarus_data_spec.manager.base import Computation
 from sarus_data_spec.manager.typing import Manager
 
 from sarus.typing import Client
 
 
 class SDKManager(Manager, t.Protocol):
     """The Manager of the SDK running on the client side.
```

### Comparing `sarus-0.5.0.dev9/sarus/manager/value_computation.py` & `sarus-0.6.0.dev0/sarus/manager/value_remote.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,79 +1,44 @@
-import pickle as pkl
-import traceback
 import typing as t
 
-import sarus_data_spec.protobuf as sp
-import sarus_data_spec.status as stt
 from sarus_data_spec import typing as st
-from sarus_data_spec.constants import SCALAR_TASK, ScalarCaching
-from sarus_data_spec.manager.asyncio.api.api_computation import ApiComputation
+from sarus_data_spec.constants import SCALAR_TASK
+from sarus_data_spec.manager.computations.remote.base import RemoteComputation
 
-from .cache_scalar_computation import CacheScalarComputationFromServer
-from .dataspec_api import launch_dataspec, scalar_result
-from .typing import SDKManager
+from .dataspec_api import launch_dataspec, scalar_result, dataspec_status
+import sarus_data_spec.status as stt
 
 
-class ValueComputationOnServer(ApiComputation[t.Any]):
+class ValueComputationOnServer(RemoteComputation[t.Any]):
     """ValueComputation on the Sarus server through the REST API."""
 
     task_name = SCALAR_TASK
 
-    def __init__(
-        self,
-        manager: SDKManager,
-        cache_scalar_computation: CacheScalarComputationFromServer,
-    ):
-        self._manager: SDKManager = manager
-        self.cache_scalar_computation = cache_scalar_computation
-
     def launch_task(self, dataspec: st.DataSpec) -> None:
         """Launch the computation of a Scalar on the server."""
         status = self.status(dataspec=dataspec)
         if status is None:
-            launch_dataspec(self._manager.client(), dataspec.uuid())
-            stt.pending(
-                dataspec=dataspec, manager=self.manager(), task=self.task_name
-            )
+            launch_dataspec(self.computing_manager().client(), dataspec.uuid())
 
-    async def read_ready_result(
+    async def result_from_stage_properties(
         self,
         dataspec: st.DataSpec,
         properties: t.Mapping[str, str],
         **kwargs: t.Any,
     ) -> t.Any:
-        if self.manager().is_cached(dataspec):
-            (
-                cache_type,
-                cache,
-            ) = await self.cache_scalar_computation.task_result(dataspec)
-            try:
-                if cache_type == ScalarCaching.PICKLE.value:
-                    with open(cache, "rb") as f:
-                        data = pkl.load(f)
-
-                else:
-                    data = sp.python_proto_factory(cache, cache_type)
-            except Exception:
-                stt.error(
-                    dataspec=dataspec,
-                    manager=self.manager(),
-                    task=self.task_name,
-                    properties={
-                        "message": traceback.format_exc(),
-                        "relaunch": str(True),
-                    },
-                )
-                stt.error(
-                    dataspec=dataspec,
-                    manager=self.manager(),
-                    task=self.cache_scalar_computation.task_name,
-                    properties={
-                        "message": traceback.format_exc(),
-                        "relaunch": str(True),
-                    },
-                )
-                raise stt.DataSpecErrorStatus((True, traceback.format_exc()))
-            else:
-                return data
-
-        return await scalar_result(self._manager.client(), dataspec.uuid())
+        return scalar_result(
+            self.computing_manager().client(), dataspec.uuid()
+        )
+
+    def status(self, dataspec: st.DataSpec) -> t.Optional[st.Status]:
+        """In this case, the computation retrieves the status from the server
+        via an API call, a local status is created but not stored in order
+        to use it just for the polling"""
+        status_proto = dataspec_status(
+            client=self.computing_manager().client(),
+            uuid=dataspec.uuid(),
+            task_names=[self.task_name],
+        )
+        if status_proto is None:
+            return None
+        else:
+            return stt.Status(protobuf=status_proto, store=False)
```

### Comparing `sarus-0.5.0.dev9/sarus/numpy/scalars.py` & `sarus-0.6.0.dev0/sarus/numpy/scalars.py`

 * *Files identical despite different names*

### Comparing `sarus-0.5.0.dev9/sarus/pandas/core.py` & `sarus-0.6.0.dev0/sarus/pandas/core.py`

 * *Files identical despite different names*

### Comparing `sarus-0.5.0.dev9/sarus/pandas/dataframe.py` & `sarus-0.6.0.dev0/sarus/pandas/dataframe.py`

 * *Files identical despite different names*

### Comparing `sarus-0.5.0.dev9/sarus/pandas_profiling/profile_report.py` & `sarus-0.6.0.dev0/sarus/pandas_profiling/profile_report.py`

 * *Files identical despite different names*

### Comparing `sarus-0.5.0.dev9/sarus/sarus.py` & `sarus-0.6.0.dev0/sarus/sarus.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,61 +38,66 @@
 import textwrap
 import time
 import typing as t
 import warnings
 import webbrowser
 from dataclasses import dataclass
 from io import BytesIO
+import http
 from typing import Any, Dict, List, Optional
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import pyarrow as pa
 import pyarrow.parquet as pq
 import sarus_data_spec
 from PIL import Image
 from requests import Session
 
 import sarus.typing as srt
 from sarus.dataspec_wrapper import DataSpecWrapper
-from sarus.manager.dataspec_api import compile_dataspec, pull_dataspec_graph
+from sarus.manager.dataspec_api import (
+    compile_dataspec,
+    pull_dataspec_graph,
+    get_dataspec,
+)
 from sarus.manager.typing import SDKManager
+from sarus.manager.dataspec_api import raise_response
+from sarus.pandas.dataframe import DataFrame
+from sarus_data_spec.attribute import attach_properties
 
 with warnings.catch_warnings():
     warnings.simplefilter("ignore")
     import sarus_data_spec.protobuf as sp
     import sarus_data_spec.typing as st
     from sarus_data_spec.constants import (
         ARROW_TASK,
         CACHE,
         CACHE_PATH,
         SCHEMA_TASK,
     )
     from sarus_data_spec.context import push_global_context
+    from sarus_data_spec.dataspec_rewriter.simple_rules import attach_variant
+    from sarus_data_spec.dataspec_validator.privacy_limit import (
+        DeltaEpsilonLimit,
+    )
     from sarus_data_spec.protobuf.utilities import (
         deserialize,
         dict_deserialize,
         serialize,
     )
-    from sarus_data_spec.dataspec_validator.privacy_limit import (
-        DeltaEpsilonLimit,
-    )
-    from sarus_data_spec.dataspec_rewriter.simple_rules import (
-        attach_variant,
-    )
     from sarus_data_spec.status import last_statuses, ready
     from sarus_data_spec.transform import extract, select_sql
     from sarus_data_spec.variant_constraint import (
         mock_constraint,
         pep_constraint,
     )
 
     from sarus.context.local_sdk import LocalSDKContext
-    from sarus.pandas.dataframe import DataFrame
 
     try:
         import tensorflow as tf
 
         import sarus.legacy.tensorflow as sltf
     except ModuleNotFoundError:
         pass  # error message in sarus_data_spec.typing
@@ -177,20 +182,26 @@
         type_metadata: Optional[str] = None,
         human_description: Optional[str] = None,
         marginals: Optional[str] = None,
         policy: Optional[dict] = None,
         synthetic: Dict[str, Synthetic] = None,
         transforms: List = [],
     ):
-        self.id: int = id
         self.client: "Client" = client
-        self.is_bigdata: Optional[bool] = is_bigdata
-        self.name = dataspec.properties().get("slugname")
-        self.desc = f"<Sarus Dataset slugname={self.name} id={self.id}>"
         self._set_dataspec(dataspec)
+        name = dataspec.properties().get("slugname")
+        attach_properties(
+            dataspec,
+            name=srt.ATTRIBUTES_DS,
+            properties={
+                "id": str(id),
+                "name": name,
+                "desc": f"<Sarus Dataset slugname={name} id={str(id)}>",
+            },
+        )
         self.type_metadata: Optional[Dict[str, Any]] = None
         if type_metadata is not None:
             self.type_metadata = json.loads(type_metadata)
         self.human_description: Optional[str] = human_description
         if synthetic is None:
             self._synthetic = dict(original=Synthetic(), encoded=Synthetic())
         else:
@@ -251,16 +262,20 @@
         pull_dataspec_graph(client=client, uuid=syn_dataset_uuid)
 
         syn_dataset: st.Dataset = (
             client.context().storage().referrable(syn_dataset_uuid)
         )
 
         # Update statuses
-        dataspec.status(task_names=[ARROW_TASK, SCHEMA_TASK])
-        syn_dataset.status(task_names=[ARROW_TASK, SCHEMA_TASK])
+        dataspec.manager().copy_status_from_server(
+            dataspec, task_names=[SCHEMA_TASK]
+        )
+        dataspec.manager().copy_status_from_server(
+            syn_dataset, task_names=[SCHEMA_TASK]
+        )
 
         # Create mock
         mock_dataset: st.Dataset = extract(size=dataspec.manager()._mock_size)(
             syn_dataset
         )
         mock_constraint(mock_dataset)
         attach_variant(dataspec, mock_dataset, st.ConstraintKind.MOCK)
@@ -285,15 +300,14 @@
         return cls(
             id=dataspec_id,
             dataspec=dataspec,
             client=client,
             type_metadata=admin_ds.get("type_metadata"),
             marginals=admin_ds.get("marginals"),
             human_description=admin_ds.get("human_description"),
-            is_bigdata=admin_ds.get("is_bigdata"),
         )
 
     def _split(
         self, split: t.Union[str, List[str]]
     ) -> t.Union[Dataset, List[Dataset]]:
         """Get subsets of the Sarus dataset.
 
@@ -401,15 +415,19 @@
                 for table in self.type_metadata
             }
         else:
             features: Dict[str, Dict] = self.type_metadata[0]["features"]
         return features
 
     def __repr__(self) -> str:
-        return self.desc
+        attributes_ds = self._dataspec.attribute(name=srt.ATTRIBUTES_DS)
+        if attributes_ds is not None:
+            return attributes_ds["desc"]
+        else:
+            return "<Sarus Dataset>"
 
     def _ipython_display_(self) -> None:
         """Custom ipython display."""
         print(repr(self))
 
     def as_tensorflow(
         self,
@@ -436,26 +454,28 @@
 
         Returns:
             A sarus_tensorflow.Dataset.
         """
         logging.warning(
             "'as_tensorflow()' uses the old API, not preprocessing."
         )
-        if self.is_bigdata:
+        if self._dataspec.manager().is_big_data(self._dataspec):
             raise Exception(
                 "`as_tensorflow()` is not supported for this dataset"
             )
         return sltf.Dataset(
             self,
             max_download_size=max_download_size,
             original=original,
         )
 
     def as_pandas(self) -> DataFrame:
-        if self.is_bigdata:
+        attributes_ds = self._dataspec.attribute(name=srt.ATTRIBUTES_DS)
+        assert attributes_ds is not None
+        if self._dataspec.manager().is_big_data(self._dataspec):
             raise Exception("`as_pandas()` is not supported for this dataset")
         return DataFrame.from_dataspec(self._dataspec)
 
     def __getitem__(self, item: t.List[str]) -> Dataset:
         return self.table(item)
 
     def table(self, table_name: t.List[str]) -> Dataset:
@@ -503,16 +523,27 @@
         )
         selected_ds = sarus_data_spec.transform.get_item(path=table_path)(
             filtered_ds
         )
 
         # create dataset
         table_ds = Dataset.from_dataspec(selected_ds)
-        table_ds.desc = f"<Sarus Table name={table_name}>"
-        table_ds.is_bigdata = self.is_bigdata
+
+        attributes_ds = self._dataspec.attribute(name=srt.ATTRIBUTES_DS)
+        assert attributes_ds is not None
+        name = f"<Sarus Table name={table_name}>"
+        attach_properties(
+            selected_ds,
+            name=srt.ATTRIBUTES_DS,
+            properties={
+                "id": attributes_ds["id"],
+                "name": name,
+                "desc": f"<Sarus Table name={table_name}>",
+            },
+        )
 
         return table_ds
 
     def tables(self) -> t.List[t.List[str]]:
         """For given parameters of a Sarus Dataset return a list
         of Sarus Tables."""
         dataspec_tables = [
@@ -531,32 +562,41 @@
         Args:
             query (str): SQL query
 
         Returns:
             an instance of Sarus Dataset.
         """
         ds = select_sql(query)(self._dataspec)
+        attributes_ds = self._dataspec.attribute(name=srt.ATTRIBUTES_DS)
+        assert attributes_ds is not None
+        attach_properties(
+            ds,
+            name=srt.ATTRIBUTES_DS,
+            properties={
+                "id": attributes_ds["id"],
+                "name": attributes_ds["name"],
+                "desc": f"<Sarus Dataset query='{query}'>",
+            },
+        )
         ds_wrapper = self.from_dataspec(ds)
-        ds_wrapper.name = self.name
-        ds_wrapper.id = self.id
-        ds_wrapper.is_bigdata = False
-        ds_wrapper.desc = f"<Sarus Dataset query='{query}'>"
         return ds_wrapper
 
     @property
     def epsilon(self) -> float:
         """Retrieve the remaining global privacy budget (epsilon) of the
         current access rule.
 
         Returns:
             float: The remaining privacy budget (global epsilon) of the access
             rule.
         """
+        attributes_ds = self._dataspec.attribute(name=srt.ATTRIBUTES_DS)
+        assert attributes_ds is not None
         resp = self.client.session().get(
-            f"{self.client.base_url}/datasets/{self.id}",
+            f"{self.client.base_url}/datasets/{attributes_ds['id']}",
         )
         if resp.status_code > 200:
             raise Exception(
                 f"Error while retrieving the current value of epsilon. "
                 f"Gateway answer was: \n{resp}"
             )
         return float(resp.json()["accesses"][0]["current_epsilon"])
@@ -566,16 +606,18 @@
         """Retrieve the maximum global privacy budget (epsilon) granted by the
         Data preparator, for the current access rule.
 
         Returns:
             float: The maximum privacy budget (global epsilon) of the access
             rule.
         """
+        attributes_ds = self._dataspec.attribute(name=srt.ATTRIBUTES_DS)
+        assert attributes_ds is not None
         resp = self.client.session().get(
-            f"{self.client.base_url}/datasets/{self.id}",
+            f"{self.client.base_url}/datasets/{attributes_ds['id']}",
         )
         if resp.status_code > 200:
             raise Exception(
                 f"Error while retrieving the current value of epsilon. "
                 f"Gateway answer was: \n{resp}"
             )
         return float(resp.json()["accesses"][0]["max_epsilon"])
@@ -625,15 +667,18 @@
         has_enough_synthetic = (
             self._synthetic[synthetic_type].rows is not None
             and rows_number <= self._synthetic[synthetic_type].rows
         )
 
         if not has_enough_synthetic or force_refresh:
             # Fetch synthetic data
-            uri = f"{self.client.base_url}/synthetic_data/{self.id}"
+            attributes_ds = self._dataspec.attribute(name=srt.ATTRIBUTES_DS)
+            uri = (
+                f"{self.client.base_url}/synthetic_data/{attributes_ds['id']}"
+            )
             if table_name is not None:
                 uri = f"{uri}/{table_name}"
 
             resp = self.client.session().get(
                 uri,
                 stream=True,
                 params={
@@ -1123,114 +1168,83 @@
 
         Returns:
             None
         """
         manager: SDKManager = self.context().manager()
 
         user_ds = wrapper.dataspec(srt.DataSpecVariant.USER_DEFINED)
-        synth_ds = wrapper.dataspec(srt.DataSpecVariant.SYNTHETIC)
-        mock_ds = wrapper.dataspec(srt.DataSpecVariant.MOCK)
-
-        user_graph = manager.computation_graph(user_ds)
-        mock_graph = manager.computation_graph(mock_ds)
-
-        user_refs = (
-            set(user_graph["dataspecs"])
-            | set(user_graph["transforms"])
-            | set(user_graph["attributes"])
-            | set(user_graph["variant_constraints"])
-        )
-
-        synth_refs = {synth_ds}
-
-        mock_refs = (
-            set(mock_graph["dataspecs"])
-            | set(mock_graph["transforms"])
-            | set(mock_graph["attributes"])
-            | set(mock_graph["variant_constraints"])
-        )
-
-        refs = user_refs | synth_refs | mock_refs
-        serialized_refs = [serialize(ref.protobuf()) for ref in refs]
+        manager.push(user_ds)
 
-        file_obj = tarfile.open(path, "w")
-
-        with open("data", "wb") as f:
-            pkl.dump(
-                {
-                    "serialized_obj": serialized_refs,
-                    "user_defined": user_ds.uuid(),
-                },
-                f,
-            )
-        file_obj.add("data")
-        os.remove("data")
+        saved_data = {
+            "user_ds_uuid": user_ds.uuid(),
+            "wrapper_type": type(wrapper).__name__,
+        }
 
-        # saving the cache is there is one for the mock
-        wrapper._mock_value()
-        for last_status in last_statuses(mock_ds, task=CACHE):
-            task_stage = last_status.task(CACHE)
-            if task_stage and task_stage.ready():
-                path_cache = task_stage[CACHE_PATH]
-                cache_name = os.path.basename(path_cache)
-                file_obj.add(path_cache, arcname=cache_name)
-        file_obj.close()
+        with open(path, "w") as save_file:
+            json.dump(saved_data, save_file)
 
-    def load(self, path: str) -> srt.DataSpecWrapper:
+    def load(
+        self,
+        path=None,
+        uuid=None,
+        to_dataset: bool = False,
+    ) -> srt.DataSpecWrapper:
         """Load a sarus object from a path.
 
         Args:
             path (str): The file path to load the sarus object from.
 
         Returns:
             DataSpecWrapper: The sarus object (eg: DataFrame,model..).
         """
-        with tarfile.open(path, mode="r") as tar:
-            tar.extract("data")
-            with open("data", "rb") as f:
-                data = pkl.load(f)
-            os.remove("data")
-        tar.close()
-
-        refs = data["serialized_obj"]
-        user_defined = data["user_defined"]
-
-        factory = self.context().factory()
-        storage = self.context().storage()
-        # Two passes to have all the correct referrings
-        refs = [factory.create(deserialize(ref)) for ref in refs]
-        _ = [storage.store(ref) for ref in refs]
-
-        user_ds = self.context().storage().referrable(user_defined)
-        mock_ds = user_ds.variant(st.ConstraintKind.MOCK)
-
-        # loading the cache of the mock (only for the dataspec we load)
-        with tarfile.open(path, mode="r") as tar:
-            tar_filenames = tar.getnames()
-            for filename in tar_filenames:
-                if f"{mock_ds.uuid()}" in filename:
-                    cache_dir = self.context().manager().parquet_dir()
-                    path_cache = os.path.join(cache_dir, filename)
-                    tar.extract(filename, cache_dir)
-                    ready(
-                        mock_ds,
-                        CACHE,
-                        properties={CACHE_PATH: path_cache},
-                    )
-        tar.close()
-        return self.context().wrapper_factory().create(user_ds)
+        if path is None and uuid is None:
+            raise ValueError(
+                "You must provide either argument 'path' or 'uuid'."
+            )
+
+        if uuid is not None:
+            user_ds_uuid = uuid
+            wrapper_type = None
+        elif path is not None:
+            with open(path, "r") as load_file:
+                saved_data = json.load(load_file)
+
+            user_ds_uuid = saved_data["user_ds_uuid"]
+            wrapper_type = saved_data["wrapper_type"]
+
+        pull_dataspec_graph(client=self, uuid=user_ds_uuid)
+        ds, _ = get_dataspec(client=self, uuid=user_ds_uuid)
+
+        sources_ds = ds.sources(sp.type_name(sp.Dataset))
+        for source in sources_ds:
+            if not source.is_public():
+                self.dataset(source["slugname"])
+
+        if to_dataset and ds.prototype() == sp.Dataset:
+            loaded_wrapper = Dataset.from_dataspec(ds)
+        elif wrapper_type is not None and ds.prototype() == sp.Dataset:
+            if wrapper_type == "Dataset":
+                loaded_wrapper = Dataset.from_dataspec(ds)
+            else:
+                loaded_wrapper = DataFrame.from_dataspec(ds)
+        else:
+            # scalar must be created using the python type
+            # transformed dataset also for now
+            loaded_wrapper = self.context().wrapper_factory().create(ds)
+
+        return loaded_wrapper
 
     def _oidc_login(self):
         oidc_login_url = f"{self.base_url}/oidc_login?headless=true"
         try:
             from IPython.display import Javascript, clear_output
 
-            display(  # noqa: F821
+            display(
                 Javascript(f'window.open("{oidc_login_url}");')
-            )
+            )  # noqa: F821
             display(clear_output())  # noqa: F821
         except Exception:
             webbrowser.open(oidc_login_url)
         token = getpass.getpass(
             "Logging in via google.\nYou will be redirected to a login page "
             "where you will obtain a token to paste below.\nIf you are not "
             f"redirected automatically, you can visit {oidc_login_url}\n"
@@ -1273,23 +1287,25 @@
     def _available_datasets(self) -> List[str]:
         """List available datasets.
 
         Returns:
             List[str]: list of available dataset names.
         """
         request = self.session().get(f"{self.base_url}/datasets")
+        raise_response(request)
         return [ds["name"] for ds in request.json()]
 
     def list_datasets(self) -> DatasetList:
         """List available Sarus datasets.
 
         Returns:
             DatasetList: List of available Sarus datasets.
         """
         request = self.session().get(f"{self.base_url}/datasets")
+        raise_response(request)
         unsorted_datasets = [
             ShallowDataset._from_dict(ds_json)
             for ds_json in request.json()
             if ds_json["status"] == "ready"
         ]
         sorted_datasets = sorted(
             unsorted_datasets,
@@ -1322,14 +1338,15 @@
         Args:
             id (int): id of the dataset to be fetched
 
         Returns:
             an instance of Dataset
         """
         request = self.session().get(f"{self.base_url}/datasets/{id}")
+        raise_response(request)
         dataset = Dataset._from_dict(request.json(), self)
         return dataset
 
     def _fetch_dataset_by_name(self, name: str) -> Dataset:
         """Fetch a dataset from the Sarus Gateway.
 
         Args:
@@ -1337,14 +1354,15 @@
 
         Returns:
             Dataset: an instance of Dataset
         """
         request = self.session().get(
             f"{self.base_url}/datasets/name/{name}",
         )
+        raise_response(request)
         dataset = Dataset._from_dict(request.json(), self)
         return dataset
 
     def query(
         self,
         query: str,
         target_epsilon: Optional[float] = None,
@@ -1387,34 +1405,38 @@
         )
         if request.status_code > 200:
             if request.status_code == 403:
                 raise ValueError(
                     "Query failed with the following error: Privacy budget "
                     "limit exceeded"
                 )
-            if request.status_code == 404:
-                raise ValueError(
-                    "Couldn't run the query: wrong table name or unauthorised "
-                    "access"
-                )
-            raise Exception(
-                f"Error while sending a query.\
-                                                     Full Gateway answer was:{request}"
-            )
+            else:
+                http_status_code = request.status_code
+                http_status_name = http.HTTPStatus(http_status_code).name
+                try:
+                    error_message = request.json()["error_message"]
+                    wrapped_message = textwrap.indent(error_message, "  |")
+
+                    raise Exception(
+                        f"{http_status_code} - {http_status_name}: {wrapped_message}"
+                    )
+                except (json.JSONDecodeError, KeyError):
+                    raise Exception(
+                        f"Error while sending a query.\
+                                                             Full Gateway answer was:{request}"
+                    )
 
         task_id = request.json()["task"]
         dataset_id = request.json()["dataset"]["id"]
         start_eps = request.json()["dataset"]["accesses"][0]["current_epsilon"]
         status = self._poll_query_status(task_id)
         error_message = status.get("error_message", None)
         if error_message is not None:
-            raise RuntimeError(
-                f"Query failed with the following error:\n"
-                f"{textwrap.indent(error_message, '  |')}"
-            )
+            wrapped_message = textwrap.indent(error_message, "  |")
+            raise Exception(wrapped_message)
         if verbose:
             ds = self._fetch_dataset_by_id(dataset_id)
             logging.info(
                 f"Actual privacy consumption (epsilon): "
                 f"{ds.epsilon-start_eps:.03f}"
             )
```

### Comparing `sarus-0.5.0.dev9/sarus/scripts/generate_op_list.py` & `sarus-0.6.0.dev0/sarus/scripts/generate_op_list.py`

 * *Files identical despite different names*

### Comparing `sarus-0.5.0.dev9/sarus/sklearn/__init__.py` & `sarus-0.6.0.dev0/sarus/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `sarus-0.5.0.dev9/sarus/sklearn/cluster.py` & `sarus-0.6.0.dev0/sarus/sklearn/cluster.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from __future__ import annotations
 
 import numpy as np
 import sarus_data_spec.protobuf as sp
 
 from sarus.dataspec_wrapper import DataSpecWrapper
-from sarus.utils import register_ops, sarus_method, sarus_model
+from sarus.utils import register_ops, sarus_method, sarus_init
 
 try:
     from sklearn import cluster
     from sklearn.cluster import *
 except ModuleNotFoundError:
     pass  # error message in sarus_data_spec.typing
 
 
 class AffinityPropagation(DataSpecWrapper[cluster.AffinityPropagation]):
-    @sarus_model(sp.Scalar.Model.ModelClass.SK_AFFINITY_PROPAGATION)
+    @sarus_init("sklearn.SK_AFFINITY_PROPAGATION")
     def __init__(
         self,
         *,
         damping=0.5,
         max_iter=200,
         convergence_iter=15,
         copy=True,
@@ -33,15 +33,15 @@
     def fit(self, X, y=None):
         ...
 
 
 class AgglomerativeClustering(
     DataSpecWrapper[cluster.AgglomerativeClustering]
 ):
-    @sarus_model(sp.Scalar.Model.ModelClass.SK_AGGLOMERATIVE_CLUSTERING)
+    @sarus_init("sklearn.SK_AGGLOMERATIVE_CLUSTERING")
     def __init__(
         self,
         n_clusters=2,
         *,
         affinity="euclidean",
         memory=None,
         connectivity=None,
@@ -54,15 +54,15 @@
 
     @sarus_method("sklearn.SK_FIT", inplace=True)
     def fit(self, X, y=None):
         ...
 
 
 class Birch(DataSpecWrapper[cluster.Birch]):
-    @sarus_model(sp.Scalar.Model.ModelClass.SK_BIRCH)
+    @sarus_init("sklearn.SK_BIRCH")
     def __init__(
         self,
         *,
         threshold=0.5,
         branching_factor=50,
         n_clusters=3,
         compute_labels=True,
@@ -73,15 +73,15 @@
 
     @sarus_method("sklearn.SK_FIT", inplace=True)
     def fit(self, X, y=None):
         ...
 
 
 class DBSCAN(DataSpecWrapper[cluster.DBSCAN]):
-    @sarus_model(sp.Scalar.Model.ModelClass.SK_DBSCAN)
+    @sarus_init("sklearn.SK_DBSCAN")
     def __init__(
         self,
         eps=0.5,
         *,
         min_samples=5,
         metric="euclidean",
         metric_params=None,
@@ -95,15 +95,15 @@
 
     @sarus_method("sklearn.SK_FIT", inplace=True)
     def fit(self, X, y=None):
         ...
 
 
 class FeatureAgglomeration(DataSpecWrapper[cluster.FeatureAgglomeration]):
-    @sarus_model(sp.Scalar.Model.ModelClass.SK_AFFINITY_PROPAGATION)
+    @sarus_init("sklearn.SK_AFFINITY_PROPAGATION")
     def __init__(
         self,
         n_clusters=2,
         *,
         affinity="euclidean",
         memory=None,
         connectivity=None,
@@ -117,15 +117,15 @@
 
     @sarus_method("sklearn.SK_FIT", inplace=True)
     def fit(self, X, y=None):
         ...
 
 
 class KMeans(DataSpecWrapper[cluster.KMeans]):
-    @sarus_model(sp.Scalar.Model.ModelClass.SK_KMEANS)
+    @sarus_init("sklearn.SK_KMEANS")
     def __init__(
         self,
         n_clusters=8,
         *,
         init="k-means++",
         n_init=10,
         max_iter=300,
@@ -142,15 +142,15 @@
 
     @sarus_method("sklearn.SK_FIT", inplace=True)
     def fit(self, X, y=None):
         ...
 
 
 class MiniBatchKMeans(DataSpecWrapper[cluster.MiniBatchKMeans]):
-    @sarus_model(sp.Scalar.Model.ModelClass.SK_MINIBATCH_KMEANS)
+    @sarus_init("sklearn.SK_MINIBATCH_KMEANS")
     def __init__(
         self,
         n_clusters=8,
         *,
         init="k-means++",
         max_iter=100,
         batch_size=100,
@@ -168,15 +168,15 @@
 
     @sarus_method("sklearn.SK_FIT", inplace=True)
     def fit(self, X, y=None):
         ...
 
 
 class MeanShift(DataSpecWrapper[cluster.MeanShift]):
-    @sarus_model(sp.Scalar.Model.ModelClass.SK_MEAN_SHIFT)
+    @sarus_init("sklearn.SK_MEAN_SHIFT")
     def __init__(
         self,
         *,
         bandwidth=None,
         seeds=None,
         bin_seeding=False,
         min_bin_freq=1,
@@ -189,15 +189,15 @@
 
     @sarus_method("sklearn.SK_FIT", inplace=True)
     def fit(self, X, y=None):
         ...
 
 
 class OPTICS(DataSpecWrapper[cluster.OPTICS]):
-    @sarus_model(sp.Scalar.Model.ModelClass.SK_OPTICS)
+    @sarus_init("sklearn.SK_OPTICS")
     def __init__(
         self,
         *,
         min_samples=5,
         max_eps=np.inf,
         metric="minkowski",
         p=2,
@@ -216,15 +216,15 @@
 
     @sarus_method("sklearn.SK_FIT", inplace=True)
     def fit(self, X, y=None):
         ...
 
 
 class SpectralClustering(DataSpecWrapper[cluster.SpectralClustering]):
-    @sarus_model(sp.Scalar.Model.ModelClass.SK_SPECTRAL_CLUSTERING)
+    @sarus_init("sklearn.SK_SPECTRAL_CLUSTERING")
     def __init__(
         self,
         n_clusters=8,
         *,
         eigen_solver=None,
         n_components=None,
         random_state=None,
@@ -244,15 +244,15 @@
 
     @sarus_method("sklearn.SK_FIT", inplace=True)
     def fit(self, X, y=None):
         ...
 
 
 class SpectralBiclustering(DataSpecWrapper[cluster.SpectralBiclustering]):
-    @sarus_model(sp.Scalar.Model.ModelClass.SK_SPECTRAL_BICLUSTERING)
+    @sarus_init("sklearn.SK_SPECTRAL_BICLUSTERING")
     def __init__(
         self,
         n_clusters=3,
         *,
         method="bistochastic",
         n_components=6,
         n_best=3,
@@ -269,15 +269,15 @@
 
     @sarus_method("sklearn.SK_FIT", inplace=True)
     def fit(self, X, y=None):
         ...
 
 
 class SpectralCoclustering(DataSpecWrapper[cluster.SpectralCoclustering]):
-    @sarus_model(sp.Scalar.Model.ModelClass.SK_AFFINITY_PROPAGATION)
+    @sarus_init("sklearn.SK_AFFINITY_PROPAGATION")
     def __init__(
         self,
         n_clusters=3,
         *,
         svd_method="randomized",
         n_svd_vecs=None,
         mini_batch=False,
```

### Comparing `sarus-0.5.0.dev9/sarus/sklearn/compose.py` & `sarus-0.6.0.dev0/sarus/sklearn/compose.py`

 * *Files identical despite different names*

### Comparing `sarus-0.5.0.dev9/sarus/sklearn/decomposition.py` & `sarus-0.6.0.dev0/sarus/sklearn/decomposition.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from __future__ import annotations
 
 import sarus_data_spec.protobuf as sp
 
 from sarus.dataspec_wrapper import DataSpecWrapper
-from sarus.utils import register_ops, sarus_method, sarus_model
+from sarus.utils import register_ops, sarus_method, sarus_init
 
 try:
     import sklearn.decomposition as decomposition
     from sklearn.decomposition import *
 except ModuleNotFoundError:
     pass  # error message in sarus_data_spec.typing
 
 
 class PCA(DataSpecWrapper[decomposition.PCA]):
-    @sarus_model(sp.Scalar.Model.ModelClass.SK_PCA)
+    @sarus_init("sklearn.SK_PCA")
     def __init__(
         self,
         n_components=None,
         *,
         copy=True,
         whiten=False,
         svd_solver="auto",
```

### Comparing `sarus-0.5.0.dev9/sarus/sklearn/ensemble.py` & `sarus-0.6.0.dev0/sarus/sklearn/ensemble.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from __future__ import annotations
 
 import sarus_data_spec.protobuf as sp
 
 from sarus.dataspec_wrapper import DataSpecWrapper
-from sarus.utils import register_ops, sarus_method, sarus_model
+from sarus.utils import register_ops, sarus_method, sarus_init
 
 try:
     import sklearn.ensemble as ensemble
     from sklearn.ensemble import *
 except ModuleNotFoundError:
     pass  # error message in sarus_data_spec.typing
 
 
 class AdaBoostClassifier(DataSpecWrapper[ensemble.AdaBoostClassifier]):
-    @sarus_model(sp.Scalar.Model.ModelClass.SK_ADABOOST_CLASSIFIER)
+    @sarus_init("sklearn.SK_ADABOOST_CLASSIFIER")
     def __init__(
         self,
         base_estimator=None,
         *,
         n_estimators=50,
         learning_rate=1.0,
         algorithm="SAMME.R",
@@ -28,15 +28,15 @@
 
     @sarus_method("sklearn.SK_FIT", inplace=True)
     def fit(self, X, y=None):
         ...
 
 
 class AdaBoostRegressor(DataSpecWrapper[ensemble.AdaBoostRegressor]):
-    @sarus_model(sp.Scalar.Model.ModelClass.SK_ADABOOST_REGRESSOR)
+    @sarus_init("sklearn.SK_ADABOOST_REGRESSOR")
     def __init__(
         self,
         base_estimator=None,
         *,
         n_estimators=50,
         learning_rate=1.0,
         loss="linear",
@@ -47,15 +47,15 @@
 
     @sarus_method("sklearn.SK_FIT", inplace=True)
     def fit(self, X, y=None):
         ...
 
 
 class BaggingClassifier(DataSpecWrapper[ensemble.BaggingClassifier]):
-    @sarus_model(sp.Scalar.Model.ModelClass.SK_BAGGING_CLASSIFIER)
+    @sarus_init("sklearn.SK_BAGGING_CLASSIFIER")
     def __init__(
         self,
         base_estimator=None,
         n_estimators=10,
         *,
         max_samples=1.0,
         max_features=1.0,
@@ -72,15 +72,15 @@
 
     @sarus_method("sklearn.SK_FIT", inplace=True)
     def fit(self, X, y=None):
         ...
 
 
 class BaggingRegressor(DataSpecWrapper[ensemble.BaggingRegressor]):
-    @sarus_model(sp.Scalar.Model.ModelClass.SK_BAGGING_REGRESSOR)
+    @sarus_init("sklearn.SK_BAGGING_REGRESSOR")
     def __init__(
         self,
         base_estimator=None,
         *,
         n_estimators=50,
         learning_rate=1.0,
         loss="linear",
@@ -91,15 +91,15 @@
 
     @sarus_method("sklearn.SK_FIT", inplace=True)
     def fit(self, X, y=None):
         ...
 
 
 class ExtraTreesClassifier(DataSpecWrapper[ensemble.ExtraTreesClassifier]):
-    @sarus_model(sp.Scalar.Model.ModelClass.SK_EXTRA_TREES_CLASSIFIER)
+    @sarus_init("sklearn.SK_EXTRA_TREES_CLASSIFIER")
     def __init__(
         self,
         n_estimators=100,
         *,
         criterion="gini",
         max_depth=None,
         min_samples_split=2,
@@ -123,15 +123,15 @@
 
     @sarus_method("sklearn.SK_FIT", inplace=True)
     def fit(self, X, y=None):
         ...
 
 
 class ExtraTreesRegressor(DataSpecWrapper[ensemble.ExtraTreesRegressor]):
-    @sarus_model(sp.Scalar.Model.ModelClass.SK_EXTRA_TREES_REGRESSOR)
+    @sarus_init("sklearn.SK_EXTRA_TREES_REGRESSOR")
     def __init__(
         self,
         n_estimators=100,
         *,
         criterion="squared_error",
         max_depth=None,
         min_samples_split=2,
@@ -156,15 +156,15 @@
     def fit(self, X, y=None):
         ...
 
 
 class GradientBoostingClassifier(
     DataSpecWrapper[ensemble.GradientBoostingClassifier]
 ):
-    @sarus_model(sp.Scalar.Model.ModelClass.SK_GRADIENT_BOOSTING_CLASSIFIER)
+    @sarus_init("sklearn.SK_GRADIENT_BOOSTING_CLASSIFIER")
     def __init__(
         self,
         *,
         loss="log_loss",
         learning_rate=0.1,
         n_estimators=100,
         subsample=1.0,
@@ -192,15 +192,15 @@
     def fit(self, X, y=None):
         ...
 
 
 class GradientBoostingRegressor(
     DataSpecWrapper[ensemble.GradientBoostingRegressor]
 ):
-    @sarus_model(sp.Scalar.Model.ModelClass.SK_GRADIENT_BOOSTING_REGRESSOR)
+    @sarus_init("sklearn.SK_GRADIENT_BOOSTING_REGRESSOR")
     def __init__(
         self,
         *,
         loss="squared_error",
         learning_rate=0.1,
         n_estimators=100,
         subsample=1.0,
@@ -227,15 +227,15 @@
 
     @sarus_method("sklearn.SK_FIT", inplace=True)
     def fit(self, X, y=None):
         ...
 
 
 class IsolationForest(DataSpecWrapper[ensemble.IsolationForest]):
-    @sarus_model(sp.Scalar.Model.ModelClass.SK_ISOLATION_FOREST)
+    @sarus_init("sklearn.SK_ISOLATION_FOREST")
     def __init__(
         self,
         *,
         n_estimators=100,
         max_samples="auto",
         contamination="auto",
         max_features=1.0,
@@ -250,15 +250,15 @@
 
     @sarus_method("sklearn.SK_FIT", inplace=True)
     def fit(self, X, y=None):
         ...
 
 
 class RandomForestClassifier(DataSpecWrapper[ensemble.RandomForestClassifier]):
-    @sarus_model(sp.Scalar.Model.ModelClass.SK_RANDOM_FOREST_CLASSIFIER)
+    @sarus_init("sklearn.SK_RANDOM_FOREST_CLASSIFIER")
     def __init__(
         self,
         n_estimators=100,
         *,
         criterion="gini",
         max_depth=None,
         min_samples_split=2,
@@ -286,15 +286,15 @@
 
     @sarus_method("sklearn.SK_PREDICT")
     def predict(self, X):
         ...
 
 
 class RandomForestRegressor(DataSpecWrapper[ensemble.RandomForestRegressor]):
-    @sarus_model(sp.Scalar.Model.ModelClass.SK_RANDOM_FOREST_REGRESSOR)
+    @sarus_init("sklearn.SK_RANDOM_FOREST_REGRESSOR")
     def __init__(
         self,
         n_estimators=100,
         *,
         criterion="squared_error",
         max_depth=None,
         min_samples_split=2,
@@ -317,15 +317,15 @@
 
     @sarus_method("sklearn.SK_FIT", inplace=True)
     def fit(self, X, y=None):
         ...
 
 
 class RandomTreesEmbedding(DataSpecWrapper[ensemble.RandomTreesEmbedding]):
-    @sarus_model(sp.Scalar.Model.ModelClass.SK_RANDOM_TREES_EMBEDDING)
+    @sarus_init("sklearn.SK_RANDOM_TREES_EMBEDDING")
     def __init__(
         self,
         n_estimators=100,
         *,
         max_depth=5,
         min_samples_split=2,
         min_samples_leaf=1,
@@ -343,15 +343,15 @@
 
     @sarus_method("sklearn.SK_FIT", inplace=True)
     def fit(self, X, y=None):
         ...
 
 
 class StackingClassifier(DataSpecWrapper[ensemble.StackingClassifier]):
-    @sarus_model(sp.Scalar.Model.ModelClass.SK_STACKING_CLASSIFIER)
+    @sarus_init("sklearn.SK_STACKING_CLASSIFIER")
     def __init__(
         self,
         estimators,
         final_estimator=None,
         *,
         cv=None,
         stack_method="auto",
@@ -364,15 +364,15 @@
 
     @sarus_method("sklearn.SK_FIT", inplace=True)
     def fit(self, X, y=None):
         ...
 
 
 class StackingRegressor(DataSpecWrapper[ensemble.StackingRegressor]):
-    @sarus_model(sp.Scalar.Model.ModelClass.SK_STACKING_REGRESSOR)
+    @sarus_init("sklearn.SK_STACKING_REGRESSOR")
     def __init__(
         self,
         estimators,
         final_estimator=None,
         *,
         cv=None,
         stack_method="auto",
@@ -385,15 +385,15 @@
 
     @sarus_method("sklearn.SK_FIT", inplace=True)
     def fit(self, X, y=None):
         ...
 
 
 class VotingClassifier(DataSpecWrapper[ensemble.VotingClassifier]):
-    @sarus_model(sp.Scalar.Model.ModelClass.SK_VOTING_CLASSIFIER)
+    @sarus_init("sklearn.SK_VOTING_CLASSIFIER")
     def __init__(
         self,
         estimators,
         *,
         voting="hard",
         weights=None,
         n_jobs=None,
@@ -405,15 +405,15 @@
 
     @sarus_method("sklearn.SK_FIT", inplace=True)
     def fit(self, X, y=None):
         ...
 
 
 class VotingRegressor(DataSpecWrapper[ensemble.VotingRegressor]):
-    @sarus_model(sp.Scalar.Model.ModelClass.SK_VOTING_REGRESSOR)
+    @sarus_init("sklearn.SK_VOTING_REGRESSOR")
     def __init__(
         self,
         estimators,
         *,
         weights=None,
         n_jobs=None,
         verbose=False,
@@ -425,17 +425,15 @@
     def fit(self, X, y=None):
         ...
 
 
 class HistGradientBoostingClassifier(
     DataSpecWrapper[ensemble.HistGradientBoostingClassifier]
 ):
-    @sarus_model(
-        sp.Scalar.Model.ModelClass.SK_HIST_GRADIENT_BOOSTING_CLASSIFIER
-    )
+    @sarus_init("sklearn.SK_HIST_GRADIENT_BOOSTING_CLASSIFIER")
     def __init__(
         self,
         loss="log_loss",
         *,
         learning_rate=0.1,
         max_iter=100,
         max_leaf_nodes=31,
@@ -464,17 +462,15 @@
     def fit(self, X, y=None):
         ...
 
 
 class HistGradientBoostingRegressor(
     DataSpecWrapper[ensemble.HistGradientBoostingRegressor]
 ):
-    @sarus_model(
-        sp.Scalar.Model.ModelClass.SK_HIST_GRADIENT_BOOSTING_REGRESSOR
-    )
+    @sarus_init("sklearn.SK_HIST_GRADIENT_BOOSTING_REGRESSOR")
     def __init__(
         self,
         estimators,
         *,
         weights=None,
         n_jobs=None,
         verbose=False,
```

### Comparing `sarus-0.5.0.dev9/sarus/sklearn/impute.py` & `sarus-0.6.0.dev0/sarus/sklearn/impute.py`

 * *Files identical despite different names*

### Comparing `sarus-0.5.0.dev9/sarus/sklearn/linear_model.py` & `sarus-0.6.0.dev0/sarus/sklearn/linear_model.py`

 * *Files identical despite different names*

### Comparing `sarus-0.5.0.dev9/sarus/sklearn/model_selection.py` & `sarus-0.6.0.dev0/sarus/sklearn/model_selection.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sarus_data_spec.protobuf as sp
 
 from sarus.dataspec_wrapper import DataSpecWrapper
-from sarus.utils import register_ops, sarus_init, sarus_model
+from sarus.utils import register_ops, sarus_init
 
 try:
     import sklearn.model_selection as sk_model_selection
     from sklearn.model_selection import *
 except ModuleNotFoundError:
     pass  # error message in sarus_data_spec.typing
 
@@ -22,26 +22,26 @@
     ):
         ...
 
 
 class RepeatedStratifiedKFold(
     DataSpecWrapper[sk_model_selection.RepeatedStratifiedKFold]
 ):
-    @sarus_model(sp.Scalar.Model.ModelClass.SK_REPEATED_STRATIFIED_KFOLD)
+    @sarus_init("sklearn.SK_REPEATED_STRATIFIED_KFOLD")
     def __init__(
         self,
         *,
         n_splits=5,
         n_repeats=10,
         random_state=None,
         _dataspec=None,
     ):
         ...
 
 
 class KFold(DataSpecWrapper[sk_model_selection.KFold]):
-    @sarus_model(sp.Scalar.Model.ModelClass.SK_KFOLD)
+    @sarus_init("sklearn.SK_KFOLD")
     def __init__(self, n_splits=5, *, shuffle=False, random_state=None):
         ...
 
 
 register_ops()
```

### Comparing `sarus-0.5.0.dev9/sarus/sklearn/pipeline.py` & `sarus-0.6.0.dev0/sarus/sklearn/pipeline.py`

 * *Files identical despite different names*

### Comparing `sarus-0.5.0.dev9/sarus/sklearn/preprocessing.py` & `sarus-0.6.0.dev0/sarus/sklearn/preprocessing.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import numpy as np
 import sarus_data_spec.protobuf as sp
 
 from sarus.dataspec_wrapper import DataSpecWrapper
-from sarus.utils import register_ops, sarus_init, sarus_method, sarus_model
+from sarus.utils import register_ops, sarus_init, sarus_method
 
 try:
     import sklearn.preprocessing as sk_preprocessing
     from sklearn.preprocessing import *
 except ModuleNotFoundError:
     pass  # error message in sarus_data_spec.typing
 
 
 class OneHotEncoder(DataSpecWrapper[sk_preprocessing.OneHotEncoder]):
-    @sarus_model(sp.Scalar.Model.ModelClass.SK_ONEHOT)
+    @sarus_init("sklearn.SK_ONEHOT")
     def __init__(
         self,
         *,
         categories="auto",
         drop=None,
         sparse=True,
         dtype=np.float64,
@@ -27,15 +27,15 @@
 
     @sarus_method("sklearn.SK_FIT", inplace=True)
     def fit(self, X, y=None):
         ...
 
 
 class LabelEncoder(DataSpecWrapper[sk_preprocessing.LabelEncoder]):
-    @sarus_model(sp.Scalar.Model.ModelClass.SK_LABEL_ENCODER)
+    @sarus_init("sklearn.SK_LABEL_ENCODER")
     def __init__(
         self,
         *,
         _dataspec=None,
     ):
         ...
```

### Comparing `sarus-0.5.0.dev9/sarus/sklearn/svm.py` & `sarus-0.6.0.dev0/sarus/sklearn/svm.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from __future__ import annotations
 
 import sarus_data_spec.protobuf as sp
 
 from sarus.dataspec_wrapper import DataSpecWrapper
-from sarus.utils import register_ops, sarus_method, sarus_model
+from sarus.utils import register_ops, sarus_init, sarus_method
 
 try:
     import sklearn.svm as svm
     from sklearn.svm import *
 except ModuleNotFoundError:
     pass  # error message in sarus_data_spec.typing
 
 
 class SVC(DataSpecWrapper[svm.SVC]):
-    @sarus_model(sp.Scalar.Model.ModelClass.SK_SVC)
+    @sarus_init("sklearn.SK_SVC")
     def __init__(self, *args, **kwargs) -> None:
         ...
 
     @sarus_method("sklearn.SK_FIT", inplace=True)
     def fit(self, X, y, sample_weight=None):
         ...
```

### Comparing `sarus-0.5.0.dev9/sarus/skopt/searchcv.py` & `sarus-0.6.0.dev0/sarus/skopt/searchcv.py`

 * *Files identical despite different names*

### Comparing `sarus-0.5.0.dev9/sarus/std/types.py` & `sarus-0.6.0.dev0/sarus/std/types.py`

 * *Files identical despite different names*

### Comparing `sarus-0.5.0.dev9/sarus/storage/legacy_local.py` & `sarus-0.6.0.dev0/sarus/storage/legacy_local.py`

 * *Files identical despite different names*

### Comparing `sarus-0.5.0.dev9/sarus/typing.py` & `sarus-0.6.0.dev0/sarus/typing.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     "_alt_policy",
     "_manager",
 ]
 
 MOCK = "mock"
 PYTHON_TYPE = "python_type"
 ADMIN_DS = "admin_ds"
+ATTRIBUTES_DS = "attributes_ds"
 
 
 @runtime_checkable
 class DataSpecWrapper(Protocol[T]):
     def python_type(self) -> Optional[str]:
         ...
```

### Comparing `sarus-0.5.0.dev9/sarus/utils.py` & `sarus-0.6.0.dev0/sarus/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import os
 from functools import partial, wraps
 from typing import Any, Callable, Dict, Optional, Type
 
 import sarus_data_spec.typing as st
 import yaml
 from sarus_data_spec.context import global_context
-from sarus_data_spec.scalar import model
 from sarus_data_spec.transform import external
 from sarus_data_spec.variant_constraint import public_constraint
 
 from .context.typing import LocalSDKContext
 from .typing import DataSpecVariant, DataSpecWrapper
 
 logger = logging.getLogger(__name__)
@@ -276,31 +275,14 @@
         wrapper_fn = register_method(wrapper_fn, code_name)
 
         return wrapper_fn
 
     return parametrized_wrapper
 
 
-def sarus_model(code):
-    """Decorator to initialize models."""
-
-    def parametrized_wrapper(ops_fn):
-        @wraps(ops_fn)
-        def wrapper_fn(self, *args, **kwargs):
-            dataspec = model(model_class=code, *args, **kwargs)
-            public_constraint(dataspec)
-            self._set_dataspec(dataspec)
-
-        wrapper_fn = register_method(wrapper_fn, code)
-
-        return wrapper_fn
-
-    return parametrized_wrapper
-
-
 def create_function(
     code_name: str, module_name: str, fn_name: str, inplace: bool = False
 ) -> Callable:
     """Create an op and register it as a function in a module."""
     global _registered_functions
     _registered_functions.append((module_name, fn_name, code_name))
```

### Comparing `sarus-0.5.0.dev9/sarus/wrapper_factory.py` & `sarus-0.6.0.dev0/sarus/wrapper_factory.py`

 * *Files identical despite different names*

### Comparing `sarus-0.5.0.dev9/sarus/xgboost/xgboost.py` & `sarus-0.6.0.dev0/sarus/xgboost/xgboost.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from __future__ import annotations
 
 from typing import Any, Optional
 
 import sarus_data_spec.protobuf as sp
 
 from sarus.dataspec_wrapper import DataSpecWrapper
-from sarus.utils import register_ops, sarus_method, sarus_model
+from sarus.utils import register_ops, sarus_method, sarus_init
 
 try:
     import xgboost
 except ModuleNotFoundError:
     pass  # error message in sarus_data_spec.typing
 
 
 class XGBClassifier(DataSpecWrapper[xgboost.XGBClassifier]):
-    @sarus_model(sp.Scalar.Model.ModelClass.XGB_CLASSIFIER)
+    @sarus_init("xgboost.XGB_CLASSIFIER")
     def __init__(
         self,
         *,
         objective="binary:logistic",
         use_label_encoder: Optional[bool] = None,
         _dataspec=None,
         **kwargs: Any,
```

### Comparing `sarus-0.5.0.dev9/sarus.egg-info/PKG-INFO` & `sarus-0.6.0.dev0/sarus.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,48 @@
 Metadata-Version: 2.1
 Name: sarus
-Version: 0.5.0.dev9
+Version: 0.6.0.dev0
 Summary: Python client for the Sarus Gateway
 Home-page: https://sarus.tech
 Author: Sarus Technologies
 Author-email: contact@sarus.tech
 License: Apache License 2.0
+Description: 
+        Sarus
+        
+        ===
+        
+        Python client for the Sarus Gateway. It provides simple connectors to leverage confidential data while ensuring data privacy. Users can explore & train AI models on sensitive data, via synthetic data browsing, remote training and differential privacy.
+        
+        Installation
+        ------------
+        
+        PIP
+        ^^^
+        
+        To install locally the latest available version :
+        
+        ``pip install sarus``
+        
+        Usage
+        -----
+        
+        Client
+        ^^^^^^
+        
+        Use this class to connect to **Sarus Gateway**.
+        
+        .. code-block:: python
+        
+           from sarus import Client
+        
+           client = Client(url="http://admin.sarus.tech:5000")
+           available = client.available_datasets()
+           print(f'Datasets available on the server: {available}')
+        
 Keywords: differential privacy,AI,Data privacy
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -21,42 +54,7 @@
 Provides-Extra: imblearn
 Provides-Extra: tensorflow
 Provides-Extra: pandas_profiling
 Provides-Extra: plotly
 Provides-Extra: xgboost
 Provides-Extra: skopt
 Provides-Extra: tests
-
-
-Sarus
-
-===
-
-Python client for the Sarus Gateway. It provides simple connectors to leverage confidential data while ensuring data privacy. Users can explore & train AI models on sensitive data, via synthetic data browsing, remote training and differential privacy.
-
-Installation
-------------
-
-PIP
-^^^
-
-To install locally the latest available version :
-
-``pip install sarus``
-
-Usage
------
-
-Client
-^^^^^^
-
-Use this class to connect to **Sarus Gateway**.
-
-.. code-block:: python
-
-   from sarus import Client
-
-   client = Client(url="http://admin.sarus.tech:5000")
-   available = client.available_datasets()
-   print(f'Datasets available on the server: {available}')
-
-
```

### Comparing `sarus-0.5.0.dev9/sarus.egg-info/SOURCES.txt` & `sarus-0.6.0.dev0/sarus.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -27,21 +27,23 @@
 sarus/legacy/__init__.py
 sarus/legacy/pandas/__init__.py
 sarus/legacy/pandas/dataframe.py
 sarus/legacy/tensorflow/__init__.py
 sarus/legacy/tensorflow/dataset.py
 sarus/legacy/tensorflow/model.py
 sarus/manager/__init__.py
-sarus/manager/arrow_computation.py
-sarus/manager/cache_scalar_computation.py
-sarus/manager/caching_computation.py
+sarus/manager/arrow_local.py
+sarus/manager/arrow_remote.py
+sarus/manager/cache_scalar_local.py
 sarus/manager/dataspec_api.py
+sarus/manager/parquet_local.py
 sarus/manager/sdk_manager.py
 sarus/manager/typing.py
-sarus/manager/value_computation.py
+sarus/manager/value_local.py
+sarus/manager/value_remote.py
 sarus/manager/ops/__init__.py
 sarus/manager/ops/api.py
 sarus/numpy/__init__.py
 sarus/numpy/random.py
 sarus/numpy/scalars.py
 sarus/pandas/__init__.py
 sarus/pandas/core.py
```

### Comparing `sarus-0.5.0.dev9/setup.cfg` & `sarus-0.6.0.dev0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 [options]
 zip_safe = False
 python_requires = >=3.7, <3.11
 packages = find:
 include_package_data = True
 install_requires = 
-	sarus_data_spec_public==2.11.1
+	sarus-data-spec-public==3.0.0
 	matplotlib>=3.1
 	cloudpickle>=1.2, <2.1
 
 [options.extras_require]
 sklearn = 
 	scikit-learn==1.1.1
 	scipy==1.9.0
```

