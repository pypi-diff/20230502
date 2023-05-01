# Comparing `tmp/tsml-0.0.7.tar.gz` & `tmp/tsml-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsml-0.0.7.tar", last modified: Thu Apr 20 11:47:38 2023, max compression
+gzip compressed data, was "tsml-0.1.0.tar", last modified: Mon May  1 23:00:03 2023, max compression
```

## Comparing `tsml-0.0.7.tar` & `tsml-0.1.0.tar`

### file list

```diff
@@ -1,97 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:47:38.603603 tsml-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-20 11:47:27.000000 tsml-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-20 11:47:27.000000 tsml-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-20 11:47:38.603603 tsml-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-20 11:47:27.000000 tsml-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-04-20 11:47:27.000000 tsml-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 11:47:38.603603 tsml-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:47:38.595602 tsml-0.0.7/tsml/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11552 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:47:38.595602 tsml-0.0.7/tsml/convolution_based/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/convolution_based/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:47:38.595602 tsml-0.0.7/tsml/datasets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:47:38.595602 tsml-0.0.7/tsml/datasets/EqualMinimalJapaneseVowels/
--rw-r--r--   0 runner    (1001) docker     (123)   120661 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/datasets/EqualMinimalJapaneseVowels/EqualMinimalJapaneseVowels_TEST.ts
--rw-r--r--   0 runner    (1001) docker     (123)   120799 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/datasets/EqualMinimalJapaneseVowels/EqualMinimalJapaneseVowels_TRAIN.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:47:38.595602 tsml-0.0.7/tsml/datasets/MinimalChinatown/
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/datasets/MinimalChinatown/MinimalChinatown_TEST.ts
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/datasets/MinimalChinatown/MinimalChinatown_TRAIN.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:47:38.595602 tsml-0.0.7/tsml/datasets/MinimalGasPrices/
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/datasets/MinimalGasPrices/MinimalGasPrices_TEST.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/datasets/MinimalGasPrices/MinimalGasPrices_TRAIN.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:47:38.595602 tsml-0.0.7/tsml/datasets/MinimalJapaneseVowels/
--rw-r--r--   0 runner    (1001) docker     (123)    36247 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/datasets/MinimalJapaneseVowels/MinimalJapaneseVowels_TEST.ts
--rw-r--r--   0 runner    (1001) docker     (123)    38758 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/datasets/MinimalJapaneseVowels/MinimalJapaneseVowels_TRAIN.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:47:38.599603 tsml-0.0.7/tsml/datasets/UnequalMinimalChinatown/
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/datasets/UnequalMinimalChinatown/UnequalMinimalChinatown_TEST.ts
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/datasets/UnequalMinimalChinatown/UnequalMinimalChinatown_TRAIN.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:47:38.599603 tsml-0.0.7/tsml/datasets/UnequalMinimalGasPrices/
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/datasets/UnequalMinimalGasPrices/UnequalMinimalGasPrices_TEST.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/datasets/UnequalMinimalGasPrices/UnequalMinimalGasPrices_TRAIN.ts
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24759 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/datasets/_data_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:47:38.599603 tsml-0.0.7/tsml/deep_learning/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/deep_learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/deep_learning/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:47:38.599603 tsml-0.0.7/tsml/dictionary_based/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/dictionary_based/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:47:38.599603 tsml-0.0.7/tsml/distance_based/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/distance_based/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:47:38.599603 tsml-0.0.7/tsml/dummy/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/dummy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12171 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/dummy/_dummy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:47:38.599603 tsml-0.0.7/tsml/feature_based/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/feature_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15184 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/feature_based/_catch22.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:47:38.599603 tsml-0.0.7/tsml/interval_based/
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/interval_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46207 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/interval_based/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    14260 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/interval_based/_cif.py
--rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/interval_based/_interval_forest.py
--rw-r--r--   0 runner    (1001) docker     (123)    21883 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/interval_based/_interval_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/interval_based/_rise.py
--rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/interval_based/_stsf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/interval_based/_tsf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:47:38.599603 tsml-0.0.7/tsml/shapelet_based/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/shapelet_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12781 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/shapelet_based/_stc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:47:38.599603 tsml-0.0.7/tsml/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47450 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/tests/_sklearn_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/tests/estimator_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/tests/test_all_estimators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/tests/test_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:47:38.603603 tsml-0.0.7/tsml/transformations/
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/transformations/_ar_coefficient.py
--rw-r--r--   0 runner    (1001) docker     (123)    46014 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/transformations/_catch22.py
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/transformations/_function_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    34766 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/transformations/_interval_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/transformations/_periodogram.py
--rw-r--r--   0 runner    (1001) docker     (123)    41527 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/transformations/_sfa.py
--rw-r--r--   0 runner    (1001) docker     (123)    24022 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/transformations/_shapelet_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/transformations/_summary_features.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:47:38.603603 tsml-0.0.7/tsml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/utils/_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/utils/discovery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:47:38.603603 tsml-0.0.7/tsml/utils/numba_functions/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/utils/numba_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/utils/numba_functions/general.py
--rw-r--r--   0 runner    (1001) docker     (123)    19873 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/utils/numba_functions/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)    22204 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/utils/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:47:38.603603 tsml-0.0.7/tsml/vector/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/vector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15951 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/vector/_cit.py
--rw-r--r--   0 runner    (1001) docker     (123)    18576 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/vector/_rotation_forest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:47:38.603603 tsml-0.0.7/tsml/vector/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/vector/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-20 11:47:27.000000 tsml-0.0.7/tsml/vector/tests/test_rotation_forest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:47:38.595602 tsml-0.0.7/tsml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-20 11:47:38.000000 tsml-0.0.7/tsml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-04-20 11:47:38.000000 tsml-0.0.7/tsml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 11:47:38.000000 tsml-0.0.7/tsml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-20 11:47:38.000000 tsml-0.0.7/tsml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-20 11:47:38.000000 tsml-0.0.7/tsml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:00:03.958170 tsml-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-01 22:59:53.000000 tsml-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-01 22:59:53.000000 tsml-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-05-01 23:00:03.958170 tsml-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-01 22:59:53.000000 tsml-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-01 22:59:53.000000 tsml-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 23:00:03.958170 tsml-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:00:03.942170 tsml-0.1.0/tsml/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11552 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:00:03.942170 tsml-0.1.0/tsml/convolution_based/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/convolution_based/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:00:03.942170 tsml-0.1.0/tsml/datasets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:00:03.942170 tsml-0.1.0/tsml/datasets/EqualMinimalJapaneseVowels/
+-rw-r--r--   0 runner    (1001) docker     (123)   120661 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/datasets/EqualMinimalJapaneseVowels/EqualMinimalJapaneseVowels_TEST.ts
+-rw-r--r--   0 runner    (1001) docker     (123)   120799 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/datasets/EqualMinimalJapaneseVowels/EqualMinimalJapaneseVowels_TRAIN.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:00:03.942170 tsml-0.1.0/tsml/datasets/MinimalChinatown/
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/datasets/MinimalChinatown/MinimalChinatown_TEST.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/datasets/MinimalChinatown/MinimalChinatown_TRAIN.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:00:03.942170 tsml-0.1.0/tsml/datasets/MinimalGasPrices/
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/datasets/MinimalGasPrices/MinimalGasPrices_TEST.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/datasets/MinimalGasPrices/MinimalGasPrices_TRAIN.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:00:03.942170 tsml-0.1.0/tsml/datasets/MinimalJapaneseVowels/
+-rw-r--r--   0 runner    (1001) docker     (123)    36247 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/datasets/MinimalJapaneseVowels/MinimalJapaneseVowels_TEST.ts
+-rw-r--r--   0 runner    (1001) docker     (123)    38758 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/datasets/MinimalJapaneseVowels/MinimalJapaneseVowels_TRAIN.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:00:03.946169 tsml-0.1.0/tsml/datasets/UnequalMinimalChinatown/
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/datasets/UnequalMinimalChinatown/UnequalMinimalChinatown_TEST.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/datasets/UnequalMinimalChinatown/UnequalMinimalChinatown_TRAIN.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:00:03.946169 tsml-0.1.0/tsml/datasets/UnequalMinimalGasPrices/
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/datasets/UnequalMinimalGasPrices/UnequalMinimalGasPrices_TEST.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/datasets/UnequalMinimalGasPrices/UnequalMinimalGasPrices_TRAIN.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24932 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/datasets/_data_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:00:03.946169 tsml-0.1.0/tsml/datasets/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/datasets/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   286342 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/datasets/tests/_expected_data_io_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/datasets/tests/test_data_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:00:03.946169 tsml-0.1.0/tsml/dictionary_based/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/dictionary_based/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:00:03.946169 tsml-0.1.0/tsml/distance_based/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/distance_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/distance_based/_pf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:00:03.946169 tsml-0.1.0/tsml/dummy/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/dummy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12171 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/dummy/_dummy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:00:03.946169 tsml-0.1.0/tsml/feature_based/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/feature_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17004 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/feature_based/_catch22.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:00:03.950170 tsml-0.1.0/tsml/interval_based/
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/interval_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46207 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/interval_based/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13914 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/interval_based/_cif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/interval_based/_interval_forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21883 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/interval_based/_interval_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/interval_based/_rise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/interval_based/_stsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/interval_based/_tsf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:00:03.950170 tsml-0.1.0/tsml/shapelet_based/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/shapelet_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/shapelet_based/_mrsqm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/shapelet_based/_rsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12725 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/shapelet_based/_stc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:00:03.950170 tsml-0.1.0/tsml/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47450 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/tests/_sklearn_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/tests/estimator_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/tests/test_all_estimators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/tests/test_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:00:03.954170 tsml-0.1.0/tsml/transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/transformations/_ar_coefficient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42302 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/transformations/_catch22.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/transformations/_function_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34766 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/transformations/_interval_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/transformations/_periodogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41527 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/transformations/_sfa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24022 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/transformations/_shapelet_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/transformations/_summary_features.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:00:03.954170 tsml-0.1.0/tsml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/utils/_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/utils/discovery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:00:03.954170 tsml-0.1.0/tsml/utils/numba_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/utils/numba_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/utils/numba_functions/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19873 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/utils/numba_functions/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9234 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22204 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/utils/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:00:03.954170 tsml-0.1.0/tsml/vector/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/vector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15951 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/vector/_cit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18576 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/vector/_rotation_forest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:00:03.958170 tsml-0.1.0/tsml/vector/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/vector/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-01 22:59:53.000000 tsml-0.1.0/tsml/vector/tests/test_rotation_forest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:00:03.942170 tsml-0.1.0/tsml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-05-01 23:00:03.000000 tsml-0.1.0/tsml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-05-01 23:00:03.000000 tsml-0.1.0/tsml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 23:00:03.000000 tsml-0.1.0/tsml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-01 23:00:03.000000 tsml-0.1.0/tsml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-01 23:00:03.000000 tsml-0.1.0/tsml.egg-info/top_level.txt
```

### Comparing `tsml-0.0.7/LICENSE` & `tsml-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tsml-0.0.7/PKG-INFO` & `tsml-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsml
-Version: 0.0.7
+Version: 0.1.0
 Summary: A toolkit for time series machine learning algorithms.
 Author-email: Matthew Middlehurst <m.middlehurst@uea.ac.uk>, Tony Bagnall <ajb@uea.ac.uk>
 License: BSD 3-Clause License
         
         Copyright (c) The Time Series Machine Learning (tsml) developers.
         All rights reserved.
         
