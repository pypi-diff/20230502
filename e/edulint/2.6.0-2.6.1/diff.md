# Comparing `tmp/edulint-2.6.0.tar.gz` & `tmp/edulint-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/edulint/edulint/dist/.tmp-qlz22kih/edulint-2.6.0.tar", last modified: Mon May  1 19:28:22 2023, max compression
+gzip compressed data, was "/home/runner/work/edulint/edulint/dist/.tmp-_6q2y1so/edulint-2.6.1.tar", last modified: Tue May  2 11:21:48 2023, max compression
```

## Comparing `edulint-2.6.0.tar` & `edulint-2.6.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:28:22.000000 edulint-2.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-01 19:28:11.000000 edulint-2.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-05-01 19:28:22.000000 edulint-2.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-01 19:28:11.000000 edulint-2.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:28:22.000000 edulint-2.6.0/edulint/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:28:22.000000 edulint-2.6.0/edulint/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/config/arg.py
--rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/config/config_translations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1873 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/edulint.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/explanations.py
--rw-r--r--   0 runner    (1001) docker     (123)   180321 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/explanations.toml
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/linters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:28:22.000000 edulint-2.6.0/edulint/linting/
--rw-r--r--   0 runner    (1001) docker     (123)    19603 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/linting/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/linting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:28:22.000000 edulint-2.6.0/edulint/linting/checkers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/linting/checkers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/linting/checkers/basic_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)    11188 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/linting/checkers/improper_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/linting/checkers/modified_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/linting/checkers/python_ta_checkers.py
--rw-r--r--   0 runner    (1001) docker     (123)    21272 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/linting/checkers/short_problems.py
--rw-r--r--   0 runner    (1001) docker     (123)    12091 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/linting/checkers/simplifiable_if.py
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/linting/checkers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/linting/linting.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/linting/overrides.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/linting/problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/linting/process_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/linting/tweakers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:28:22.000000 edulint-2.6.0/edulint/prepare_explanations/
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/prepare_explanations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:28:22.000000 edulint-2.6.0/edulint/prepare_explanations/pylint_data/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/prepare_explanations/pylint_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/prepare_explanations/pylint_data/extract_from_pylint.py
--rw-r--r--   0 runner    (1001) docker     (123)    15286 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/prepare_explanations/pylint_data/pylint_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/prepare_explanations/pylint_data/thonny_process_slim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:28:22.000000 edulint-2.6.0/edulint/prepare_explanations/thonny_data/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/prepare_explanations/thonny_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/prepare_explanations/thonny_data/extract_from_edulint.py
--rw-r--r--   0 runner    (1001) docker     (123)   155599 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/prepare_explanations/thonny_data/thonny_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/prepare_explanations/thonny_data/thonny_process_backup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:28:22.000000 edulint-2.6.0/edulint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-05-01 19:28:22.000000 edulint-2.6.0/edulint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-01 19:28:22.000000 edulint-2.6.0/edulint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 19:28:22.000000 edulint-2.6.0/edulint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-01 19:28:22.000000 edulint-2.6.0/edulint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-01 19:28:22.000000 edulint-2.6.0/edulint.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-01 19:28:11.000000 edulint-2.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-01 19:28:22.000000 edulint-2.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-01 19:28:11.000000 edulint-2.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:28:22.000000 edulint-2.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-05-01 19:28:11.000000 edulint-2.6.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7271 2023-05-01 19:28:11.000000 edulint-2.6.0/tests/test_improper_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)    18600 2023-05-01 19:28:11.000000 edulint-2.6.0/tests/test_lint.py
--rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-05-01 19:28:11.000000 edulint-2.6.0/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)    15775 2023-05-01 19:28:11.000000 edulint-2.6.0/tests/test_short_problems.py
--rw-r--r--   0 runner    (1001) docker     (123)    15909 2023-05-01 19:28:11.000000 edulint-2.6.0/tests/test_simplifiable_if.py
--rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-05-01 19:28:11.000000 edulint-2.6.0/tests/test_visitors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:21:48.000000 edulint-2.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-02 11:21:37.000000 edulint-2.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-05-02 11:21:48.000000 edulint-2.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-02 11:21:37.000000 edulint-2.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:21:48.000000 edulint-2.6.1/edulint/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:21:48.000000 edulint-2.6.1/edulint/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/config/arg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/config/config_translations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1873 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/edulint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/explanations.py
+-rw-r--r--   0 runner    (1001) docker     (123)   180321 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/explanations.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/linters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:21:48.000000 edulint-2.6.1/edulint/linting/
+-rw-r--r--   0 runner    (1001) docker     (123)    19627 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/linting/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/linting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:21:48.000000 edulint-2.6.1/edulint/linting/checkers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/linting/checkers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/linting/checkers/basic_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11188 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/linting/checkers/improper_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/linting/checkers/modified_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/linting/checkers/python_ta_checkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21272 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/linting/checkers/short_problems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12091 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/linting/checkers/simplifiable_if.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/linting/checkers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/linting/linting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/linting/overrides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/linting/problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/linting/process_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/linting/tweakers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:21:48.000000 edulint-2.6.1/edulint/prepare_explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/prepare_explanations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:21:48.000000 edulint-2.6.1/edulint/prepare_explanations/pylint_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/prepare_explanations/pylint_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/prepare_explanations/pylint_data/extract_from_pylint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15286 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/prepare_explanations/pylint_data/pylint_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/prepare_explanations/pylint_data/thonny_process_slim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:21:48.000000 edulint-2.6.1/edulint/prepare_explanations/thonny_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/prepare_explanations/thonny_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/prepare_explanations/thonny_data/extract_from_edulint.py
+-rw-r--r--   0 runner    (1001) docker     (123)   155599 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/prepare_explanations/thonny_data/thonny_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/prepare_explanations/thonny_data/thonny_process_backup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:21:48.000000 edulint-2.6.1/edulint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-05-02 11:21:48.000000 edulint-2.6.1/edulint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-02 11:21:48.000000 edulint-2.6.1/edulint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 11:21:48.000000 edulint-2.6.1/edulint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-02 11:21:48.000000 edulint-2.6.1/edulint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-02 11:21:48.000000 edulint-2.6.1/edulint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-02 11:21:37.000000 edulint-2.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-02 11:21:48.000000 edulint-2.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-02 11:21:37.000000 edulint-2.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:21:48.000000 edulint-2.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-05-02 11:21:37.000000 edulint-2.6.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7271 2023-05-02 11:21:37.000000 edulint-2.6.1/tests/test_improper_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18600 2023-05-02 11:21:37.000000 edulint-2.6.1/tests/test_lint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-05-02 11:21:37.000000 edulint-2.6.1/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15775 2023-05-02 11:21:37.000000 edulint-2.6.1/tests/test_short_problems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15909 2023-05-02 11:21:37.000000 edulint-2.6.1/tests/test_simplifiable_if.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-05-02 11:21:37.000000 edulint-2.6.1/tests/test_visitors.py
```

### Comparing `edulint-2.6.0/LICENSE` & `edulint-2.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `edulint-2.6.0/PKG-INFO` & `edulint-2.6.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edulint
-Version: 2.6.0
+Version: 2.6.1
 Summary: A Python Educational Linter
 Home-page: https://github.com/GiraffeReversed/edulint
 Author: Anna Rechtackova
 Author-email: anna.rechtackova@mail.muni.cz
 Project-URL: Bug Tracker, https://github.com/GiraffeReversed/edulint/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `edulint-2.6.0/README.md` & `edulint-2.6.1/README.md`

 * *Files identical despite different names*

### Comparing `edulint-2.6.0/edulint/config/config.py` & `edulint-2.6.1/edulint/config/config.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.0/edulint/config/config_translations.py` & `edulint-2.6.1/edulint/config/config_translations.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.0/edulint/edulint.py` & `edulint-2.6.1/edulint/edulint.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.0/edulint/explanations.toml` & `edulint-2.6.1/edulint/explanations.toml`

 * *Files identical despite different names*

### Comparing `edulint-2.6.0/edulint/linters.py` & `edulint-2.6.1/edulint/linters.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.0/edulint/linting/.pylintrc` & `edulint-2.6.1/edulint/linting/.pylintrc`

 * *Files 0% similar despite different names*

```diff
@@ -108,14 +108,15 @@
        trailing-comma-tuple,
        unnecessary-dict-index-lookup,
        unnecessary-pass,
        unneeded-not,
        unreachable,
        used-before-assignment,
        disallowed-name,
