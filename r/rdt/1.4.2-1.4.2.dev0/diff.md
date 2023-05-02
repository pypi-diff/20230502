# Comparing `tmp/rdt-1.4.2.tar.gz` & `tmp/rdt-1.4.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdt-1.4.2.tar", last modified: Tue May  2 18:00:30 2023, max compression
+gzip compressed data, was "rdt-1.4.2.dev0.tar", last modified: Mon May  1 18:10:49 2023, max compression
```

## Comparing `rdt-1.4.2.tar` & `rdt-1.4.2.dev0.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-02 18:00:30.982602 rdt-1.4.2/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       56 2023-01-18 20:52:41.000000 rdt-1.4.2/AUTHORS.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    25996 2023-01-18 20:52:41.000000 rdt-1.4.2/CONTRIBUTING.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    43337 2023-05-02 18:00:28.000000 rdt-1.4.2/HISTORY.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4872 2023-01-18 20:52:41.000000 rdt-1.4.2/LICENSE
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      284 2022-08-17 01:38:30.000000 rdt-1.4.2/MANIFEST.in
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    51391 2023-05-02 18:00:30.982810 rdt-1.4.2/PKG-INFO
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7109 2023-01-18 20:52:41.000000 rdt-1.4.2/README.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6499 2022-08-17 01:38:30.000000 rdt-1.4.2/RELEASE.md
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-02 18:00:30.963723 rdt-1.4.2/rdt/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2641 2023-05-02 18:00:28.000000 rdt-1.4.2/rdt/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      861 2023-04-13 17:39:49.000000 rdt-1.4.2/rdt/_addons.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      729 2023-01-18 20:52:41.000000 rdt-1.4.2/rdt/errors.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    30929 2023-01-18 20:52:41.000000 rdt-1.4.2/rdt/hyper_transformer.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-02 18:00:30.965438 rdt-1.4.2/rdt/performance/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      262 2022-08-17 01:38:30.000000 rdt-1.4.2/rdt/performance/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-02 18:00:30.967575 rdt-1.4.2/rdt/performance/datasets/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      847 2022-08-17 01:38:30.000000 rdt-1.4.2/rdt/performance/datasets/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1158 2022-08-17 01:38:30.000000 rdt-1.4.2/rdt/performance/datasets/base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6125 2022-08-18 00:01:17.000000 rdt-1.4.2/rdt/performance/datasets/boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    11724 2023-01-18 20:52:41.000000 rdt-1.4.2/rdt/performance/datasets/categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5734 2023-01-18 20:52:41.000000 rdt-1.4.2/rdt/performance/datasets/datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8406 2023-01-18 20:52:41.000000 rdt-1.4.2/rdt/performance/datasets/numerical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1893 2022-08-17 01:38:30.000000 rdt-1.4.2/rdt/performance/datasets/pii.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1898 2022-08-17 01:38:30.000000 rdt-1.4.2/rdt/performance/datasets/text.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      558 2022-08-17 01:38:30.000000 rdt-1.4.2/rdt/performance/datasets/utils.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3294 2023-01-18 20:52:41.000000 rdt-1.4.2/rdt/performance/performance.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3442 2022-08-18 00:01:17.000000 rdt-1.4.2/rdt/performance/profiling.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-02 18:00:30.970203 rdt-1.4.2/rdt/transformers/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4940 2023-04-13 17:39:49.000000 rdt-1.4.2/rdt/transformers/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-02 18:00:30.970507 rdt-1.4.2/rdt/transformers/addons/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3398 2023-01-18 20:52:41.000000 rdt-1.4.2/rdt/transformers/addons/addons_setup.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    13951 2023-01-18 20:52:41.000000 rdt-1.4.2/rdt/transformers/base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3023 2023-01-18 20:52:41.000000 rdt-1.4.2/rdt/transformers/boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    21411 2023-04-13 17:39:49.000000 rdt-1.4.2/rdt/transformers/categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7790 2023-05-02 18:00:28.000000 rdt-1.4.2/rdt/transformers/datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5166 2023-05-02 18:00:28.000000 rdt-1.4.2/rdt/transformers/null.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    20097 2023-01-18 20:52:41.000000 rdt-1.4.2/rdt/transformers/numerical.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-02 18:00:30.971190 rdt-1.4.2/rdt/transformers/pii/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      212 2022-08-18 00:01:17.000000 rdt-1.4.2/rdt/transformers/pii/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    12429 2023-04-13 17:39:49.000000 rdt-1.4.2/rdt/transformers/pii/anonymizer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1052 2023-01-18 20:52:41.000000 rdt-1.4.2/rdt/transformers/pii/utils.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4847 2023-01-18 20:52:41.000000 rdt-1.4.2/rdt/transformers/text.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4576 2023-04-26 21:05:25.000000 rdt-1.4.2/rdt/transformers/utils.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-02 18:00:30.964898 rdt-1.4.2/rdt.egg-info/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    51391 2023-05-02 18:00:30.000000 rdt-1.4.2/rdt.egg-info/PKG-INFO
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2987 2023-05-02 18:00:30.000000 rdt-1.4.2/rdt.egg-info/SOURCES.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-05-02 18:00:30.000000 rdt-1.4.2/rdt.egg-info/dependency_links.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-05-02 18:00:30.000000 rdt-1.4.2/rdt.egg-info/not-zip-safe
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1448 2023-05-02 18:00:30.000000 rdt-1.4.2/rdt.egg-info/requires.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        4 2023-05-02 18:00:30.000000 rdt-1.4.2/rdt.egg-info/top_level.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1590 2023-05-02 18:00:30.983373 rdt-1.4.2/setup.cfg
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4178 2023-05-02 18:00:28.000000 rdt-1.4.2/setup.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-02 18:00:30.971806 rdt-1.4.2/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      536 2022-08-17 01:38:30.000000 rdt-1.4.2/tests/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8197 2023-01-18 20:52:41.000000 rdt-1.4.2/tests/code_style.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    21679 2023-01-18 20:52:41.000000 rdt-1.4.2/tests/contributing.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-02 18:00:30.959765 rdt-1.4.2/tests/datasets/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-02 18:00:30.972882 rdt-1.4.2/tests/datasets/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3770 2022-08-17 01:38:30.000000 rdt-1.4.2/tests/datasets/tests/test_boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4044 2022-08-17 01:38:30.000000 rdt-1.4.2/tests/datasets/tests/test_categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1980 2022-08-17 01:38:30.000000 rdt-1.4.2/tests/datasets/tests/test_datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2886 2022-08-17 01:38:30.000000 rdt-1.4.2/tests/datasets/tests/test_numerical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      671 2022-08-17 01:38:30.000000 rdt-1.4.2/tests/datasets/tests/test_utils.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-02 18:00:30.973442 rdt-1.4.2/tests/integration/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-08-17 01:38:30.000000 rdt-1.4.2/tests/integration/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    43103 2023-05-02 18:00:28.000000 rdt-1.4.2/tests/integration/test_hyper_transformer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     9356 2023-04-13 17:39:49.000000 rdt-1.4.2/tests/integration/test_transformers.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-02 18:00:30.975111 rdt-1.4.2/tests/integration/transformers/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       52 2022-08-17 01:38:30.000000 rdt-1.4.2/tests/integration/transformers/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-02 18:00:30.975501 rdt-1.4.2/tests/integration/transformers/pii/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       86 2022-08-17 01:38:30.000000 rdt-1.4.2/tests/integration/transformers/pii/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6410 2023-01-18 20:52:41.000000 rdt-1.4.2/tests/integration/transformers/pii/test_anonymizer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3880 2023-01-18 20:52:41.000000 rdt-1.4.2/tests/integration/transformers/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2512 2023-01-18 20:52:41.000000 rdt-1.4.2/tests/integration/transformers/test_boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    13328 2023-04-13 17:39:49.000000 rdt-1.4.2/tests/integration/transformers/test_categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2312 2023-01-18 20:52:41.000000 rdt-1.4.2/tests/integration/transformers/test_datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8679 2023-01-18 20:52:41.000000 rdt-1.4.2/tests/integration/transformers/test_numerical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8389 2023-04-13 17:39:49.000000 rdt-1.4.2/tests/integration/transformers/test_text.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-02 18:00:30.976240 rdt-1.4.2/tests/performance/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       81 2022-08-17 01:38:30.000000 rdt-1.4.2/tests/performance/README.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      190 2022-08-17 01:38:30.000000 rdt-1.4.2/tests/performance/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5112 2023-04-13 17:39:49.000000 rdt-1.4.2/tests/performance/test_performance.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-02 18:00:30.976608 rdt-1.4.2/tests/performance/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       39 2022-08-17 01:38:30.000000 rdt-1.4.2/tests/performance/tests/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3224 2022-08-18 00:01:17.000000 rdt-1.4.2/tests/performance/tests/test_profiling.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-02 18:00:30.977455 rdt-1.4.2/tests/quality/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       35 2022-08-17 01:38:30.000000 rdt-1.4.2/tests/quality/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    30119 2022-08-17 01:38:30.000000 rdt-1.4.2/tests/quality/dataset_info.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10137 2023-05-02 18:00:28.000000 rdt-1.4.2/tests/quality/test_quality.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1531 2022-08-17 01:38:30.000000 rdt-1.4.2/tests/quality/utils.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-02 18:00:30.978159 rdt-1.4.2/tests/unit/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       32 2022-08-17 01:38:30.000000 rdt-1.4.2/tests/unit/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1192 2023-04-13 17:39:49.000000 rdt-1.4.2/tests/unit/test___init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1359 2023-04-13 17:39:49.000000 rdt-1.4.2/tests/unit/test__addons.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)   103818 2023-01-18 20:52:41.000000 rdt-1.4.2/tests/unit/test_hyper_transformer.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-02 18:00:30.981024 rdt-1.4.2/tests/unit/transformers/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       45 2022-08-17 01:38:30.000000 rdt-1.4.2/tests/unit/transformers/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-02 18:00:30.981279 rdt-1.4.2/tests/unit/transformers/addons/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       33 2022-08-17 01:38:30.000000 rdt-1.4.2/tests/unit/transformers/addons/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-02 18:00:30.981623 rdt-1.4.2/tests/unit/transformers/addons/identity/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       41 2022-08-17 01:38:30.000000 rdt-1.4.2/tests/unit/transformers/addons/identity/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2234 2023-01-18 20:52:41.000000 rdt-1.4.2/tests/unit/transformers/addons/identity/test_identity.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-02 18:00:30.982317 rdt-1.4.2/tests/unit/transformers/pii/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       60 2022-08-17 01:38:30.000000 rdt-1.4.2/tests/unit/transformers/pii/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    27923 2023-04-13 17:39:49.000000 rdt-1.4.2/tests/unit/transformers/pii/test_anonymizer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      985 2023-01-18 20:52:41.000000 rdt-1.4.2/tests/unit/transformers/pii/test_utils.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2475 2023-01-18 20:52:41.000000 rdt-1.4.2/tests/unit/transformers/test___init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    38553 2023-04-13 17:39:49.000000 rdt-1.4.2/tests/unit/transformers/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8522 2023-01-18 20:52:41.000000 rdt-1.4.2/tests/unit/transformers/test_boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    60429 2023-04-13 17:39:49.000000 rdt-1.4.2/tests/unit/transformers/test_categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    18913 2023-01-18 20:52:41.000000 rdt-1.4.2/tests/unit/transformers/test_datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    21103 2023-05-02 18:00:28.000000 rdt-1.4.2/tests/unit/transformers/test_null.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    61010 2023-01-18 20:52:41.000000 rdt-1.4.2/tests/unit/transformers/test_numerical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    12685 2023-04-13 17:39:49.000000 rdt-1.4.2/tests/unit/transformers/test_text.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1513 2023-04-26 21:05:25.000000 rdt-1.4.2/tests/unit/transformers/test_utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:49.255604 rdt-1.4.2.dev0/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       56 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/AUTHORS.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    25996 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/CONTRIBUTING.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    42880 2023-04-26 21:05:25.000000 rdt-1.4.2.dev0/HISTORY.md
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4872 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/LICENSE
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      284 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/MANIFEST.in
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    50939 2023-05-01 18:10:49.255756 rdt-1.4.2.dev0/PKG-INFO
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     7109 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/README.md
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6499 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/RELEASE.md
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:49.238888 rdt-1.4.2.dev0/rdt/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2646 2023-05-01 18:10:03.000000 rdt-1.4.2.dev0/rdt/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      861 2023-04-13 17:39:49.000000 rdt-1.4.2.dev0/rdt/_addons.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      729 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/rdt/errors.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    30929 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/rdt/hyper_transformer.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:49.240742 rdt-1.4.2.dev0/rdt/performance/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      262 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/rdt/performance/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:49.242811 rdt-1.4.2.dev0/rdt/performance/datasets/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      847 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/rdt/performance/datasets/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1158 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/rdt/performance/datasets/base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6125 2022-08-18 00:01:17.000000 rdt-1.4.2.dev0/rdt/performance/datasets/boolean.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    11724 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/rdt/performance/datasets/categorical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5734 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/rdt/performance/datasets/datetime.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8406 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/rdt/performance/datasets/numerical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1893 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/rdt/performance/datasets/pii.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1898 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/rdt/performance/datasets/text.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      558 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/rdt/performance/datasets/utils.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3294 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/rdt/performance/performance.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3442 2022-08-18 00:01:17.000000 rdt-1.4.2.dev0/rdt/performance/profiling.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:49.244572 rdt-1.4.2.dev0/rdt/transformers/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4940 2023-04-13 17:39:49.000000 rdt-1.4.2.dev0/rdt/transformers/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:49.244851 rdt-1.4.2.dev0/rdt/transformers/addons/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3398 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/rdt/transformers/addons/addons_setup.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    13951 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/rdt/transformers/base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3023 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/rdt/transformers/boolean.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    21411 2023-04-13 17:39:49.000000 rdt-1.4.2.dev0/rdt/transformers/categorical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     7790 2023-05-01 18:10:03.000000 rdt-1.4.2.dev0/rdt/transformers/datetime.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5166 2023-05-01 18:10:03.000000 rdt-1.4.2.dev0/rdt/transformers/null.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    20097 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/rdt/transformers/numerical.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:49.245461 rdt-1.4.2.dev0/rdt/transformers/pii/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      212 2022-08-18 00:01:17.000000 rdt-1.4.2.dev0/rdt/transformers/pii/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    12429 2023-04-13 17:39:49.000000 rdt-1.4.2.dev0/rdt/transformers/pii/anonymizer.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1052 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/rdt/transformers/pii/utils.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4847 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/rdt/transformers/text.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4576 2023-04-26 21:05:25.000000 rdt-1.4.2.dev0/rdt/transformers/utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:49.240117 rdt-1.4.2.dev0/rdt.egg-info/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    50939 2023-05-01 18:10:49.000000 rdt-1.4.2.dev0/rdt.egg-info/PKG-INFO
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2987 2023-05-01 18:10:49.000000 rdt-1.4.2.dev0/rdt.egg-info/SOURCES.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-05-01 18:10:49.000000 rdt-1.4.2.dev0/rdt.egg-info/dependency_links.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-05-01 18:10:49.000000 rdt-1.4.2.dev0/rdt.egg-info/not-zip-safe
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1448 2023-05-01 18:10:49.000000 rdt-1.4.2.dev0/rdt.egg-info/requires.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        4 2023-05-01 18:10:49.000000 rdt-1.4.2.dev0/rdt.egg-info/top_level.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1595 2023-05-01 18:10:49.256264 rdt-1.4.2.dev0/setup.cfg
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4183 2023-05-01 18:10:03.000000 rdt-1.4.2.dev0/setup.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:49.245932 rdt-1.4.2.dev0/tests/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      536 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/tests/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8197 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/tests/code_style.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    21679 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/tests/contributing.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:49.234862 rdt-1.4.2.dev0/tests/datasets/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:49.246762 rdt-1.4.2.dev0/tests/datasets/tests/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3770 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/tests/datasets/tests/test_boolean.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4044 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/tests/datasets/tests/test_categorical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1980 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/tests/datasets/tests/test_datetime.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2886 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/tests/datasets/tests/test_numerical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      671 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/tests/datasets/tests/test_utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:49.247255 rdt-1.4.2.dev0/tests/integration/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/tests/integration/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    43103 2023-05-01 18:10:03.000000 rdt-1.4.2.dev0/tests/integration/test_hyper_transformer.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     9356 2023-04-13 17:39:49.000000 rdt-1.4.2.dev0/tests/integration/test_transformers.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:49.248385 rdt-1.4.2.dev0/tests/integration/transformers/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       52 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/tests/integration/transformers/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:49.248715 rdt-1.4.2.dev0/tests/integration/transformers/pii/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       86 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/tests/integration/transformers/pii/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6410 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/tests/integration/transformers/pii/test_anonymizer.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3880 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/tests/integration/transformers/test_base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2512 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/tests/integration/transformers/test_boolean.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    13328 2023-04-13 17:39:49.000000 rdt-1.4.2.dev0/tests/integration/transformers/test_categorical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2312 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/tests/integration/transformers/test_datetime.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8679 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/tests/integration/transformers/test_numerical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8389 2023-04-13 17:39:49.000000 rdt-1.4.2.dev0/tests/integration/transformers/test_text.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:49.249385 rdt-1.4.2.dev0/tests/performance/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       81 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/tests/performance/README.md
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      190 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/tests/performance/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5112 2023-04-13 17:39:49.000000 rdt-1.4.2.dev0/tests/performance/test_performance.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:49.249732 rdt-1.4.2.dev0/tests/performance/tests/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       39 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/tests/performance/tests/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3224 2022-08-18 00:01:17.000000 rdt-1.4.2.dev0/tests/performance/tests/test_profiling.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:49.250566 rdt-1.4.2.dev0/tests/quality/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       35 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/tests/quality/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    30119 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/tests/quality/dataset_info.csv
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10137 2023-05-01 18:10:03.000000 rdt-1.4.2.dev0/tests/quality/test_quality.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1531 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/tests/quality/utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:49.251327 rdt-1.4.2.dev0/tests/unit/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       32 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/tests/unit/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1192 2023-04-13 17:39:49.000000 rdt-1.4.2.dev0/tests/unit/test___init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1359 2023-04-13 17:39:49.000000 rdt-1.4.2.dev0/tests/unit/test__addons.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)   103818 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/tests/unit/test_hyper_transformer.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:49.254095 rdt-1.4.2.dev0/tests/unit/transformers/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       45 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/tests/unit/transformers/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:49.254369 rdt-1.4.2.dev0/tests/unit/transformers/addons/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       33 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/tests/unit/transformers/addons/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:49.254693 rdt-1.4.2.dev0/tests/unit/transformers/addons/identity/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       41 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/tests/unit/transformers/addons/identity/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2234 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/tests/unit/transformers/addons/identity/test_identity.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:49.255340 rdt-1.4.2.dev0/tests/unit/transformers/pii/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       60 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/tests/unit/transformers/pii/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    27923 2023-04-13 17:39:49.000000 rdt-1.4.2.dev0/tests/unit/transformers/pii/test_anonymizer.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      985 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/tests/unit/transformers/pii/test_utils.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2475 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/tests/unit/transformers/test___init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    38553 2023-04-13 17:39:49.000000 rdt-1.4.2.dev0/tests/unit/transformers/test_base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8522 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/tests/unit/transformers/test_boolean.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    60429 2023-04-13 17:39:49.000000 rdt-1.4.2.dev0/tests/unit/transformers/test_categorical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    18913 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/tests/unit/transformers/test_datetime.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    21103 2023-05-01 18:10:03.000000 rdt-1.4.2.dev0/tests/unit/transformers/test_null.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    61010 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/tests/unit/transformers/test_numerical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    12685 2023-04-13 17:39:49.000000 rdt-1.4.2.dev0/tests/unit/transformers/test_text.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1513 2023-04-26 21:05:25.000000 rdt-1.4.2.dev0/tests/unit/transformers/test_utils.py
```

### Comparing `rdt-1.4.2/CONTRIBUTING.rst` & `rdt-1.4.2.dev0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/HISTORY.md` & `rdt-1.4.2.dev0/HISTORY.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,9 @@
 # History
 
