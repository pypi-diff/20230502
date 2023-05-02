# Comparing `tmp/rdt_identity-1.4.2.tar.gz` & `tmp/rdt_identity-1.4.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdt_identity-1.4.2.tar", last modified: Tue May  2 18:00:33 2023, max compression
+gzip compressed data, was "rdt_identity-1.4.2.dev0.tar", last modified: Mon May  1 18:10:53 2023, max compression
```

## Comparing `rdt_identity-1.4.2.tar` & `rdt_identity-1.4.2.dev0.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-02 18:00:33.294681 rdt_identity-1.4.2/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       56 2023-01-18 20:52:41.000000 rdt_identity-1.4.2/AUTHORS.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    25996 2023-01-18 20:52:41.000000 rdt_identity-1.4.2/CONTRIBUTING.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    43337 2023-05-02 18:00:28.000000 rdt_identity-1.4.2/HISTORY.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4872 2023-01-18 20:52:41.000000 rdt_identity-1.4.2/LICENSE
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      284 2022-08-17 01:38:30.000000 rdt_identity-1.4.2/MANIFEST.in
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8009 2023-05-02 18:00:33.294788 rdt_identity-1.4.2/PKG-INFO
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7109 2023-01-18 20:52:41.000000 rdt_identity-1.4.2/README.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6499 2022-08-17 01:38:30.000000 rdt_identity-1.4.2/RELEASE.md
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-02 18:00:33.283045 rdt_identity-1.4.2/rdt/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-02 18:00:33.283109 rdt_identity-1.4.2/rdt/transformers/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-02 18:00:33.283175 rdt_identity-1.4.2/rdt/transformers/addons/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-02 18:00:33.286622 rdt_identity-1.4.2/rdt/transformers/addons/identity/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-08-17 01:38:30.000000 rdt_identity-1.4.2/rdt/transformers/addons/identity/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1170 2023-01-18 20:52:41.000000 rdt_identity-1.4.2/rdt/transformers/addons/identity/identity.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1590 2023-05-02 18:00:33.295338 rdt_identity-1.4.2/setup.cfg
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4178 2023-05-02 18:00:28.000000 rdt_identity-1.4.2/setup.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-02 18:00:33.287063 rdt_identity-1.4.2/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      536 2022-08-17 01:38:30.000000 rdt_identity-1.4.2/tests/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8197 2023-01-18 20:52:41.000000 rdt_identity-1.4.2/tests/code_style.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    21679 2023-01-18 20:52:41.000000 rdt_identity-1.4.2/tests/contributing.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-02 18:00:33.283492 rdt_identity-1.4.2/tests/datasets/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-02 18:00:33.287811 rdt_identity-1.4.2/tests/datasets/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3770 2022-08-17 01:38:30.000000 rdt_identity-1.4.2/tests/datasets/tests/test_boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4044 2022-08-17 01:38:30.000000 rdt_identity-1.4.2/tests/datasets/tests/test_categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1980 2022-08-17 01:38:30.000000 rdt_identity-1.4.2/tests/datasets/tests/test_datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2886 2022-08-17 01:38:30.000000 rdt_identity-1.4.2/tests/datasets/tests/test_numerical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      671 2022-08-17 01:38:30.000000 rdt_identity-1.4.2/tests/datasets/tests/test_utils.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-02 18:00:33.288277 rdt_identity-1.4.2/tests/integration/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-08-17 01:38:30.000000 rdt_identity-1.4.2/tests/integration/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    43103 2023-05-02 18:00:28.000000 rdt_identity-1.4.2/tests/integration/test_hyper_transformer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     9356 2023-04-13 17:39:49.000000 rdt_identity-1.4.2/tests/integration/test_transformers.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-02 18:00:33.289337 rdt_identity-1.4.2/tests/integration/transformers/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       52 2022-08-17 01:38:30.000000 rdt_identity-1.4.2/tests/integration/transformers/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-02 18:00:33.289625 rdt_identity-1.4.2/tests/integration/transformers/pii/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       86 2022-08-17 01:38:30.000000 rdt_identity-1.4.2/tests/integration/transformers/pii/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6410 2023-01-18 20:52:41.000000 rdt_identity-1.4.2/tests/integration/transformers/pii/test_anonymizer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3880 2023-01-18 20:52:41.000000 rdt_identity-1.4.2/tests/integration/transformers/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2512 2023-01-18 20:52:41.000000 rdt_identity-1.4.2/tests/integration/transformers/test_boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    13328 2023-04-13 17:39:49.000000 rdt_identity-1.4.2/tests/integration/transformers/test_categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2312 2023-01-18 20:52:41.000000 rdt_identity-1.4.2/tests/integration/transformers/test_datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8679 2023-01-18 20:52:41.000000 rdt_identity-1.4.2/tests/integration/transformers/test_numerical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8389 2023-04-13 17:39:49.000000 rdt_identity-1.4.2/tests/integration/transformers/test_text.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-02 18:00:33.290199 rdt_identity-1.4.2/tests/performance/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       81 2022-08-17 01:38:30.000000 rdt_identity-1.4.2/tests/performance/README.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      190 2022-08-17 01:38:30.000000 rdt_identity-1.4.2/tests/performance/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5112 2023-04-13 17:39:49.000000 rdt_identity-1.4.2/tests/performance/test_performance.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-02 18:00:33.290518 rdt_identity-1.4.2/tests/performance/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       39 2022-08-17 01:38:30.000000 rdt_identity-1.4.2/tests/performance/tests/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3224 2022-08-18 00:01:17.000000 rdt_identity-1.4.2/tests/performance/tests/test_profiling.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-02 18:00:33.291154 rdt_identity-1.4.2/tests/quality/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       35 2022-08-17 01:38:30.000000 rdt_identity-1.4.2/tests/quality/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    30119 2022-08-17 01:38:30.000000 rdt_identity-1.4.2/tests/quality/dataset_info.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10137 2023-05-02 18:00:28.000000 rdt_identity-1.4.2/tests/quality/test_quality.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1531 2022-08-17 01:38:30.000000 rdt_identity-1.4.2/tests/quality/utils.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-02 18:00:33.291731 rdt_identity-1.4.2/tests/unit/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       32 2022-08-17 01:38:30.000000 rdt_identity-1.4.2/tests/unit/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1192 2023-04-13 17:39:49.000000 rdt_identity-1.4.2/tests/unit/test___init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1359 2023-04-13 17:39:49.000000 rdt_identity-1.4.2/tests/unit/test__addons.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)   103818 2023-01-18 20:52:41.000000 rdt_identity-1.4.2/tests/unit/test_hyper_transformer.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-02 18:00:33.293481 rdt_identity-1.4.2/tests/unit/transformers/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       45 2022-08-17 01:38:30.000000 rdt_identity-1.4.2/tests/unit/transformers/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-02 18:00:33.293629 rdt_identity-1.4.2/tests/unit/transformers/addons/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       33 2022-08-17 01:38:30.000000 rdt_identity-1.4.2/tests/unit/transformers/addons/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-02 18:00:33.293928 rdt_identity-1.4.2/tests/unit/transformers/addons/identity/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       41 2022-08-17 01:38:30.000000 rdt_identity-1.4.2/tests/unit/transformers/addons/identity/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2234 2023-01-18 20:52:41.000000 rdt_identity-1.4.2/tests/unit/transformers/addons/identity/test_identity.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-02 18:00:33.294483 rdt_identity-1.4.2/tests/unit/transformers/pii/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       60 2022-08-17 01:38:30.000000 rdt_identity-1.4.2/tests/unit/transformers/pii/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    27923 2023-04-13 17:39:49.000000 rdt_identity-1.4.2/tests/unit/transformers/pii/test_anonymizer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      985 2023-01-18 20:52:41.000000 rdt_identity-1.4.2/tests/unit/transformers/pii/test_utils.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2475 2023-01-18 20:52:41.000000 rdt_identity-1.4.2/tests/unit/transformers/test___init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    38553 2023-04-13 17:39:49.000000 rdt_identity-1.4.2/tests/unit/transformers/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8522 2023-01-18 20:52:41.000000 rdt_identity-1.4.2/tests/unit/transformers/test_boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    60429 2023-04-13 17:39:49.000000 rdt_identity-1.4.2/tests/unit/transformers/test_categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    18913 2023-01-18 20:52:41.000000 rdt_identity-1.4.2/tests/unit/transformers/test_datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    21103 2023-05-02 18:00:28.000000 rdt_identity-1.4.2/tests/unit/transformers/test_null.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    61010 2023-01-18 20:52:41.000000 rdt_identity-1.4.2/tests/unit/transformers/test_numerical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    12685 2023-04-13 17:39:49.000000 rdt_identity-1.4.2/tests/unit/transformers/test_text.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1513 2023-04-26 21:05:25.000000 rdt_identity-1.4.2/tests/unit/transformers/test_utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.139033 rdt_identity-1.4.2.dev0/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       56 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/AUTHORS.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    25996 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/CONTRIBUTING.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    42880 2023-04-26 21:05:25.000000 rdt_identity-1.4.2.dev0/HISTORY.md
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4872 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/LICENSE
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      284 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/MANIFEST.in
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8014 2023-05-01 18:10:53.139134 rdt_identity-1.4.2.dev0/PKG-INFO
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     7109 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/README.md
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6499 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/RELEASE.md
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.127908 rdt_identity-1.4.2.dev0/rdt/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.127971 rdt_identity-1.4.2.dev0/rdt/transformers/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.128033 rdt_identity-1.4.2.dev0/rdt/transformers/addons/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.131330 rdt_identity-1.4.2.dev0/rdt/transformers/addons/identity/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/rdt/transformers/addons/identity/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1170 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/rdt/transformers/addons/identity/identity.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1595 2023-05-01 18:10:53.139824 rdt_identity-1.4.2.dev0/setup.cfg
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4183 2023-05-01 18:10:03.000000 rdt_identity-1.4.2.dev0/setup.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.131804 rdt_identity-1.4.2.dev0/tests/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      536 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8197 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/tests/code_style.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    21679 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/tests/contributing.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.128281 rdt_identity-1.4.2.dev0/tests/datasets/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.132518 rdt_identity-1.4.2.dev0/tests/datasets/tests/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3770 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/datasets/tests/test_boolean.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4044 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/datasets/tests/test_categorical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1980 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/datasets/tests/test_datetime.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2886 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/datasets/tests/test_numerical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      671 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/datasets/tests/test_utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.133022 rdt_identity-1.4.2.dev0/tests/integration/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/integration/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    43103 2023-05-01 18:10:03.000000 rdt_identity-1.4.2.dev0/tests/integration/test_hyper_transformer.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     9356 2023-04-13 17:39:49.000000 rdt_identity-1.4.2.dev0/tests/integration/test_transformers.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.134071 rdt_identity-1.4.2.dev0/tests/integration/transformers/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       52 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/integration/transformers/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.134360 rdt_identity-1.4.2.dev0/tests/integration/transformers/pii/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       86 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/integration/transformers/pii/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6410 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/tests/integration/transformers/pii/test_anonymizer.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3880 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/tests/integration/transformers/test_base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2512 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/tests/integration/transformers/test_boolean.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    13328 2023-04-13 17:39:49.000000 rdt_identity-1.4.2.dev0/tests/integration/transformers/test_categorical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2312 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/tests/integration/transformers/test_datetime.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8679 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/tests/integration/transformers/test_numerical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8389 2023-04-13 17:39:49.000000 rdt_identity-1.4.2.dev0/tests/integration/transformers/test_text.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.134809 rdt_identity-1.4.2.dev0/tests/performance/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       81 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/performance/README.md
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      190 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/performance/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5112 2023-04-13 17:39:49.000000 rdt_identity-1.4.2.dev0/tests/performance/test_performance.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.135130 rdt_identity-1.4.2.dev0/tests/performance/tests/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       39 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/performance/tests/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3224 2022-08-18 00:01:17.000000 rdt_identity-1.4.2.dev0/tests/performance/tests/test_profiling.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.135715 rdt_identity-1.4.2.dev0/tests/quality/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       35 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/quality/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    30119 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/quality/dataset_info.csv
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10137 2023-05-01 18:10:03.000000 rdt_identity-1.4.2.dev0/tests/quality/test_quality.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1531 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/quality/utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.136295 rdt_identity-1.4.2.dev0/tests/unit/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       32 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/unit/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1192 2023-04-13 17:39:49.000000 rdt_identity-1.4.2.dev0/tests/unit/test___init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1359 2023-04-13 17:39:49.000000 rdt_identity-1.4.2.dev0/tests/unit/test__addons.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)   103818 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/tests/unit/test_hyper_transformer.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.137949 rdt_identity-1.4.2.dev0/tests/unit/transformers/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       45 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/unit/transformers/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.138108 rdt_identity-1.4.2.dev0/tests/unit/transformers/addons/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       33 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/unit/transformers/addons/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.138407 rdt_identity-1.4.2.dev0/tests/unit/transformers/addons/identity/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       41 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/unit/transformers/addons/identity/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2234 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/tests/unit/transformers/addons/identity/test_identity.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.138889 rdt_identity-1.4.2.dev0/tests/unit/transformers/pii/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       60 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/unit/transformers/pii/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    27923 2023-04-13 17:39:49.000000 rdt_identity-1.4.2.dev0/tests/unit/transformers/pii/test_anonymizer.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      985 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/tests/unit/transformers/pii/test_utils.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2475 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/tests/unit/transformers/test___init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    38553 2023-04-13 17:39:49.000000 rdt_identity-1.4.2.dev0/tests/unit/transformers/test_base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8522 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/tests/unit/transformers/test_boolean.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    60429 2023-04-13 17:39:49.000000 rdt_identity-1.4.2.dev0/tests/unit/transformers/test_categorical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    18913 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/tests/unit/transformers/test_datetime.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    21103 2023-05-01 18:10:03.000000 rdt_identity-1.4.2.dev0/tests/unit/transformers/test_null.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    61010 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/tests/unit/transformers/test_numerical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    12685 2023-04-13 17:39:49.000000 rdt_identity-1.4.2.dev0/tests/unit/transformers/test_text.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1513 2023-04-26 21:05:25.000000 rdt_identity-1.4.2.dev0/tests/unit/transformers/test_utils.py
```

### Comparing `rdt_identity-1.4.2/CONTRIBUTING.rst` & `rdt_identity-1.4.2.dev0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2/HISTORY.md` & `rdt_identity-1.4.2.dev0/HISTORY.md`

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

### Comparing `rdt_identity-1.4.2/LICENSE` & `rdt_identity-1.4.2.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2/PKG-INFO` & `rdt_identity-1.4.2.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdt_identity
-Version: 1.4.2
+Version: 1.4.2.dev0
 Summary: Reversible Data Transforms
 Home-page: https://github.com/sdv-dev/RDT
 Author: DataCebo, Inc.
 Author-email: info@sdv.dev
 License: BSL-1.1
 Keywords: rdt,rdt_identity
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1 Name: rdt_identity Version: 1.4.2 Summary: Reversible
-Data Transforms Home-page: https://github.com/sdv-dev/RDT Author: DataCebo,
-Inc. Author-email: info@sdv.dev License: BSL-1.1 Keywords: rdt,rdt_identity
-Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
-:: Developers Classifier: License :: Free for non-commercial use Classifier:
-Natural Language :: English Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Topic :: Scientific/Engineering ::
-Artificial Intelligence Requires-Python: >=3.7,<3.12 Description-Content-Type:
-text/markdown License-File: LICENSE License-File: AUTHORS.rst
+Metadata-Version: 2.1 Name: rdt_identity Version: 1.4.2.dev0 Summary:
+Reversible Data Transforms Home-page: https://github.com/sdv-dev/RDT Author:
+DataCebo, Inc. Author-email: info@sdv.dev License: BSL-1.1 Keywords:
+rdt,rdt_identity Classifier: Development Status :: 2 - Pre-Alpha Classifier:
+Intended Audience :: Developers Classifier: License :: Free for non-commercial
+use Classifier: Natural Language :: English Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Topic :: Scientific/
+Engineering :: Artificial Intelligence Requires-Python: >=3.7,<3.12
+Description-Content-Type: text/markdown License-File: LICENSE License-File:
+AUTHORS.rst
 
   This repository is part of The_Synthetic_Data_Vault_Project, a project from
                                    DataCebo.
 [![Development Status](https://img.shields.io/badge/Development%20Status-3%20--
                   %20Alpha-yellow)](https://pypi.org/search/
     ?q=&o=&c=Development+Status+%3A%3A+3+-+Alpha) [![PyPi Shield](https://
    img.shields.io/pypi/v/RDT.svg)](https://pypi.python.org/pypi/RDT) [![Unit
```

### Comparing `rdt_identity-1.4.2/README.md` & `rdt_identity-1.4.2.dev0/README.md`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2/RELEASE.md` & `rdt_identity-1.4.2.dev0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2/rdt/transformers/addons/identity/identity.py` & `rdt_identity-1.4.2.dev0/rdt/transformers/addons/identity/identity.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2/setup.cfg` & `rdt_identity-1.4.2.dev0/setup.cfg`

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

### Comparing `rdt_identity-1.4.2/setup.py` & `rdt_identity-1.4.2.dev0/setup.py`

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

### Comparing `rdt_identity-1.4.2/tests/__init__.py` & `rdt_identity-1.4.2.dev0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2/tests/code_style.py` & `rdt_identity-1.4.2.dev0/tests/code_style.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2/tests/contributing.py` & `rdt_identity-1.4.2.dev0/tests/contributing.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2/tests/datasets/tests/test_boolean.py` & `rdt_identity-1.4.2.dev0/tests/datasets/tests/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2/tests/datasets/tests/test_categorical.py` & `rdt_identity-1.4.2.dev0/tests/datasets/tests/test_categorical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2/tests/datasets/tests/test_datetime.py` & `rdt_identity-1.4.2.dev0/tests/datasets/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2/tests/datasets/tests/test_numerical.py` & `rdt_identity-1.4.2.dev0/tests/datasets/tests/test_numerical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2/tests/datasets/tests/test_utils.py` & `rdt_identity-1.4.2.dev0/tests/datasets/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2/tests/integration/test_hyper_transformer.py` & `rdt_identity-1.4.2.dev0/tests/integration/test_hyper_transformer.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2/tests/integration/test_transformers.py` & `rdt_identity-1.4.2.dev0/tests/integration/test_transformers.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2/tests/integration/transformers/pii/test_anonymizer.py` & `rdt_identity-1.4.2.dev0/tests/integration/transformers/pii/test_anonymizer.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2/tests/integration/transformers/test_base.py` & `rdt_identity-1.4.2.dev0/tests/integration/transformers/test_base.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2/tests/integration/transformers/test_boolean.py` & `rdt_identity-1.4.2.dev0/tests/integration/transformers/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2/tests/integration/transformers/test_categorical.py` & `rdt_identity-1.4.2.dev0/tests/integration/transformers/test_categorical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2/tests/integration/transformers/test_datetime.py` & `rdt_identity-1.4.2.dev0/tests/integration/transformers/test_datetime.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2/tests/integration/transformers/test_numerical.py` & `rdt_identity-1.4.2.dev0/tests/integration/transformers/test_numerical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2/tests/integration/transformers/test_text.py` & `rdt_identity-1.4.2.dev0/tests/integration/transformers/test_text.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2/tests/performance/test_performance.py` & `rdt_identity-1.4.2.dev0/tests/performance/test_performance.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2/tests/performance/tests/test_profiling.py` & `rdt_identity-1.4.2.dev0/tests/performance/tests/test_profiling.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2/tests/quality/dataset_info.csv` & `rdt_identity-1.4.2.dev0/tests/quality/dataset_info.csv`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2/tests/quality/test_quality.py` & `rdt_identity-1.4.2.dev0/tests/quality/test_quality.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2/tests/quality/utils.py` & `rdt_identity-1.4.2.dev0/tests/quality/utils.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2/tests/unit/test___init__.py` & `rdt_identity-1.4.2.dev0/tests/unit/test___init__.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2/tests/unit/test__addons.py` & `rdt_identity-1.4.2.dev0/tests/unit/test__addons.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2/tests/unit/test_hyper_transformer.py` & `rdt_identity-1.4.2.dev0/tests/unit/test_hyper_transformer.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2/tests/unit/transformers/addons/identity/test_identity.py` & `rdt_identity-1.4.2.dev0/tests/unit/transformers/addons/identity/test_identity.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2/tests/unit/transformers/pii/test_anonymizer.py` & `rdt_identity-1.4.2.dev0/tests/unit/transformers/pii/test_anonymizer.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2/tests/unit/transformers/pii/test_utils.py` & `rdt_identity-1.4.2.dev0/tests/unit/transformers/pii/test_utils.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2/tests/unit/transformers/test___init__.py` & `rdt_identity-1.4.2.dev0/tests/unit/transformers/test___init__.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2/tests/unit/transformers/test_base.py` & `rdt_identity-1.4.2.dev0/tests/unit/transformers/test_base.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2/tests/unit/transformers/test_boolean.py` & `rdt_identity-1.4.2.dev0/tests/unit/transformers/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2/tests/unit/transformers/test_categorical.py` & `rdt_identity-1.4.2.dev0/tests/unit/transformers/test_categorical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2/tests/unit/transformers/test_datetime.py` & `rdt_identity-1.4.2.dev0/tests/unit/transformers/test_datetime.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2/tests/unit/transformers/test_null.py` & `rdt_identity-1.4.2.dev0/tests/unit/transformers/test_null.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2/tests/unit/transformers/test_numerical.py` & `rdt_identity-1.4.2.dev0/tests/unit/transformers/test_numerical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2/tests/unit/transformers/test_text.py` & `rdt_identity-1.4.2.dev0/tests/unit/transformers/test_text.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.2/tests/unit/transformers/test_utils.py` & `rdt_identity-1.4.2.dev0/tests/unit/transformers/test_utils.py`

 * *Files identical despite different names*