+       wildcard-import,
        simplifiable-if-return,
        simplifiable-if-assignment,
        simplifiable-if-expr,
        simplifiable-if-pass,
        no-value-in-one-branch-return,
        no-while-true,
        use-tighter-boundaries,
```

### Comparing `edulint-2.6.0/edulint/linting/checkers/basic_checker.py` & `edulint-2.6.1/edulint/linting/checkers/basic_checker.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.0/edulint/linting/checkers/improper_loop.py` & `edulint-2.6.1/edulint/linting/checkers/improper_loop.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.0/edulint/linting/checkers/modified_listener.py` & `edulint-2.6.1/edulint/linting/checkers/modified_listener.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.0/edulint/linting/checkers/python_ta_checkers.py` & `edulint-2.6.1/edulint/linting/checkers/python_ta_checkers.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.0/edulint/linting/checkers/short_problems.py` & `edulint-2.6.1/edulint/linting/checkers/short_problems.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.0/edulint/linting/checkers/simplifiable_if.py` & `edulint-2.6.1/edulint/linting/checkers/simplifiable_if.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.0/edulint/linting/checkers/utils.py` & `edulint-2.6.1/edulint/linting/checkers/utils.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.0/edulint/linting/linting.py` & `edulint-2.6.1/edulint/linting/linting.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.0/edulint/linting/overrides.py` & `edulint-2.6.1/edulint/linting/overrides.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.0/edulint/linting/problem.py` & `edulint-2.6.1/edulint/linting/problem.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.0/edulint/linting/process_handler.py` & `edulint-2.6.1/edulint/linting/process_handler.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.0/edulint/linting/tweakers.py` & `edulint-2.6.1/edulint/linting/tweakers.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.0/edulint/options.py` & `edulint-2.6.1/edulint/options.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.0/edulint/prepare_explanations/__init__.py` & `edulint-2.6.1/edulint/prepare_explanations/__init__.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.0/edulint/prepare_explanations/pylint_data/extract_from_pylint.py` & `edulint-2.6.1/edulint/prepare_explanations/pylint_data/extract_from_pylint.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.0/edulint/prepare_explanations/pylint_data/pylint_messages.py` & `edulint-2.6.1/edulint/prepare_explanations/pylint_data/pylint_messages.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.0/edulint/prepare_explanations/pylint_data/thonny_process_slim.py` & `edulint-2.6.1/edulint/prepare_explanations/pylint_data/thonny_process_slim.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.0/edulint/prepare_explanations/thonny_data/extract_from_edulint.py` & `edulint-2.6.1/edulint/prepare_explanations/thonny_data/extract_from_edulint.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.0/edulint/prepare_explanations/thonny_data/thonny_messages.py` & `edulint-2.6.1/edulint/prepare_explanations/thonny_data/thonny_messages.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.0/edulint/prepare_explanations/thonny_data/thonny_process_backup.py` & `edulint-2.6.1/edulint/prepare_explanations/thonny_data/thonny_process_backup.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.0/edulint.egg-info/PKG-INFO` & `edulint-2.6.1/edulint.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edulint
-Version: 2.6.0
+Version: 2.6.1
 Summary: A Python Educational Linter
 Home-page: https://github.com/GiraffeReversed/edulint
 Author: Anna Rechtackova
 Author-email: anna.rechtackova@mail.muni.cz
 Project-URL: Bug Tracker, https://github.com/GiraffeReversed/edulint/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `edulint-2.6.0/edulint.egg-info/SOURCES.txt` & `edulint-2.6.1/edulint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edulint-2.6.0/setup.cfg` & `edulint-2.6.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `edulint-2.6.0/setup.py` & `edulint-2.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.0/tests/test_config.py` & `edulint-2.6.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.0/tests/test_improper_loop.py` & `edulint-2.6.1/tests/test_improper_loop.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.0/tests/test_lint.py` & `edulint-2.6.1/tests/test_lint.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.0/tests/test_main.py` & `edulint-2.6.1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.0/tests/test_short_problems.py` & `edulint-2.6.1/tests/test_short_problems.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.0/tests/test_simplifiable_if.py` & `edulint-2.6.1/tests/test_simplifiable_if.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.0/tests/test_visitors.py` & `edulint-2.6.1/tests/test_visitors.py`

 * *Files identical despite different names*