@@ -46,14 +46,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: extras
+Provides-Extra: unstable_extras
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE
 
 # tsml
 
 A toolkit for time series machine learning algorithms
```

### Comparing `tsml-0.0.7/pyproject.toml` & `tsml-0.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tsml"
-version = "0.0.7"
+version = "0.1.0"
 description = "A toolkit for time series machine learning algorithms."
 authors = [
     {name = "Matthew Middlehurst", email = "m.middlehurst@uea.ac.uk"},
     {name = "Tony Bagnall", email = "ajb@uea.ac.uk"},
 ]
 readme = "README.md"
 requires-python = ">=3.8,<3.11"
@@ -39,17 +39,21 @@
     "numpy>=1.21.0",
     "scikit-learn>=1.0.2",
     "pandas",
 ]
 
 [project.optional-dependencies]
 extras = [
-    "pycatch22>=0.4.2",
     "pyfftw>=0.12.0",
     "statsmodels>=0.12.1",
+    "wildboar>=1.1.0",
+]
+unstable_extras = [
+    "mrsqm>=0.0.1 ; platform_system == 'Darwin'",  # requires gcc and fftw to be installed for Windows and some other OS (see http://www.fftw.org/index.html)
+    "pycatch22>=0.4.2",  # Known to fail installation on some setups
 ]
 dev = [
     "pre-commit",
     "pytest",
     "pytest-randomly",
     "pytest-timeout",
     "pytest-xdist",
```

### Comparing `tsml-0.0.7/tsml/base.py` & `tsml-0.1.0/tsml/base.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.7/tsml/datasets/EqualMinimalJapaneseVowels/EqualMinimalJapaneseVowels_TEST.ts` & `tsml-0.1.0/tsml/datasets/EqualMinimalJapaneseVowels/EqualMinimalJapaneseVowels_TEST.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.0.7/tsml/datasets/EqualMinimalJapaneseVowels/EqualMinimalJapaneseVowels_TRAIN.ts` & `tsml-0.1.0/tsml/datasets/EqualMinimalJapaneseVowels/EqualMinimalJapaneseVowels_TRAIN.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.0.7/tsml/datasets/MinimalChinatown/MinimalChinatown_TEST.ts` & `tsml-0.1.0/tsml/datasets/MinimalChinatown/MinimalChinatown_TEST.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.0.7/tsml/datasets/MinimalChinatown/MinimalChinatown_TRAIN.ts` & `tsml-0.1.0/tsml/datasets/MinimalChinatown/MinimalChinatown_TRAIN.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.0.7/tsml/datasets/MinimalGasPrices/MinimalGasPrices_TEST.ts` & `tsml-0.1.0/tsml/datasets/MinimalGasPrices/MinimalGasPrices_TEST.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.0.7/tsml/datasets/MinimalGasPrices/MinimalGasPrices_TRAIN.ts` & `tsml-0.1.0/tsml/datasets/MinimalGasPrices/MinimalGasPrices_TRAIN.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.0.7/tsml/datasets/MinimalJapaneseVowels/MinimalJapaneseVowels_TEST.ts` & `tsml-0.1.0/tsml/datasets/MinimalJapaneseVowels/MinimalJapaneseVowels_TEST.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.0.7/tsml/datasets/MinimalJapaneseVowels/MinimalJapaneseVowels_TRAIN.ts` & `tsml-0.1.0/tsml/datasets/MinimalJapaneseVowels/MinimalJapaneseVowels_TRAIN.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.0.7/tsml/datasets/UnequalMinimalChinatown/UnequalMinimalChinatown_TEST.ts` & `tsml-0.1.0/tsml/datasets/UnequalMinimalChinatown/UnequalMinimalChinatown_TEST.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.0.7/tsml/datasets/UnequalMinimalChinatown/UnequalMinimalChinatown_TRAIN.ts` & `tsml-0.1.0/tsml/datasets/UnequalMinimalChinatown/UnequalMinimalChinatown_TRAIN.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.0.7/tsml/datasets/UnequalMinimalGasPrices/UnequalMinimalGasPrices_TEST.ts` & `tsml-0.1.0/tsml/datasets/UnequalMinimalGasPrices/UnequalMinimalGasPrices_TEST.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.0.7/tsml/datasets/UnequalMinimalGasPrices/UnequalMinimalGasPrices_TRAIN.ts` & `tsml-0.1.0/tsml/datasets/UnequalMinimalGasPrices/UnequalMinimalGasPrices_TRAIN.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.0.7/tsml/datasets/__init__.py` & `tsml-0.1.0/tsml/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.7/tsml/datasets/_data_io.py` & `tsml-0.1.0/tsml/datasets/_data_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,17 +26,17 @@
 ) -> Union[np.ndarray, list, Tuple[np.ndarray, np.ndarray], Tuple[list, np.ndarray]]:
     """Load data from a .ts file into a 3D numpy array or list of 2D numpy arrays.
 
     If the data to be loaded is equal length, a 3D numpy array will be returned. If the
     data is unequal length, a list of 2D numpy arrays will be returned. If labels are
     present, they will be returned as well as the data.
 
-    The only mandatory tags in the loaded file are @equallength and one of
-    @targetlabels or @classlabels. Other details can be inferred, though some error
-    checking will be done if they are present.
+    The only mandatory tags in the loaded file are one of @targetlabels or @classlabels.
+    Other details can be inferred, though some error checking will be done if they are
+    present.
 
     Parameters
     ----------
     file_path: str
         The full pathname of the .ts file to read.
     replace_missing_vals_with: str, int or float, default="NaN"
         The value that missing values reprented by '?' in the text file should be
@@ -300,19 +300,17 @@
                 has_labels = classlabel
             else:
                 raise IOError(
                     "Unable to read .ts file. A @classlabel or @targetlabel tag is "
                     "required."
                 )
 
-            # Equal length tag is required.
+            # Assume equal length if no tag.
             if not equallength_tag:
-                raise IOError(
-                    "Unable to read .ts file. The @equallength tag is required."
-                )
+                equallength = True
 
             n_instances = len(lines) - data_start_line
             data_dims = len(first_line) - 1 if has_labels else len(first_line)
             first_line = first_line[0].split(",")
             data_length = len(first_line)
 
             # Do some verification on remaining tags
@@ -380,21 +378,27 @@
             if read_dims != data_dims:
                 raise IOError(
                     "Unable to read .ts file. Inconsistent number of channels."
                     f"Expected {data_dims} but read {read_dims} on line {data_idx}."
                 )
 
             dimensions = line[:data_dims]
-            if not equallength:
-                data_length = len(dimensions[0].strip().split(","))
+            split = dimensions[0].strip().split(",")
+            length = len(split)
+            if equallength and length != data_length:
+                raise IOError(
+                    "Unable to read .ts file. Inconsistent number of channels."
+                    f"Expected {data_dims} but read {read_dims} on line {data_idx}."
+                )
 
             # Process the data for each channel
-            series = np.zeros((data_dims, data_length), dtype=X_dtype)
-            for i in range(data_dims):
-                series[i, :] = dimensions[i].strip().split(",")
+            series = np.zeros((data_dims, length), dtype=X_dtype)
+            series[0, :] = split
+            for n in range(1, data_dims):
+                series[n, :] = dimensions[n].strip().split(",")
 
             X[data_idx] = series
 
             if has_labels:
                 label = line[-1].strip()
 
                 if classlabel and label not in class_label_list:
```

### Comparing `tsml-0.0.7/tsml/dummy/_dummy.py` & `tsml-0.1.0/tsml/dummy/_dummy.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.7/tsml/feature_based/_catch22.py` & `tsml-0.1.0/tsml/feature_based/_catch22.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,32 +11,54 @@
 from sklearn.base import ClassifierMixin, RegressorMixin
 from sklearn.ensemble import RandomForestClassifier, RandomForestRegressor
 from sklearn.utils.multiclass import check_classification_targets
 from sklearn.utils.validation import check_is_fitted
 
 from tsml.base import BaseTimeSeriesEstimator, _clone_estimator
 from tsml.transformations._catch22 import Catch22Transformer
-from tsml.utils.validation import check_n_jobs
+from tsml.utils.validation import _check_optional_dependency, check_n_jobs
 
 
 class Catch22Classifier(ClassifierMixin, BaseTimeSeriesEstimator):
     """Canonical Time-series Characteristics (catch22) classifier.
 
     This classifier simply transforms the input data using the Catch22 [1]
     transformer and builds a provided estimator using the transformed data.
 