-## 1.4.2 - 2023-05-02
-
-This release fixes a bug that caused datetime and numerical transformers to crash if a column was all NaNs. Additionally, it adds support for Pandas 2.0!
-
-### Bugs
-
-* Numerical & datetime transformers crash if the entire column is null - Issue [#637](https://github.com/sdv-dev/RDT/issues/637) by @fraces-h
-
-### Maintenance
-
-* Remove upper bound for pandas - Issue [#633](https://github.com/sdv-dev/RDT/issues/633) by @pvk-developer
-
 ## 1.4.1 - 2023-04-25
 
 This release patches an issue that prevented the `RegexGenerator` from working with regexes that had a very large number of possible combinations.
 
 ### Bugs
 
 * RegexGenerator continues to have problems if there are too many possibilities - Issue [#635](https://github.com/sdv-dev/RDT/issues/635) by @pvk-developer
```

### Comparing `rdt-1.4.2/LICENSE` & `rdt-1.4.2.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/PKG-INFO` & `rdt-1.4.2.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdt
-Version: 1.4.2
+Version: 1.4.2.dev0
 Summary: Reversible Data Transforms
 Home-page: https://github.com/sdv-dev/RDT
 Author: DataCebo, Inc.
 Author-email: info@sdv.dev
 License: BSL-1.1
 Keywords: rdt
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -222,26 +222,14 @@
 [Get started using the SDV package](https://sdv.dev/SDV/getting_started/install.html) -- a fully
 integrated solution and your one-stop shop for synthetic data. Or, use the standalone libraries
 for specific needs.
 
 
 # History
 
-## 1.4.2 - 2023-05-02
-
-This release fixes a bug that caused datetime and numerical transformers to crash if a column was all NaNs. Additionally, it adds support for Pandas 2.0!
-
-### Bugs
-
-* Numerical & datetime transformers crash if the entire column is null - Issue [#637](https://github.com/sdv-dev/RDT/issues/637) by @fraces-h
-
-### Maintenance
-
-* Remove upper bound for pandas - Issue [#633](https://github.com/sdv-dev/RDT/issues/633) by @pvk-developer
-
 ## 1.4.1 - 2023-04-25
 
 This release patches an issue that prevented the `RegexGenerator` from working with regexes that had a very large number of possible combinations.
 
 ### Bugs
 
 * RegexGenerator continues to have problems if there are too many possibilities - Issue [#635](https://github.com/sdv-dev/RDT/issues/635) by @pvk-developer
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rdt Version: 1.4.2 Summary: Reversible Data
+Metadata-Version: 2.1 Name: rdt Version: 1.4.2.dev0 Summary: Reversible Data
 Transforms Home-page: https://github.com/sdv-dev/RDT Author: DataCebo, Inc.
 Author-email: info@sdv.dev License: BSL-1.1 Keywords: rdt Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: Free for non-commercial use Classifier: Natural Language
 :: English Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
@@ -92,31 +92,25 @@
 including: * ð Data discovery & transformation. Reverse the transforms to
 reproduce realistic data. * ð§  Multiple machine learning models -- ranging
 from Copulas to Deep Learning -- to create tabular, multi table and time series
 data. * ð Measuring quality and privacy of synthetic data, and comparing
 different synthetic data generation models. [Get started using the SDV package]
 (https://sdv.dev/SDV/getting_started/install.html) -- a fully integrated
 solution and your one-stop shop for synthetic data. Or, use the standalone
-libraries for specific needs. # History ## 1.4.2 - 2023-05-02 This release
-fixes a bug that caused datetime and numerical transformers to crash if a
-column was all NaNs. Additionally, it adds support for Pandas 2.0! ### Bugs *
-Numerical & datetime transformers crash if the entire column is null - Issue
-[#637](https://github.com/sdv-dev/RDT/issues/637) by @fraces-h ### Maintenance
-* Remove upper bound for pandas - Issue [#633](https://github.com/sdv-dev/RDT/
-issues/633) by @pvk-developer ## 1.4.1 - 2023-04-25 This release patches an
-issue that prevented the `RegexGenerator` from working with regexes that had a
-very large number of possible combinations. ### Bugs * RegexGenerator continues
-to have problems if there are too many possibilities - Issue [#635](https://
-github.com/sdv-dev/RDT/issues/635) by @pvk-developer ## 1.4.0 - 2023-04-13 This
-release adds a couple of new features including adding the
-`OrderedLabelEncoder` and deprecating the `CustomLabelEncoder`. It also adds a
-change that makes all generator type transformers in the `HyperTransformer` use
-a different random seed. Additionally, bugs were patched in the
-`RegexGenerator` that caused it to crash or take too long in certain cases.
-Finally, this release improved the detection of Faker functions in the
+libraries for specific needs. # History ## 1.4.1 - 2023-04-25 This release
+patches an issue that prevented the `RegexGenerator` from working with regexes
+that had a very large number of possible combinations. ### Bugs *
+RegexGenerator continues to have problems if there are too many possibilities -
+Issue [#635](https://github.com/sdv-dev/RDT/issues/635) by @pvk-developer ##
+1.4.0 - 2023-04-13 This release adds a couple of new features including adding
+the `OrderedLabelEncoder` and deprecating the `CustomLabelEncoder`. It also
+adds a change that makes all generator type transformers in the
+`HyperTransformer` use a different random seed. Additionally, bugs were patched
+in the `RegexGenerator` that caused it to crash or take too long in certain
+cases. Finally, this release improved the detection of Faker functions in the
 `AnonymizedFaker`. ### Bugs * Find nested Faker provider submodules - PR [#630]
 (https://github.com/sdv-dev/RDT/pull/630) by @frances-h * RegexGenerator fails
 to generate values if there are too many possibilities - Issue [#623](https://
 github.com/sdv-dev/RDT/issues/623) by @R-Palazzo * RegexGenerator takes too
 much time and runs out of memory if there are too many possibilities - Issue
 [#624](https://github.com/sdv-dev/RDT/issues/624) by @R-Palazzo ### New
 Features * Choose a different seed for each transformer - Issue [#619](https://
```

### Comparing `rdt-1.4.2/README.md` & `rdt-1.4.2.dev0/README.md`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/RELEASE.md` & `rdt-1.4.2.dev0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/rdt/__init__.py` & `rdt-1.4.2.dev0/rdt/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 """Top-level package for RDT."""
 
 
 __author__ = 'DataCebo, Inc.'
 __email__ = 'info@sdv.dev'
-__version__ = '1.4.2'
+__version__ = '1.4.2.dev0'
 
 
 import numpy as np
 import pandas as pd
 
 from rdt import transformers
 from rdt._addons import _find_addons
```

### Comparing `rdt-1.4.2/rdt/_addons.py` & `rdt-1.4.2.dev0/rdt/_addons.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/rdt/errors.py` & `rdt-1.4.2.dev0/rdt/errors.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/rdt/hyper_transformer.py` & `rdt-1.4.2.dev0/rdt/hyper_transformer.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/rdt/performance/datasets/__init__.py` & `rdt-1.4.2.dev0/rdt/performance/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/rdt/performance/datasets/base.py` & `rdt-1.4.2.dev0/rdt/performance/datasets/base.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/rdt/performance/datasets/boolean.py` & `rdt-1.4.2.dev0/rdt/performance/datasets/boolean.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/rdt/performance/datasets/categorical.py` & `rdt-1.4.2.dev0/rdt/performance/datasets/categorical.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/rdt/performance/datasets/datetime.py` & `rdt-1.4.2.dev0/rdt/performance/datasets/datetime.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/rdt/performance/datasets/numerical.py` & `rdt-1.4.2.dev0/rdt/performance/datasets/numerical.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/rdt/performance/datasets/pii.py` & `rdt-1.4.2.dev0/rdt/performance/datasets/pii.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/rdt/performance/datasets/text.py` & `rdt-1.4.2.dev0/rdt/performance/datasets/text.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/rdt/performance/datasets/utils.py` & `rdt-1.4.2.dev0/rdt/performance/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/rdt/performance/performance.py` & `rdt-1.4.2.dev0/rdt/performance/performance.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/rdt/performance/profiling.py` & `rdt-1.4.2.dev0/rdt/performance/profiling.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/rdt/transformers/__init__.py` & `rdt-1.4.2.dev0/rdt/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/rdt/transformers/addons/addons_setup.py` & `rdt-1.4.2.dev0/rdt/transformers/addons/addons_setup.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/rdt/transformers/base.py` & `rdt-1.4.2.dev0/rdt/transformers/base.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/rdt/transformers/boolean.py` & `rdt-1.4.2.dev0/rdt/transformers/boolean.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/rdt/transformers/categorical.py` & `rdt-1.4.2.dev0/rdt/transformers/categorical.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/rdt/transformers/datetime.py` & `rdt-1.4.2.dev0/rdt/transformers/datetime.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/rdt/transformers/null.py` & `rdt-1.4.2.dev0/rdt/transformers/null.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/rdt/transformers/numerical.py` & `rdt-1.4.2.dev0/rdt/transformers/numerical.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/rdt/transformers/pii/anonymizer.py` & `rdt-1.4.2.dev0/rdt/transformers/pii/anonymizer.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/rdt/transformers/pii/utils.py` & `rdt-1.4.2.dev0/rdt/transformers/pii/utils.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/rdt/transformers/text.py` & `rdt-1.4.2.dev0/rdt/transformers/text.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/rdt/transformers/utils.py` & `rdt-1.4.2.dev0/rdt/transformers/utils.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/rdt.egg-info/PKG-INFO` & `rdt-1.4.2.dev0/rdt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdt
-Version: 1.4.2
+Version: 1.4.2.dev0
 Summary: Reversible Data Transforms
 Home-page: https://github.com/sdv-dev/RDT
 Author: DataCebo, Inc.
 Author-email: info@sdv.dev
 License: BSL-1.1
 Keywords: rdt
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -222,26 +222,14 @@
 [Get started using the SDV package](https://sdv.dev/SDV/getting_started/install.html) -- a fully
 integrated solution and your one-stop shop for synthetic data. Or, use the standalone libraries
 for specific needs.
 
 
 # History
 
-## 1.4.2 - 2023-05-02
-
-This release fixes a bug that caused datetime and numerical transformers to crash if a column was all NaNs. Additionally, it adds support for Pandas 2.0!
-
-### Bugs
-
-* Numerical & datetime transformers crash if the entire column is null - Issue [#637](https://github.com/sdv-dev/RDT/issues/637) by @fraces-h
-
-### Maintenance
-
-* Remove upper bound for pandas - Issue [#633](https://github.com/sdv-dev/RDT/issues/633) by @pvk-developer
-
 ## 1.4.1 - 2023-04-25
 
 This release patches an issue that prevented the `RegexGenerator` from working with regexes that had a very large number of possible combinations.
 
 ### Bugs
 
 * RegexGenerator continues to have problems if there are too many possibilities - Issue [#635](https://github.com/sdv-dev/RDT/issues/635) by @pvk-developer
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rdt Version: 1.4.2 Summary: Reversible Data
+Metadata-Version: 2.1 Name: rdt Version: 1.4.2.dev0 Summary: Reversible Data
 Transforms Home-page: https://github.com/sdv-dev/RDT Author: DataCebo, Inc.
 Author-email: info@sdv.dev License: BSL-1.1 Keywords: rdt Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: Free for non-commercial use Classifier: Natural Language
 :: English Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
@@ -92,31 +92,25 @@
 including: * ð Data discovery & transformation. Reverse the transforms to
 reproduce realistic data. * ð§  Multiple machine learning models -- ranging
 from Copulas to Deep Learning -- to create tabular, multi table and time series
 data. * ð Measuring quality and privacy of synthetic data, and comparing
 different synthetic data generation models. [Get started using the SDV package]
 (https://sdv.dev/SDV/getting_started/install.html) -- a fully integrated
 solution and your one-stop shop for synthetic data. Or, use the standalone
-libraries for specific needs. # History ## 1.4.2 - 2023-05-02 This release
-fixes a bug that caused datetime and numerical transformers to crash if a
-column was all NaNs. Additionally, it adds support for Pandas 2.0! ### Bugs *
-Numerical & datetime transformers crash if the entire column is null - Issue
-[#637](https://github.com/sdv-dev/RDT/issues/637) by @fraces-h ### Maintenance
-* Remove upper bound for pandas - Issue [#633](https://github.com/sdv-dev/RDT/
-issues/633) by @pvk-developer ## 1.4.1 - 2023-04-25 This release patches an
-issue that prevented the `RegexGenerator` from working with regexes that had a
-very large number of possible combinations. ### Bugs * RegexGenerator continues
-to have problems if there are too many possibilities - Issue [#635](https://
-github.com/sdv-dev/RDT/issues/635) by @pvk-developer ## 1.4.0 - 2023-04-13 This
-release adds a couple of new features including adding the
-`OrderedLabelEncoder` and deprecating the `CustomLabelEncoder`. It also adds a
-change that makes all generator type transformers in the `HyperTransformer` use
-a different random seed. Additionally, bugs were patched in the
-`RegexGenerator` that caused it to crash or take too long in certain cases.
-Finally, this release improved the detection of Faker functions in the
+libraries for specific needs. # History ## 1.4.1 - 2023-04-25 This release
+patches an issue that prevented the `RegexGenerator` from working with regexes
+that had a very large number of possible combinations. ### Bugs *
+RegexGenerator continues to have problems if there are too many possibilities -
+Issue [#635](https://github.com/sdv-dev/RDT/issues/635) by @pvk-developer ##
+1.4.0 - 2023-04-13 This release adds a couple of new features including adding
+the `OrderedLabelEncoder` and deprecating the `CustomLabelEncoder`. It also
+adds a change that makes all generator type transformers in the
+`HyperTransformer` use a different random seed. Additionally, bugs were patched
+in the `RegexGenerator` that caused it to crash or take too long in certain
+cases. Finally, this release improved the detection of Faker functions in the
 `AnonymizedFaker`. ### Bugs * Find nested Faker provider submodules - PR [#630]
 (https://github.com/sdv-dev/RDT/pull/630) by @frances-h * RegexGenerator fails
 to generate values if there are too many possibilities - Issue [#623](https://
 github.com/sdv-dev/RDT/issues/623) by @R-Palazzo * RegexGenerator takes too
 much time and runs out of memory if there are too many possibilities - Issue
 [#624](https://github.com/sdv-dev/RDT/issues/624) by @R-Palazzo ### New
 Features * Choose a different seed for each transformer - Issue [#619](https://
```

### Comparing `rdt-1.4.2/rdt.egg-info/SOURCES.txt` & `rdt-1.4.2.dev0/rdt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/rdt.egg-info/requires.txt` & `rdt-1.4.2.dev0/rdt.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/setup.cfg` & `rdt-1.4.2.dev0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.4.2
+current_version = 1.4.2.dev0
 commit = True
 tag = True
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\.(?P<release>[a-z]+)(?P<candidate>\d+))?
 serialize = 
 	{major}.{minor}.{patch}.{release}{candidate}
 	{major}.{minor}.{patch}
```

### Comparing `rdt-1.4.2/setup.py` & `rdt-1.4.2.dev0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,10 +136,10 @@
         exclude=['rdt.transformers.addons.*']
     ),
     python_requires='>=3.7,<3.12',
     setup_requires=setup_requires,
     test_suite='tests',
     tests_require=tests_require,
     url='https://github.com/sdv-dev/RDT',
-    version='1.4.2',
+    version='1.4.2.dev0',
     zip_safe=False,
 )
```

### Comparing `rdt-1.4.2/tests/__init__.py` & `rdt-1.4.2.dev0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/tests/code_style.py` & `rdt-1.4.2.dev0/tests/code_style.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/tests/contributing.py` & `rdt-1.4.2.dev0/tests/contributing.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/tests/datasets/tests/test_boolean.py` & `rdt-1.4.2.dev0/tests/datasets/tests/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/tests/datasets/tests/test_categorical.py` & `rdt-1.4.2.dev0/tests/datasets/tests/test_categorical.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/tests/datasets/tests/test_datetime.py` & `rdt-1.4.2.dev0/tests/datasets/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/tests/datasets/tests/test_numerical.py` & `rdt-1.4.2.dev0/tests/datasets/tests/test_numerical.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/tests/datasets/tests/test_utils.py` & `rdt-1.4.2.dev0/tests/datasets/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/tests/integration/test_hyper_transformer.py` & `rdt-1.4.2.dev0/tests/integration/test_hyper_transformer.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/tests/integration/test_transformers.py` & `rdt-1.4.2.dev0/tests/integration/test_transformers.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/tests/integration/transformers/pii/test_anonymizer.py` & `rdt-1.4.2.dev0/tests/integration/transformers/pii/test_anonymizer.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/tests/integration/transformers/test_base.py` & `rdt-1.4.2.dev0/tests/integration/transformers/test_base.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/tests/integration/transformers/test_boolean.py` & `rdt-1.4.2.dev0/tests/integration/transformers/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/tests/integration/transformers/test_categorical.py` & `rdt-1.4.2.dev0/tests/integration/transformers/test_categorical.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/tests/integration/transformers/test_datetime.py` & `rdt-1.4.2.dev0/tests/integration/transformers/test_datetime.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/tests/integration/transformers/test_numerical.py` & `rdt-1.4.2.dev0/tests/integration/transformers/test_numerical.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/tests/integration/transformers/test_text.py` & `rdt-1.4.2.dev0/tests/integration/transformers/test_text.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/tests/performance/test_performance.py` & `rdt-1.4.2.dev0/tests/performance/test_performance.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/tests/performance/tests/test_profiling.py` & `rdt-1.4.2.dev0/tests/performance/tests/test_profiling.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/tests/quality/dataset_info.csv` & `rdt-1.4.2.dev0/tests/quality/dataset_info.csv`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/tests/quality/test_quality.py` & `rdt-1.4.2.dev0/tests/quality/test_quality.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/tests/quality/utils.py` & `rdt-1.4.2.dev0/tests/quality/utils.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/tests/unit/test___init__.py` & `rdt-1.4.2.dev0/tests/unit/test___init__.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/tests/unit/test__addons.py` & `rdt-1.4.2.dev0/tests/unit/test__addons.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/tests/unit/test_hyper_transformer.py` & `rdt-1.4.2.dev0/tests/unit/test_hyper_transformer.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/tests/unit/transformers/addons/identity/test_identity.py` & `rdt-1.4.2.dev0/tests/unit/transformers/addons/identity/test_identity.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/tests/unit/transformers/pii/test_anonymizer.py` & `rdt-1.4.2.dev0/tests/unit/transformers/pii/test_anonymizer.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/tests/unit/transformers/pii/test_utils.py` & `rdt-1.4.2.dev0/tests/unit/transformers/pii/test_utils.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/tests/unit/transformers/test___init__.py` & `rdt-1.4.2.dev0/tests/unit/transformers/test___init__.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/tests/unit/transformers/test_base.py` & `rdt-1.4.2.dev0/tests/unit/transformers/test_base.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/tests/unit/transformers/test_boolean.py` & `rdt-1.4.2.dev0/tests/unit/transformers/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/tests/unit/transformers/test_categorical.py` & `rdt-1.4.2.dev0/tests/unit/transformers/test_categorical.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/tests/unit/transformers/test_datetime.py` & `rdt-1.4.2.dev0/tests/unit/transformers/test_datetime.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/tests/unit/transformers/test_null.py` & `rdt-1.4.2.dev0/tests/unit/transformers/test_null.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/tests/unit/transformers/test_numerical.py` & `rdt-1.4.2.dev0/tests/unit/transformers/test_numerical.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/tests/unit/transformers/test_text.py` & `rdt-1.4.2.dev0/tests/unit/transformers/test_text.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.2/tests/unit/transformers/test_utils.py` & `rdt-1.4.2.dev0/tests/unit/transformers/test_utils.py`

 * *Files identical despite different names*

