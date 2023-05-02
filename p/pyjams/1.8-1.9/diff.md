# Comparing `tmp/pyjams-1.8.tar.gz` & `tmp/pyjams-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjams-1.8.tar", last modified: Sat Nov 13 23:46:21 2021, max compression
+gzip compressed data, was "pyjams-1.9.tar", last modified: Sun Nov 14 01:32:38 2021, max compression
```

## Comparing `pyjams-1.8.tar` & `pyjams-1.9.tar`

### file list

```diff
@@ -1,64 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-13 23:46:21.366451 pyjams-1.8/
--rw-r--r--   0 runner    (1001) docker     (121)      780 2021-11-13 23:45:29.000000 pyjams-1.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3797 2021-11-13 23:45:29.000000 pyjams-1.8/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1199 2021-11-13 23:45:29.000000 pyjams-1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     9470 2021-11-13 23:46:21.366451 pyjams-1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7516 2021-11-13 23:45:29.000000 pyjams-1.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      598 2021-11-13 23:45:29.000000 pyjams-1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     2054 2021-11-13 23:46:21.366451 pyjams-1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-13 23:46:21.362451 pyjams-1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-13 23:46:21.362451 pyjams-1.8/src/pyjams/
--rw-r--r--   0 runner    (1001) docker     (121)     3328 2021-11-13 23:45:29.000000 pyjams-1.8/src/pyjams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       19 2021-11-13 23:46:21.000000 pyjams-1.8/src/pyjams/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     5511 2021-11-13 23:45:29.000000 pyjams-1.8/src/pyjams/alpha_equ_h2o.py
--rw-r--r--   0 runner    (1001) docker     (121)     4483 2021-11-13 23:45:29.000000 pyjams-1.8/src/pyjams/alpha_kin_h2o.py
--rw-r--r--   0 runner    (1001) docker     (121)    10215 2021-11-13 23:45:29.000000 pyjams-1.8/src/pyjams/argsort.py
--rw-r--r--   0 runner    (1001) docker     (121)     2459 2021-11-13 23:45:29.000000 pyjams-1.8/src/pyjams/closest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-13 23:46:21.366451 pyjams-1.8/src/pyjams/color/
--rw-r--r--   0 runner    (1001) docker     (121)     1220 2021-11-13 23:45:29.000000 pyjams-1.8/src/pyjams/color/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    43611 2021-11-13 23:45:29.000000 pyjams-1.8/src/pyjams/color/brewer_palettes.py
--rw-r--r--   0 runner    (1001) docker     (121)    16248 2021-11-13 23:45:29.000000 pyjams-1.8/src/pyjams/color/color.py
--rw-r--r--   0 runner    (1001) docker     (121)    11759 2021-11-13 23:45:29.000000 pyjams-1.8/src/pyjams/color/mathematica_palettes.py
--rw-r--r--   0 runner    (1001) docker     (121)   272761 2021-11-13 23:45:29.000000 pyjams-1.8/src/pyjams/color/ncl_palettes.py
--rw-r--r--   0 runner    (1001) docker     (121)     6526 2021-11-13 23:45:29.000000 pyjams-1.8/src/pyjams/color/oregon_palettes.py
--rw-r--r--   0 runner    (1001) docker     (121)     8866 2021-11-13 23:45:29.000000 pyjams-1.8/src/pyjams/color/sron2012_palettes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-13 23:46:21.366451 pyjams-1.8/src/pyjams/const/
--rw-r--r--   0 runner    (1001) docker     (121)     1079 2021-11-13 23:45:29.000000 pyjams-1.8/src/pyjams/const/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5704 2021-11-13 23:45:29.000000 pyjams-1.8/src/pyjams/const/const.py
--rw-r--r--   0 runner    (1001) docker     (121)     4416 2021-11-13 23:45:29.000000 pyjams-1.8/src/pyjams/division.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-13 23:46:21.366451 pyjams-1.8/src/pyjams/functions/
--rw-r--r--   0 runner    (1001) docker     (121)     4629 2021-11-13 23:45:29.000000 pyjams-1.8/src/pyjams/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    40080 2021-11-13 23:45:29.000000 pyjams-1.8/src/pyjams/functions/fit_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2590 2021-11-13 23:45:29.000000 pyjams-1.8/src/pyjams/functions/general_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)    14019 2021-11-13 23:45:29.000000 pyjams-1.8/src/pyjams/functions/logistic_function.py
--rw-r--r--   0 runner    (1001) docker     (121)     5294 2021-11-13 23:45:29.000000 pyjams-1.8/src/pyjams/functions/opti_test_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)    20835 2021-11-13 23:45:29.000000 pyjams-1.8/src/pyjams/functions/sa_test_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)    33869 2021-11-13 23:45:29.000000 pyjams-1.8/src/pyjams/mcplot.py
--rw-r--r--   0 runner    (1001) docker     (121)    45231 2021-11-13 23:45:29.000000 pyjams-1.8/src/pyjams/morris_method.py
--rw-r--r--   0 runner    (1001) docker     (121)    22607 2021-11-13 23:45:29.000000 pyjams-1.8/src/pyjams/screening.py
--rw-r--r--   0 runner    (1001) docker     (121)     9150 2021-11-13 23:45:29.000000 pyjams-1.8/src/pyjams/str2tex.py
--rw-r--r--   0 runner    (1001) docker     (121)     3434 2021-11-13 23:45:29.000000 pyjams-1.8/src/pyjams/tee.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-13 23:46:21.362451 pyjams-1.8/src/pyjams.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9470 2021-11-13 23:46:21.000000 pyjams-1.8/src/pyjams.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1499 2021-11-13 23:46:21.000000 pyjams-1.8/src/pyjams.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-13 23:46:21.000000 pyjams-1.8/src/pyjams.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-13 23:45:40.000000 pyjams-1.8/src/pyjams.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      178 2021-11-13 23:46:21.000000 pyjams-1.8/src/pyjams.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-11-13 23:46:21.000000 pyjams-1.8/src/pyjams.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-13 23:46:21.366451 pyjams-1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-13 23:45:29.000000 pyjams-1.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2437 2021-11-13 23:45:29.000000 pyjams-1.8/tests/test_alpha_equ_h2o.py
--rw-r--r--   0 runner    (1001) docker     (121)     1280 2021-11-13 23:45:29.000000 pyjams-1.8/tests/test_alpha_kin_h2o.py
--rw-r--r--   0 runner    (1001) docker     (121)     5482 2021-11-13 23:45:29.000000 pyjams-1.8/tests/test_argsort.py
--rw-r--r--   0 runner    (1001) docker     (121)      954 2021-11-13 23:45:29.000000 pyjams-1.8/tests/test_closest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2520 2021-11-13 23:45:29.000000 pyjams-1.8/tests/test_const.py
--rw-r--r--   0 runner    (1001) docker     (121)     3632 2021-11-13 23:45:29.000000 pyjams-1.8/tests/test_division.py
--rw-r--r--   0 runner    (1001) docker     (121)     9160 2021-11-13 23:45:29.000000 pyjams-1.8/tests/test_fit_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1153 2021-11-13 23:45:29.000000 pyjams-1.8/tests/test_general_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3777 2021-11-13 23:45:29.000000 pyjams-1.8/tests/test_logistic_function.py
--rw-r--r--   0 runner    (1001) docker     (121)    12853 2021-11-13 23:45:29.000000 pyjams-1.8/tests/test_morris_method.py
--rw-r--r--   0 runner    (1001) docker     (121)     1467 2021-11-13 23:45:29.000000 pyjams-1.8/tests/test_opti_test_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     4664 2021-11-13 23:45:29.000000 pyjams-1.8/tests/test_sa_test_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)    12689 2021-11-13 23:45:29.000000 pyjams-1.8/tests/test_screening.py
--rw-r--r--   0 runner    (1001) docker     (121)     6904 2021-11-13 23:45:29.000000 pyjams-1.8/tests/test_str2tex.py
--rw-r--r--   0 runner    (1001) docker     (121)      848 2021-11-13 23:45:29.000000 pyjams-1.8/tests/test_tee.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-14 01:32:38.251723 pyjams-1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      780 2021-11-14 01:31:38.000000 pyjams-1.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3916 2021-11-14 01:31:38.000000 pyjams-1.9/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1199 2021-11-14 01:31:38.000000 pyjams-1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     9630 2021-11-14 01:32:38.251723 pyjams-1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     7676 2021-11-14 01:31:38.000000 pyjams-1.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      630 2021-11-14 01:31:38.000000 pyjams-1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     2054 2021-11-14 01:32:38.255723 pyjams-1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-14 01:32:38.243722 pyjams-1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-14 01:32:38.247722 pyjams-1.9/src/pyjams/
+-rw-r--r--   0 runner    (1001) docker     (121)     3468 2021-11-14 01:31:38.000000 pyjams-1.9/src/pyjams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       19 2021-11-14 01:32:38.000000 pyjams-1.9/src/pyjams/_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5511 2021-11-14 01:31:38.000000 pyjams-1.9/src/pyjams/alpha_equ_h2o.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4483 2021-11-14 01:31:38.000000 pyjams-1.9/src/pyjams/alpha_kin_h2o.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10215 2021-11-14 01:31:38.000000 pyjams-1.9/src/pyjams/argsort.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2459 2021-11-14 01:31:38.000000 pyjams-1.9/src/pyjams/closest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-14 01:32:38.251723 pyjams-1.9/src/pyjams/color/
+-rw-r--r--   0 runner    (1001) docker     (121)     1220 2021-11-14 01:31:38.000000 pyjams-1.9/src/pyjams/color/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    43611 2021-11-14 01:31:38.000000 pyjams-1.9/src/pyjams/color/brewer_palettes.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16248 2021-11-14 01:31:38.000000 pyjams-1.9/src/pyjams/color/color.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11759 2021-11-14 01:31:38.000000 pyjams-1.9/src/pyjams/color/mathematica_palettes.py
+-rw-r--r--   0 runner    (1001) docker     (121)   272761 2021-11-14 01:31:38.000000 pyjams-1.9/src/pyjams/color/ncl_palettes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6526 2021-11-14 01:31:38.000000 pyjams-1.9/src/pyjams/color/oregon_palettes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8866 2021-11-14 01:31:38.000000 pyjams-1.9/src/pyjams/color/sron2012_palettes.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-14 01:32:38.251723 pyjams-1.9/src/pyjams/const/
+-rw-r--r--   0 runner    (1001) docker     (121)     1079 2021-11-14 01:31:38.000000 pyjams-1.9/src/pyjams/const/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5704 2021-11-14 01:31:38.000000 pyjams-1.9/src/pyjams/const/const.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4416 2021-11-14 01:31:38.000000 pyjams-1.9/src/pyjams/division.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-14 01:32:38.251723 pyjams-1.9/src/pyjams/functions/
+-rw-r--r--   0 runner    (1001) docker     (121)     4629 2021-11-14 01:31:38.000000 pyjams-1.9/src/pyjams/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    40080 2021-11-14 01:31:38.000000 pyjams-1.9/src/pyjams/functions/fit_functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2590 2021-11-14 01:31:38.000000 pyjams-1.9/src/pyjams/functions/general_functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14019 2021-11-14 01:31:38.000000 pyjams-1.9/src/pyjams/functions/logistic_function.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5294 2021-11-14 01:31:38.000000 pyjams-1.9/src/pyjams/functions/opti_test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20835 2021-11-14 01:31:38.000000 pyjams-1.9/src/pyjams/functions/sa_test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33869 2021-11-14 01:31:38.000000 pyjams-1.9/src/pyjams/mcplot.py
+-rw-r--r--   0 runner    (1001) docker     (121)    45231 2021-11-14 01:31:38.000000 pyjams-1.9/src/pyjams/morris_method.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8137 2021-11-14 01:31:38.000000 pyjams-1.9/src/pyjams/position.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22607 2021-11-14 01:31:38.000000 pyjams-1.9/src/pyjams/screening.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9150 2021-11-14 01:31:38.000000 pyjams-1.9/src/pyjams/str2tex.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3434 2021-11-14 01:31:38.000000 pyjams-1.9/src/pyjams/tee.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-14 01:32:38.247722 pyjams-1.9/src/pyjams.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     9630 2021-11-14 01:32:38.000000 pyjams-1.9/src/pyjams.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1545 2021-11-14 01:32:38.000000 pyjams-1.9/src/pyjams.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-14 01:32:38.000000 pyjams-1.9/src/pyjams.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-14 01:31:49.000000 pyjams-1.9/src/pyjams.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      178 2021-11-14 01:32:38.000000 pyjams-1.9/src/pyjams.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-11-14 01:32:38.000000 pyjams-1.9/src/pyjams.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-14 01:32:38.251723 pyjams-1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-14 01:31:38.000000 pyjams-1.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2437 2021-11-14 01:31:38.000000 pyjams-1.9/tests/test_alpha_equ_h2o.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1280 2021-11-14 01:31:38.000000 pyjams-1.9/tests/test_alpha_kin_h2o.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5482 2021-11-14 01:31:38.000000 pyjams-1.9/tests/test_argsort.py
+-rw-r--r--   0 runner    (1001) docker     (121)      954 2021-11-14 01:31:38.000000 pyjams-1.9/tests/test_closest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2520 2021-11-14 01:31:38.000000 pyjams-1.9/tests/test_const.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3632 2021-11-14 01:31:38.000000 pyjams-1.9/tests/test_division.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9160 2021-11-14 01:31:38.000000 pyjams-1.9/tests/test_fit_functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1153 2021-11-14 01:31:38.000000 pyjams-1.9/tests/test_general_functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3777 2021-11-14 01:31:38.000000 pyjams-1.9/tests/test_logistic_function.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12853 2021-11-14 01:31:38.000000 pyjams-1.9/tests/test_morris_method.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1467 2021-11-14 01:31:38.000000 pyjams-1.9/tests/test_opti_test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3568 2021-11-14 01:31:38.000000 pyjams-1.9/tests/test_position.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4664 2021-11-14 01:31:38.000000 pyjams-1.9/tests/test_sa_test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12689 2021-11-14 01:31:38.000000 pyjams-1.9/tests/test_screening.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6904 2021-11-14 01:31:38.000000 pyjams-1.9/tests/test_str2tex.py
+-rw-r--r--   0 runner    (1001) docker     (121)      848 2021-11-14 01:31:38.000000 pyjams-1.9/tests/test_tee.py
```

### Comparing `pyjams-1.8/AUTHORS.rst` & `pyjams-1.9/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `pyjams-1.8/CHANGELOG.rst` & `pyjams-1.9/CHANGELOG.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Changelog
 ---------
 
+v1.9 (Nov 2021)
+    * Add `position`, which positions arrays of subplots to be used with
+      Matplotlib's add_axes.
+
 v1.8 (Nov 2021)
     * Write standard output file of mcPlot into current folder.
     * Add `str2tex`, converting strings to LaTeX strings
     * Bug in masked array input to `alpha_equ_h2o`, needed to check masked array
       before ndarray because the former is also the latter.
     * Enhanced tests of `alpha_equ_h2o`, `alpha_kin_h2o`, `fit_functions`,
       `argsort` so that have 100% coverage.
```