-    Shorthand for the pipeline `Catch22(outlier_norm, replace_nans) * estimator`
-
     Parameters
     ----------
+    features : int/str or List of int/str, optional, default="all"
+        The Catch22 features to extract by feature index, feature name as a str or as a
+        list of names or indices for multiple features. If "all", all features are
+        extracted.
+        Valid features are as follows:
+            ["DN_HistogramMode_5", "DN_HistogramMode_10",
+            "SB_BinaryStats_diff_longstretch0", "DN_OutlierInclude_p_001_mdrmd",
+            "DN_OutlierInclude_n_001_mdrmd", "CO_f1ecac", "CO_FirstMin_ac",
+            "SP_Summaries_welch_rect_area_5_1", "SP_Summaries_welch_rect_centroid",
+            "FC_LocalSimple_mean3_stderr", "CO_trev_1_num", "CO_HistogramAMI_even_2_5",
+            "IN_AutoMutualInfoStats_40_gaussian_fmmi", "MD_hrv_classic_pnn40",
+            "SB_BinaryStats_mean_longstretch1", "SB_MotifThree_quantile_hh",
+            "FC_LocalSimple_mean1_tauresrat", "CO_Embed2_Dist_tau_d_expfit_meandiff",
+            "SC_FluctAnal_2_dfa_50_1_2_logi_prop_r1",
+            "SC_FluctAnal_2_rsrangefit_50_1_logi_prop_r1",
+            "SB_TransitionMatrix_3ac_sumdiagcov", "PD_PeriodicityWang_th0_01"]
+    catch24 : bool, optional, default=False
+        Extract the mean and standard deviation as well as the 22 Catch22 features if
+        true. If a List of specific features to extract is provided, "Mean" and/or
+        "StandardDeviation" must be added to the List to extract these features.
     outlier_norm : bool, optional, default=False
         Normalise each series during the two outlier Catch22 features, which can take a
         while to process for large values.
     replace_nans : bool, optional, default=True
         Replace NaN or inf values from the Catch22 transform with 0.
