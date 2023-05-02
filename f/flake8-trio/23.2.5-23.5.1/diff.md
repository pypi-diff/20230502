# Comparing `tmp/flake8-trio-23.2.5.tar.gz` & `tmp/flake8-trio-23.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8-trio-23.2.5.tar", last modified: Wed Feb 15 02:22:36 2023, max compression
+gzip compressed data, was "flake8-trio-23.5.1.tar", last modified: Tue May  2 05:54:27 2023, max compression
```

## Comparing `flake8-trio-23.2.5.tar` & `flake8-trio-23.5.1.tar`

### file list

```diff
@@ -1,86 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 02:22:36.976074 flake8-trio-23.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14988 2023-02-15 02:22:36.976074 flake8-trio-23.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7912 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 02:22:36.968074 flake8-trio-23.2.5/flake8_trio/
--rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/flake8_trio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/flake8_trio/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/flake8_trio/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 02:22:36.972074 flake8-trio-23.2.5/flake8_trio/visitors/
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/flake8_trio/visitors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/flake8_trio/visitors/flake8triovisitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/flake8_trio/visitors/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/flake8_trio/visitors/visitor102.py
--rw-r--r--   0 runner    (1001) docker     (123)     7672 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/flake8_trio/visitors/visitor103_104.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/flake8_trio/visitors/visitor105.py
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/flake8_trio/visitors/visitor111.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/flake8_trio/visitors/visitor118.py
--rw-r--r--   0 runner    (1001) docker     (123)    10873 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/flake8_trio/visitors/visitor2xx.py
--rw-r--r--   0 runner    (1001) docker     (123)    13485 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/flake8_trio/visitors/visitor91x.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/flake8_trio/visitors/visitor_utility.py
--rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/flake8_trio/visitors/visitors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 02:22:36.968074 flake8-trio-23.2.5/flake8_trio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14988 2023-02-15 02:22:36.000000 flake8-trio-23.2.5/flake8_trio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-02-15 02:22:36.000000 flake8-trio-23.2.5/flake8_trio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 02:22:36.000000 flake8-trio-23.2.5/flake8_trio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-02-15 02:22:36.000000 flake8-trio-23.2.5/flake8_trio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 02:22:36.000000 flake8-trio-23.2.5/flake8_trio.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-15 02:22:36.000000 flake8-trio-23.2.5/flake8_trio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-15 02:22:36.000000 flake8-trio-23.2.5/flake8_trio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-15 02:22:36.976074 flake8-trio-23.2.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1637 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 02:22:36.972074 flake8-trio-23.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 02:22:36.976074 flake8-trio-23.2.5/tests/eval_files/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/tests/eval_files/anyio_trio.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/tests/eval_files/no_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/tests/eval_files/trio100.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/tests/eval_files/trio101.py
--rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/tests/eval_files/trio102.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/tests/eval_files/trio102_anyio.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/tests/eval_files/trio102_trio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/tests/eval_files/trio103.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/tests/eval_files/trio103_both_imported.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/tests/eval_files/trio103_no_104.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/tests/eval_files/trio103_trio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/tests/eval_files/trio104.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/tests/eval_files/trio104_anyio.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/tests/eval_files/trio104_trio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/tests/eval_files/trio105.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/tests/eval_files/trio105_anyio.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/tests/eval_files/trio106.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/tests/eval_files/trio109.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/tests/eval_files/trio110.py
--rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/tests/eval_files/trio111.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/tests/eval_files/trio112.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/tests/eval_files/trio113.py
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/tests/eval_files/trio113_trio.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/tests/eval_files/trio114.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/tests/eval_files/trio115.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/tests/eval_files/trio116.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/tests/eval_files/trio117.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/tests/eval_files/trio118.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/tests/eval_files/trio200.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/tests/eval_files/trio210.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/tests/eval_files/trio211.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/tests/eval_files/trio212.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/tests/eval_files/trio22x.py
--rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/tests/eval_files/trio232.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/tests/eval_files/trio23x.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/tests/eval_files/trio240.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/tests/eval_files/trio900.py
--rw-r--r--   0 runner    (1001) docker     (123)     9268 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/tests/eval_files/trio910.py
--rw-r--r--   0 runner    (1001) docker     (123)    18736 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/tests/eval_files/trio911.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/tests/eval_files/trio_anyio.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/tests/test_all_visitors_imported.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/tests/test_changelog_and_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    22326 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/tests/test_flake8_trio.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/tests/test_formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/tests/trio_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-02-15 02:22:20.000000 flake8-trio-23.2.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:54:27.173614 flake8-trio-23.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17245 2023-05-02 05:54:27.173614 flake8-trio-23.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9961 2023-05-02 05:54:20.000000 flake8-trio-23.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:54:27.161613 flake8-trio-23.5.1/flake8_trio/
+-rw-r--r--   0 runner    (1001) docker     (123)    12902 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/flake8_trio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/flake8_trio/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/flake8_trio/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/flake8_trio/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:54:27.165614 flake8-trio-23.5.1/flake8_trio/visitors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/flake8_trio/visitors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/flake8_trio/visitors/flake8triovisitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13135 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/flake8_trio/visitors/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/flake8_trio/visitors/visitor100.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/flake8_trio/visitors/visitor101.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/flake8_trio/visitors/visitor102.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/flake8_trio/visitors/visitor103_104.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/flake8_trio/visitors/visitor105.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/flake8_trio/visitors/visitor111.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/flake8_trio/visitors/visitor118.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10867 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/flake8_trio/visitors/visitor2xx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31413 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/flake8_trio/visitors/visitor91x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6844 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/flake8_trio/visitors/visitor_utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10394 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/flake8_trio/visitors/visitors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:54:27.165614 flake8-trio-23.5.1/flake8_trio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17245 2023-05-02 05:54:27.000000 flake8-trio-23.5.1/flake8_trio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-05-02 05:54:27.000000 flake8-trio-23.5.1/flake8_trio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 05:54:27.000000 flake8-trio-23.5.1/flake8_trio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-02 05:54:27.000000 flake8-trio-23.5.1/flake8_trio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 05:54:27.000000 flake8-trio-23.5.1/flake8_trio.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-02 05:54:27.000000 flake8-trio-23.5.1/flake8_trio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-02 05:54:27.000000 flake8-trio-23.5.1/flake8_trio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 05:54:27.173614 flake8-trio-23.5.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1708 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:54:27.165614 flake8-trio-23.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:54:27.169613 flake8-trio-23.5.1/tests/autofix_files/
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/autofix_files/trio100.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/autofix_files/trio100_simple_autofix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11557 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/autofix_files/trio910.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28361 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/autofix_files/trio911.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/autofix_files/trio91x_autofix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:54:27.173614 flake8-trio-23.5.1/tests/eval_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/eval_files/anyio_trio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/eval_files/no_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/eval_files/noqa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/eval_files/trio100.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/eval_files/trio100_noautofix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/eval_files/trio100_simple_autofix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/eval_files/trio101.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/eval_files/trio102.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/eval_files/trio102_anyio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/eval_files/trio102_trio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/eval_files/trio103.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/eval_files/trio103_both_imported.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/eval_files/trio103_no_104.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/eval_files/trio103_trio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/eval_files/trio104.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/eval_files/trio104_anyio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/eval_files/trio104_trio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/eval_files/trio105.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/eval_files/trio105_anyio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/eval_files/trio106.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/eval_files/trio109.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/eval_files/trio110.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/eval_files/trio111.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/eval_files/trio112.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/eval_files/trio113.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/eval_files/trio113_trio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/eval_files/trio114.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/eval_files/trio115.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/eval_files/trio116.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/eval_files/trio117.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/eval_files/trio118.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/eval_files/trio200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/eval_files/trio210.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/eval_files/trio211.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/eval_files/trio212.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/eval_files/trio22x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/eval_files/trio232.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/eval_files/trio23x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/eval_files/trio240.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/eval_files/trio900.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10464 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/eval_files/trio910.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23629 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/eval_files/trio911.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/eval_files/trio91x_autofix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/eval_files/trio91x_noautofix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/eval_files/trio_anyio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/test_all_visitors_imported.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3369 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/test_changelog_and_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9016 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/test_config_and_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/test_exception_on_invalid_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25127 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/test_flake8_trio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/test_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/test_messages_documented.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tests/trio_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-02 05:54:10.000000 flake8-trio-23.5.1/tox.ini
```

### Comparing `flake8-trio-23.2.5/CHANGELOG.md` & `flake8-trio-23.5.1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 # Changelog
 *[CalVer, YY.month.patch](https://calver.org/)*
 
+## 23.5.1
+- TRIO91X now supports comprehensions
+- TRIO100 and TRIO91X now supports autofixing
+- Renamed `--enable-visitor-codes-regex` to `--enable`
+- Added `--disable`, `--autofix` and `--error-on-autofix`
+
 ## 23.2.5
 - Fix false alarms for `@pytest.fixture`-decorated functions in TRIO101, TRIO910 and TRIO911
 
 ## 23.2.4
 - Fix TRIO900 false alarm on nested functions
 - TRIO113 now also works on `anyio.TaskGroup`
```

### Comparing `flake8-trio-23.2.5/CONTRIBUTING.md` & `flake8-trio-23.5.1/CONTRIBUTING.md`

 * *Files 10% similar despite different names*

```diff
@@ -28,14 +28,19 @@
 
 ## Meta-tests
 To check that all codes are tested and documented there's a test that error codes mentioned in `README.md`, `CHANGELOG.md` (matching `TRIO\d\d\d`), the keys in `flake8_trio.Error_codes` and codes parsed from filenames and files in `tests/eval_files/`, are all equal.
 
 ## Test generator
 Tests are automatically generated for files in the `tests/eval_files/` directory, with the code that it's testing interpreted from the file name. The file extension is split off, if there's a match for for `_py\d*` it strips that off and uses it to determine if there's a minimum python version for which the test should only run.
 
+### `# AUTOFIX`
+Files in `tests/eval_files` with this marker will have two files in `tests/autofix_files/`. One with the same name containing the code after being autofixed, and a diff file between those two.  
+During tests the result of running the checker on the eval file with autofix enabled will be compared to the content of the autofix file and will print a diff (if `-s` is on) and assert that the content is the same. `--generate-autofix` is added as a pytest flag to ease development, which will print a diff (with `-s`) and overwrite the content of the autofix file.  
+Files without this marker will be checked that they *don't* modify the file content.
+
 ### `error:`
 Lines containing `error:` are parsed as expecting an error of the code matching the file name, with everything on the line after the colon `eval`'d and passed as arguments to `flake8_trio.Error_codes[<error_code>].str_format`. The `globals` argument to `eval` contains a `lineno` variable assigned the current line number, and the `flake8_trio.Statement` namedtuple. The first element after `error:` *must* be an integer containing the column where the error on that line originates.
 #### `TRIOxxx:`
 You can instead of `error` specify the error code.
 
 ### `# ARG`
 With `# ARG` lines you can also specify command-line arguments that should be passed to the plugin when parsing a file. Can be specified multiple times for several different arguments.
```

### Comparing `flake8-trio-23.2.5/LICENSE` & `flake8-trio-23.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8-trio-23.2.5/PKG-INFO` & `flake8-trio-23.5.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-trio
-Version: 23.2.5
+Version: 23.5.1
 Summary: A highly opinionated flake8 plugin for Trio-related problems.
 Home-page: https://github.com/Zac-HD/flake8-trio
 Author: Zac Hatfield-Dodds, John Litborn, and Contributors
 Author-email: zac@zhd.dev
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Flake8
@@ -37,34 +37,34 @@
 
 ```console
 pip install flake8-trio
 ```
 
 ## List of warnings
 
-- **TRIO100**: a `with trio.fail_after(...):` or `with trio.move_on_after(...):`
+- **TRIO100**: A `with trio.fail_after(...):` or `with trio.move_on_after(...):`
   context does not contain any `await` statements.  This makes it pointless, as
   the timeout can only be triggered by a checkpoint.
 - **TRIO101**: `yield` inside a nursery or cancel scope is only safe when implementing a context manager - otherwise, it breaks exception handling.
-- **TRIO102**: it's unsafe to await inside `finally:` or `except BaseException/trio.Cancelled` unless you use a shielded
+- **TRIO102**: It's unsafe to await inside `finally:` or `except BaseException/trio.Cancelled` unless you use a shielded
   cancel scope with a timeout.
 - **TRIO103**: `except BaseException`, `except trio.Cancelled` or a bare `except:` with a code path that doesn't re-raise. If you don't want to re-raise `BaseException`, add a separate handler for `trio.Cancelled` before.
 - **TRIO104**: `Cancelled` and `BaseException` must be re-raised - when a user tries to `return` or `raise` a different exception.
 - **TRIO105**: Calling a trio async function without immediately `await`ing it.
-- **TRIO106**: trio must be imported with `import trio` for the linter to work.
+- **TRIO106**: `trio` must be imported with `import trio` for the linter to work.
 - **TRIO107**: Renamed to TRIO910
 - **TRIO108**: Renamed to TRIO911
 - **TRIO109**: Async function definition with a `timeout` parameter - use `trio.[fail/move_on]_[after/at]` instead
 - **TRIO110**: `while <condition>: await trio.sleep()` should be replaced by a `trio.Event`.
 - **TRIO111**: Variable, from context manager opened inside nursery, passed to `start[_soon]` might be invalidly accessed while in use, due to context manager closing before the nursery. This is usually a bug, and nurseries should generally be the inner-most context manager.
-- **TRIO112**: nursery body with only a call to `nursery.start[_soon]` and not passing itself as a parameter can be replaced with a regular function call.
-- **TRIO113**: using `nursery.start_soon` in `__aenter__` doesn't wait for the task to begin. Consider replacing with `nursery.start`.
+- **TRIO112**: Nursery body with only a call to `nursery.start[_soon]` and not passing itself as a parameter can be replaced with a regular function call.
+- **TRIO113**: Using `nursery.start_soon` in `__aenter__` doesn't wait for the task to begin. Consider replacing with `nursery.start`.
 - **TRIO114**: Startable function (i.e. has a `task_status` keyword parameter) not in `--startable-in-context-manager` parameter list, please add it so TRIO113 can catch errors when using it.
 - **TRIO115**: Replace `trio.sleep(0)` with the more suggestive `trio.lowlevel.checkpoint()`.
-- **TRIO116**: `trio.sleep()` with >24 hour interval should usually be`trio.sleep_forever()`.
+- **TRIO116**: `trio.sleep()` with >24 hour interval should usually be `trio.sleep_forever()`.
 - **TRIO117**: Don't raise or catch `trio.[NonBase]MultiError`, prefer `[exceptiongroup.]BaseExceptionGroup`. Even if Trio still raises `MultiError` for legacy code, it can be caught with `BaseExceptionGroup` so it's fully redundant.
 - **TRIO118**: Don't assign the value of `anyio.get_cancelled_exc_class()` to a variable, since that breaks linter checks and multi-backend programs.
 
 ### Warnings for blocking sync calls in async functions
 - **TRIO200**: User-configured error for blocking sync calls in async functions. Does nothing by default, see [`trio200-blocking-calls`](#trio200-blocking-calls) for how to configure it.
 - **TRIO210**: Sync HTTP call in async function, use `httpx.AsyncClient`.
 - **TRIO211**: Likely sync HTTP call in async function, use `httpx.AsyncClient`. Looks for `urllib3` method calls on pool objects, but only matching on the method signature and not the object.
@@ -76,24 +76,88 @@
 - **TRIO231**: Sync IO call in async function, use `trio.wrap_file(...)`.
 - **TRIO232**: Blocking sync call on file object, wrap the file object in `trio.wrap_file()` to get an async file object.
 - **TRIO240**: Avoid using `os.path` in async functions, prefer using `trio.Path` objects.
 
 
 ### Warnings disabled by default
 - **TRIO900**: Async generator without `@asynccontextmanager` not allowed.
-- **TRIO910**: exit or `return` from async function with no guaranteed checkpoint or exception since function definition.
-- **TRIO911**: exit, yield or return from async iterable with no guaranteed checkpoint since possible function entry (yield or function definition)
+- **TRIO910**: Exit or `return` from async function with no guaranteed checkpoint or exception since function definition.
+- **TRIO911**: Exit, `yield` or `return` from async iterable with no guaranteed checkpoint since possible function entry (yield or function definition)
   Checkpoints are `await`, `async for`, and `async with` (on one of enter/exit).
 
+## Examples
+### install and run through flake8
+```sh
+pip install flake8 flake8-trio
+flake8 .
+```
+### install and run with pre-commit
+If you use [pre-commit](https://pre-commit.com/), you can use it with flake8-trio by
+adding the following to your `.pre-commit-config.yaml`:
+
+```yaml
+minimum_pre_commit_version: '2.9.0'
+repos:
+- repo: https://github.com/Zac-HD/flake8-trio
+  rev: 23.5.1
+  hooks:
+    - id: flake8-trio
+      # args: [--enable=TRIO, --disable=TRIO9, --autofix=TRIO]
+```
+
+This is often considerably faster for large projects, because `pre-commit`
+can avoid running `flake8-trio` on unchanged files.
+
+
+Afterwards, run
+```sh
+pip install pre-commit flake8-trio
+pre-commit run .
+```
+### install and run as standalone
+If inside a git repository, running without arguments will run it against all `*.py` files in the repository.
+```sh
+pip install flake8-trio
+flake8-trio
+```
+#### with autofixes
+```sh
+flake8-trio --autofix=TRIO
+```
+#### specifying source files
+```sh
+flake8-trio my_python_file.py
+```
+##### zsh-only
+```zsh
+flake8-trio **/*.py
+```
+
 ## Configuration
 [You can configure `flake8` with command-line options](https://flake8.pycqa.org/en/latest/user/configuration.html),
 but we prefer using a config file. The file needs to start with a section marker `[flake8]` and the following options are then parsed using flake8's config parser, and can be used just like any other flake8 options.
+Note that it's not currently possible to use a configuration file when running `flake8-trio` standalone.
+
+### `--enable`
+Comma-separated list of error codes to enable, similar to flake8 --select but is additionally more performant as it will disable non-enabled visitors from running instead of just silencing their errors.
+
+### `--disable`
+Comma-separated list of error codes to disable, similar to flake8 --ignore but is additionally more performant as it will disable non-enabled visitors from running instead of just silencing their errors.
+
+### `--autofix`
+Comma-separated list of error-codes to enable autofixing for if implemented. Requires running as a standalone program. Pass `--autofix=TRIO` to enable all autofixes.
+
+### `--error-on-autofix`
+Whether to also print an error message for autofixed errors.
+
+### `--anyio`
+Change the default library to be anyio instead of trio. If trio is imported it will assume both are available and print suggestions with [anyio|trio].
 
 ### `no-checkpoint-warning-decorators`
-Specify a list of decorators to disable checkpointing checks for, turning off TRIO910 and TRIO911 warnings for functions decorated with any decorator matching any in the list. Matching is done with [fnmatch](https://docs.python.org/3/library/fnmatch.html). Defaults to disabling for `asynccontextmanager`.
+Comma-separated list of decorators to disable checkpointing checks for, turning off TRIO910 and TRIO911 warnings for functions decorated with any decorator matching any in the list. Matching is done with [fnmatch](https://docs.python.org/3/library/fnmatch.html). Defaults to disabling for `asynccontextmanager`.
 
 Decorators-to-match must be identifiers or dotted names only (not PEP-614 expressions), and will match against the name only - e.g. `foo.bar` matches `foo.bar`, `foo.bar()`, and `foo.bar(args, here)`, etc.
 
 For example:
 ```
 no-checkpoint-warning-decorators =
   mydecorator,
@@ -142,14 +206,20 @@
     arbitrary_other_function(my_blocking_call=None)
 ```
 
 
 # Changelog
 *[CalVer, YY.month.patch](https://calver.org/)*
 
+## 23.5.1
+- TRIO91X now supports comprehensions
+- TRIO100 and TRIO91X now supports autofixing
+- Renamed `--enable-visitor-codes-regex` to `--enable`
+- Added `--disable`, `--autofix` and `--error-on-autofix`
+
 ## 23.2.5
 - Fix false alarms for `@pytest.fixture`-decorated functions in TRIO101, TRIO910 and TRIO911
 
 ## 23.2.4
 - Fix TRIO900 false alarm on nested functions
 - TRIO113 now also works on `anyio.TaskGroup`
```

### Comparing `flake8-trio-23.2.5/README.md` & `flake8-trio-23.5.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -16,34 +16,34 @@
 
 ```console
 pip install flake8-trio
 ```
 
 ## List of warnings
 
-- **TRIO100**: a `with trio.fail_after(...):` or `with trio.move_on_after(...):`
+- **TRIO100**: A `with trio.fail_after(...):` or `with trio.move_on_after(...):`
   context does not contain any `await` statements.  This makes it pointless, as
   the timeout can only be triggered by a checkpoint.
 - **TRIO101**: `yield` inside a nursery or cancel scope is only safe when implementing a context manager - otherwise, it breaks exception handling.
-- **TRIO102**: it's unsafe to await inside `finally:` or `except BaseException/trio.Cancelled` unless you use a shielded
+- **TRIO102**: It's unsafe to await inside `finally:` or `except BaseException/trio.Cancelled` unless you use a shielded
   cancel scope with a timeout.
 - **TRIO103**: `except BaseException`, `except trio.Cancelled` or a bare `except:` with a code path that doesn't re-raise. If you don't want to re-raise `BaseException`, add a separate handler for `trio.Cancelled` before.
 - **TRIO104**: `Cancelled` and `BaseException` must be re-raised - when a user tries to `return` or `raise` a different exception.
 - **TRIO105**: Calling a trio async function without immediately `await`ing it.
-- **TRIO106**: trio must be imported with `import trio` for the linter to work.
+- **TRIO106**: `trio` must be imported with `import trio` for the linter to work.
 - **TRIO107**: Renamed to TRIO910
 - **TRIO108**: Renamed to TRIO911
 - **TRIO109**: Async function definition with a `timeout` parameter - use `trio.[fail/move_on]_[after/at]` instead
 - **TRIO110**: `while <condition>: await trio.sleep()` should be replaced by a `trio.Event`.
 - **TRIO111**: Variable, from context manager opened inside nursery, passed to `start[_soon]` might be invalidly accessed while in use, due to context manager closing before the nursery. This is usually a bug, and nurseries should generally be the inner-most context manager.
-- **TRIO112**: nursery body with only a call to `nursery.start[_soon]` and not passing itself as a parameter can be replaced with a regular function call.
-- **TRIO113**: using `nursery.start_soon` in `__aenter__` doesn't wait for the task to begin. Consider replacing with `nursery.start`.
+- **TRIO112**: Nursery body with only a call to `nursery.start[_soon]` and not passing itself as a parameter can be replaced with a regular function call.
+- **TRIO113**: Using `nursery.start_soon` in `__aenter__` doesn't wait for the task to begin. Consider replacing with `nursery.start`.
 - **TRIO114**: Startable function (i.e. has a `task_status` keyword parameter) not in `--startable-in-context-manager` parameter list, please add it so TRIO113 can catch errors when using it.
 - **TRIO115**: Replace `trio.sleep(0)` with the more suggestive `trio.lowlevel.checkpoint()`.
-- **TRIO116**: `trio.sleep()` with >24 hour interval should usually be`trio.sleep_forever()`.
+- **TRIO116**: `trio.sleep()` with >24 hour interval should usually be `trio.sleep_forever()`.
 - **TRIO117**: Don't raise or catch `trio.[NonBase]MultiError`, prefer `[exceptiongroup.]BaseExceptionGroup`. Even if Trio still raises `MultiError` for legacy code, it can be caught with `BaseExceptionGroup` so it's fully redundant.
 - **TRIO118**: Don't assign the value of `anyio.get_cancelled_exc_class()` to a variable, since that breaks linter checks and multi-backend programs.
 
 ### Warnings for blocking sync calls in async functions
 - **TRIO200**: User-configured error for blocking sync calls in async functions. Does nothing by default, see [`trio200-blocking-calls`](#trio200-blocking-calls) for how to configure it.
 - **TRIO210**: Sync HTTP call in async function, use `httpx.AsyncClient`.
 - **TRIO211**: Likely sync HTTP call in async function, use `httpx.AsyncClient`. Looks for `urllib3` method calls on pool objects, but only matching on the method signature and not the object.
@@ -55,24 +55,88 @@
 - **TRIO231**: Sync IO call in async function, use `trio.wrap_file(...)`.
 - **TRIO232**: Blocking sync call on file object, wrap the file object in `trio.wrap_file()` to get an async file object.
 - **TRIO240**: Avoid using `os.path` in async functions, prefer using `trio.Path` objects.
 
 
 ### Warnings disabled by default
 - **TRIO900**: Async generator without `@asynccontextmanager` not allowed.
-- **TRIO910**: exit or `return` from async function with no guaranteed checkpoint or exception since function definition.
-- **TRIO911**: exit, yield or return from async iterable with no guaranteed checkpoint since possible function entry (yield or function definition)
+- **TRIO910**: Exit or `return` from async function with no guaranteed checkpoint or exception since function definition.
+- **TRIO911**: Exit, `yield` or `return` from async iterable with no guaranteed checkpoint since possible function entry (yield or function definition)
   Checkpoints are `await`, `async for`, and `async with` (on one of enter/exit).
 
+## Examples
+### install and run through flake8
+```sh
+pip install flake8 flake8-trio
+flake8 .
+```
+### install and run with pre-commit
+If you use [pre-commit](https://pre-commit.com/), you can use it with flake8-trio by
+adding the following to your `.pre-commit-config.yaml`:
+
+```yaml
+minimum_pre_commit_version: '2.9.0'
+repos:
+- repo: https://github.com/Zac-HD/flake8-trio
+  rev: 23.5.1
+  hooks:
+    - id: flake8-trio
+      # args: [--enable=TRIO, --disable=TRIO9, --autofix=TRIO]
+```
+
+This is often considerably faster for large projects, because `pre-commit`
+can avoid running `flake8-trio` on unchanged files.
+
+
+Afterwards, run
+```sh
+pip install pre-commit flake8-trio
+pre-commit run .
+```
+### install and run as standalone
+If inside a git repository, running without arguments will run it against all `*.py` files in the repository.
+```sh
+pip install flake8-trio
+flake8-trio
+```
+#### with autofixes
+```sh
+flake8-trio --autofix=TRIO
+```
+#### specifying source files
+```sh
+flake8-trio my_python_file.py
+```
+##### zsh-only
+```zsh
+flake8-trio **/*.py
+```
+
 ## Configuration
 [You can configure `flake8` with command-line options](https://flake8.pycqa.org/en/latest/user/configuration.html),
 but we prefer using a config file. The file needs to start with a section marker `[flake8]` and the following options are then parsed using flake8's config parser, and can be used just like any other flake8 options.
+Note that it's not currently possible to use a configuration file when running `flake8-trio` standalone.
+
+### `--enable`
+Comma-separated list of error codes to enable, similar to flake8 --select but is additionally more performant as it will disable non-enabled visitors from running instead of just silencing their errors.
+
+### `--disable`
+Comma-separated list of error codes to disable, similar to flake8 --ignore but is additionally more performant as it will disable non-enabled visitors from running instead of just silencing their errors.
+
+### `--autofix`
+Comma-separated list of error-codes to enable autofixing for if implemented. Requires running as a standalone program. Pass `--autofix=TRIO` to enable all autofixes.
+
+### `--error-on-autofix`
+Whether to also print an error message for autofixed errors.
+
+### `--anyio`
+Change the default library to be anyio instead of trio. If trio is imported it will assume both are available and print suggestions with [anyio|trio].
 
 ### `no-checkpoint-warning-decorators`
-Specify a list of decorators to disable checkpointing checks for, turning off TRIO910 and TRIO911 warnings for functions decorated with any decorator matching any in the list. Matching is done with [fnmatch](https://docs.python.org/3/library/fnmatch.html). Defaults to disabling for `asynccontextmanager`.
+Comma-separated list of decorators to disable checkpointing checks for, turning off TRIO910 and TRIO911 warnings for functions decorated with any decorator matching any in the list. Matching is done with [fnmatch](https://docs.python.org/3/library/fnmatch.html). Defaults to disabling for `asynccontextmanager`.
 
 Decorators-to-match must be identifiers or dotted names only (not PEP-614 expressions), and will match against the name only - e.g. `foo.bar` matches `foo.bar`, `foo.bar()`, and `foo.bar(args, here)`, etc.
 
 For example:
 ```
 no-checkpoint-warning-decorators =
   mydecorator,
```

### Comparing `flake8-trio-23.2.5/flake8_trio/base.py` & `flake8-trio-23.5.1/flake8_trio/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,30 @@
 """Contains base classes used across multiple parts of the package."""
 
 from __future__ import annotations
 
-from typing import Any, NamedTuple
+from dataclasses import dataclass
+from typing import TYPE_CHECKING, Any, NamedTuple
+
+if TYPE_CHECKING:
+    from collections.abc import Collection
+
+
+@dataclass
+class Options:
+    # error codes to give errors for
+    enabled_codes: set[str]
+    # error codes to autofix
+    autofix_codes: set[str]
+    # whether to print an error message even when autofixed
+    error_on_autofix: bool
+    no_checkpoint_warning_decorators: Collection[str]
+    startable_in_context_manager: Collection[str]
+    trio200_blocking_calls: dict[str, str]
+    anyio: bool
 
 
 class Statement(NamedTuple):
     name: str
     lineno: int
     col_offset: int = -1
 
@@ -28,30 +46,38 @@
         super().__init__()
         self.line = lineno
         self.col = col
         self.code = error_code
         self.message = message
         self.args = args
 
+    def format_message(self):
+        return f"{self.code} " + self.message.format(*self.args)
+
     # for yielding to flake8
     def __iter__(self):
         yield self.line
         yield self.col
-        yield f"{self.code} " + self.message.format(*self.args)
+        yield self.format_message()
         # We are no longer yielding `type(Plugin)` since that's quite tricky to do
         # without circular imports, and afaik flake8 doesn't care anymore.
         yield None
 
     def cmp(self):
-        return self.line, self.col, self.code, self.args
+        # column may be ignored/modified when autofixing, so sort on that last
+        return self.line, self.code, self.args, self.col
 
     # for sorting in tests
     def __lt__(self, other: Any) -> bool:
         assert isinstance(other, Error)
         return self.cmp() < other.cmp()
 
     def __eq__(self, other: Any) -> bool:
         return isinstance(other, Error) and self.cmp() == other.cmp()
 
     def __repr__(self) -> str:  # pragma: no cover
         trailer = "".join(f", {x!r}" for x in self.args)
         return f"<{self.code} error at {self.line}:{self.col}{trailer}>"
+
+    def __str__(self) -> str:
+        # flake8 adds 1 to the yielded column from `__iter__`, so we do the same here
+        return f"{self.line}:{self.col+1}: {self.format_message()}"
```

### Comparing `flake8-trio-23.2.5/flake8_trio/visitors/flake8triovisitor.py` & `flake8-trio-23.5.1/flake8_trio/visitors/flake8triovisitor.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 """Contains the base class that all error classes inherit from."""
 
 from __future__ import annotations
 
 import ast
-import re
 from abc import ABC
 from typing import TYPE_CHECKING, Any, Union
 
+import libcst as cst
+from libcst.metadata import PositionProvider
+
 from ..base import Error, Statement
 
 if TYPE_CHECKING:
     from collections.abc import Iterable
 
     from ..runner import SharedState
 
     HasLineCol = Union[
         ast.expr, ast.stmt, ast.arg, ast.excepthandler, ast.alias, Statement
     ]
 
 
 class Flake8TrioVisitor(ast.NodeVisitor, ABC):
     # abstract attribute by not providing a value
-    error_codes: dict[str, str]  # pyright: reportUninitializedInstanceVariable=false
+    error_codes: dict[str, str]  # pyright: ignore[reportUninitializedInstanceVariable]
 
     def __init__(self, shared_state: SharedState):
         super().__init__()
         self.outer: dict[ast.AST, dict[str, Any]] = {}
         self.novisit = False
         self.__state = shared_state
 
@@ -39,16 +41,14 @@
             "nocopy",
             "novisit",
             "options",
             "outer",
             "typed_calls",
         }
 
-        self.suppress_errors = False
-
     # `variables` can be saved/loaded, but need a setter to not clear the reference
     @property
     def variables(self) -> dict[str, str]:
         return self.__state.variables
 
     @variables.setter
     def variables(self, value: dict[str, str]) -> None:
@@ -94,28 +94,27 @@
     ):
         if error_code is None:
             assert (
                 len(self.error_codes) == 1
             ), "No error code defined, but class has multiple codes"
             error_code = next(iter(self.error_codes))
         # don't emit an error if this code is disabled in a multi-code visitor
-        elif not re.match(self.options.enable_visitor_codes_regex, error_code):
+        elif error_code[:7] not in self.options.enabled_codes:
             return
 
-        if not self.suppress_errors:
-            self.__state.problems.append(
-                Error(
-                    # 7 == len('TRIO...'), so alt messages raise the original code
-                    error_code[:7],
-                    node.lineno,
-                    node.col_offset,
-                    self.error_codes[error_code],
-                    *args,
-                )
+        self.__state.problems.append(
+            Error(
+                # 7 == len('TRIO...'), so alt messages raise the original code
+                error_code[:7],
+                node.lineno,
+                node.col_offset,
+                self.error_codes[error_code],
+                *args,
             )
+        )
 
     def get_state(self, *attrs: str, copy: bool = False) -> dict[str, Any]:
         if not attrs:
             # get all attributes, unless they're marked as nocopy
             attrs = tuple(set(self.__dict__.keys()) - self.nocopy)
         res: dict[str, Any] = {}
         for attr in attrs:
@@ -123,16 +122,14 @@
             if copy and hasattr(value, "copy"):
                 value = value.copy()
             res[attr] = value
         return res
 
     def set_state(self, attrs: dict[str, Any], copy: bool = False):
         for attr, value in attrs.items():
-            if copy and hasattr(value, "copy"):
-                value = value.copy()
             setattr(self, attr, value)
 
     def save_state(self, node: ast.AST, *attrs: str, copy: bool = False):
         state = self.get_state(*attrs, copy=copy)
         if node in self.outer:
             # not currently used, and not gonna bother adding dedicated test
             # visitors atm
@@ -153,7 +150,93 @@
         if len(self.library) == 1:
             return self.library[0]
         return "[" + "|".join(self.library) + "]"
 
     def add_library(self, name: str) -> None:
         if name not in self.__state.library:
             self.__state.library = self.__state.library + (name,)
+
+
+class Flake8TrioVisitor_cst(cst.CSTTransformer, ABC):
+    # abstract attribute by not providing a value
+    error_codes: dict[str, str]  # pyright: ignore[reportUninitializedInstanceVariable]
+    METADATA_DEPENDENCIES = (PositionProvider,)
+
+    def __init__(self, shared_state: SharedState):
+        super().__init__()
+        self.outer: dict[cst.CSTNode, dict[str, Any]] = {}
+        self.__state = shared_state
+
+        self.options = self.__state.options
+        self.noqas = self.__state.noqas
+
+    def get_state(self, *attrs: str, copy: bool = False) -> dict[str, Any]:
+        # require attrs, since we inherit a *ton* of stuff which we don't want to copy
+        assert attrs
+        res: dict[str, Any] = {}
+        for attr in attrs:
+            value = getattr(self, attr)
+            if copy and hasattr(value, "copy"):
+                value = value.copy()
+            res[attr] = value
+        return res
+
+    def set_state(self, attrs: dict[str, Any], copy: bool = False):
+        for attr, value in attrs.items():
+            if copy and hasattr(value, "copy"):  # pragma: no cover
+                # not used by visitors yet
+                value = value.copy()
+            setattr(self, attr, value)
+
+    def save_state(self, node: cst.CSTNode, *attrs: str, copy: bool = False):
+        state = self.get_state(*attrs, copy=copy)
+        if node in self.outer:
+            self.outer[node].update(state)
+        else:
+            self.outer[node] = state
+
+    def restore_state(self, node: cst.CSTNode):
+        self.set_state(self.outer.pop(node, {}))
+
+    def error(
+        self,
+        node: cst.CSTNode,
+        *args: str | Statement | int,
+        error_code: str | None = None,
+    ):
+        if error_code is None:
+            assert (
+                len(self.error_codes) == 1
+            ), "No error code defined, but class has multiple codes"
+            error_code = next(iter(self.error_codes))
+        # don't emit an error if this code is disabled in a multi-code visitor
+        # TODO: write test for only one of 910/911 enabled/autofixed
+        elif error_code[:7] not in self.options.enabled_codes:
+            return  # pragma: no cover
+        pos = self.get_metadata(PositionProvider, node).start
+
+        self.__state.problems.append(
+            Error(
+                # 7 == len('TRIO...'), so alt messages raise the original code
+                error_code[:7],
+                pos.line,
+                pos.column,
+                self.error_codes[error_code],
+                *args,
+            )
+        )
+
+    def should_autofix(self, code: str | None = None):
+        if code is None:
+            assert len(self.error_codes) == 1
+            code = next(iter(self.error_codes))
+        return code in self.options.autofix_codes
+
+    @property
+    def library(self) -> tuple[str, ...]:
+        return self.__state.library if self.__state.library else ("trio",)
+
+    # library_str not used in cst yet
+
+    def add_library(self, name: str) -> None:
+        if name not in self.__state.library:
+            self.__state.library = self.__state.library + (name,)
```

### Comparing `flake8-trio-23.2.5/flake8_trio/visitors/visitor102.py` & `flake8-trio-23.5.1/flake8_trio/visitors/visitor102.py`

 * *Files identical despite different names*

### Comparing `flake8-trio-23.2.5/flake8_trio/visitors/visitor103_104.py` & `flake8-trio-23.5.1/flake8_trio/visitors/visitor103_104.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,17 +27,17 @@
 @error_class
 class Visitor103_104(Flake8TrioVisitor):
     error_codes = {
         "TRIO103": _trio103_common_msg,
         "TRIO104": "Cancelled (and therefore BaseException) must be re-raised.",
     }
     for poss_library in _suggestion_dict:
-        error_codes[
-            f"TRIO103_{'_'.join(poss_library)}"
-        ] = _trio103_common_msg + _suggestion.format(_suggestion_dict[poss_library])
+        error_codes[f"TRIO103_{'_'.join(poss_library)}"] = (
+            _trio103_common_msg + _suggestion.format(_suggestion_dict[poss_library])
+        )
 
     def __init__(self, *args: Any, **kwargs: Any):
         super().__init__(*args, **kwargs)
         self.except_name: str | None = ""
         self.unraised: bool = False
         self.unraised_break: bool = False
         self.unraised_continue: bool = False
```

### Comparing `flake8-trio-23.2.5/flake8_trio/visitors/visitor105.py` & `flake8-trio-23.5.1/flake8_trio/visitors/visitor105.py`

 * *Files identical despite different names*

### Comparing `flake8-trio-23.2.5/flake8_trio/visitors/visitor111.py` & `flake8-trio-23.5.1/flake8_trio/visitors/visitor111.py`

 * *Files identical despite different names*

### Comparing `flake8-trio-23.2.5/flake8_trio/visitors/visitor118.py` & `flake8-trio-23.5.1/flake8_trio/visitors/visitor118.py`

 * *Files identical despite different names*

### Comparing `flake8-trio-23.2.5/flake8_trio/visitors/visitor2xx.py` & `flake8-trio-23.5.1/flake8_trio/visitors/visitor2xx.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,16 +222,16 @@
         if error_code is not None:
             self.error(node, func_name, self.library_str, error_code=error_code)
 
 
 @error_class
 class Visitor23X(Visitor200):
     error_codes = {
-        "TRIO230": ("Sync call {0} in async function, use `{1}.open_file(...)`."),
-        "TRIO231": ("Sync call {0} in async function, use `{1}.wrap_file({0})`."),
+        "TRIO230": "Sync call {0} in async function, use `{1}.open_file(...)`.",
+        "TRIO231": "Sync call {0} in async function, use `{1}.wrap_file({0})`.",
     }
 
     def visit_Call(self, node: ast.Call):
         func_name = ast.unparse(node.func)
         if re.fullmatch(r"(trio|anyio)\.wrap_file", func_name) and len(node.args) == 1:
             setattr(node.args[0], "wrapped", True)  # noqa: B010
         super().visit_Call(node)
@@ -278,15 +278,15 @@
         ):
             self.error(node, node.func.attr, node.func.value.id, self.library_str)
 
 
 @error_class
 class Visitor24X(Visitor200):
     error_codes = {
-        "TRIO240": ("Avoid using os.path, prefer using {1}.Path objects."),
+        "TRIO240": "Avoid using os.path, prefer using {1}.Path objects.",
     }
 
     def __init__(self, *args: Any, **kwargs: Any):
         super().__init__(*args, **kwargs)
         self.imports_from_ospath: set[str] = set()
 
     os_funcs = (
```

### Comparing `flake8-trio-23.2.5/flake8_trio/visitors/visitor_utility.py` & `flake8-trio-23.5.1/flake8_trio/runner.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,118 +1,134 @@
-"""Utility visitors for tracking shared state and modifying the tree."""
+"""Contains Flake8TrioRunner.
+
+The runner is what's run by the Plugin, and handles traversing
+the AST and letting all registered ERROR_CLASSES do their visit'ing on them.
+"""
 
 from __future__ import annotations
 
 import ast
-from typing import Any
-
-from .flake8triovisitor import Flake8TrioVisitor
-from .helpers import utility_visitor
-
+from dataclasses import dataclass, field
+from typing import TYPE_CHECKING
 
-@utility_visitor
-class VisitorTypeTracker(Flake8TrioVisitor):
-    def visit_AsyncFunctionDef(
-        self, node: ast.AsyncFunctionDef | ast.FunctionDef | ast.Lambda
-    ):
-        def or_none(node: ast.AST | None):
-            if not isinstance(node, ast.BinOp) or not isinstance(node.op, ast.BitOr):
-                return None
-            if isinstance(node.left, ast.Constant) and node.left.value is None:
-                return node.right
-            if isinstance(node.right, ast.Constant) and node.right.value is None:
-                return node.left
-            return None
-
-        self.save_state(node, "variables", copy=True)
-
-        args = node.args
-        for arg in *args.args, *args.posonlyargs, *args.kwonlyargs:
-            annotation = arg.annotation
-
-            if (
-                isinstance(annotation, ast.Subscript)
-                and isinstance(annotation.value, ast.Name)
-                and annotation.value.id == "Optional"
-            ):
-                annotation = annotation.slice
-            elif res := or_none(annotation):
-                annotation = res
-
-            if isinstance(annotation, (ast.Name, ast.Attribute, ast.Constant)):
-                annotation_type = ast.unparse(annotation)
-            else:
-                annotation_type = "Any"
-
-            self.variables[arg.arg] = annotation_type
-
-    visit_FunctionDef = visit_AsyncFunctionDef
-    visit_Lambda = visit_AsyncFunctionDef
-
-    # Does not handle class members, or attributes in general
-    def visit_ClassDef(self, node: ast.ClassDef):
-        self.save_state(node, "variables", copy=True)
+import libcst as cst
 
-    def visit_AnnAssign(self, node: ast.AnnAssign):
-        if not isinstance(node.target, ast.Name):
-            return
-        target = node.target.id
-        typename = ast.unparse(node.annotation)
-        self.variables[target] = typename
+from .visitors import (
+    ERROR_CLASSES,
+    ERROR_CLASSES_CST,
+    utility_visitors,
+    utility_visitors_cst,
+)
+
+if TYPE_CHECKING:
+    from collections.abc import Iterable
+
+    from libcst import Module
+
+    from .base import Error, Options
+    from .visitors.flake8triovisitor import Flake8TrioVisitor, Flake8TrioVisitor_cst
+
+
+@dataclass
+class SharedState:
+    options: Options
+    problems: list[Error] = field(default_factory=list)
+    noqas: dict[int, set[str]] = field(default_factory=dict)
+    library: tuple[str, ...] = ()
+    typed_calls: dict[str, str] = field(default_factory=dict)
+    variables: dict[str, str] = field(default_factory=dict)
+
+
+class __CommonRunner:
+    """Common functionality used in both runners."""
+
+    def __init__(self, options: Options):
+        super().__init__()
+        self.state = SharedState(options)
+
+    def selected(self, error_codes: dict[str, str]) -> bool:
+        enabled_or_autofix = (
+            self.state.options.enabled_codes | self.state.options.autofix_codes
+        )
+        return bool(set(error_codes) & enabled_or_autofix)
+
+
+class Flake8TrioRunner(ast.NodeVisitor, __CommonRunner):
+    def __init__(self, options: Options):
+        super().__init__(options)
+        # utility visitors that need to run before the error-checking visitors
+        self.utility_visitors = {v(self.state) for v in utility_visitors}
+
+        self.visitors = {
+            v(self.state) for v in ERROR_CLASSES if self.selected(v.error_codes)
+        }
+
+    @classmethod
+    def run(cls, tree: ast.AST, options: Options) -> Iterable[Error]:
+        runner = cls(options)
+        runner.visit(tree)
+        yield from runner.state.problems
+
+    def visit(self, node: ast.AST):
+        """Visit a node."""
+        # tracks the subclasses that, from this node on, iterated through it's subfields
+        # we need to remember it so we can restore it at the end of the function.
+        novisit: set[Flake8TrioVisitor] = set()
+
+        method = "visit_" + node.__class__.__name__
+
+        for subclass in *self.utility_visitors, *self.visitors:
+            # check if subclass has defined a visitor for this type
+            class_method = getattr(subclass, method, None)
+            if class_method is None:
+                continue
+
+            # call it
+            class_method(node)
+
+            # it will set `.novisit` if it has itself handled iterating through subfields
+            # so we add it to our novisit set
+            if subclass.novisit:
+                novisit.add(subclass)
+
+        # Remove all subclasses that iterated through subfields from our list of
+        # visitors, so we don't visit them twice.
+        self.visitors.difference_update(novisit)
+
+        # iterate through subfields using NodeVisitor
+        self.generic_visit(node)
+
+        # reset the novisit flag for the classes in novisit
+        for subclass in novisit:
+            subclass.novisit = False
+
+        # and add them back to our visitors
+        self.visitors.update(novisit)
+
+        # restore any outer state that was saved in the visitor method
+        for subclass in *self.utility_visitors, *self.visitors:
+            subclass.set_state(subclass.outer.pop(node, {}))
+
+
+class Flake8TrioRunner_cst(__CommonRunner):
+    def __init__(self, options: Options, module: Module):
+        super().__init__(options)
+        self.options = options
+
+        # Could possibly enable/disable utility visitors here, if visitors declared
+        # dependencies
+        self.utility_visitors: tuple[Flake8TrioVisitor_cst, ...] = tuple(
+            v(self.state) for v in utility_visitors_cst
+        )
+
+        self.visitors: tuple[Flake8TrioVisitor_cst, ...] = tuple(
+            v(self.state) for v in ERROR_CLASSES_CST if self.selected(v.error_codes)
+        )
+        self.module = module
 
-    def visit_Assign(self, node: ast.Assign):
-        if len(node.targets) != 1 or not isinstance(node.targets[0], ast.Name):
+    def run(self) -> Iterable[Error]:
+        if not self.visitors:
             return
+        for v in (*self.utility_visitors, *self.visitors):
+            self.module = cst.MetadataWrapper(self.module).visit(v)
 
-        # `f = open(...)`
-        if isinstance(node.value, ast.Call) and (
-            vartype := self.typed_calls.get(ast.unparse(node.value.func), None)
-        ):
-            self.variables[node.targets[0].id] = vartype
-
-        # f = ff (and ff is a variable with known type)
-        elif isinstance(node.value, ast.Name) and (
-            value := self.variables.get(node.value.id, None)
-        ):
-            self.variables[node.targets[0].id] = value
-
-    def visit_With(self, node: ast.With | ast.AsyncWith):
-        if len(node.items) != 1:
-            return
-        item = node.items[0]
-        if (
-            isinstance(item.context_expr, ast.Call)
-            and isinstance(item.optional_vars, ast.Name)
-            and (
-                vartype := self.typed_calls.get(
-                    ast.unparse(item.context_expr.func), None
-                )
-            )
-        ):
-            self.variables[item.optional_vars.id] = vartype
-
-    visit_AsyncWith = visit_With
-
-
-@utility_visitor
-class VisitorAwaitModifier(Flake8TrioVisitor):
-    def visit_Await(self, node: ast.Await):
-        if isinstance(node.value, ast.Call):
-            # add attribute to indicate it's awaited
-            setattr(node.value, "awaited", True)  # noqa: B010
-
-
-@utility_visitor
-class VisitorLibraryHandler(Flake8TrioVisitor):
-    def __init__(self, *args: Any, **kwargs: Any):
-        super().__init__(*args, **kwargs)
-        # check whether library we're working towards has been explicitly
-        # specified with --anyio, otherwise assume Trio - but we update if we
-        # see imports
-        if self.options.anyio:
-            self.add_library("anyio")
-
-    def visit_Import(self, node: ast.Import):
-        for alias in node.names:
-            name = alias.name
-            if name in ("trio", "anyio") and alias.asname is None:
-                self.add_library(name)
+        yield from self.state.problems
```

### Comparing `flake8-trio-23.2.5/flake8_trio/visitors/visitors.py` & `flake8-trio-23.5.1/flake8_trio/visitors/visitors.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,92 +2,15 @@
 
 from __future__ import annotations
 
 import ast
 from typing import Any, cast
 
 from .flake8triovisitor import Flake8TrioVisitor
-from .helpers import (
-    cancel_scope_names,
-    disabled_by_default,
-    error_class,
-    get_matching_call,
-    has_decorator,
-)
-
-# used in 100
-checkpoint_node_types = (ast.Await, ast.AsyncFor, ast.AsyncWith)
-
-
-@error_class
-class Visitor100(Flake8TrioVisitor):
-    error_codes = {
-        "TRIO100": (
-            "{0}.{1} context contains no checkpoints, remove the context or add"
-            " `await {0}.lowlevel.checkpoint()`."
-        ),
-    }
-
-    def visit_With(self, node: ast.With | ast.AsyncWith):
-        for item in (i.context_expr for i in node.items):
-            call = get_matching_call(item, *cancel_scope_names)
-            if call and not any(
-                isinstance(x, checkpoint_node_types) and x != node
-                for x in ast.walk(node)
-            ):
-                # type checking has been done inside get_matching_call
-                self.error(item, call[2], call[1])
-
-    visit_AsyncWith = visit_With
-
-
-@error_class
-class Visitor101(Flake8TrioVisitor):
-    error_codes = {
-        "TRIO101": (
-            "`yield` inside a nursery or cancel scope is only safe when implementing "
-            "a context manager - otherwise, it breaks exception handling."
-        ),
-    }
-
-    def __init__(self, *args: Any, **kwargs: Any):
-        super().__init__(*args, **kwargs)
-        self._yield_is_error = False
-        self._safe_decorator = False
-
-    def visit_With(self, node: ast.With | ast.AsyncWith):
-        self.save_state(node, "_yield_is_error", copy=True)
-        for item in node.items:
-            # if there's no safe decorator,
-            # and it's not yet been determined that yield is error
-            # and this withitem opens a cancelscope:
-            # then yielding is unsafe
-            if (
-                not self._safe_decorator
-                and not self._yield_is_error
-                and get_matching_call(
-                    item.context_expr, "open_nursery", *cancel_scope_names
-                )
-                is not None
-            ):
-                self._yield_is_error = True
-
-    def visit_FunctionDef(self, node: ast.FunctionDef | ast.AsyncFunctionDef):
-        self.save_state(node)
-        self._yield_is_error = False
-        self._safe_decorator = has_decorator(
-            node, "contextmanager", "asynccontextmanager", "fixture"
-        )
-
-    visit_AsyncWith = visit_With
-    visit_AsyncFunctionDef = visit_FunctionDef
-
-    def visit_Yield(self, node: ast.Yield):
-        if self._yield_is_error:
-            self.error(node)
+from .helpers import disabled_by_default, error_class, get_matching_call, has_decorator
 
 
 @error_class
 class Visitor106(Flake8TrioVisitor):
     error_codes = {
         "TRIO106": "{0} must be imported with `import {0}` for the linter to work.",
     }
@@ -164,15 +87,15 @@
                 continue
             var_name = item.optional_vars.id
 
             # check for trio.open_nursery
             nursery = get_matching_call(item.context_expr, "open_nursery")
 
             # `isinstance(..., ast.Call)` is done in get_matching_call
-            body_call = cast(ast.Call, node.body[0].value)
+            body_call = cast("ast.Call", node.body[0].value)
 
             if (
                 nursery is not None
                 and get_matching_call(body_call, "start", "start_soon", base=var_name)
                 # check for presence of <X> as parameter
                 and not any(
                     (isinstance(n, ast.Name) and n.id == var_name)
@@ -341,15 +264,15 @@
 DEPRECATED_ERRORS = ("MultiError", "NonBaseMultiError")
 
 
 # anyio does not have MultiError, so this check is trio-only
 @error_class
 class Visitor117(Flake8TrioVisitor):
     error_codes = {
-        "TRIO117": ("Reference to {}, prefer [exceptiongroup.]BaseExceptionGroup."),
+        "TRIO117": "Reference to {}, prefer [exceptiongroup.]BaseExceptionGroup.",
     }
 
     # This should never actually happen given TRIO106
     def visit_Name(self, node: ast.Name):
         if node.id in DEPRECATED_ERRORS and "trio" in self.library:
             self.error(node, node.id)
 
@@ -358,15 +281,15 @@
             self.error(node, n)
 
 
 @error_class
 @disabled_by_default
 class Visitor900(Flake8TrioVisitor):
     error_codes = {
-        "TRIO900": ("Async generator without `@asynccontextmanager` not allowed.")
+        "TRIO900": "Async generator without `@asynccontextmanager` not allowed."
     }
 
     def __init__(self, *args: Any, **kwargs: Any):
         super().__init__(*args, **kwargs)
         self.unsafe_function: ast.AsyncFunctionDef | None = None
 
     def visit_AsyncFunctionDef(
```

### Comparing `flake8-trio-23.2.5/flake8_trio.egg-info/PKG-INFO` & `flake8-trio-23.5.1/flake8_trio.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-trio
-Version: 23.2.5
+Version: 23.5.1
 Summary: A highly opinionated flake8 plugin for Trio-related problems.
 Home-page: https://github.com/Zac-HD/flake8-trio
 Author: Zac Hatfield-Dodds, John Litborn, and Contributors
 Author-email: zac@zhd.dev
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Flake8
@@ -37,34 +37,34 @@
 
 ```console
 pip install flake8-trio
 ```
 
 ## List of warnings
 
-- **TRIO100**: a `with trio.fail_after(...):` or `with trio.move_on_after(...):`
+- **TRIO100**: A `with trio.fail_after(...):` or `with trio.move_on_after(...):`
   context does not contain any `await` statements.  This makes it pointless, as
   the timeout can only be triggered by a checkpoint.
 - **TRIO101**: `yield` inside a nursery or cancel scope is only safe when implementing a context manager - otherwise, it breaks exception handling.
-- **TRIO102**: it's unsafe to await inside `finally:` or `except BaseException/trio.Cancelled` unless you use a shielded
+- **TRIO102**: It's unsafe to await inside `finally:` or `except BaseException/trio.Cancelled` unless you use a shielded
   cancel scope with a timeout.
 - **TRIO103**: `except BaseException`, `except trio.Cancelled` or a bare `except:` with a code path that doesn't re-raise. If you don't want to re-raise `BaseException`, add a separate handler for `trio.Cancelled` before.
 - **TRIO104**: `Cancelled` and `BaseException` must be re-raised - when a user tries to `return` or `raise` a different exception.
 - **TRIO105**: Calling a trio async function without immediately `await`ing it.
-- **TRIO106**: trio must be imported with `import trio` for the linter to work.
+- **TRIO106**: `trio` must be imported with `import trio` for the linter to work.
 - **TRIO107**: Renamed to TRIO910
 - **TRIO108**: Renamed to TRIO911
 - **TRIO109**: Async function definition with a `timeout` parameter - use `trio.[fail/move_on]_[after/at]` instead
 - **TRIO110**: `while <condition>: await trio.sleep()` should be replaced by a `trio.Event`.
 - **TRIO111**: Variable, from context manager opened inside nursery, passed to `start[_soon]` might be invalidly accessed while in use, due to context manager closing before the nursery. This is usually a bug, and nurseries should generally be the inner-most context manager.
-- **TRIO112**: nursery body with only a call to `nursery.start[_soon]` and not passing itself as a parameter can be replaced with a regular function call.
-- **TRIO113**: using `nursery.start_soon` in `__aenter__` doesn't wait for the task to begin. Consider replacing with `nursery.start`.
+- **TRIO112**: Nursery body with only a call to `nursery.start[_soon]` and not passing itself as a parameter can be replaced with a regular function call.
+- **TRIO113**: Using `nursery.start_soon` in `__aenter__` doesn't wait for the task to begin. Consider replacing with `nursery.start`.
 - **TRIO114**: Startable function (i.e. has a `task_status` keyword parameter) not in `--startable-in-context-manager` parameter list, please add it so TRIO113 can catch errors when using it.
 - **TRIO115**: Replace `trio.sleep(0)` with the more suggestive `trio.lowlevel.checkpoint()`.
-- **TRIO116**: `trio.sleep()` with >24 hour interval should usually be`trio.sleep_forever()`.
+- **TRIO116**: `trio.sleep()` with >24 hour interval should usually be `trio.sleep_forever()`.
 - **TRIO117**: Don't raise or catch `trio.[NonBase]MultiError`, prefer `[exceptiongroup.]BaseExceptionGroup`. Even if Trio still raises `MultiError` for legacy code, it can be caught with `BaseExceptionGroup` so it's fully redundant.
 - **TRIO118**: Don't assign the value of `anyio.get_cancelled_exc_class()` to a variable, since that breaks linter checks and multi-backend programs.
 
 ### Warnings for blocking sync calls in async functions
 - **TRIO200**: User-configured error for blocking sync calls in async functions. Does nothing by default, see [`trio200-blocking-calls`](#trio200-blocking-calls) for how to configure it.
 - **TRIO210**: Sync HTTP call in async function, use `httpx.AsyncClient`.
 - **TRIO211**: Likely sync HTTP call in async function, use `httpx.AsyncClient`. Looks for `urllib3` method calls on pool objects, but only matching on the method signature and not the object.
@@ -76,24 +76,88 @@
 - **TRIO231**: Sync IO call in async function, use `trio.wrap_file(...)`.
 - **TRIO232**: Blocking sync call on file object, wrap the file object in `trio.wrap_file()` to get an async file object.
 - **TRIO240**: Avoid using `os.path` in async functions, prefer using `trio.Path` objects.
 
 
 ### Warnings disabled by default
 - **TRIO900**: Async generator without `@asynccontextmanager` not allowed.
-- **TRIO910**: exit or `return` from async function with no guaranteed checkpoint or exception since function definition.
-- **TRIO911**: exit, yield or return from async iterable with no guaranteed checkpoint since possible function entry (yield or function definition)
+- **TRIO910**: Exit or `return` from async function with no guaranteed checkpoint or exception since function definition.
+- **TRIO911**: Exit, `yield` or `return` from async iterable with no guaranteed checkpoint since possible function entry (yield or function definition)
   Checkpoints are `await`, `async for`, and `async with` (on one of enter/exit).
 
+## Examples
+### install and run through flake8
+```sh
+pip install flake8 flake8-trio
+flake8 .
+```
+### install and run with pre-commit
+If you use [pre-commit](https://pre-commit.com/), you can use it with flake8-trio by
+adding the following to your `.pre-commit-config.yaml`:
+
+```yaml
+minimum_pre_commit_version: '2.9.0'
+repos:
+- repo: https://github.com/Zac-HD/flake8-trio
+  rev: 23.5.1
+  hooks:
+    - id: flake8-trio
+      # args: [--enable=TRIO, --disable=TRIO9, --autofix=TRIO]
+```
+
+This is often considerably faster for large projects, because `pre-commit`
+can avoid running `flake8-trio` on unchanged files.
+
+
+Afterwards, run
+```sh
+pip install pre-commit flake8-trio
+pre-commit run .
+```
+### install and run as standalone
+If inside a git repository, running without arguments will run it against all `*.py` files in the repository.
+```sh
+pip install flake8-trio
+flake8-trio
+```
+#### with autofixes
+```sh
+flake8-trio --autofix=TRIO
+```
+#### specifying source files
+```sh
+flake8-trio my_python_file.py
+```
+##### zsh-only
+```zsh
+flake8-trio **/*.py
+```
+
 ## Configuration
 [You can configure `flake8` with command-line options](https://flake8.pycqa.org/en/latest/user/configuration.html),
 but we prefer using a config file. The file needs to start with a section marker `[flake8]` and the following options are then parsed using flake8's config parser, and can be used just like any other flake8 options.
+Note that it's not currently possible to use a configuration file when running `flake8-trio` standalone.
+
+### `--enable`
+Comma-separated list of error codes to enable, similar to flake8 --select but is additionally more performant as it will disable non-enabled visitors from running instead of just silencing their errors.
+
+### `--disable`
+Comma-separated list of error codes to disable, similar to flake8 --ignore but is additionally more performant as it will disable non-enabled visitors from running instead of just silencing their errors.
+
+### `--autofix`
+Comma-separated list of error-codes to enable autofixing for if implemented. Requires running as a standalone program. Pass `--autofix=TRIO` to enable all autofixes.
+
+### `--error-on-autofix`
+Whether to also print an error message for autofixed errors.
+
+### `--anyio`
+Change the default library to be anyio instead of trio. If trio is imported it will assume both are available and print suggestions with [anyio|trio].
 
 ### `no-checkpoint-warning-decorators`
-Specify a list of decorators to disable checkpointing checks for, turning off TRIO910 and TRIO911 warnings for functions decorated with any decorator matching any in the list. Matching is done with [fnmatch](https://docs.python.org/3/library/fnmatch.html). Defaults to disabling for `asynccontextmanager`.
+Comma-separated list of decorators to disable checkpointing checks for, turning off TRIO910 and TRIO911 warnings for functions decorated with any decorator matching any in the list. Matching is done with [fnmatch](https://docs.python.org/3/library/fnmatch.html). Defaults to disabling for `asynccontextmanager`.
 
 Decorators-to-match must be identifiers or dotted names only (not PEP-614 expressions), and will match against the name only - e.g. `foo.bar` matches `foo.bar`, `foo.bar()`, and `foo.bar(args, here)`, etc.
 
 For example:
 ```
 no-checkpoint-warning-decorators =
   mydecorator,
@@ -142,14 +206,20 @@
     arbitrary_other_function(my_blocking_call=None)
 ```
 
 
 # Changelog
 *[CalVer, YY.month.patch](https://calver.org/)*
 
+## 23.5.1
+- TRIO91X now supports comprehensions
+- TRIO100 and TRIO91X now supports autofixing
+- Renamed `--enable-visitor-codes-regex` to `--enable`
+- Added `--disable`, `--autofix` and `--error-on-autofix`
+
 ## 23.2.5
 - Fix false alarms for `@pytest.fixture`-decorated functions in TRIO101, TRIO910 and TRIO911
 
 ## 23.2.4
 - Fix TRIO900 false alarm on nested functions
 - TRIO113 now also works on `anyio.TaskGroup`
```

### Comparing `flake8-trio-23.2.5/flake8_trio.egg-info/SOURCES.txt` & `flake8-trio-23.5.1/flake8_trio.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -3,46 +3,60 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 tox.ini
 flake8_trio/__init__.py
+flake8_trio/__main__.py
 flake8_trio/base.py
 flake8_trio/runner.py
 flake8_trio.egg-info/PKG-INFO
 flake8_trio.egg-info/SOURCES.txt
 flake8_trio.egg-info/dependency_links.txt
 flake8_trio.egg-info/entry_points.txt
 flake8_trio.egg-info/not-zip-safe
 flake8_trio.egg-info/requires.txt
 flake8_trio.egg-info/top_level.txt
 flake8_trio/visitors/__init__.py
 flake8_trio/visitors/flake8triovisitor.py
 flake8_trio/visitors/helpers.py
+flake8_trio/visitors/visitor100.py
+flake8_trio/visitors/visitor101.py
 flake8_trio/visitors/visitor102.py
 flake8_trio/visitors/visitor103_104.py
 flake8_trio/visitors/visitor105.py
 flake8_trio/visitors/visitor111.py
 flake8_trio/visitors/visitor118.py
 flake8_trio/visitors/visitor2xx.py
 flake8_trio/visitors/visitor91x.py
 flake8_trio/visitors/visitor_utility.py
 flake8_trio/visitors/visitors.py
 tests/__init__.py
 tests/conftest.py
 tests/test_all_visitors_imported.py
 tests/test_changelog_and_version.py
+tests/test_config_and_args.py
 tests/test_decorator.py
+tests/test_exception_on_invalid_code.py
 tests/test_flake8_trio.py
 tests/test_formatting.py
+tests/test_messages_documented.py
 tests/trio_options.py
+tests/autofix_files/trio100.py
+tests/autofix_files/trio100_simple_autofix.py
+tests/autofix_files/trio910.py
+tests/autofix_files/trio911.py
+tests/autofix_files/trio91x_autofix.py
 tests/eval_files/anyio_trio.py
 tests/eval_files/no_library.py
+tests/eval_files/noqa.py
 tests/eval_files/trio100.py
+tests/eval_files/trio100_noautofix.py
+tests/eval_files/trio100_simple_autofix.py
 tests/eval_files/trio101.py
 tests/eval_files/trio102.py
 tests/eval_files/trio102_anyio.py
 tests/eval_files/trio102_trio.py
 tests/eval_files/trio103.py
 tests/eval_files/trio103_both_imported.py
 tests/eval_files/trio103_no_104.py
@@ -71,8 +85,10 @@
 tests/eval_files/trio22x.py
 tests/eval_files/trio232.py
 tests/eval_files/trio23x.py
 tests/eval_files/trio240.py
 tests/eval_files/trio900.py
 tests/eval_files/trio910.py
 tests/eval_files/trio911.py
+tests/eval_files/trio91x_autofix.py
+tests/eval_files/trio91x_noautofix.py
 tests/eval_files/trio_anyio.py
```

### Comparing `flake8-trio-23.2.5/setup.py` & `flake8-trio-23.5.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     author="Zac Hatfield-Dodds, John Litborn, and Contributors",
     author_email="zac@zhd.dev",
     packages=find_packages(include=["flake8_trio", "flake8_trio.*"]),
     url="https://github.com/Zac-HD/flake8-trio",
     license="MIT",
     description="A highly opinionated flake8 plugin for Trio-related problems.",
     zip_safe=False,
-    install_requires=["flake8"],
+    install_requires=["flake8", "libcst"],
     python_requires=">=3.9",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Framework :: Flake8",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
@@ -46,9 +46,10 @@
         local_file("README.md").open().read()
         + "\n\n"
         + local_file("CHANGELOG.md").open().read()
     ),
     long_description_content_type="text/markdown",
     entry_points={
         "flake8.extension": ["TRI = flake8_trio:Plugin"],
+        "console_scripts": ["flake8-trio=flake8_trio:main"],
     },
 )
```

### Comparing `flake8-trio-23.2.5/tests/conftest.py` & `flake8-trio-23.5.1/tests/conftest.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,32 +6,53 @@
 
 
 def pytest_addoption(parser: pytest.Parser):
     parser.addoption(
         "--runfuzz", action="store_true", default=False, help="run fuzz tests"
     )
     parser.addoption(
-        "--enable-visitor-codes-regex",
-        default=".*",
+        "--onlyfuzz", action="store_true", default=False, help="only run fuzz tests"
+    )
+    parser.addoption(
+        "--generate-autofix",
+        action="store_true",
+        default=False,
+        help="generate autofix file content",
+    )
+    parser.addoption(
+        "--enable-codes",
+        default="TRIO",
         help="select error codes whose visitors to run.",
     )
 
 
 def pytest_configure(config: pytest.Config):
     config.addinivalue_line(
         "markers", "fuzz: mark test as a slow fuzzer to not run by default"
     )
 
 
 def pytest_collection_modifyitems(config: pytest.Config, items: list[pytest.Item]):
     if config.getoption("--runfuzz"):
         # --runfuzz given in cli: do not skip fuzz tests
         return
+
+    if config.getoption("--onlyfuzz"):
+        for item in items.copy():
+            if "fuzz" not in item.keywords:
+                items.remove(item)
+        return
+
     skip_fuzz = pytest.mark.skip(reason="need --runfuzz option to run")
     for item in items:
         if "fuzz" in item.keywords:
             item.add_marker(skip_fuzz)
 
 
 @pytest.fixture()
-def enable_visitor_codes_regex(request: pytest.FixtureRequest):
-    return request.config.getoption("--enable-visitor-codes-regex")
+def generate_autofix(request: pytest.FixtureRequest):
+    return request.config.getoption("generate_autofix")
+
+
+@pytest.fixture()
+def enable_codes(request: pytest.FixtureRequest):
+    return request.config.getoption("--enable-codes")
```

### Comparing `flake8-trio-23.2.5/tests/eval_files/trio101.py` & `flake8-trio-23.5.1/tests/eval_files/trio101.py`

 * *Files identical despite different names*

### Comparing `flake8-trio-23.2.5/tests/eval_files/trio102.py` & `flake8-trio-23.5.1/tests/eval_files/trio102.py`

 * *Files identical despite different names*

### Comparing `flake8-trio-23.2.5/tests/eval_files/trio102_anyio.py` & `flake8-trio-23.5.1/tests/eval_files/trio102_anyio.py`

 * *Files identical despite different names*

### Comparing `flake8-trio-23.2.5/tests/eval_files/trio102_trio.py` & `flake8-trio-23.5.1/tests/eval_files/trio102_trio.py`

 * *Files identical despite different names*

### Comparing `flake8-trio-23.2.5/tests/eval_files/trio103.py` & `flake8-trio-23.5.1/tests/eval_files/trio103.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# ARG --enable-visitor-codes-regex=(TRIO103)|(TRIO104)
+# ARG --enable=TRIO103,TRIO104
 
 from typing import Any
 
 
 def foo() -> Any:
     ...
 
@@ -44,33 +44,33 @@
 except BaseException:  # TRIO103_trio: 7, "BaseException"
     ...
 
 # if
 try:
     ...
 except BaseException as e:  # TRIO103_trio: 7, "BaseException"
-    if True:
+    if ...:
         raise e
-    elif True:
+    elif ...:
         ...
     else:
         raise e
 
 try:
     ...
 except BaseException:  # TRIO103_trio: 7, "BaseException"
     if True:
         raise
 
 try:
     ...
 except BaseException:  # safe
-    if True:
+    if ...:
         raise
-    elif True:
+    elif ...:
         raise
     else:
         raise
 
 # loops
 # raises inside the body are never guaranteed to run and are ignored
 try:
@@ -117,15 +117,15 @@
         raise
 
 # ensure we don't ignore previous guaranteed raise (although that's unreachable code)
 try:
     ...
 except BaseException:
     raise
-    for _ in "":
+    for _ in "": # type: ignore[unreachable]
         if ...:
             break
         raise
     else:
         raise
 
 # nested try
@@ -207,14 +207,24 @@
 
 # loop over non-empty static collection
 try:
     ...
 except BaseException as e:
     for i in [1, 2, 3]:
         raise
+try:
+    ...
+except BaseException as e:
+    for i in (1, 2, 3):
+        raise
+try:
+    ...
+except BaseException as e:
+    for i in {1, 2, 3}:
+        raise
 
 try:
     ...
 except BaseException:  # TRIO103_trio: 7, "BaseException"
     for i in [1, 2, 3]:
         ...
 
@@ -224,14 +234,68 @@
     for i in [1, 2, 3]:
         if ...:
             continue
         raise
 
 try:
     ...
+except BaseException:  # TRIO103_trio: 7, "BaseException"
+    for i in foo():
+        raise
+
+try:
+    ...
+except BaseException:
+    for i in (*(), *(1, 2),):
+        raise
+
+try:
+    ...
+except BaseException:
+    for i in {**{}, **{1: 2}}: # type: ignore[arg-type]
+        raise
+
+try:
+    ...
+except BaseException:
+    for i in range(3):
+        raise
+
+try:
+    ...
+except BaseException:
+    for i in range(27670116110564327421):
+        raise
+
+try:
+    ...
+except BaseException:  # TRIO103_trio: 7, "BaseException"
+    for i in range(foo()):
+        raise
+
+try:
+    ...
+except BaseException:  # TRIO103_trio: 7, "BaseException"
+    for i in []:
+        raise
+
+try:
+    ...
+except BaseException:  # TRIO103_trio: 7, "BaseException"
+    for i in {}:
+        raise
+
+try:
+    ...
+except BaseException:
+    for i in {1: 2}:
+        raise
+
+try:
+    ...
 except BaseException:
     while True:
         raise
 
 try:
     ...
 except BaseException:  # TRIO103_trio: 7, "BaseException"
```

### Comparing `flake8-trio-23.2.5/tests/eval_files/trio103_both_imported.py` & `flake8-trio-23.5.1/tests/eval_files/trio103_both_imported.py`

 * *Files identical despite different names*

### Comparing `flake8-trio-23.2.5/tests/eval_files/trio103_trio.py` & `flake8-trio-23.5.1/tests/eval_files/trio103_trio.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# ARG --enable-visitor-codes-regex=(TRIO103)|(TRIO104)
+# ARG --enable=TRIO103,TRIO104
 # NOANYIO
 
 from typing import Any
 
 import trio
```

### Comparing `flake8-trio-23.2.5/tests/eval_files/trio104.py` & `flake8-trio-23.5.1/tests/eval_files/trio104.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# ARG --enable-visitor-codes-regex=(TRIO103)|(TRIO104)
+# ARG --enable=TRIO103,TRIO104
 try:
     ...
 # raise different exception
 except BaseException:
     raise ValueError()  # error: 4
 
 try:
@@ -78,54 +78,57 @@
     ...
 except ValueError as e:
     try:
         ...
     except BaseException:
         raise e  # error: 8
 
-# check for avoiding re-raise by returning from function
 def foo():
     if True:  # for code coverage
         return
 
+# check for avoiding re-raise by returning from function
+def foo2():
     try:
         ...
     except BaseException:  # TRIO103_trio: 11, "BaseException"
         return  # error: 8
 
     # check that we properly iterate over all nodes in try
     try:
         ...
     except BaseException:  # TRIO103_trio: 11, "BaseException"
         try:
             return  # error: 12
         except ValueError:
             return  # error: 12
         else:
-            return  # error: 12
+            return  # type: ignore[unreachable] # error: 12
         finally:
             return  # error: 12
 
 
 # don't avoid re-raise with continue/break
-while True:
-    try:
-        ...
-    except BaseException:
-        if True:
-            continue  # error: 12
-        raise
+def foo3():
+    while True:
+        try:
+            ...
+        except BaseException:
+            if True:
+                continue  # error: 16
+            raise
 
-while True:
-    try:
-        ...
-    except BaseException:
-        if True:
-            break  # error: 12
-        raise
+def foo4():
+    while True:
+        try:
+            ...
+        except BaseException:
+            if True:
+                break  # error: 16
+            raise
 
 try:
     ...
 except BaseException:  # safe
     while True:
         break
     raise
```

### Comparing `flake8-trio-23.2.5/tests/eval_files/trio104_anyio.py` & `flake8-trio-23.5.1/tests/eval_files/trio104_anyio.py`

 * *Files identical despite different names*

### Comparing `flake8-trio-23.2.5/tests/eval_files/trio105.py` & `flake8-trio-23.5.1/tests/eval_files/trio105.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,93 +1,113 @@
 # NOANYIO
 from typing import Any
+from collections.abc import Coroutine
 
 import trio
 
 par: Any = ...
+async_funpar: Coroutine[Any, Any, Any] = ...  # type: ignore
 
 
-async def foo():
+async def myasyncfun(task_status):
+    ...
+
+
+# calls that don't return
+async def inf1() -> None:
+    await trio.serve_listeners(par, par)
+
+
+async def inf2() -> None:
+    await trio.serve_ssl_over_tcp()
+
+
+async def inf3() -> None:
+    await trio.serve_tcp()
+
+
+async def inf4() -> None:
+    await trio.sleep_forever()
+
+
+async def foo() -> None:
     # not async
     trio.run(par)
 
     # safely awaited
     await trio.aclose_forcefully(par)
     await trio.open_file(par)
     await trio.open_ssl_over_tcp_listeners(par, par)
     await trio.open_ssl_over_tcp_stream(par, par)
     await trio.open_tcp_listeners(par)
     await trio.open_tcp_stream(par, par)
     await trio.open_unix_socket(par)
     await trio.run_process(par)
-    await trio.serve_listeners(par, par)
-    await trio.serve_ssl_over_tcp()
-    await trio.serve_tcp()
-    await trio.sleep()
-    await trio.sleep_forever()
-    await trio.sleep_until()
+    await trio.sleep(5)
+    await trio.sleep_until(5)
     await trio.lowlevel.cancel_shielded_checkpoint()
     await trio.lowlevel.checkpoint()
     await trio.lowlevel.checkpoint_if_cancelled()
-    await trio.lowlevel.open_process()
-    await trio.lowlevel.permanently_detach_coroutine_object()
-    await trio.lowlevel.reattach_detached_coroutine_object()
-    await trio.lowlevel.temporarily_detach_coroutine_object()
-    await trio.lowlevel.wait_readable()
-    await trio.lowlevel.wait_task_rescheduled()
-    await trio.lowlevel.wait_writable()
+    await trio.lowlevel.open_process(par)
+    await trio.lowlevel.permanently_detach_coroutine_object(par)
+    await trio.lowlevel.reattach_detached_coroutine_object(par, par)
+    await trio.lowlevel.temporarily_detach_coroutine_object(par)
+    await trio.lowlevel.wait_readable(par)
+    await trio.lowlevel.wait_task_rescheduled(par)
+    await trio.lowlevel.wait_writable(par)
 
     # all async functions
-    trio.aclose_forcefully()  # error: 4, "trio.aclose_forcefully", "function"
-    trio.open_file()  # error: 4, "trio.open_file", "function"
-    trio.open_ssl_over_tcp_listeners()  # error: 4, "trio.open_ssl_over_tcp_listeners", "function"
-    trio.open_ssl_over_tcp_stream()  # error: 4, "trio.open_ssl_over_tcp_stream", "function"
-    trio.open_tcp_listeners()  # error: 4, "trio.open_tcp_listeners", "function"
-    trio.open_tcp_stream()  # error: 4, "trio.open_tcp_stream", "function"
-    trio.open_unix_socket()  # error: 4, "trio.open_unix_socket", "function"
-    trio.run_process()  # error: 4, "trio.run_process", "function"
-    trio.serve_listeners()  # error: 4, "trio.serve_listeners", "function"
-    trio.serve_ssl_over_tcp()  # error: 4, "trio.serve_ssl_over_tcp", "function"
-    trio.serve_tcp()  # error: 4, "trio.serve_tcp", "function"
-    trio.sleep()  # error: 4, "trio.sleep", "function"
+    # fmt: off
+    trio.aclose_forcefully(par)  # error: 4, "trio.aclose_forcefully", "function"
+    trio.open_file(par)  # error: 4, "trio.open_file", "function"
+    trio.open_ssl_over_tcp_listeners(par, par)  # error: 4, "trio.open_ssl_over_tcp_listeners", "function"
+    trio.open_ssl_over_tcp_stream(par, par)  # error: 4, "trio.open_ssl_over_tcp_stream", "function"
+    trio.open_tcp_listeners(par)  # error: 4, "trio.open_tcp_listeners", "function"
+    trio.open_tcp_stream(par, par)  # error: 4, "trio.open_tcp_stream", "function"
+    trio.open_unix_socket(par)  # error: 4, "trio.open_unix_socket", "function"
+    trio.run_process(par)  # error: 4, "trio.run_process", "function"
+    trio.serve_listeners(par, par)  # error: 4, "trio.serve_listeners", "function"
+    trio.serve_ssl_over_tcp(par, par, par)  # error: 4, "trio.serve_ssl_over_tcp", "function"
+    trio.serve_tcp(par, par)  # error: 4, "trio.serve_tcp", "function"
+    trio.sleep(par)  # error: 4, "trio.sleep", "function"
     trio.sleep_forever()  # error: 4, "trio.sleep_forever", "function"
-    trio.sleep_until()  # error: 4, "trio.sleep_until", "function"
+    trio.sleep_until(par)  # error: 4, "trio.sleep_until", "function"
 
     # long lines, wheee
     trio.lowlevel.cancel_shielded_checkpoint()  # error: 4, "trio.lowlevel.cancel_shielded_checkpoint", "function"
     trio.lowlevel.checkpoint()  # error: 4, "trio.lowlevel.checkpoint", "function"
     trio.lowlevel.checkpoint_if_cancelled()  # error: 4, "trio.lowlevel.checkpoint_if_cancelled", "function"
     trio.lowlevel.open_process()  # error: 4, "trio.lowlevel.open_process", "function"
-    trio.lowlevel.permanently_detach_coroutine_object()  # error: 4, "trio.lowlevel.permanently_detach_coroutine_object", "function"
-    trio.lowlevel.reattach_detached_coroutine_object()  # error: 4, "trio.lowlevel.reattach_detached_coroutine_object", "function"
-    trio.lowlevel.temporarily_detach_coroutine_object()  # error: 4, "trio.lowlevel.temporarily_detach_coroutine_object", "function"
-    trio.lowlevel.wait_readable()  # error: 4, "trio.lowlevel.wait_readable", "function"
-    trio.lowlevel.wait_task_rescheduled()  # error: 4, "trio.lowlevel.wait_task_rescheduled", "function"
-    trio.lowlevel.wait_writable()  # error: 4, "trio.lowlevel.wait_writable", "function"
-
+    trio.lowlevel.permanently_detach_coroutine_object(par)  # error: 4, "trio.lowlevel.permanently_detach_coroutine_object", "function"
+    trio.lowlevel.reattach_detached_coroutine_object(par, par)  # error: 4, "trio.lowlevel.reattach_detached_coroutine_object", "function"
+    trio.lowlevel.temporarily_detach_coroutine_object(par)  # error: 4, "trio.lowlevel.temporarily_detach_coroutine_object", "function"
+    trio.lowlevel.wait_readable(par)  # error: 4, "trio.lowlevel.wait_readable", "function"
+    trio.lowlevel.wait_task_rescheduled(par)  # error: 4, "trio.lowlevel.wait_task_rescheduled", "function"
+    trio.lowlevel.wait_writable(par)  # error: 4, "trio.lowlevel.wait_writable", "function"
+    # fmt: on
     # safe
-    async with await trio.open_file() as f:
+    async with await trio.open_file(par) as f:
         pass
 
-    async with trio.open_file() as f:  # error: 15, "trio.open_file", "function"
+    async with trio.open_file(par) as f:  # error: 15, "trio.open_file", "function"
         pass
 
     # safe in theory, but deemed sufficiently poor style that parsing
     # it isn't supported
-    k = trio.open_file()  # error: 8, "trio.open_file", "function"
+    k = trio.open_file(par)  # error: 8, "trio.open_file", "function"
     await k
 
     # issue #56
-    nursery = trio.open_nursery()
-    await nursery.start()
-    await nursery.start_foo()
-
-    nursery.start()  # error: 4, "trio.Nursery.start", "method"
-    None.start()  # type: ignore
-    nursery.start_soon()
-    nursery.start_foo()
+    async with trio.open_nursery() as nursery:
+        await nursery.start(myasyncfun)
+        await nursery.start_foo()
+
+        nursery.start(myasyncfun)  # error: 8, "trio.Nursery.start", "method"
+        None.start()  # type: ignore
+        nursery.start_soon(par)
+        nursery.start_foo()
 
-    with trio.open_nursery() as booboo:
-        booboo.start()  # error: 8, "trio.Nursery.start", "method"
+        async with trio.open_nursery() as booboo:
+            booboo.start(myasyncfun)  # error: 12, "trio.Nursery.start", "method"
 
-    barbar: trio.Nursery = ...
-    barbar.start()  # error: 4, "trio.Nursery.start", "method"
+        barbar: trio.Nursery = ...
+        barbar.start(myasyncfun)  # error: 8, "trio.Nursery.start", "method"
```

### Comparing `flake8-trio-23.2.5/tests/eval_files/trio106.py` & `flake8-trio-23.5.1/tests/eval_files/trio106.py`

 * *Files identical despite different names*

### Comparing `flake8-trio-23.2.5/tests/eval_files/trio109.py` & `flake8-trio-23.5.1/tests/eval_files/trio109.py`

 * *Files identical despite different names*

### Comparing `flake8-trio-23.2.5/tests/eval_files/trio110.py` & `flake8-trio-23.5.1/tests/eval_files/trio110.py`

 * *Files identical despite different names*

### Comparing `flake8-trio-23.2.5/tests/eval_files/trio111.py` & `flake8-trio-23.5.1/tests/eval_files/trio111.py`

 * *Files identical despite different names*

### Comparing `flake8-trio-23.2.5/tests/eval_files/trio112.py` & `flake8-trio-23.5.1/tests/eval_files/trio112.py`

 * *Files identical despite different names*

### Comparing `flake8-trio-23.2.5/tests/eval_files/trio113.py` & `flake8-trio-23.5.1/tests/eval_files/trio113.py`

 * *Files identical despite different names*

### Comparing `flake8-trio-23.2.5/tests/eval_files/trio113_trio.py` & `flake8-trio-23.5.1/tests/eval_files/trio113_trio.py`

 * *Files identical despite different names*

### Comparing `flake8-trio-23.2.5/tests/eval_files/trio114.py` & `flake8-trio-23.5.1/tests/eval_files/trio114.py`

 * *Files identical despite different names*

### Comparing `flake8-trio-23.2.5/tests/eval_files/trio115.py` & `flake8-trio-23.5.1/tests/eval_files/trio115.py`

 * *Files identical despite different names*

### Comparing `flake8-trio-23.2.5/tests/eval_files/trio116.py` & `flake8-trio-23.5.1/tests/eval_files/trio116.py`

 * *Files identical despite different names*

### Comparing `flake8-trio-23.2.5/tests/eval_files/trio117.py` & `flake8-trio-23.5.1/tests/eval_files/trio117.py`

 * *Files identical despite different names*

### Comparing `flake8-trio-23.2.5/tests/eval_files/trio118.py` & `flake8-trio-23.5.1/tests/eval_files/trio118.py`

 * *Files identical despite different names*

### Comparing `flake8-trio-23.2.5/tests/eval_files/trio200.py` & `flake8-trio-23.5.1/tests/eval_files/trio200.py`

 * *Files identical despite different names*

### Comparing `flake8-trio-23.2.5/tests/eval_files/trio210.py` & `flake8-trio-23.5.1/tests/eval_files/trio210.py`

 * *Files identical despite different names*

### Comparing `flake8-trio-23.2.5/tests/eval_files/trio211.py` & `flake8-trio-23.5.1/tests/eval_files/trio211.py`

 * *Files identical despite different names*

### Comparing `flake8-trio-23.2.5/tests/eval_files/trio212.py` & `flake8-trio-23.5.1/tests/eval_files/trio212.py`

 * *Files identical despite different names*

### Comparing `flake8-trio-23.2.5/tests/eval_files/trio22x.py` & `flake8-trio-23.5.1/tests/eval_files/trio22x.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # type: ignore
-# ARG --enable-visitor-codes-regex=(TRIO220|TRIO221|TRIO222)
+# ARG --enable=TRIO220,TRIO221,TRIO222
 
 
 async def foo():
     subprocess.Popen()  # TRIO220: 4, 'subprocess.Popen', "trio"
     os.system()  # TRIO221: 4, 'os.system', "trio"
 
     system()
```

### Comparing `flake8-trio-23.2.5/tests/eval_files/trio232.py` & `flake8-trio-23.5.1/tests/eval_files/trio232.py`

 * *Files identical despite different names*

### Comparing `flake8-trio-23.2.5/tests/eval_files/trio23x.py` & `flake8-trio-23.5.1/tests/eval_files/trio23x.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # type: ignore
-# ARG --enable-visitor-codes-regex=(TRIO230)|(TRIO231)
+# ARG --enable=TRIO230,TRIO231
 import io
 import os
 
 import trio
 
 
 async def foo():
```

### Comparing `flake8-trio-23.2.5/tests/eval_files/trio240.py` & `flake8-trio-23.5.1/tests/eval_files/trio240.py`

 * *Files identical despite different names*

### Comparing `flake8-trio-23.2.5/tests/eval_files/trio900.py` & `flake8-trio-23.5.1/tests/eval_files/trio900.py`

 * *Files identical despite different names*

### Comparing `flake8-trio-23.2.5/tests/eval_files/trio910.py` & `flake8-trio-23.5.1/tests/eval_files/trio910.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,30 @@
-# type: ignore
+# AUTOFIX
+# mypy: disable-error-code="unreachable"
 import typing
 from typing import Any, overload
 
+import pytest
 import trio
 
 _ = ""
 
+custom_disabled_decorator: Any = ...
 
-def __() -> Any:
+
+async def foo() -> Any:
+    await foo()
+
+
+def bar() -> Any:
     ...
 
 
-# ARG --enable-visitor-codes-regex=(TRIO910)|(TRIO911)
+# ARG --enable=TRIO910,TRIO911
+# ARG --no-checkpoint-warning-decorator=custom_disabled_decorator
 
 
 # function whose body solely consists of pass, ellipsis, or string constants is safe
 async def foo_empty_1():
     ...
 
 
@@ -30,20 +39,16 @@
 async def foo_empty_4():
     ...
     """comment"""
     ...
     """comment2"""
 
 
-async def foo() -> Any:
-    await foo()
-
-
 async def foo1():  # error: 0, "exit", Statement("function definition", lineno)
-    __()
+    bar()
 
 
 # If
 async def foo_if_1():  # error: 0, "exit", Statement("function definition", lineno)
     if _:
         await foo()
 
@@ -79,31 +84,35 @@
 
 
 # nested function definition
 async def foo_func_1():
     await foo()
 
     async def foo_func_2():  # error: 4, "exit", Statement("function definition", lineno)
-        __()
+        bar()
 
 
+# we don't get a newline after the nested function definition before the checkpoint
+# when autofixing
+# fmt: off
 async def foo_func_3():  # error: 0, "exit", Statement("function definition", lineno)
     async def foo_func_4():
         await foo()
 
 
 async def foo_func_5():  # error: 0, "exit", Statement("function definition", lineno)
     def foo_func_6():  # safe
         async def foo_func_7():  # error: 8, "exit", Statement("function definition", lineno)
-            __()
+            bar()
 
 
 async def foo_func_8():  # error: 0, "exit", Statement("function definition", lineno)
     def foo_func_9():
         raise
+# fmt: on
 
 
 # normal function
 def foo_normal_func_1():
     return
 
 
@@ -172,96 +181,101 @@
 
 async def foo_while_3():  # safe
     await foo()
     while _:
         ...
 
 
+async def foo_while_4():  # error: 0, "exit", Statement("function definition", lineno)
+    while False:
+        await foo()
+
+
 # for
 async def foo_for_1():  # error: 0, "exit", Statement("function definition", lineno)
     for _ in "":
         await foo()
 
 
 async def foo_for_2():  # now safe
     for _ in "":
         await foo()
     else:
         await foo()
 
 
 async def foo_while_break_1():  # safe
-    while foo():
+    while bar():
         await foo()
         break
     else:
         await foo()
 
 
 async def foo_while_break_2():  # error: 0, "exit", Statement("function definition", lineno)
-    while foo():
+    while bar():
         break
     else:
         await foo()
 
 
 async def foo_while_break_3():  # error: 0, "exit", Statement("function definition", lineno)
-    while foo():
+    while bar():
         await foo()
         break
     else:
         ...
 
 
 async def foo_while_break_4():  # error: 0, "exit", Statement("function definition", lineno)
-    while foo():
+    while bar():
         break
     else:
         ...
 
 
 async def foo_while_continue_1():  # safe
-    while foo():
+    while bar():
         await foo()
         continue
     else:
         await foo()
 
 
 async def foo_while_continue_2():  # safe
-    while foo():
+    while bar():
         continue
     else:
         await foo()
 
 
 async def foo_while_continue_3():  # error: 0, "exit", Statement("function definition", lineno)
-    while foo():
+    while bar():
         await foo()
         continue
     else:
         ...
 
 
 async def foo_while_continue_4():  # error: 0, "exit", Statement("function definition", lineno)
-    while foo():
+    while bar():
         continue
     else:
         ...
 
 
 async def foo_async_for_1():
-    async for _ in trio.trick_pyright:
+    async for _ in bar():
         ...
 
 
 # async with
 # async with guarantees checkpoint on at least one of entry or exit
 async def foo_async_with():
-    async with trio.trick_pyright:
+    async with bar():
         ...
 
 
 # raise
 async def foo_raise_1():  # safe
     raise ValueError()
 
@@ -271,15 +285,15 @@
         await foo()
     else:
         raise ValueError()
 
 
 # try
 # safe only if (try or else) and all except bodies either await or raise
-# if foo() raises a ValueError it's not checkpointed
+# if `foo()` raises a ValueError it's not checkpointed
 async def foo_try_1():  # error: 0, "exit", Statement("function definition", lineno)
     try:
         await foo()
     except ValueError:
         ...
     except:
         raise
@@ -448,27 +462,27 @@
 async def foo_range_4():  # error: 0, "exit", Statement("function definition", lineno)
     for i in range(10, 5):
         await foo()
 
 
 # error on complex parameters
 async def foo_range_5():  # error: 0, "exit", Statement("function definition", lineno)
-    for i in range(2 - 2):
+    for i in range(3 - 2):
         await foo()
 
 
 # https://github.com/Zac-HD/flake8-trio/issues/47
 async def f():
     while True:
         if ...:
             await trio.sleep(0)
             return
         # If you delete this loop, no warning.
-        while foo():
-            await __()
+        while bar():
+            await foo()
 
 
 async def f1():
     while True:
         if ...:
             await trio.sleep(0)
             return
@@ -492,29 +506,67 @@
     while True:
         if ...:
             continue
         if ...:
             break
 
     # boolop in sync function
-    True and True
+    True and True  # type: ignore
 
 
 # don't warn on pytest.fixture
 @pytest.fixture
 async def foo_test():
     print("...")
 
 
 @pytest.fixture()
 async def foo_test2():
     print("...")
 
 
+@custom_disabled_decorator
+async def foo_ARG_test():
+    print("...")
+
+
+@custom_disabled_decorator()
+async def foo_ARG_test2():
+    print("...")
+
+
 @pytest.fixture
 async def foo_test_return():
     return
 
 
 @pytest.fixture()
 async def foo_test_return2():
     return
+
+
+async def foo_comprehension_1():
+    [... for x in range(10) if await foo()]
+
+
+# should error
+async def foo_comprehension_2():  # error: 0, "exit", Statement("function definition", lineno)
+    [await foo() for x in range(10) if bar()]
+
+
+async def foo_comprehension_3():
+    [... async for x in bar()]
+
+
+# Issue #714
+# (await x async for y in await z)
+#  ^       ^              ^ this always runs!
+#  ^       ^ this might not run
+#  ^ this might not run
+
+
+async def await_in_gen_target():
+    (print(x) for x in await foo())
+
+
+async def await_everywhere_except_gen_target():  # error: 0, "exit", Statement("function definition", lineno)
+    (await x async for x in bar())
```

### Comparing `flake8-trio-23.2.5/tests/eval_files/trio911.py` & `flake8-trio-23.5.1/tests/eval_files/trio911.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,26 @@
-# type: ignore
+# AUTOFIX
 from typing import Any
 
+import pytest
 import trio
 
 _: Any = ""
 
-# ARG --enable-visitor-codes-regex=(TRIO910)|(TRIO911)
+# ARG --enable=TRIO910,TRIO911
 
 
 async def foo() -> Any:
     await foo()
 
 
+def bar(*args) -> Any:
+    ...
+
+
 async def foo_yield_1():
     await foo()
     yield 5
     await foo()
 
 
 async def foo_yield_2():
@@ -56,33 +61,23 @@
 # async with
 # checkpoint on both entry and exit
 async def foo_async_with():
     async with trio.fail_after(5):
         yield
 
 
-# fmt: off
-async def foo_async_with_2():
-    # with'd expression evaluated before checkpoint
-    async with (yield):  # error: 16, "yield", Statement("function definition", lineno-2)
-        yield
-# fmt: on
-
-
 async def foo_async_with_3():
     async with trio.fail_after(5):
         yield
         yield  # error: 8, "yield", Statement("yield", lineno-1)
 
 
 # async for
-async def foo_async_for():  # error: 0, "exit", Statement("yield", lineno+6)
-    async for i in (
-        yield  # error: 8, "yield", Statement("function definition", lineno-2)
-    ):
+async def foo_async_for():  # error: 0, "exit", Statement("yield", lineno+4)
+    async for i in bar():
         yield  # safe
     else:
         yield  # safe
 
 
 # await anext(iter) is not called on break
 async def foo_async_for_2():  # error: 0, "exit", Statement("yield", lineno+2)
@@ -151,22 +146,33 @@
         yield  # error: 8, "yield", Statement("yield", lineno) # error: 8, "yield", Statement("yield", lineno+2) # error: 8, "yield", Statement("yield", lineno+4)
         while foo():
             yield  # error: 12, "yield", Statement("yield", lineno)# error: 12, "yield", Statement("yield", lineno-2)# error: 12, "yield", Statement("yield", lineno+2)
             while foo():
                 yield  # error: 16, "yield", Statement("yield", lineno-2)# error: 16, "yield", Statement("yield", lineno)
 
 
+# check that state management is handled in for loops as well
+async def foo_while_4_for():  # error: 0, "exit", Statement("yield", lineno+3) # error: 0, "exit", Statement("yield", lineno+5) # error: 0, "exit", Statement("yield", lineno+7)
+    await foo()
+    for i in bar():
+        yield  # error: 8, "yield", Statement("yield", lineno) # error: 8, "yield", Statement("yield", lineno+2) # error: 8, "yield", Statement("yield", lineno+4)
+        for i in bar():
+            yield  # error: 12, "yield", Statement("yield", lineno)# error: 12, "yield", Statement("yield", lineno-2)# error: 12, "yield", Statement("yield", lineno+2)
+            for i in bar():
+                yield  # error: 16, "yield", Statement("yield", lineno-2)# error: 16, "yield", Statement("yield", lineno)
+
+
 # check error suppression is reset
 async def foo_while_5():
     await foo()
     while foo():
         yield  # error: 8, "yield", Statement("yield", lineno)
 
-        async def foo_nested_error():  # error: 8, "exit", Statement("yield", lineno+1)# error: 8, "exit", Statement("yield", lineno+1)
-            yield  # error: 12, "yield", Statement("function definition", lineno-1)# error: 12, "yield", Statement("function definition", lineno-1)
+        async def foo_nested_error():  # error: 8, "exit", Statement("yield", lineno+1)
+            yield  # error: 12, "yield", Statement("function definition", lineno-1)
 
     await foo()
 
 
 # --- while + continue ---
 # no checkpoint on continue
 async def foo_while_continue_1():  # error: 0, "exit", Statement("yield", lineno+3)
@@ -284,14 +290,30 @@
 
 async def foo_while_endless_2():  # error: 0, "exit", Statement("function definition", lineno)# error: 0, "exit", Statement("yield", lineno+3)
     while foo():
         await foo()
         yield
 
 
+async def foo_while_endless_3():
+    while True:
+        ...
+    yield  # type: ignore[unreachable]
+    await foo()
+
+
+async def foo_while_endless_4():
+    await foo()
+    while True:
+        yield
+        while True:
+            await foo()
+            yield
+
+
 # try
 async def foo_try_1():  # error: 0, "exit", Statement("function definition", lineno) # error: 0, "exit", Statement("yield", lineno+2)
     try:
         yield  # error: 8, "yield", Statement("function definition", lineno-2)
     except:
         pass
 
@@ -562,14 +584,17 @@
 async def foo_func_1():
     await foo()
 
     async def foo_func_2():  # error: 4, "exit", Statement("yield", lineno+1)
         yield  # error: 8, "yield", Statement("function definition", lineno-1)
 
 
+# autofix doesn't insert newline after nested function def and before checkpoint
+# so we need to disable black
+# fmt: off
 async def foo_func_3():  # error: 0, "exit", Statement("yield", lineno+2)
     await foo()
     yield
 
     async def foo_func_4():
         await foo()
 
@@ -580,37 +605,22 @@
 
     def foo_func_6():  # safe
         yield
 
         async def foo_func_7():
             await foo()
             ...
+# fmt: on
 
 
 # No error from function definition, but may shortcut after yield
 async def foo_boolops_1():  # error: 0, "exit", Stmt("yield", line+1)
     _ = await foo() and (yield) and await foo()
 
 
-# may shortcut after any of the yields
-async def foo_boolops_2():  # error: 0, "exit", Stmt("yield", line+1) # error: 0, "exit", Stmt("yield", line+1)
-    _ = await foo() and (yield) and await foo() and (yield)
-
-
-# fmt: off
-async def foo_boolops_3():  # error: 0, "exit", Stmt("yield", line+1) # error: 0, "exit", Stmt("yield", line+4) # error: 0, "exit", Stmt("yield", line+5)
-    _ = (await foo() or (yield) or await foo()) or (
-        ...
-        or (
-            (yield)  # error: 13, "yield", Stmt("yield", line-3)
-            and (yield))  # error: 17, "yield", Stmt("yield", line-1)
-    )
-# fmt: on
-
-
 # loop over non-empty static collection
 async def foo_loop_static():
     # break/else behaviour on guaranteed body execution
     for _ in [1, 2, 3]:
         await foo()
     else:
         yield
@@ -717,15 +727,15 @@
         await foo()
     yield
 
     for _ in (*range(0), *[1, 2, 3]):
         await foo()
     yield
 
-    for _ in {**{}, **{1: 2}}:
+    for _ in {**{}, **{1: 2}}:  # type: ignore[arg-type]
         await foo()
     yield
 
     x: Any = ...
     for _ in (*x, *[1, 2, 3]):
         await foo()
     yield
@@ -738,14 +748,18 @@
         await foo()
     yield  # error: 4, "yield", Stmt("yield", line-4)
 
     for _ in "":
         await foo()
     yield  # error: 4, "yield", Stmt("yield", line-4)
 
+    for _ in """""":
+        await foo()
+    yield  # error: 4, "yield", Stmt("yield", line-4)
+
     for _ in [[], []][0]:
         await foo()
     yield  # error: 4, "yield", Stmt("yield", line-4)
 
     for _ in [[], []].__getitem__(0):
         await foo()
     yield  # error: 4, "yield", Stmt("yield", line-4)
@@ -776,29 +790,197 @@
         if ...:
             continue
         await foo()
         if ...:
             break
     yield
 
+    while False:
+        await foo()  # type: ignore[unreachable]
+    yield  # error: 4, "yield", Stmt("yield", line-4)
+
+    while "hello":
+        await foo()
+    yield
+
+    # false positive on containers
+    while [1, 2]:
+        await foo()
+    yield  # error: 4, "yield", Stmt("yield", line-5)
+
     # will get caught by any number of linters, but trio911 will also complain
     for _ in 5:  # type: ignore
         await foo()
     yield  # error: 4, "yield", Stmt("yield", line-5)
 
     # range with constant arguments also handled, see more extensive tests in 910
     for i in range(5):
         await foo()
     yield
 
+    for i in range(0x23):
+        await foo()
+    yield
+
+    for i in range(0b01):
+        await foo()
+    yield
+
+    for i in range(1 + 1):  # not handled
+        await foo()
+    yield  # error: 4, "yield", Stmt("yield", line-4)
+
+    for i in range(None):  # type: ignore
+        await foo()
+    yield  # error: 4, "yield", Stmt("yield", line-4)
+
+    for i in range(+3):
+        await foo()
+    yield
+
+    for i in range(-3.5):  # type: ignore
+        await foo()
+    yield  # error: 4, "yield", Stmt("yield", line-4)
+
+    # duplicated from 910 to have all range tests in one place
+    for i in range(5, 10):
+        await foo()
+    yield
+
+    for i in range(10, 5, -1):
+        await foo()
+    yield
+
+    # ~0 == -1
+    for i in range(10, 5, ~0):
+        await foo()
+    yield
+
+    # length > sys.maxsize
+    for i in range(27670116110564327421):
+        await foo()
+    yield
+
+    for i in range(10, 5):
+        await foo()
+    yield  # error: 4, "yield", Stmt("yield", line-4)
+
+    # binary operations are not handled
+    for i in range(3 - 2):
+        await foo()
+    yield  # error: 4, "yield", Stmt("yield", line-5)
+
+    for i in range(10**3):
+        await foo()
+    yield  # error: 4, "yield", Stmt("yield", line-4)
+
+    # nor nested unary operations
+    for i in range(--3):
+        await foo()
+    yield  # error: 4, "yield", Stmt("yield", line-5)
+
     await foo()
 
 
 # don't warn on pytest.fixture
 @pytest.fixture
 async def foo_test():
     yield
 
 
 @pytest.fixture()
 async def foo_test2():
     yield
+
+
+async def comprehensions():
+    # guaranteed iteration with await in test
+    [... for x in range(10) if await foo()]
+    yield  # safe
+
+    # guaranteed iteration and await in value, but test is not guaranteed
+    [await foo() for x in range(10) if bar()]
+    yield  # error: 4, "yield", Stmt("yield", line-4)
+
+    # guaranteed iteration and await in value
+    [await foo() for x in range(10)]
+    yield  # safe
+
+    # not guaranteed to iter
+    [await foo() for x in bar()]
+    yield  # error: 4, "yield", Stmt("yield", line-4)
+
+    # await statement in loop expression
+    [... for x in bar(await foo())]
+    yield
+
+    # set comprehensions use same logic as list
+    {await foo() for x in range(10)}
+    yield  # safe
+
+    {await foo() for x in bar()}
+    yield  # error: 4, "yield", Stmt("yield", line-3)
+
+    # dict comprehensions use same logic as list
+    {await foo(): 5 for x in bar()}
+    yield  # error: 4, "yield", Stmt("yield", line-4)
+
+    # other than `await` can be in both key&val
+    {await foo(): 5 for x in range(10)}
+    yield
+
+    {5: await foo() for x in range(10)}
+    yield
+
+    # generator expressions are never treated as safe
+    (await foo() for x in range(10))
+    yield  # error: 4, "yield", Stmt("yield", line-4)
+
+    (await foo() for x in bar() if await foo())
+    yield  # error: 4, "yield", Stmt("yield", line-3)
+
+    # async for always safe
+    [... async for x in bar()]
+    yield  # safe
+    {... async for x in bar()}
+    yield  # safe
+    {...: ... async for x in bar()}
+    yield  # safe
+
+    # other than in generator expression
+    (... async for x in bar())
+    yield  # error: 4, "yield", Stmt("yield", line-4)
+
+    # multiple loops
+    [... for x in range(10) for y in range(10) if await foo()]
+    yield
+    [... for x in range(10) for y in bar() if await foo()]
+    yield  # error: 4, "yield", Stmt("yield", line-2)
+    [... for x in bar() for y in range(10) if await foo()]
+    yield  # error: 4, "yield", Stmt("yield", line-2)
+
+    [await foo() for x in range(10) for y in range(10)]
+    yield
+    [await foo() for x in range(10) for y in bar()]
+    yield  # error: 4, "yield", Stmt("yield", line-2)
+    [await foo() for x in bar() for y in range(10)]
+    yield  # error: 4, "yield", Stmt("yield", line-2)
+
+    # trip loops!
+    [... for x in range(10) for y in range(10) async for z in bar()]
+    yield
+    [... for x in range(10) for y in range(10) for z in range(10)]
+    yield  # error: 4, "yield", Stmt("yield", line-2)
+
+    # multiple ifs
+    [... for x in range(10) for y in range(10) if await foo() if await foo()]
+    yield
+
+    [... for x in range(10) for y in bar() if await foo() if await foo()]
+    yield  # error: 4, "yield", Stmt("yield", line-3)
+
+    # nested comprehensions
+    [[await foo() for x in range(10)] for y in range(10)]
+    yield
+
+    # code coverage: inner comprehension with no checkpointed statements
+    [... for x in [await foo()] for y in x]
```

### Comparing `flake8-trio-23.2.5/tests/test_all_visitors_imported.py` & `flake8-trio-23.5.1/tests/test_all_visitors_imported.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,12 +12,21 @@
 
 def test_all_visitors_imported():
     visitor_dir = Path(__file__).parent.parent / "flake8_trio" / "visitors"
     visitor_files = {
         f.stem for f in visitor_dir.iterdir() if f.stem.startswith("visitor")
     }
     visited_files: set[str] = set()
+    in_import: bool | None = None
     with open(visitor_dir / "__init__.py") as f:
         for line in f:
-            if m := re.match(r"from \. import (?P<module>\w*)", line):
+            if m := re.fullmatch(r"from \. import \(\n", line):
+                in_import = True
+            elif in_import and (m := re.fullmatch(r" *(?P<module>\w*),\n", line)):
                 visited_files.add(m.group("module"))
+            elif in_import and re.fullmatch(r"\)\n", line):
+                in_import = False
+
+    # check that parsing succeeded
+    assert in_import is False
+
     assert visitor_files == visited_files
```

### Comparing `flake8-trio-23.2.5/tests/test_decorator.py` & `flake8-trio-23.5.1/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `flake8-trio-23.2.5/tests/test_flake8_trio.py` & `flake8-trio-23.5.1/tests/test_flake8_trio.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,172 +1,321 @@
 """Main test file for the plugin."""
 
 from __future__ import annotations
 
 import ast
 import copy
+import difflib
 import itertools
 import os
 import re
 import site
-import subprocess  # noqa: S404
 import sys
 import tokenize
 import unittest
+from argparse import ArgumentParser
 from collections import deque
+from dataclasses import dataclass, fields
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, DefaultDict
 
+import libcst as cst
 import pytest
-from flake8 import __version_info__ as flake8_version_info
-from flake8.options.manager import OptionManager
 from hypothesis import HealthCheck, given, settings
 from hypothesmith import from_grammar, from_node
 
 from flake8_trio import Plugin
 from flake8_trio.base import Error, Statement
-from flake8_trio.visitors import ERROR_CLASSES
+from flake8_trio.visitors import ERROR_CLASSES, ERROR_CLASSES_CST
 
 if TYPE_CHECKING:
     from collections.abc import Iterable, Sequence
 
+    from flake8_trio.visitors.flake8triovisitor import Flake8TrioVisitor
+
+AUTOFIX_DIR = Path(__file__).parent / "autofix_files"
 
 test_files: list[tuple[str, Path]] = sorted(
     (f.stem.upper(), f) for f in (Path(__file__).parent / "eval_files").iterdir()
 )
+autofix_files: dict[str, Path] = {
+    f.stem.upper(): f for f in AUTOFIX_DIR.iterdir() if f.suffix == ".py"
+}
+# check that there's an eval file for each autofix file
+assert set(autofix_files.keys()) - {f[0] for f in test_files} == set()
 
 
 class ParseError(Exception):
     ...
 
 
-# flake8 6 added a required named parameter formatter_names
-def _default_option_manager():
-    kwargs = {}
-    if flake8_version_info[0] >= 6:
-        kwargs["formatter_names"] = ["default"]
-    return OptionManager(version="", plugin_versions="", parents=[], **kwargs)
-
-
 # check for presence of _pyXX, skip if version is later, and prune parameter
 def check_version(test: str):
     python_version = re.search(r"(?<=_PY)\d*", test)
     if python_version:
         version_str = python_version.group()
         major, minor = version_str[0], version_str[1:]
         v_i = sys.version_info
         if (v_i.major, v_i.minor) < (int(major), int(minor)):
             pytest.skip(f"python version {v_i} smaller than {major}, {minor}")
 
 
-ERROR_CODES = {
-    err_code: err_class
-    for err_class in ERROR_CLASSES
-    for err_code in err_class.error_codes.keys()
+# mypy does not see that both types have error_codes
+ERROR_CODES: dict[str, Flake8TrioVisitor] = {
+    err_code: err_class  # type: ignore[misc]
+    for err_class in (*ERROR_CLASSES, *ERROR_CLASSES_CST)
+    for err_code in err_class.error_codes.keys()  # type: ignore[attr-defined]
 }
 
 
-@pytest.mark.parametrize(("test", "path"), test_files)
-def test_eval(test: str, path: Path):
-    content = path.read_text()
-    if "# NOTRIO" in content:
-        pytest.skip("file marked with NOTRIO")
+def format_difflib_line(s: str) -> str:
+    # replace line markers with x's, to not generate massive diffs when lines get moved
+    s = re.sub(r"(?<= )[+-]\d*(?=,)", "x", s)
+
+    # difflib generates lots of lines with one trailing space, which is an eyesore
+    # and trips up pre-commit, git diffs, etc. If there actually was diff trailing
+    # space in the content it's picked up elsewhere and by pre-commit.
+    if s[-2:] == " \n":
+        return s[:-2] + "\n"
+    return s
+
+
+def diff_strings(first: str, second: str, /) -> str:
+    return "".join(
+        map(
+            format_difflib_line,
+            difflib.unified_diff(
+                first.splitlines(keepends=True),
+                second.splitlines(keepends=True),
+            ),
+        )
+    )
 
-    expected, parsed_args = _parse_eval_file(test, content)
-    if "# TRIO_NO_ERROR" in content:
-        expected = []
 
-    plugin = Plugin(ast.parse(content))
-    _ = assert_expected_errors(plugin, *expected, args=parsed_args)
+# replaces all instances of `original` with `new` in string
+# unless it's preceded by a `-`, which indicates it's part of a command-line flag
+def replace_library(string: str, original: str = "trio", new: str = "anyio") -> str:
+    return re.sub(rf"(?<!-){original}", new, string)
 
 
-@pytest.mark.parametrize(("test", "path"), test_files)
-def test_eval_anyio(test: str, path: Path):
-    # read content, replace instances of trio with anyio, and write to tmp_file
-    content = path.read_text()
+def check_autofix(
+    test: str,
+    plugin: Plugin,
+    unfixed_code: str,
+    generate_autofix: bool,
+    anyio: bool = False,
+):
+    # the source code after it's been visited by current transformers
+    visited_code = plugin.module.code
+
+    if "# AUTOFIX" not in unfixed_code:
+        # if the file is specifically marked with NOAUTOFIX, that means it has visitors
+        # that will autofix with --autofix, but the file explicitly doesn't want to check
+        # the result of doing that. THIS IS DANGEROUS
+        if "# NOAUTOFIX" in unfixed_code:
+            print(f"eval file {test} marked with dangerous marker NOAUTOFIX")
+        else:
+            assert unfixed_code == visited_code
+        return
 
-    if "# NOANYIO" in content:
+    # the full generated source code, saved from a previous run
+    if test not in autofix_files:
+        autofix_files[test] = AUTOFIX_DIR / (test.lower() + ".py")
+        autofix_files[test].write_text("")
+    previous_autofixed = autofix_files[test].read_text()
+
+    # file contains a previous diff showing what's added/removed by the autofixer
+    # i.e. a diff between "eval_files/{test}.py" and "autofix_files/{test}.py"
+    autofix_diff_file = AUTOFIX_DIR / f"{test.lower()}.py.diff"
+    if not autofix_diff_file.exists():
+        assert generate_autofix, "autofix diff file doesn't exist"
+        # if generate_autofix is set, the diff content isn't used and the file
+        # content will be created
+        autofix_diff_content = ""
+    else:
+        autofix_diff_content = autofix_diff_file.read_text()
+
+    # if running against anyio, since "eval_files/{test.py}" have replaced trio->anyio,
+    # meaning it's replaced in visited_code, we also replace it in previous generated code
+    # and in the previous diff
+    if anyio:
+        previous_autofixed = replace_library(previous_autofixed)
+        autofix_diff_content = replace_library(autofix_diff_content)
+
+    # save any difference in the autofixed code
+    diff = diff_strings(previous_autofixed, visited_code)
+
+    # generate diff between unfixed and visited code, i.e. what's added/removed
+    added_autofix_diff = diff_strings(unfixed_code, visited_code)
+
+    # print diff, mainly helpful during development
+    if diff:
+        print("\n", diff)
+
+    # if --generate-autofix is specified, which it may be during development,
+    # just silently overwrite the content.
+    if generate_autofix and not anyio:
+        autofix_files[test].write_text(visited_code)
+        autofix_diff_file.write_text(added_autofix_diff)
+        return
+
+    # assert that there's no difference in the autofixed code from before
+    assert visited_code == previous_autofixed, (
+        "autofix diff, run with --generate-autofix if the test file has changed to"
+        " update the autofix files."
+    )
+    # and assert that the diff is the same, which it should be if the above passes
+    assert added_autofix_diff == autofix_diff_content, (
+        "THIS SHOULD NOT HAPPEN: diff in the autofix diff - without there being a diff"
+        " in the autofixed code, run with --generate-autofix if the test file has"
+        " changed to update the autofix files."
+    )
+
+
+# This can be further cleaned up by adding the other return values from
+# parse_eval_file (Errors, args and enabled_codes) to this class - and find magic
+# markers in the same pass as we parse out errors etc.
+@dataclass
+class MagicMarkers:
+    NOANYIO: bool = False
+    NOTRIO: bool = False
+    ANYIO_NO_ERROR: bool = False
+    TRIO_NO_ERROR: bool = False
+
+
+def find_magic_markers(
+    content: str,
+) -> MagicMarkers:
+    found_markers = MagicMarkers()
+    markers = (f.name for f in fields(found_markers))
+    pattern = rf'# ({"|".join(markers)})'
+    for f in re.findall(pattern, content):
+        setattr(found_markers, f, True)
+    return found_markers
+
+
+# This could be optimized not to reopen+reread+reparse the same file over and over
+# when testing the same file
+@pytest.mark.parametrize(("test", "path"), test_files, ids=[f[0] for f in test_files])
+@pytest.mark.parametrize("autofix", [False, True], ids=["noautofix", "autofix"])
+@pytest.mark.parametrize("anyio", [False, True], ids=["trio", "anyio"])
+def test_eval(
+    test: str, path: Path, autofix: bool, anyio: bool, generate_autofix: bool
+):
+    content = path.read_text()
+    magic_markers = find_magic_markers(content)
+    if anyio and magic_markers.NOANYIO:
         pytest.skip("file marked with NOANYIO")
 
-    # if test is marked NOTRIO, it's not written to require substitution
-    if "# NOTRIO" not in content:
-        # replace instances of trio with anyio, unless it's part of a flag
-        # (which all conveniently start with --trio... atm)
-        content = re.sub(r"(?<!-)trio", "anyio", content)
+    # if autofixing, columns may get messed up
+    ignore_column = autofix
+
+    if magic_markers.NOTRIO:
+        if not anyio:
+            pytest.skip("file marked with NOTRIO")
+
+        # if test is marked NOTRIO, it's not written to require substitution
+    elif anyio:
+        content = replace_library(content)
 
         # if substituting we're messing up columns
         ignore_column = True
-    else:
-        ignore_column = False
-
-    # parse args and expected errors
-    expected, parsed_args = _parse_eval_file(test, content)
-
-    parsed_args.insert(0, "--anyio")
 
-    # initialize plugin and check errors, ignoring columns since they occasionally are
-    # wrong due to len("anyio") > len("trio")
-    plugin = Plugin(ast.parse(content))
+    expected, parsed_args, enable = _parse_eval_file(test, content)
+    if anyio:
+        parsed_args.insert(0, "--anyio")
+    if autofix:
+        parsed_args.append(f"--autofix={enable}")
 
-    if "# ANYIO_NO_ERROR" in content:
+    if (anyio and magic_markers.ANYIO_NO_ERROR) or (
+        not anyio and magic_markers.TRIO_NO_ERROR
+    ):
         expected = []
 
+    plugin = Plugin.from_source(content)
     errors = assert_expected_errors(
         plugin, *expected, args=parsed_args, ignore_column=ignore_column
     )
 
-    # check that error messages refer to 'anyio', or to neither library
-    for error in errors:
-        message = error.message.format(*error.args)
-        assert "anyio" in message or "trio" not in message
+    if anyio:
+        # check that error messages refer to 'anyio', or to neither library
+        for error in errors:
+            message = error.message.format(*error.args)
+            assert "anyio" in message or "trio" not in message
+
+    if autofix:
+        check_autofix(test, plugin, content, generate_autofix, anyio=anyio)
+    else:
+        # make sure content isn't modified
+        assert content == plugin.module.code
+
+
+# check that autofixed files raise no errors and doesn't get autofixed (again)
+@pytest.mark.parametrize("test", autofix_files)
+def test_autofix(test: str):
+    content = autofix_files[test].read_text()
+    assert content, "empty file"
+
+    if "# NOTRIO" in content:
+        pytest.skip("file marked with NOTRIO")
+
+    _, parsed_args, enable = _parse_eval_file(test, content)
+    parsed_args.append(f"--autofix={enable}")
+
+    plugin = Plugin.from_source(content)
+    # not passing any expected errors
+    _ = assert_expected_errors(plugin, args=parsed_args)
 
+    diff = diff_strings(plugin.module.code, content)
+    if diff:
+        print(diff)
+    assert plugin.module.code == content, "autofixed file changed when autofixed again"
 
-def _parse_eval_file(test: str, content: str) -> tuple[list[Error], list[str]]:
+
+def _parse_eval_file(test: str, content: str) -> tuple[list[Error], list[str], str]:
     # version check
     check_version(test)
     test = test.split("_")[0]
 
     parsed_args = []
 
-    # only enable the tested visitor to save performance and ease debugging
-    # if a test requires enabling multiple visitors they specify a
-    # `# ARG --enable-vis...` that comes later in the arg list, overriding this
-    visitor_codes_regex = ""
+    # Only enable the tested visitor to save performance and ease debugging.
+    # If a test requires enabling multiple visitors they specify a
+    # `# ARG --enable=` that comes later in the arg list, overriding this.
+    enabled_codes = ""
     if test in ERROR_CODES:
-        parsed_args = [f"--enable-visitor-codes-regex={test}"]
-        visitor_codes_regex = f"{test}"
+        parsed_args = [f"--enable={test}"]
+        enabled_codes = f"{test}"
 
     expected: list[Error] = []
 
     for lineno, line in enumerate(content.split("\n"), start=1):
         # interpret '\n' in comments as actual newlines
         line = line.replace("\\n", "\n")
 
         line = line.strip()
 
         # add command-line args if specified with #ARG
         if reg_match := re.search(r"(?<=ARG ).*", line):
             argument = reg_match.group().strip()
             parsed_args.append(argument)
-            if m := re.match(r"--enable-visitor-codes-regex=(.*)", argument):
-                visitor_codes_regex = m.groups()[0]
+            if m := re.match(r"--enable=(.*)", argument):
+                enabled_codes = m.groups()[0]
 
         # skip commented out lines
         if not line or line[0] == "#":
             continue
 
         # get text between `error:` and (end of line or another comment)
         k = re.findall(r"(error|TRIO...)(_.*)?:([^#]*)(?=#|$)", line)
 
         for err_code, alt_code, err_args in k:
             try:
-                # Append a bunch of empty strings so string formatting gives garbage
-                # instead of throwing an exception
                 try:
-                    args = eval(  # noqa: S307
+                    args = eval(
                         f"[{err_args}]",
                         {
                             "lineno": lineno,
                             "line": lineno,
                             "Statement": Statement,
                             "Stmt": Statement,
                         },
@@ -190,23 +339,33 @@
             if err_code == "error":
                 err_code = test
             error_class = ERROR_CODES[err_code + alt_code]
             message = error_class.error_codes[err_code + alt_code]
             try:
                 expected.append(Error(err_code, lineno, int(col), message, *args))
             except AttributeError as e:
-                msg = (
-                    f"Line {lineno}: Failed to format\n {message!r}\n" f'"with\n{args}'
-                )
+                msg = f"Line {lineno}: Failed to format\n {message!r}\nwith\n{args}"
                 raise ParseError(msg) from e
 
+    enabled_codes_list = enabled_codes.split(",")
+    for code in enabled_codes_list:
+        assert re.fullmatch(
+            r"TRIO\d\d\d", code
+        ), f"invalid code {code} in list {enabled_codes_list}"
+
     for error in expected:
-        assert re.match(visitor_codes_regex, error.code)
+        for code in enabled_codes.split(","):
+            if error.code.startswith(code):
+                break
+        else:
+            assert (
+                error.code in enabled_codes_list
+            ), f"Expected error code {error.code} not enabled"
 
-    return expected, parsed_args
+    return expected, parsed_args, enabled_codes
 
 
 # Codes that are supposed to also raise errors when run on sync code, and should
 # be excluded from the SyncTransformer check.
 # Expand this list when adding a new check if it does not care about whether the code
 # is asynchronous or not.
 error_codes_ignored_when_checking_transformed_sync_code = {
@@ -249,29 +408,27 @@
 def test_noerror_on_sync_code(test: str, path: Path):
     if any(e in test for e in error_codes_ignored_when_checking_transformed_sync_code):
         return
     with tokenize.open(path) as f:
         source = f.read()
     tree = SyncTransformer().visit(ast.parse(source))
 
-    ignored_codes_regex = (
-        "(?!("
-        + "|".join(error_codes_ignored_when_checking_transformed_sync_code)
-        + "))"
-    )
     _ = assert_expected_errors(
-        Plugin(tree),
-        args=[f"--enable-visitor-codes-regex={ignored_codes_regex}"],
+        Plugin(tree, [ast.unparse(tree)]),
+        args=[
+            "--disable="
+            + ",".join(error_codes_ignored_when_checking_transformed_sync_code)
+        ],
     )
 
 
 def initialize_options(plugin: Plugin, args: list[str] | None = None):
-    om = _default_option_manager()
-    plugin.add_options(om)
-    plugin.parse_options(om.parse_args(args=(args if args else [])))
+    parser = ArgumentParser(prog="flake8-trio")
+    Plugin.add_options(parser)
+    Plugin.parse_options(parser.parse_args(args))
 
 
 def assert_expected_errors(
     plugin: Plugin,
     *expected: Error,
     args: list[str] | None = None,
     ignore_column: bool = False,
@@ -304,17 +461,17 @@
 
 def print_first_diff(errors: Sequence[Error], expected: Sequence[Error]):
     first_error_line: list[Error] = []
     first_expected_line: list[Error] = []
     for err, exp in zip(errors, expected):
         if err == exp:
             continue
-        if not first_error_line or err.line == first_error_line[0]:
+        if not first_error_line or err.line == first_error_line[0].line:
             first_error_line.append(err)
-        if not first_expected_line or exp.line == first_expected_line[0]:
+        if not first_expected_line or exp.line == first_expected_line[0].line:
             first_expected_line.append(exp)
 
     if first_expected_line != first_error_line:
         print(
             "\nFirst lines with different errors",
             f"  actual: {[e.cmp() for e in first_error_line]}",
             f"expected: {[e.cmp() for e in first_expected_line]}",
@@ -335,40 +492,40 @@
 
     # populate dicts with number of errors per line
     for e in errors:
         error_dict[e.line][e.code] += 1
     for e in expected:
         expected_dict[e.line][e.code] += 1
 
-    any_error = False
+    error_count = 0
     for line in all_lines:
         if error_dict[line] == expected_dict[line]:
             continue
 
         # go through all the codes on the line
         for code in sorted({*error_dict[line], *expected_dict[line]}):
-            if not any_error:
+            if error_count == 0:
                 print(
                     "Lines with different # of errors:",
                     "-" * 38,
                     f"| line | {'code':7} | actual | expected |",
                     sep="\n",
                     file=sys.stderr,
                 )
-                any_error = True
 
             print(
                 f"| {line:4}",
                 f"{code}",
                 f"{error_dict[line][code]:6}",
                 f"{expected_dict[line][code]:8} |",
                 sep=" | ",
                 file=sys.stderr,
             )
-    assert not any_error
+            error_count += abs(error_dict[line][code] - expected_dict[line][code])
+    assert error_count == 0
 
 
 def assert_correct_attribute(
     errors: Iterable[Error], expected: Iterable[Error], attribute: str
 ):
     # check errors have correct messages
     args_error = False
@@ -415,14 +572,32 @@
     for err, exp in zip(errors, expected):
         err_msg = info_tuple(err)
         for err, type_ in zip(err_msg, (int, int, str, type(None))):
             assert isinstance(err, type_)
         assert err_msg == info_tuple(exp)
 
 
+# eval_files tests check that noqa is respected when running as standalone, but
+# they don't check anything when running as plugin.
+# When run as a plugin, flake8 will handle parsing of `noqa`.
+def test_noqa_respected_depending_on_standalone(tmp_path: Path):
+    text = """import trio
+with trio.move_on_after(10): ... # noqa
+"""
+    plugin = Plugin.from_source(text)
+    initialize_options(plugin, args=["--enable=TRIO100"])
+
+    assert plugin.standalone
+    assert not tuple(plugin.run())
+
+    plugin.standalone = False
+    assert len(tuple(plugin.run())) == 1
+
+
+@pytest.mark.fuzz()
 def test_910_permutations():
     """Tests all possible permutations for TRIO910.
 
     Since each test is so fast, and there's so many permutations, manually doing
     the permutations in a single test is much faster than the permutations from using
     pytest parametrization - and does not clutter up the output massively.
 
@@ -439,16 +614,16 @@
         except:
             await foo() | ... | raise | return | None
         else:
             await foo() | ... | return | None
         finally:
             await foo() | ... | return | None
     """
-    plugin = Plugin(ast.AST())
-    initialize_options(plugin, args=["--enable-visitor-codes-regex=TRIO910"])
+    plugin = Plugin(ast.AST(), [])
+    initialize_options(plugin, args=["--enable=TRIO910"])
 
     check = "await foo()"
 
     # loop over all the possible content of the different blocks
     for try_, exc1, exc2, bare_exc, else_, finally_ in itertools.product(
         (check, "..."),  # try_
         (check, "...", "raise", "return", None),  # exc1
@@ -473,19 +648,17 @@
             "except": bare_exc,
             "else": else_,
             "finally": finally_,
         }.items():
             if val is not None:
                 function_str += f"  {arg}:\n    {val}\n"
 
-        tree = ast.parse(function_str)
+        module = cst.parse_module(function_str)
 
-        # not a type error per se, but it's pyright warning about assigning to a
-        # protected class member - hence we silence it with a `type: ignore`.
-        plugin._tree = tree  # type: ignore
+        plugin.module = module
         errors = list(plugin.run())
 
         if (
             # return in exception
             "return" in (exc1, exc2, bare_exc)
             # exception and finally doesn't checkpoint, checkpoint in try might not run
             or ("..." in (exc1, exc2, bare_exc) and finally_ != check)
@@ -497,163 +670,37 @@
             or (finally_ == "return" and bare_exc is None)
         ):
             assert errors, "# missing alarm:\n" + function_str
         else:
             assert not errors, "# false alarm:\n" + function_str
 
 
-def test_114_raises_on_invalid_parameter(capsys: pytest.CaptureFixture[str]):
-    plugin = Plugin(ast.AST())
-    # flake8 will reraise ArgumentError as SystemExit
-    for arg in "blah.foo", "foo*", "*":
-        with pytest.raises(SystemExit):
-            initialize_options(plugin, args=[f"--startable-in-context-manager={arg}"])
-        out, err = capsys.readouterr()
-        assert not out
-        assert f"{arg!r} is not a valid method identifier" in err
-
-
-def test_200_options(capsys: pytest.CaptureFixture[str]):
-    plugin = Plugin(ast.AST())
-    for i, arg in (0, "foo"), (2, "foo->->bar"), (2, "foo->bar->fee"):
-        with pytest.raises(SystemExit):
-            initialize_options(plugin, args=[f"--trio200-blocking-calls={arg}"])
-        out, err = capsys.readouterr()
-        assert not out, out
-        assert all(word in err for word in (str(i), arg, "->"))
-
-
-def test_anyio_from_config(tmp_path: Path, capsys: pytest.CaptureFixture[str]):
-    assert tmp_path.joinpath(".flake8").write_text(
-        """
-[flake8]
-anyio = True
-select = TRIO220
-"""
-    )
-
-    from flake8_trio.visitors.visitor2xx import Visitor22X
-
-    err_msg = Visitor22X.error_codes["TRIO220"].format(
-        "subprocess.Popen",
-        "[anyio|trio]",
-    )
-    err_file = str(Path(__file__).parent / "eval_files" / "anyio_trio.py")
-    expected = f"{err_file}:10:5: TRIO220 {err_msg}\n"
-    from flake8.main.cli import main
-
-    returnvalue = main(
-        argv=[
-            err_file,
-            "--append-config",
-            str(tmp_path / ".flake8"),
-        ]
-    )
-    assert returnvalue == 1
-    out, err = capsys.readouterr()
-    assert not err
-    assert expected == out
-
-
-def _test_trio200_from_config_common(tmp_path: Path) -> str:
-    assert tmp_path.joinpath(".flake8").write_text(
-        """
-[flake8]
-trio200-blocking-calls =
-  other -> async,
-  sync_fns.* -> the_async_equivalent,
-select = TRIO200
-"""
-    )
-    assert tmp_path.joinpath("example.py").write_text(
-        """
-import sync_fns
-
-async def foo():
-    sync_fns.takes_a_long_time()
-"""
-    )
-    return (
-        "./example.py:5:5: TRIO200 User-configured blocking sync call sync_fns.* "
-        "in async function, consider replacing with the_async_equivalent.\n"
-    )
-
-
-def test_200_from_config_flake8_internals(
-    tmp_path: Path, capsys: pytest.CaptureFixture[str]
-):
-    # abuse flake8 internals to avoid having to use subprocess
-    # which breaks breakpoints and hinders debugging
-    # TODO: fixture (?) to change working directory
-
-    err_msg = _test_trio200_from_config_common(tmp_path)
-    # replace ./ with tmp_path/
-    err_msg = str(tmp_path) + err_msg[1:]
-
-    from flake8.main.cli import main
-
-    returnvalue = main(
-        argv=[
-            str(tmp_path / "example.py"),
-            "--append-config",
-            str(tmp_path / ".flake8"),
-        ]
-    )
-    out, err = capsys.readouterr()
-    assert returnvalue == 1
-    assert not err
-    assert err_msg == out
-
-
-def test_200_from_config_subprocess(tmp_path: Path):
-    err_msg = _test_trio200_from_config_common(tmp_path)
-    res = subprocess.run(  # noqa: S603,S607
-        ["flake8"], cwd=tmp_path, capture_output=True
-    )
-    assert not res.stderr
-    assert res.stdout == err_msg.encode("ascii")
-
-
-def test_900_default_off(capsys: pytest.CaptureFixture[str]):
-    from flake8.main.cli import main
-
-    returnvalue = main(
-        argv=[
-            "tests/trio900.py",
-        ]
-    )
-    out, err = capsys.readouterr()
-    assert returnvalue == 1
-    assert not err
-    assert "TRIO900" not in out
-
-
 # from https://docs.python.org/3/library/itertools.html#itertools-recipes
 def consume(iterator: Iterable[Any]):
-    deque(iterator, maxlen=0)  # pyright: reportUnusedCallResult=false
+    deque(iterator, maxlen=0)
 
 
 @pytest.mark.fuzz()
 class TestFuzz(unittest.TestCase):
-    @settings(max_examples=1_000, suppress_health_check=[HealthCheck.too_slow])
+    @settings(
+        max_examples=1_000, deadline=None, suppress_health_check=[HealthCheck.too_slow]
+    )
     @given((from_grammar() | from_node()).map(ast.parse))
     def test_does_not_crash_on_any_valid_code(self, syntax_tree: ast.AST):
         # TODO: figure out how to get unittest to play along with pytest options
-        # so `--enable-visitor-codes-regex` can be passed through.
+        # so `--enable-codes` can be passed through.
         # Though I barely notice a difference manually changing this value, or even
         # not running the plugin at all, so overhead looks to be vast majority of runtime
-        enable_visitor_codes_regex = ".*"
+        enabled_codes = "TRIO"
 
         # Given any syntatically-valid source code, the checker should
         # not crash.  This tests doesn't check that we do the *right* thing,
         # just that we don't crash on valid-if-poorly-styled code!
-        plugin = Plugin(syntax_tree)
-        initialize_options(
-            plugin, [f"--enable-visitor-codes-regex={enable_visitor_codes_regex}"]
-        )
+        plugin = Plugin(syntax_tree, [ast.unparse(syntax_tree)])
+        initialize_options(plugin, [f"--enable={enabled_codes}"])
 
         consume(plugin.run())
 
 
 def _iter_python_files():
     # Because the generator isn't perfect, we'll also test on all the code
     # we can easily find in our current Python environment - this includes
@@ -662,17 +709,15 @@
         for dirname, _, files in os.walk(base):
             for f in files:
                 if f.endswith(".py"):
                     yield Path(dirname) / f
 
 
 @pytest.mark.fuzz()
-def test_does_not_crash_on_site_code(enable_visitor_codes_regex: str):
+def test_does_not_crash_on_site_code(enable_codes: str):
     for path in _iter_python_files():
         try:
             plugin = Plugin.from_filename(str(path))
-            initialize_options(
-                plugin, [f"--enable-visitor-codes-regex={enable_visitor_codes_regex}"]
-            )
+            initialize_options(plugin, [f"--enable={enable_codes}"])
             consume(plugin.run())
         except Exception as err:
             raise AssertionError(f"Failed on {path}") from err
```

### Comparing `flake8-trio-23.2.5/tox.ini` & `flake8-trio-23.5.1/tox.ini`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 [testenv]
 description = Runs pytest, optionally with posargs
 deps =
     flake8_6: flake8>=6.0
     flake8_5: flake8>=5.0,<6.0
     pytest
     pytest-cov
-    #pytest-xdist
+    pytest-xdist
     hypothesis
     hypothesmith
     trio
 commands =
     pytest {posargs} #{posargs:-n auto}
 
 # Settings for other tools
@@ -31,22 +31,31 @@
     error
 
 [coverage:paths]
 source =
     flake8_trio
     */site-packages/flake8_trio
 
-[flake8]
-max-line-length = 90
-extend-ignore = S101, D101, D102, D103, D105, D106, D107, TC006
-per-file-ignores = flake8_trio/visitors/__init__.py: F401, E402
-
 [coverage:report]
 exclude_lines =
     # Have to re-enable the standard pragma
     pragma: no cover
 
     # Don't complain about abstract methods, they aren't run:
     @(abc\.)?abstractmethod
 
     # Don't check guarded type imports
     if (typing.)?TYPE_CHECKING:
+
+[flake8]
+max-line-length = 90
+extend-ignore = S101, D101, D102, D103, D105, D106, D107
+extend-enable = TC10
+exclude = .*, tests/eval_files/*, tests/autofix_files/*
+per-file-ignores =
+    flake8_trio/visitors/__init__.py: F401, E402
+# visitor_utility contains comments specifying how it parses noqa comments, which get
+# parsed as noqa comments
+    flake8_trio/visitors/visitor_utility.py: NQA101, NQA102
+# (E301, E302) black formats stub files without excessive blank lines
+# (D) we don't care about docstrings in stub files
+    *.pyi: D, E301, E302
```