### Comparing `pyjams-1.8/LICENSE` & `pyjams-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjams-1.8/PKG-INFO` & `pyjams-1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjams
-Version: 1.8
+Version: 1.9
 Summary: pyjams: a general Python package with miscellaneous utility functions used in several other packages.
 Home-page: https://github.com/mcuntz/pyjams
 Author: Matthias Cuntz, Juliane Mai, Stephan Thober, Arndt Piayda
 Author-email: mc@macu.de
 Maintainer: Matthias Cuntz
 Maintainer-email: mc@macu.de
 License: MIT
@@ -165,14 +165,16 @@
        several forms of the logistic function and its derivatives, and other
        functions to be used with scipy.optimize
    * - mcPlot
      - Matthias Cuntz' standard plotting class
    * - morris_sampling
      - Sampling of optimised trajectories for Morris measures / Elementary
        Effects
+   * - position
+     - Position arrays of subplots to be used with add_axes
    * - screening
      - Parameter screening using Morris' method of Elementary Effects
    * - str2tex
      - Convert strings to LaTeX strings in math environment used by matplotlib's
        usetex
    * - tee
      - Prints arguments on screen and in file, like Unix/Linux tee utility
@@ -264,14 +266,16 @@
 
        * - Function/module
          - Short description
        * - color
          - Collection of color palettes and continuous color maps
        * - mcPlot
          - Matthias Cuntz' standard plotting class