+    use_pycatch22 : bool, optional, default=True
+        Wraps the C based pycatch22 implementation for tsml.
+        (https://github.com/DynamicsAndNeuralSystems/pycatch22). This requires the
+        ``pycatch22`` package to be installed if True.
     estimator : sklearn classifier, optional, default=None
         An sklearn estimator to be built using the transformed data.
         Defaults to sklearn RandomForestClassifier(n_estimators=200)
     n_jobs : int, optional, default=1
         The number of jobs to run in parallel for both `fit` and `predict`.
         ``-1`` means using all processors.
     random_state : int or None, optional, default=None
@@ -71,27 +93,32 @@
 
     def __init__(
         self,
         features="all",
         catch24=False,
         outlier_norm=False,
         replace_nans=True,
+        use_pycatch22=True,
         estimator=None,
         n_jobs=1,
         random_state=None,
     ):
         self.features = features
         self.catch24 = catch24
         self.outlier_norm = outlier_norm
         self.replace_nans = replace_nans
+        self.use_pycatch22 = use_pycatch22
         self.estimator = estimator
 
         self.n_jobs = n_jobs
         self.random_state = random_state
 
+        if use_pycatch22:
+            _check_optional_dependency("pycatch22", "pycatch22", self)
+
         super(Catch22Classifier, self).__init__()
 
     def fit(self, X, y):
         """Fit a pipeline on cases (X,y), where y is the target variable.
 
         Parameters
         ----------
@@ -129,14 +156,15 @@
         self._n_jobs = check_n_jobs(self.n_jobs)
 
         self._transformer = Catch22Transformer(
             features=self.features,
             catch24=self.catch24,
             outlier_norm=self.outlier_norm,
             replace_nans=self.replace_nans,
+            use_pycatch22=self.use_pycatch22,
             n_jobs=self._n_jobs,
         )
 
         self._estimator = _clone_estimator(
             RandomForestClassifier(n_estimators=200)
             if self.estimator is None
             else self.estimator,
```

### Comparing `tsml-0.0.7/tsml/interval_based/__init__.py` & `tsml-0.1.0/tsml/interval_based/__init__.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.7/tsml/interval_based/_base.py` & `tsml-0.1.0/tsml/interval_based/_base.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.7/tsml/interval_based/_cif.py` & `tsml-0.1.0/tsml/interval_based/_cif.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # -*- coding: utf-8 -*-
 
 __author__ = ["MatthewMiddlehurst"]
 __all__ = ["CIFClassifier", "CIFRegressor", "DrCIFClassifier", "DrCIFRegressor"]
 
 import numpy as np
 from sklearn.base import ClassifierMixin, RegressorMixin
-from sklearn.tree import DecisionTreeClassifier, DecisionTreeRegressor
 
 from tsml.interval_based._base import BaseIntervalForest
 from tsml.transformations import FunctionTransformer, PeriodogramTransformer
-from tsml.transformations._catch22 import Catch22Transformer, Catch22WrapperTransformer
+from tsml.transformations._catch22 import Catch22Transformer
 from tsml.utils.numba_functions.general import first_order_differences_3d
 from tsml.utils.numba_functions.stats import (
     row_iqr,
     row_mean,
     row_median,
     row_numba_max,
     row_numba_min,
@@ -49,17 +48,15 @@
 
         if isinstance(base_estimator, CITClassifier):
             replace_nan = "nan"
         else:
             replace_nan = 0
 
         interval_features = [
-            Catch22WrapperTransformer(outlier_norm=True)
-            if use_pycatch22
-            else Catch22Transformer(outlier_norm=True),
+            Catch22Transformer(outlier_norm=True, use_pycatch22=use_pycatch22),
             row_mean,
             row_std,
             row_slope,
         ]
 
         super(CIFClassifier, self).__init__(
             base_estimator=base_estimator,
@@ -137,17 +134,15 @@
         parallel_backend=None,
     ):
         self.use_pycatch22 = use_pycatch22
         if use_pycatch22:
             _check_optional_dependency("pycatch22", "pycatch22", self)
 
         interval_features = [
-            Catch22WrapperTransformer(outlier_norm=True)
-            if use_pycatch22
-            else Catch22Transformer(outlier_norm=True),
+            Catch22Transformer(outlier_norm=True, use_pycatch22=use_pycatch22),
             row_mean,
             row_std,
             row_slope,
         ]
 
         super(CIFRegressor, self).__init__(
             base_estimator=base_estimator,
@@ -238,17 +233,15 @@
         series_transformers = [
             None,
             FunctionTransformer(func=first_order_differences_3d, validate=False),
             PeriodogramTransformer(use_pyfftw=use_pyfftw),
         ]
 
         interval_features = [
-            Catch22WrapperTransformer(outlier_norm=True)
-            if use_pycatch22
-            else Catch22Transformer(outlier_norm=True),
+            Catch22Transformer(outlier_norm=True, use_pycatch22=use_pycatch22),
             row_mean,
             row_std,
             row_slope,
             row_median,
             row_iqr,
             row_numba_min,
             row_numba_max,
@@ -341,17 +334,15 @@
         series_transformers = [
             None,
             FunctionTransformer(func=first_order_differences_3d, validate=False),
             PeriodogramTransformer(use_pyfftw=True),
         ]
 
         interval_features = [
-            Catch22WrapperTransformer(outlier_norm=True)
-            if use_pycatch22
-            else Catch22Transformer(outlier_norm=True),
+            Catch22Transformer(outlier_norm=True, use_pycatch22=use_pycatch22),
             row_mean,
             row_std,
             row_slope,
             row_median,
             row_iqr,
             row_numba_min,
             row_numba_max,
```

### Comparing `tsml-0.0.7/tsml/interval_based/_interval_forest.py` & `tsml-0.1.0/tsml/interval_based/_interval_forest.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.7/tsml/interval_based/_interval_pipelines.py` & `tsml-0.1.0/tsml/interval_based/_interval_pipelines.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.7/tsml/interval_based/_rise.py` & `tsml-0.1.0/tsml/interval_based/_rise.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.7/tsml/interval_based/_stsf.py` & `tsml-0.1.0/tsml/interval_based/_stsf.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.7/tsml/interval_based/_tsf.py` & `tsml-0.1.0/tsml/interval_based/_tsf.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.7/tsml/shapelet_based/_stc.py` & `tsml-0.1.0/tsml/shapelet_based/_stc.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,15 +238,15 @@
         """
         check_is_fitted(self)
 
         # treat case of single class seen in fit
         if self.n_classes_ == 1:
             return np.repeat(list(self.class_dictionary_.keys()), X.shape[0], axis=0)
 
-        X = self._validate_data(X=X, reset=False, ensure_min_series_length=3)
+        X = self._validate_data(X=X, reset=False)
 
         return self._estimator.predict(self._transformer.transform(X))
 
     def predict_proba(self, X) -> np.ndarray:
         """Predicts labels probabilities for sequences in X.
 
         Parameters
@@ -261,15 +261,15 @@
         """
         check_is_fitted(self)
 
         # treat case of single class seen in fit
         if self.n_classes_ == 1:
             return np.repeat([[1]], X.shape[0], axis=0)
 
-        X = self._validate_data(X=X, reset=False, ensure_min_series_length=3)
+        X = self._validate_data(X=X, reset=False)
 
         m = getattr(self._estimator, "predict_proba", None)
         if callable(m):
             return self._estimator.predict_proba(self._transformer.transform(X))
         else:
             dists = np.zeros((X.shape[0], self.n_classes_))
             preds = self._estimator.predict(self._transformer.transform(X))
```

### Comparing `tsml-0.0.7/tsml/tests/_sklearn_checks.py` & `tsml-0.1.0/tsml/tests/_sklearn_checks.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.7/tsml/tests/estimator_checks.py` & `tsml-0.1.0/tsml/tests/estimator_checks.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,7 +201,10 @@
     pass
 
 
 @ignore_warnings(category=FutureWarning)
 def check_n_features_unequal(name, estimator_orig):
     pass
 
+
+# @ignore_warnings(category=FutureWarning)
+# X_types
```

### Comparing `tsml-0.0.7/tsml/tests/test_interface.py` & `tsml-0.1.0/tsml/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.7/tsml/transformations/__init__.py` & `tsml-0.1.0/tsml/transformations/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # -*- coding: utf-8 -*-
 """tsml transformations."""
 
 __all__ = [
     "ARCoefficientTransformer",
     "Catch22Transformer",
-    "Catch22WrapperTransformer",
     "FunctionTransformer",
     "RandomIntervalTransformer",
     "SupervisedIntervalTransformer",
     "PeriodogramTransformer",
     # "SFATransformer",
     "RandomShapeletTransformer",
     "SevenNumberSummaryTransformer",
 ]
 
 from tsml.transformations._ar_coefficient import ARCoefficientTransformer
-from tsml.transformations._catch22 import Catch22Transformer, Catch22WrapperTransformer
+from tsml.transformations._catch22 import Catch22Transformer
 from tsml.transformations._function_transformer import FunctionTransformer
 from tsml.transformations._interval_extraction import (
     RandomIntervalTransformer,
     SupervisedIntervalTransformer,
 )
 from tsml.transformations._periodogram import PeriodogramTransformer
 from tsml.transformations._shapelet_transform import RandomShapeletTransformer
```

### Comparing `tsml-0.0.7/tsml/transformations/_ar_coefficient.py` & `tsml-0.1.0/tsml/transformations/_ar_coefficient.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.7/tsml/transformations/_catch22.py` & `tsml-0.1.0/tsml/transformations/_catch22.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 """Catch22 features.
 
 A transformer for the Catch22 features.
 """
 
 __author__ = ["MatthewMiddlehurst"]
-__all__ = ["Catch22Transformer", "Catch22WrapperTransformer"]
+__all__ = ["Catch22Transformer"]
 
 import math
 
 import numpy as np
 from joblib import Parallel
 from numba import njit
 from sklearn.base import TransformerMixin
@@ -79,14 +79,18 @@
         true. If a List of specific features to extract is provided, "Mean" and/or
         "StandardDeviation" must be added to the List to extract these features.
     outlier_norm : bool, optional, default=False
         Normalise each series during the two outlier Catch22 features, which can take a
         while to process for large values.
     replace_nans : bool, optional, default=True
         Replace NaN or inf values from the Catch22 transform with 0.
+    use_pycatch22 : bool, optional, default=True
+        Wraps the C based pycatch22 implementation for tsml.
+        (https://github.com/DynamicsAndNeuralSystems/pycatch22). This requires the
+        ``pycatch22`` package to be installed if True.
     n_jobs : int, optional, default=1
         The number of jobs to run in parallel for transform. Requires multiple input
         cases. ``-1`` means using all processors.
 
     See Also
     --------
     Catch22Classifier
@@ -112,22 +116,27 @@
 
     def __init__(
         self,
         features="all",
         catch24=False,
         outlier_norm=False,
         replace_nans=False,
+        use_pycatch22=True,
         n_jobs=1,
     ):
         self.features = features
         self.catch24 = catch24
         self.outlier_norm = outlier_norm
         self.replace_nans = replace_nans
+        self.use_pycatch22 = use_pycatch22
         self.n_jobs = n_jobs
 
+        if use_pycatch22:
+            _check_optional_dependency("pycatch22", "pycatch22", self)
+
         super(Catch22Transformer, self).__init__()
 
     features_arguments_ = feature_names
 
     def fit(self, X, y=None):
         self._validate_data(X=X)
 
@@ -174,41 +183,73 @@
 
         n_instances = len(X)
 
         f_idx = _verify_features(self.features, self.catch24)
 
         threads_to_use = check_n_jobs(self.n_jobs)
 
-        features = [
-            Catch22Transformer._DN_HistogramMode_5,
-            Catch22Transformer._DN_HistogramMode_10,
-            Catch22Transformer._SB_BinaryStats_diff_longstretch0,
-            Catch22Transformer._DN_OutlierInclude_p_001_mdrmd,
-            Catch22Transformer._DN_OutlierInclude_n_001_mdrmd,
-            Catch22Transformer._CO_f1ecac,
-            Catch22Transformer._CO_FirstMin_ac,
-            Catch22Transformer._SP_Summaries_welch_rect_area_5_1,
-            Catch22Transformer._SP_Summaries_welch_rect_centroid,
-            Catch22Transformer._FC_LocalSimple_mean3_stderr,
-            Catch22Transformer._CO_trev_1_num,
-            Catch22Transformer._CO_HistogramAMI_even_2_5,
-            Catch22Transformer._IN_AutoMutualInfoStats_40_gaussian_fmmi,
-            Catch22Transformer._MD_hrv_classic_pnn40,
-            Catch22Transformer._SB_BinaryStats_mean_longstretch1,
-            Catch22Transformer._SB_MotifThree_quantile_hh,
-            Catch22Transformer._FC_LocalSimple_mean1_tauresrat,
-            Catch22Transformer._CO_Embed2_Dist_tau_d_expfit_meandiff,
-            Catch22Transformer._SC_FluctAnal_2_dfa_50_1_2_logi_prop_r1,
-            Catch22Transformer._SC_FluctAnal_2_rsrangefit_50_1_logi_prop_r1,
-            Catch22Transformer._SB_TransitionMatrix_3ac_sumdiagcov,
-            Catch22Transformer._PD_PeriodicityWang_th0_01,
-        ]
+        if self.use_pycatch22:
+            import pycatch22
+
+            features = [
+                pycatch22.DN_HistogramMode_5,
+                pycatch22.DN_HistogramMode_10,
+                pycatch22.SB_BinaryStats_diff_longstretch0,
+                pycatch22.DN_OutlierInclude_p_001_mdrmd,
+                pycatch22.DN_OutlierInclude_n_001_mdrmd,
+                pycatch22.CO_f1ecac,
+                pycatch22.CO_FirstMin_ac,
+                pycatch22.SP_Summaries_welch_rect_area_5_1,
+                pycatch22.SP_Summaries_welch_rect_centroid,
+                pycatch22.FC_LocalSimple_mean3_stderr,
+                pycatch22.CO_trev_1_num,
+                pycatch22.CO_HistogramAMI_even_2_5,
+                pycatch22.IN_AutoMutualInfoStats_40_gaussian_fmmi,
+                pycatch22.MD_hrv_classic_pnn40,
+                pycatch22.SB_BinaryStats_mean_longstretch1,
+                pycatch22.SB_MotifThree_quantile_hh,
+                pycatch22.FC_LocalSimple_mean1_tauresrat,
+                pycatch22.CO_Embed2_Dist_tau_d_expfit_meandiff,
+                pycatch22.SC_FluctAnal_2_dfa_50_1_2_logi_prop_r1,
+                pycatch22.SC_FluctAnal_2_rsrangefit_50_1_logi_prop_r1,
+                pycatch22.SB_TransitionMatrix_3ac_sumdiagcov,
+                pycatch22.PD_PeriodicityWang_th0_01,
+            ]
+        else:
+            features = [
+                Catch22Transformer._DN_HistogramMode_5,
+                Catch22Transformer._DN_HistogramMode_10,
+                Catch22Transformer._SB_BinaryStats_diff_longstretch0,
+                Catch22Transformer._DN_OutlierInclude_p_001_mdrmd,
+                Catch22Transformer._DN_OutlierInclude_n_001_mdrmd,
+                Catch22Transformer._CO_f1ecac,
+                Catch22Transformer._CO_FirstMin_ac,
+                Catch22Transformer._SP_Summaries_welch_rect_area_5_1,
+                Catch22Transformer._SP_Summaries_welch_rect_centroid,
+                Catch22Transformer._FC_LocalSimple_mean3_stderr,
+                Catch22Transformer._CO_trev_1_num,
+                Catch22Transformer._CO_HistogramAMI_even_2_5,
+                Catch22Transformer._IN_AutoMutualInfoStats_40_gaussian_fmmi,
+                Catch22Transformer._MD_hrv_classic_pnn40,
+                Catch22Transformer._SB_BinaryStats_mean_longstretch1,
+                Catch22Transformer._SB_MotifThree_quantile_hh,
+                Catch22Transformer._FC_LocalSimple_mean1_tauresrat,
+                Catch22Transformer._CO_Embed2_Dist_tau_d_expfit_meandiff,
+                Catch22Transformer._SC_FluctAnal_2_dfa_50_1_2_logi_prop_r1,
+                Catch22Transformer._SC_FluctAnal_2_rsrangefit_50_1_logi_prop_r1,
+                Catch22Transformer._SB_TransitionMatrix_3ac_sumdiagcov,
+                Catch22Transformer._PD_PeriodicityWang_th0_01,
+            ]
 
         c22_list = Parallel(n_jobs=threads_to_use)(
-            delayed(self._transform_case)(
+            delayed(
+                self._transform_case_pycatch22
+                if self.use_pycatch22
+                else self._transform_case
+            )(
                 X[i],
                 f_idx,
                 features,
             )
             for i in range(n_instances)
         )
 
@@ -303,16 +344,76 @@
                 elif feature == 23:
                     c22[dim + n] = np.std(series)
                 else:
                     c22[dim + n] = features[feature](*args)
 
         return c22
 
+    def _transform_case_pycatch22(self, X, f_idx, features):
+        c22 = np.zeros(len(f_idx) * len(X))
+
+        if self._transform_features is not None and len(
+            self._transform_features
+        ) == len(c22):
+            transform_feature = self._transform_features
+        else:
+            transform_feature = [True] * len(c22)
+
+        f_count = -1
+        for i in range(len(X)):
+            dim = i * len(f_idx)
+            series = list(X[i])
+
+            if self.outlier_norm and (3 in f_idx or 4 in f_idx):
+                outlier_series = list(z_normalise_series(X[i]))
+
+            for n, feature in enumerate(f_idx):
+                f_count += 1
+                if not transform_feature[f_count]:
+                    continue
+
+                if self.outlier_norm and feature in [3, 4]:
+                    c22[dim + n] = features[feature](outlier_series)
+                if feature == 22:
+                    c22[dim + n] = np.mean(series)
+                elif feature == 23:
+                    c22[dim + n] = np.std(series)
+                else:
+                    c22[dim + n] = features[feature](series)
+
+        return c22
+
     def _more_tags(self):
-        return {"X_types": ["np_list", "3darray"], "requires_fit": False}
+        return {
+            "X_types": ["np_list", "3darray"],
+            "requires_fit": False,
+            "optional_dependency": self.use_pycatch22,
+        }
+
+    @classmethod
+    def get_test_params(cls, parameter_set="default"):
+        """Return testing parameter settings for the estimator.
+
+        Parameters
+        ----------
+        parameter_set : str, default="default"
+            Name of the set of test parameters to return, for use in tests. If no
+            special parameters are defined for a value, will return `"default"` set.
+
+        Returns
+        -------
+        params : dict or list of dict, default = {}
+            Parameters to create testing instances of the class
+            Each dict are parameters to construct an "interesting" test instance, i.e.,
+            `MyClass(**params)` or `MyClass(**params[i])` creates a valid test instance.
+            `create_test_instance` uses the first (or only) dictionary in `params`
+        """
+        return {
+            "use_pycatch22": False,
+        }
 
     @staticmethod
     def _DN_HistogramMode_5(X, smin, smax):
         # Mode of z-scored distribution (5-bin histogram).
         return _histogram_mode(X, 5, smin, smax)
 
     @staticmethod
@@ -1226,215 +1327,7 @@
                     raise ValueError("Invalid feature selection.")
         else:
             raise ValueError("Invalid feature selection.")
     else:
         raise ValueError("Invalid feature selection.")
 
     return f_idx
-
-
-class Catch22WrapperTransformer(TransformerMixin, BaseTimeSeriesEstimator):
-    """Canonical Time-series Characteristics (Catch22) C Wrapper.
-
-    Wraps the pycatch22 implementation for sktime
-    (https://github.com/DynamicsAndNeuralSystems/pycatch22).
-
-    Overview: Input n series with d dimensions of length m
-    Transforms series into the 22 Catch22 [1]_ features extracted from the hctsa [2]_
-    toolbox.
-
-    Parameters
-    ----------
-    features : int/str or List of int/str, optional, default="all"
-        The Catch22 features to extract by feature index, feature name as a str or as a
-        list of names or indices for multiple features. If "all", all features are
-        extracted.
-        Valid features are as follows:
-            ["DN_HistogramMode_5", "DN_HistogramMode_10",
-            "SB_BinaryStats_diff_longstretch0", "DN_OutlierInclude_p_001_mdrmd",
-            "DN_OutlierInclude_n_001_mdrmd", "CO_f1ecac", "CO_FirstMin_ac",
-            "SP_Summaries_welch_rect_area_5_1", "SP_Summaries_welch_rect_centroid",
-            "FC_LocalSimple_mean3_stderr", "CO_trev_1_num", "CO_HistogramAMI_even_2_5",
-            "IN_AutoMutualInfoStats_40_gaussian_fmmi", "MD_hrv_classic_pnn40",
-            "SB_BinaryStats_mean_longstretch1", "SB_MotifThree_quantile_hh",
-            "FC_LocalSimple_mean1_tauresrat", "CO_Embed2_Dist_tau_d_expfit_meandiff",
-            "SC_FluctAnal_2_dfa_50_1_2_logi_prop_r1",
-            "SC_FluctAnal_2_rsrangefit_50_1_logi_prop_r1",
-            "SB_TransitionMatrix_3ac_sumdiagcov", "PD_PeriodicityWang_th0_01"]
-    catch24 : bool, optional, default=False
-        Extract the mean and standard deviation as well as the 22 Catch22 features if
-        true. If a List of specific features to extract is provided, "Mean" and/or
-        "StandardDeviation" must be added to the List to extract these features.
-    outlier_norm : bool, optional, default=False
-        Normalise each series during the two outlier Catch22 features, which can take a
-        while to process for large values.
-    replace_nans : bool, optional, default=True
-        Replace NaN or inf values from the Catch22 transform with 0.
-    n_jobs : int, optional, default=1
-        The number of jobs to run in parallel for transform. Requires multiple input
-        cases. ``-1`` means using all processors.
-
-    See Also
-    --------
-    Catch22 Catch22Classifier
-
-    References
-    ----------
-    .. [1] Lubba, C. H., Sethi, S. S., Knaute, P., Schultz, S. R., Fulcher, B. D., &
-    Jones, N. S. (2019). catch22: Canonical time-series characteristics. Data Mining
-    and Knowledge Discovery, 33(6), 1821-1852.
-    .. [2] Fulcher, B. D., Little, M. A., & Jones, N. S. (2013). Highly comparative
-    time-series analysis: the empirical structure of time series and their methods.
-    Journal of the Royal Society Interface, 10(83), 20130048.
-    """
-
-    def __init__(
-        self,
-        features="all",
-        catch24=False,
-        outlier_norm=False,
-        replace_nans=False,
-        n_jobs=1,
-    ):
-        self.features = features
-        self.catch24 = catch24
-        self.outlier_norm = outlier_norm
-        self.replace_nans = replace_nans
-        self.n_jobs = n_jobs
-
-        _check_optional_dependency("pycatch22", "pycatch22", self)
-
-        super(Catch22WrapperTransformer, self).__init__()
-
-    features_arguments_ = feature_names
-
-    def fit(self, X, y=None):
-        self._validate_data(X=X)
-
-        self.features_arguments_ = (
-            self.features
-            if self.features != "all"
-            else (
-                feature_names + ["Mean", "StandardDeviation"]
-                if self.catch24
-                else feature_names
-            )
-        )
-
-        if isinstance(self.features, str):
-            if self.features == "all":
-                self.n_transformed_features_ = 24 if self.catch24 else 22
-            else:
-                self.n_transformed_features_ = 1
-        elif isinstance(self.features, (list, tuple)):
-            self.n_transformed_features_ = len(self.features)
-        else:
-            raise ValueError("features must be a str, list or tuple")
-
-        self._transform_features = None
-
-        return self
-
-    def transform(self, X, y=None):
-        """Transform data into the Catch22 features.
-
-        Parameters
-        ----------
-        X : 3D numpy array of shape [n_instances, n_dimensions, n_features],
-            input time series panel.
-        y : ignored.
-
-        Returns
-        -------
-        c22 : Pandas DataFrame of shape [n_instances, c*n_dimensions] where c is the
-             number of features requested, containing Catch22 features for X.
-        """
-        X = self._validate_data(X=X, reset=False)
-        X = self._convert_X(X)
-
-        n_instances = len(X)
-
-        f_idx = _verify_features(self.features, self.catch24)
-
-        import pycatch22
-
-        features = [
-            pycatch22.DN_HistogramMode_5,
-            pycatch22.DN_HistogramMode_10,
-            pycatch22.SB_BinaryStats_diff_longstretch0,
-            pycatch22.DN_OutlierInclude_p_001_mdrmd,
-            pycatch22.DN_OutlierInclude_n_001_mdrmd,
-            pycatch22.CO_f1ecac,
-            pycatch22.CO_FirstMin_ac,
-            pycatch22.SP_Summaries_welch_rect_area_5_1,
-            pycatch22.SP_Summaries_welch_rect_centroid,
-            pycatch22.FC_LocalSimple_mean3_stderr,
-            pycatch22.CO_trev_1_num,
-            pycatch22.CO_HistogramAMI_even_2_5,
-            pycatch22.IN_AutoMutualInfoStats_40_gaussian_fmmi,
-            pycatch22.MD_hrv_classic_pnn40,
-            pycatch22.SB_BinaryStats_mean_longstretch1,
-            pycatch22.SB_MotifThree_quantile_hh,
-            pycatch22.FC_LocalSimple_mean1_tauresrat,
-            pycatch22.CO_Embed2_Dist_tau_d_expfit_meandiff,
-            pycatch22.SC_FluctAnal_2_dfa_50_1_2_logi_prop_r1,
-            pycatch22.SC_FluctAnal_2_rsrangefit_50_1_logi_prop_r1,
-            pycatch22.SB_TransitionMatrix_3ac_sumdiagcov,
-            pycatch22.PD_PeriodicityWang_th0_01,
-        ]
-
-        threads_to_use = check_n_jobs(self.n_jobs)
-
-        c22_list = Parallel(n_jobs=threads_to_use)(
-            delayed(self._transform_case)(
-                X[i],
-                f_idx,
-                features,
-            )
-            for i in range(n_instances)
-        )
-
-        if self.replace_nans:
-            c22_list = np.nan_to_num(c22_list, False, 0, 0, 0)
-
-        return np.array(c22_list)
-
-    def _transform_case(self, X, f_idx, features):
-        c22 = np.zeros(len(f_idx) * len(X))
-
-        if self._transform_features is not None and len(
-            self._transform_features
-        ) == len(c22):
-            transform_feature = self._transform_features
-        else:
-            transform_feature = [True] * len(c22)
-
-        f_count = -1
-        for i in range(len(X)):
-            dim = i * len(f_idx)
-            series = list(X[i])
-
-            if self.outlier_norm and (3 in f_idx or 4 in f_idx):
-                outlier_series = list(z_normalise_series(X[i]))
-
-            for n, feature in enumerate(f_idx):
-                f_count += 1
-                if not transform_feature[f_count]:
-                    continue
-
-                if self.outlier_norm and feature in [3, 4]:
-                    c22[dim + n] = features[feature](outlier_series)
-                if feature == 22:
-                    c22[dim + n] = np.mean(series)
-                elif feature == 23:
-                    c22[dim + n] = np.std(series)
-                else:
-                    c22[dim + n] = features[feature](series)
-
-        return c22
-
-    def _more_tags(self):
-        return {
-            "X_types": ["np_list", "3darray"],
-            "requires_fit": False,
-            "optional_dependency": True,
-        }
```

### Comparing `tsml-0.0.7/tsml/transformations/_function_transformer.py` & `tsml-0.1.0/tsml/transformations/_function_transformer.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.7/tsml/transformations/_interval_extraction.py` & `tsml-0.1.0/tsml/transformations/_interval_extraction.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.7/tsml/transformations/_periodogram.py` & `tsml-0.1.0/tsml/transformations/_periodogram.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.7/tsml/transformations/_sfa.py` & `tsml-0.1.0/tsml/transformations/_sfa.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.7/tsml/transformations/_shapelet_transform.py` & `tsml-0.1.0/tsml/transformations/_shapelet_transform.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.7/tsml/transformations/_summary_features.py` & `tsml-0.1.0/tsml/transformations/_summary_features.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.7/tsml/utils/_tags.py` & `tsml-0.1.0/tsml/utils/_tags.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.7/tsml/utils/discovery.py` & `tsml-0.1.0/tsml/utils/discovery.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.7/tsml/utils/numba_functions/general.py` & `tsml-0.1.0/tsml/utils/numba_functions/general.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.7/tsml/utils/numba_functions/stats.py` & `tsml-0.1.0/tsml/utils/numba_functions/stats.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.7/tsml/utils/testing.py` & `tsml-0.1.0/tsml/utils/testing.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 __author__ = ["MatthewMiddlehurst"]
 __all__ = [
     "generate_test_estimators",
     "parametrize_with_checks",
     "generate_3d_test_data",
 ]
 
+import warnings
 from functools import partial
 from typing import Callable, List, Tuple, Union
 
 import numpy as np
 from sklearn.base import BaseEstimator
 from sklearn.utils.estimator_checks import (
     _get_check_estimator_ids,
@@ -25,14 +26,17 @@
 
 
 def generate_test_estimators() -> List[BaseEstimator]:
     """Generate a list of all estimators in tsml with test parameters.
 
     Uses estimator parameters from `get_test_params` if available.
 
+    If an optional dependency is not present, the estimator is skipped and a warning is
+    raised.
+
     Returns
     -------
     estimators : list
         A list of estimators using test parameters.
     """
     classes = all_estimators()
     estimators = []
@@ -41,17 +45,31 @@
         if callable(m):
             params = c[1].get_test_params()
         else:
             params = {}
 
         if isinstance(params, list):
             for p in params:
-                estimators.append(c[1](**p))
+                try:
+                    estimators.append(c[1](**p))
+                except ModuleNotFoundError:
+                    warnings.warn(
+                        f"Unable to create estimator {c[0]} with parameters {p}. "
+                        f"Most likely an optional dependency is not present.",
+                        ImportWarning,
+                    )
         else:
-            estimators.append(c[1](**params))
+            try:
+                estimators.append(c[1](**params))
+            except ModuleNotFoundError:
+                warnings.warn(
+                    f"Unable to create estimator {c[0]} with parameters {params}. "
+                    f"Most likely an optional dependency is not present.",
+                    ImportWarning,
+                )
     return estimators
 
 
 def parametrize_with_checks(estimators: List[BaseEstimator]) -> Callable:
     """Pytest specific decorator for parametrizing estimator checks.
 
     If the estimator is a `BaseTimeSeriesEstimator` then the `tsml` checks are used,
```

### Comparing `tsml-0.0.7/tsml/utils/validation.py` & `tsml-0.1.0/tsml/utils/validation.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.7/tsml/vector/_cit.py` & `tsml-0.1.0/tsml/vector/_cit.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.7/tsml/vector/_rotation_forest.py` & `tsml-0.1.0/tsml/vector/_rotation_forest.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.7/tsml/vector/tests/test_rotation_forest.py` & `tsml-0.1.0/tsml/vector/tests/test_rotation_forest.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.7/tsml.egg-info/PKG-INFO` & `tsml-0.1.0/tsml.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsml
-Version: 0.0.7
+Version: 0.1.0
 Summary: A toolkit for time series machine learning algorithms.
 Author-email: Matthew Middlehurst <m.middlehurst@uea.ac.uk>, Tony Bagnall <ajb@uea.ac.uk>
 License: BSD 3-Clause License
         
         Copyright (c) The Time Series Machine Learning (tsml) developers.
         All rights reserved.
         
@@ -46,14 +46,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: extras
+Provides-Extra: unstable_extras
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE
 
 # tsml
 
 A toolkit for time series machine learning algorithms
```

### Comparing `tsml-0.0.7/tsml.egg-info/SOURCES.txt` & `tsml-0.1.0/tsml.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -20,31 +20,35 @@
 tsml/datasets/MinimalGasPrices/MinimalGasPrices_TRAIN.ts
 tsml/datasets/MinimalJapaneseVowels/MinimalJapaneseVowels_TEST.ts
 tsml/datasets/MinimalJapaneseVowels/MinimalJapaneseVowels_TRAIN.ts
 tsml/datasets/UnequalMinimalChinatown/UnequalMinimalChinatown_TEST.ts
 tsml/datasets/UnequalMinimalChinatown/UnequalMinimalChinatown_TRAIN.ts
 tsml/datasets/UnequalMinimalGasPrices/UnequalMinimalGasPrices_TEST.ts
 tsml/datasets/UnequalMinimalGasPrices/UnequalMinimalGasPrices_TRAIN.ts
-tsml/deep_learning/__init__.py
-tsml/deep_learning/base.py
+tsml/datasets/tests/__init__.py
+tsml/datasets/tests/_expected_data_io_output.py
+tsml/datasets/tests/test_data_io.py
 tsml/dictionary_based/__init__.py
 tsml/distance_based/__init__.py
+tsml/distance_based/_pf.py
 tsml/dummy/__init__.py
 tsml/dummy/_dummy.py
 tsml/feature_based/__init__.py
 tsml/feature_based/_catch22.py
 tsml/interval_based/__init__.py
 tsml/interval_based/_base.py
 tsml/interval_based/_cif.py
 tsml/interval_based/_interval_forest.py
 tsml/interval_based/_interval_pipelines.py
 tsml/interval_based/_rise.py
 tsml/interval_based/_stsf.py
 tsml/interval_based/_tsf.py
 tsml/shapelet_based/__init__.py
+tsml/shapelet_based/_mrsqm.py
+tsml/shapelet_based/_rsf.py
 tsml/shapelet_based/_stc.py
 tsml/tests/__init__.py
 tsml/tests/_sklearn_checks.py
 tsml/tests/estimator_checks.py
 tsml/tests/test_all_estimators.py
 tsml/tests/test_interface.py
 tsml/transformations/__init__.py
```