+       * - position
+         - Position arrays of subplots to be used with add_axes
        * - str2tex
          - Convert strings to LaTeX strings in math environment used by
            matplotlib's usetex
 
 
 License
 -------
```

### Comparing `pyjams-1.8/README.rst` & `pyjams-1.9/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -119,14 +119,16 @@
        several forms of the logistic function and its derivatives, and other
        functions to be used with scipy.optimize
    * - mcPlot
      - Matthias Cuntz' standard plotting class
    * - morris_sampling
      - Sampling of optimised trajectories for Morris measures / Elementary
        Effects
+   * - position
+     - Position arrays of subplots to be used with add_axes
    * - screening
      - Parameter screening using Morris' method of Elementary Effects
    * - str2tex
      - Convert strings to LaTeX strings in math environment used by matplotlib's
        usetex
    * - tee
      - Prints arguments on screen and in file, like Unix/Linux tee utility
@@ -218,14 +220,16 @@
 
        * - Function/module
          - Short description
        * - color
          - Collection of color palettes and continuous color maps
        * - mcPlot
          - Matthias Cuntz' standard plotting class
+       * - position
+         - Position arrays of subplots to be used with add_axes
        * - str2tex
          - Convert strings to LaTeX strings in math environment used by
            matplotlib's usetex
 
 
 License
 -------
```

### Comparing `pyjams-1.8/pyproject.toml` & `pyjams-1.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 [tool.coverage]
     [tool.coverage.run]
     source = ["src"]
     omit = [
         "*docs*",
         "*tests*",
+        "src/pyjams/mcplot.py",
     ]
 
     [tool.coverage.report]
     exclude_lines = [
         "pragma: no cover",
         "if __name__ == '__main__':",
         "def __repr__",
```

### Comparing `pyjams-1.8/setup.cfg` & `pyjams-1.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyjams-1.8/src/pyjams/__init__.py` & `pyjams-1.9/src/pyjams/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,14 +25,15 @@
    closest
    color
    const
    division
    functions
    mcplot
    morris_method
+   position
    screening
    str2tex
    tee
 
 
 History
     * Written Oct 2021 by Matthias Cuntz (mc (at) macu (dot) de)
@@ -41,14 +42,15 @@
     * v1.2, added closest, Oct 2021, Matthias Cuntz
     * v1.3, added argsort, Oct 2021, Matthias Cuntz
     * v1.4, added division, Oct 2021, Matthias Cuntz
     * v1.5, added alpha_equ_h2o, Oct 2021, Matthias Cuntz
     * v1.6, added alpha_kin_h2o, Nov 2021, Matthias Cuntz
     * v1.7, added mcPlot, Nov 2021, Matthias Cuntz
     * v1.8, added str2tex and color, Nov 2021, Matthias Cuntz
+    * v1.9, added position, Nov 2021, Matthias Cuntz
 
 """
 # version, author
 try:
     from ._version import __version__
 except ImportError:  # pragma: nocover
     # package is not installed
@@ -74,14 +76,16 @@
 # catch division by zero
 from .division import division, div
 # Matthias Cuntz' standard plotting class.
 from .mcplot import mcPlot
 # has to be ordered for import: morris -> screening
 # Sampling of optimised trajectories for and calculation of Morris Measures / Elementary Effects
 from .morris_method import morris_sampling, elementary_effects
+# positions of subplots, used with add_axes
+from .position import position
 # Sample trajectories, run model and return Morris Elementary Effects
 from .screening import screening, ee
 # Convert strings to LaTeX strings
 from .str2tex import str2tex
 # like unix tee
 from .tee import tee
```

### Comparing `pyjams-1.8/src/pyjams/alpha_equ_h2o.py` & `pyjams-1.9/src/pyjams/alpha_equ_h2o.py`

 * *Files identical despite different names*

### Comparing `pyjams-1.8/src/pyjams/alpha_kin_h2o.py` & `pyjams-1.9/src/pyjams/alpha_kin_h2o.py`

 * *Files identical despite different names*

### Comparing `pyjams-1.8/src/pyjams/argsort.py` & `pyjams-1.9/src/pyjams/argsort.py`

 * *Files identical despite different names*

### Comparing `pyjams-1.8/src/pyjams/closest.py` & `pyjams-1.9/src/pyjams/closest.py`

 * *Files identical despite different names*

### Comparing `pyjams-1.8/src/pyjams/color/__init__.py` & `pyjams-1.9/src/pyjams/color/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjams-1.8/src/pyjams/color/brewer_palettes.py` & `pyjams-1.9/src/pyjams/color/brewer_palettes.py`

 * *Files identical despite different names*

### Comparing `pyjams-1.8/src/pyjams/color/color.py` & `pyjams-1.9/src/pyjams/color/color.py`

 * *Files identical despite different names*

### Comparing `pyjams-1.8/src/pyjams/color/mathematica_palettes.py` & `pyjams-1.9/src/pyjams/color/mathematica_palettes.py`

 * *Files identical despite different names*

### Comparing `pyjams-1.8/src/pyjams/color/ncl_palettes.py` & `pyjams-1.9/src/pyjams/color/ncl_palettes.py`

 * *Files identical despite different names*

### Comparing `pyjams-1.8/src/pyjams/color/oregon_palettes.py` & `pyjams-1.9/src/pyjams/color/oregon_palettes.py`

 * *Files identical despite different names*

### Comparing `pyjams-1.8/src/pyjams/color/sron2012_palettes.py` & `pyjams-1.9/src/pyjams/color/sron2012_palettes.py`

 * *Files identical despite different names*

### Comparing `pyjams-1.8/src/pyjams/const/__init__.py` & `pyjams-1.9/src/pyjams/const/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjams-1.8/src/pyjams/const/const.py` & `pyjams-1.9/src/pyjams/const/const.py`

 * *Files identical despite different names*

### Comparing `pyjams-1.8/src/pyjams/division.py` & `pyjams-1.9/src/pyjams/division.py`

 * *Files identical despite different names*

### Comparing `pyjams-1.8/src/pyjams/functions/__init__.py` & `pyjams-1.9/src/pyjams/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjams-1.8/src/pyjams/functions/fit_functions.py` & `pyjams-1.9/src/pyjams/functions/fit_functions.py`

 * *Files identical despite different names*

### Comparing `pyjams-1.8/src/pyjams/functions/general_functions.py` & `pyjams-1.9/src/pyjams/functions/general_functions.py`

 * *Files identical despite different names*

### Comparing `pyjams-1.8/src/pyjams/functions/logistic_function.py` & `pyjams-1.9/src/pyjams/functions/logistic_function.py`

 * *Files identical despite different names*

### Comparing `pyjams-1.8/src/pyjams/functions/opti_test_functions.py` & `pyjams-1.9/src/pyjams/functions/opti_test_functions.py`

 * *Files identical despite different names*

### Comparing `pyjams-1.8/src/pyjams/functions/sa_test_functions.py` & `pyjams-1.9/src/pyjams/functions/sa_test_functions.py`

 * *Files identical despite different names*

### Comparing `pyjams-1.8/src/pyjams/mcplot.py` & `pyjams-1.9/src/pyjams/mcplot.py`

 * *Files identical despite different names*

### Comparing `pyjams-1.8/src/pyjams/morris_method.py` & `pyjams-1.9/src/pyjams/morris_method.py`

 * *Files identical despite different names*

### Comparing `pyjams-1.8/src/pyjams/screening.py` & `pyjams-1.9/src/pyjams/screening.py`

 * *Files identical despite different names*

### Comparing `pyjams-1.8/src/pyjams/str2tex.py` & `pyjams-1.9/src/pyjams/str2tex.py`

 * *Files identical despite different names*

### Comparing `pyjams-1.8/src/pyjams/tee.py` & `pyjams-1.9/src/pyjams/tee.py`

 * *Files identical despite different names*

### Comparing `pyjams-1.8/src/pyjams.egg-info/PKG-INFO` & `pyjams-1.9/src/pyjams.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjams
-Version: 1.8
+Version: 1.9
 Summary: pyjams: a general Python package with miscellaneous utility functions used in several other packages.
 Home-page: https://github.com/mcuntz/pyjams
 Author: Matthias Cuntz, Juliane Mai, Stephan Thober, Arndt Piayda
 Author-email: mc@macu.de
 Maintainer: Matthias Cuntz
 Maintainer-email: mc@macu.de
 License: MIT
@@ -165,14 +165,16 @@
        several forms of the logistic function and its derivatives, and other
        functions to be used with scipy.optimize
    * - mcPlot
      - Matthias Cuntz' standard plotting class
    * - morris_sampling
      - Sampling of optimised trajectories for Morris measures / Elementary
        Effects
+   * - position
+     - Position arrays of subplots to be used with add_axes
    * - screening
      - Parameter screening using Morris' method of Elementary Effects
    * - str2tex
      - Convert strings to LaTeX strings in math environment used by matplotlib's
        usetex
    * - tee
      - Prints arguments on screen and in file, like Unix/Linux tee utility
@@ -264,14 +266,16 @@
 
        * - Function/module
          - Short description
        * - color
          - Collection of color palettes and continuous color maps
        * - mcPlot
          - Matthias Cuntz' standard plotting class
+       * - position
+         - Position arrays of subplots to be used with add_axes
        * - str2tex
          - Convert strings to LaTeX strings in math environment used by
            matplotlib's usetex
 
 
 License
 -------
```

### Comparing `pyjams-1.8/src/pyjams.egg-info/SOURCES.txt` & `pyjams-1.9/src/pyjams.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 src/pyjams/alpha_equ_h2o.py
 src/pyjams/alpha_kin_h2o.py
 src/pyjams/argsort.py
 src/pyjams/closest.py
 src/pyjams/division.py
 src/pyjams/mcplot.py
 src/pyjams/morris_method.py
+src/pyjams/position.py
 src/pyjams/screening.py
 src/pyjams/str2tex.py
 src/pyjams/tee.py
 src/pyjams.egg-info/PKG-INFO
 src/pyjams.egg-info/SOURCES.txt
 src/pyjams.egg-info/dependency_links.txt
 src/pyjams.egg-info/not-zip-safe
@@ -45,11 +46,12 @@
 tests/test_const.py
 tests/test_division.py
 tests/test_fit_functions.py
 tests/test_general_functions.py
 tests/test_logistic_function.py
 tests/test_morris_method.py
 tests/test_opti_test_functions.py
+tests/test_position.py
 tests/test_sa_test_functions.py
 tests/test_screening.py
 tests/test_str2tex.py
 tests/test_tee.py
```

### Comparing `pyjams-1.8/tests/test_alpha_equ_h2o.py` & `pyjams-1.9/tests/test_alpha_equ_h2o.py`

 * *Files identical despite different names*

### Comparing `pyjams-1.8/tests/test_alpha_kin_h2o.py` & `pyjams-1.9/tests/test_alpha_kin_h2o.py`

 * *Files identical despite different names*

### Comparing `pyjams-1.8/tests/test_argsort.py` & `pyjams-1.9/tests/test_argsort.py`

 * *Files identical despite different names*

### Comparing `pyjams-1.8/tests/test_closest.py` & `pyjams-1.9/tests/test_closest.py`

 * *Files identical despite different names*

### Comparing `pyjams-1.8/tests/test_const.py` & `pyjams-1.9/tests/test_const.py`

 * *Files identical despite different names*

### Comparing `pyjams-1.8/tests/test_division.py` & `pyjams-1.9/tests/test_division.py`

 * *Files identical despite different names*

### Comparing `pyjams-1.8/tests/test_fit_functions.py` & `pyjams-1.9/tests/test_fit_functions.py`

 * *Files identical despite different names*

### Comparing `pyjams-1.8/tests/test_general_functions.py` & `pyjams-1.9/tests/test_general_functions.py`

 * *Files identical despite different names*

### Comparing `pyjams-1.8/tests/test_logistic_function.py` & `pyjams-1.9/tests/test_logistic_function.py`

 * *Files identical despite different names*

### Comparing `pyjams-1.8/tests/test_morris_method.py` & `pyjams-1.9/tests/test_morris_method.py`

 * *Files identical despite different names*

### Comparing `pyjams-1.8/tests/test_opti_test_functions.py` & `pyjams-1.9/tests/test_opti_test_functions.py`

 * *Files identical despite different names*

### Comparing `pyjams-1.8/tests/test_sa_test_functions.py` & `pyjams-1.9/tests/test_sa_test_functions.py`

 * *Files identical despite different names*

### Comparing `pyjams-1.8/tests/test_screening.py` & `pyjams-1.9/tests/test_screening.py`

 * *Files identical despite different names*

### Comparing `pyjams-1.8/tests/test_str2tex.py` & `pyjams-1.9/tests/test_str2tex.py`

 * *Files identical despite different names*

### Comparing `pyjams-1.8/tests/test_tee.py` & `pyjams-1.9/tests/test_tee.py`

 * *Files identical despite different names*

