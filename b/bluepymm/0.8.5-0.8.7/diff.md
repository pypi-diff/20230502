# Comparing `tmp/bluepymm-0.8.5.tar.gz` & `tmp/bluepymm-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bluepymm-0.8.5.tar", last modified: Fri Jan 27 13:39:52 2023, max compression
+gzip compressed data, was "bluepymm-0.8.7.tar", last modified: Mon Feb 27 15:16:16 2023, max compression
```

## Comparing `bluepymm-0.8.5.tar` & `bluepymm-0.8.7.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 13:39:52.000000 bluepymm-0.8.5/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-01-27 13:39:45.000000 bluepymm-0.8.5/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35151 2023-01-27 13:39:45.000000 bluepymm-0.8.5/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-01-27 13:39:45.000000 bluepymm-0.8.5/COPYING.lesser
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-01-27 13:39:45.000000 bluepymm-0.8.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-01-27 13:39:45.000000 bluepymm-0.8.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-01-27 13:39:52.000000 bluepymm-0.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-01-27 13:39:45.000000 bluepymm-0.8.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 13:39:52.000000 bluepymm-0.8.5/bluepymm/
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-01-27 13:39:45.000000 bluepymm-0.8.5/bluepymm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-01-27 13:39:52.000000 bluepymm-0.8.5/bluepymm/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 13:39:52.000000 bluepymm-0.8.5/bluepymm/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-01-27 13:39:45.000000 bluepymm-0.8.5/bluepymm/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-01-27 13:39:45.000000 bluepymm-0.8.5/bluepymm/legacy/create_hoc_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-01-27 13:39:45.000000 bluepymm-0.8.5/bluepymm/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 13:39:52.000000 bluepymm-0.8.5/bluepymm/prepare_combos/
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-01-27 13:39:45.000000 bluepymm-0.8.5/bluepymm/prepare_combos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16419 2023-01-27 13:39:45.000000 bluepymm-0.8.5/bluepymm/prepare_combos/create_mm_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-01-27 13:39:45.000000 bluepymm-0.8.5/bluepymm/prepare_combos/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    10472 2023-01-27 13:39:45.000000 bluepymm-0.8.5/bluepymm/prepare_combos/parse_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    12066 2023-01-27 13:39:45.000000 bluepymm-0.8.5/bluepymm/prepare_combos/prepare_emodel_dirs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 13:39:52.000000 bluepymm-0.8.5/bluepymm/run_combos/
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-01-27 13:39:45.000000 bluepymm-0.8.5/bluepymm/run_combos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14246 2023-01-27 13:39:45.000000 bluepymm-0.8.5/bluepymm/run_combos/calculate_scores.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-01-27 13:39:45.000000 bluepymm-0.8.5/bluepymm/run_combos/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 13:39:52.000000 bluepymm-0.8.5/bluepymm/select_combos/
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-01-27 13:39:45.000000 bluepymm-0.8.5/bluepymm/select_combos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-01-27 13:39:45.000000 bluepymm-0.8.5/bluepymm/select_combos/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-01-27 13:39:45.000000 bluepymm-0.8.5/bluepymm/select_combos/megate_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-01-27 13:39:45.000000 bluepymm-0.8.5/bluepymm/select_combos/process_megate_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    15005 2023-01-27 13:39:45.000000 bluepymm-0.8.5/bluepymm/select_combos/reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-01-27 13:39:45.000000 bluepymm-0.8.5/bluepymm/select_combos/sqlite_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    16435 2023-01-27 13:39:45.000000 bluepymm-0.8.5/bluepymm/select_combos/table_processing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 13:39:52.000000 bluepymm-0.8.5/bluepymm/templates/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6660 2023-01-27 13:39:45.000000 bluepymm-0.8.5/bluepymm/templates/cell_template_neurodamus.jinja2
--rwxr-xr-x   0 runner    (1001) docker     (123)     4762 2023-01-27 13:39:45.000000 bluepymm-0.8.5/bluepymm/templates/cell_template_neuron.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     6915 2023-01-27 13:39:45.000000 bluepymm-0.8.5/bluepymm/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 13:39:52.000000 bluepymm-0.8.5/bluepymm/validate_output/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-01-27 13:39:45.000000 bluepymm-0.8.5/bluepymm/validate_output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-01-27 13:39:45.000000 bluepymm-0.8.5/bluepymm/validate_output/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 13:39:52.000000 bluepymm-0.8.5/bluepymm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-01-27 13:39:52.000000 bluepymm-0.8.5/bluepymm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-01-27 13:39:52.000000 bluepymm-0.8.5/bluepymm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-27 13:39:52.000000 bluepymm-0.8.5/bluepymm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-01-27 13:39:52.000000 bluepymm-0.8.5/bluepymm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-01-27 13:39:52.000000 bluepymm-0.8.5/bluepymm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-01-27 13:39:52.000000 bluepymm-0.8.5/bluepymm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-01-27 13:39:52.000000 bluepymm-0.8.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-01-27 13:39:45.000000 bluepymm-0.8.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 13:39:52.000000 bluepymm-0.8.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 13:39:45.000000 bluepymm-0.8.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-01-27 13:39:45.000000 bluepymm-0.8.5/tests/test_bluepymm.py
--rw-r--r--   0 runner    (1001) docker     (123)    13594 2023-01-27 13:39:45.000000 bluepymm-0.8.5/tests/test_calculate_scores.py
--rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-01-27 13:39:45.000000 bluepymm-0.8.5/tests/test_create_mm_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)    10714 2023-01-27 13:39:45.000000 bluepymm-0.8.5/tests/test_legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7490 2023-01-27 13:39:45.000000 bluepymm-0.8.5/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-01-27 13:39:45.000000 bluepymm-0.8.5/tests/test_megate_output.py
--rw-r--r--   0 runner    (1001) docker     (123)    10501 2023-01-27 13:39:45.000000 bluepymm-0.8.5/tests/test_parse_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-01-27 13:39:45.000000 bluepymm-0.8.5/tests/test_prepare_combos.py
--rw-r--r--   0 runner    (1001) docker     (123)    15360 2023-01-27 13:39:45.000000 bluepymm-0.8.5/tests/test_prepare_emodel_dirs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-01-27 13:39:45.000000 bluepymm-0.8.5/tests/test_process_megate_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-01-27 13:39:45.000000 bluepymm-0.8.5/tests/test_reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-01-27 13:39:45.000000 bluepymm-0.8.5/tests/test_run_combos.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-01-27 13:39:45.000000 bluepymm-0.8.5/tests/test_select_combos.py
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-01-27 13:39:45.000000 bluepymm-0.8.5/tests/test_sqlite_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    15008 2023-01-27 13:39:45.000000 bluepymm-0.8.5/tests/test_table_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-01-27 13:39:45.000000 bluepymm-0.8.5/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    69513 2023-01-27 13:39:45.000000 bluepymm-0.8.5/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 15:16:16.835696 bluepymm-0.8.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-02-27 15:16:14.000000 bluepymm-0.8.7/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35151 2023-02-27 15:16:14.000000 bluepymm-0.8.7/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-02-27 15:16:14.000000 bluepymm-0.8.7/COPYING.lesser
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-02-27 15:16:14.000000 bluepymm-0.8.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-02-27 15:16:14.000000 bluepymm-0.8.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-02-27 15:16:16.835696 bluepymm-0.8.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-02-27 15:16:14.000000 bluepymm-0.8.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 15:16:16.835696 bluepymm-0.8.7/bluepymm/
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-02-27 15:16:14.000000 bluepymm-0.8.7/bluepymm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-02-27 15:16:16.835696 bluepymm-0.8.7/bluepymm/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 15:16:16.835696 bluepymm-0.8.7/bluepymm/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-02-27 15:16:14.000000 bluepymm-0.8.7/bluepymm/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-02-27 15:16:14.000000 bluepymm-0.8.7/bluepymm/legacy/create_hoc_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-02-27 15:16:14.000000 bluepymm-0.8.7/bluepymm/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 15:16:16.835696 bluepymm-0.8.7/bluepymm/prepare_combos/
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-02-27 15:16:14.000000 bluepymm-0.8.7/bluepymm/prepare_combos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16419 2023-02-27 15:16:14.000000 bluepymm-0.8.7/bluepymm/prepare_combos/create_mm_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-02-27 15:16:14.000000 bluepymm-0.8.7/bluepymm/prepare_combos/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10472 2023-02-27 15:16:14.000000 bluepymm-0.8.7/bluepymm/prepare_combos/parse_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12066 2023-02-27 15:16:14.000000 bluepymm-0.8.7/bluepymm/prepare_combos/prepare_emodel_dirs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 15:16:16.835696 bluepymm-0.8.7/bluepymm/run_combos/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-02-27 15:16:14.000000 bluepymm-0.8.7/bluepymm/run_combos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14246 2023-02-27 15:16:14.000000 bluepymm-0.8.7/bluepymm/run_combos/calculate_scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-02-27 15:16:14.000000 bluepymm-0.8.7/bluepymm/run_combos/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 15:16:16.835696 bluepymm-0.8.7/bluepymm/select_combos/
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-02-27 15:16:14.000000 bluepymm-0.8.7/bluepymm/select_combos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-02-27 15:16:14.000000 bluepymm-0.8.7/bluepymm/select_combos/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-02-27 15:16:14.000000 bluepymm-0.8.7/bluepymm/select_combos/megate_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-02-27 15:16:14.000000 bluepymm-0.8.7/bluepymm/select_combos/process_megate_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15005 2023-02-27 15:16:14.000000 bluepymm-0.8.7/bluepymm/select_combos/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-02-27 15:16:14.000000 bluepymm-0.8.7/bluepymm/select_combos/sqlite_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16435 2023-02-27 15:16:14.000000 bluepymm-0.8.7/bluepymm/select_combos/table_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 15:16:16.835696 bluepymm-0.8.7/bluepymm/templates/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6660 2023-02-27 15:16:14.000000 bluepymm-0.8.7/bluepymm/templates/cell_template_neurodamus.jinja2
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4762 2023-02-27 15:16:14.000000 bluepymm-0.8.7/bluepymm/templates/cell_template_neuron.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     6915 2023-02-27 15:16:14.000000 bluepymm-0.8.7/bluepymm/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 15:16:16.835696 bluepymm-0.8.7/bluepymm/validate_output/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-02-27 15:16:14.000000 bluepymm-0.8.7/bluepymm/validate_output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-02-27 15:16:14.000000 bluepymm-0.8.7/bluepymm/validate_output/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 15:16:16.831696 bluepymm-0.8.7/bluepymm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-02-27 15:16:16.000000 bluepymm-0.8.7/bluepymm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-02-27 15:16:16.000000 bluepymm-0.8.7/bluepymm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 15:16:16.000000 bluepymm-0.8.7/bluepymm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-02-27 15:16:16.000000 bluepymm-0.8.7/bluepymm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-02-27 15:16:16.000000 bluepymm-0.8.7/bluepymm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-27 15:16:16.000000 bluepymm-0.8.7/bluepymm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-02-27 15:16:16.835696 bluepymm-0.8.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-02-27 15:16:14.000000 bluepymm-0.8.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 15:16:16.835696 bluepymm-0.8.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 15:16:14.000000 bluepymm-0.8.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-02-27 15:16:14.000000 bluepymm-0.8.7/tests/test_bluepymm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13594 2023-02-27 15:16:14.000000 bluepymm-0.8.7/tests/test_calculate_scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-02-27 15:16:14.000000 bluepymm-0.8.7/tests/test_create_mm_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10714 2023-02-27 15:16:14.000000 bluepymm-0.8.7/tests/test_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7490 2023-02-27 15:16:14.000000 bluepymm-0.8.7/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-02-27 15:16:14.000000 bluepymm-0.8.7/tests/test_megate_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10501 2023-02-27 15:16:14.000000 bluepymm-0.8.7/tests/test_parse_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-02-27 15:16:14.000000 bluepymm-0.8.7/tests/test_prepare_combos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15360 2023-02-27 15:16:14.000000 bluepymm-0.8.7/tests/test_prepare_emodel_dirs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-02-27 15:16:14.000000 bluepymm-0.8.7/tests/test_process_megate_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-02-27 15:16:14.000000 bluepymm-0.8.7/tests/test_reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-02-27 15:16:14.000000 bluepymm-0.8.7/tests/test_run_combos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-02-27 15:16:14.000000 bluepymm-0.8.7/tests/test_select_combos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-02-27 15:16:14.000000 bluepymm-0.8.7/tests/test_sqlite_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15008 2023-02-27 15:16:14.000000 bluepymm-0.8.7/tests/test_table_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-02-27 15:16:14.000000 bluepymm-0.8.7/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69513 2023-02-27 15:16:14.000000 bluepymm-0.8.7/versioneer.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `bluepymm-0.8.5/COPYING` & `bluepymm-0.8.7/COPYING`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.5/COPYING.lesser` & `bluepymm-0.8.7/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.5/LICENSE.txt` & `bluepymm-0.8.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.5/README.rst` & `bluepymm-0.8.7/README.rst`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.5/bluepymm/__init__.py` & `bluepymm-0.8.7/bluepymm/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.5/bluepymm/legacy/__init__.py` & `bluepymm-0.8.7/bluepymm/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.5/bluepymm/legacy/create_hoc_files.py` & `bluepymm-0.8.7/bluepymm/legacy/create_hoc_files.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.5/bluepymm/main.py` & `bluepymm-0.8.7/bluepymm/main.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.5/bluepymm/prepare_combos/__init__.py` & `bluepymm-0.8.7/bluepymm/prepare_combos/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.5/bluepymm/prepare_combos/create_mm_sqlite.py` & `bluepymm-0.8.7/bluepymm/prepare_combos/create_mm_sqlite.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.5/bluepymm/prepare_combos/main.py` & `bluepymm-0.8.7/bluepymm/prepare_combos/main.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.5/bluepymm/prepare_combos/parse_files.py` & `bluepymm-0.8.7/bluepymm/prepare_combos/parse_files.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.5/bluepymm/prepare_combos/prepare_emodel_dirs.py` & `bluepymm-0.8.7/bluepymm/prepare_combos/prepare_emodel_dirs.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.5/bluepymm/run_combos/__init__.py` & `bluepymm-0.8.7/bluepymm/run_combos/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.5/bluepymm/run_combos/calculate_scores.py` & `bluepymm-0.8.7/bluepymm/run_combos/calculate_scores.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.5/bluepymm/run_combos/main.py` & `bluepymm-0.8.7/bluepymm/run_combos/main.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.5/bluepymm/select_combos/__init__.py` & `bluepymm-0.8.7/bluepymm/select_combos/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.5/bluepymm/select_combos/main.py` & `bluepymm-0.8.7/bluepymm/select_combos/main.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.5/bluepymm/select_combos/megate_output.py` & `bluepymm-0.8.7/bluepymm/select_combos/megate_output.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.5/bluepymm/select_combos/process_megate_config.py` & `bluepymm-0.8.7/bluepymm/select_combos/process_megate_config.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.5/bluepymm/select_combos/reporting.py` & `bluepymm-0.8.7/bluepymm/select_combos/reporting.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.5/bluepymm/select_combos/sqlite_io.py` & `bluepymm-0.8.7/bluepymm/select_combos/sqlite_io.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.5/bluepymm/select_combos/table_processing.py` & `bluepymm-0.8.7/bluepymm/select_combos/table_processing.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.5/bluepymm/templates/cell_template_neurodamus.jinja2` & `bluepymm-0.8.7/bluepymm/templates/cell_template_neurodamus.jinja2`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.5/bluepymm/templates/cell_template_neuron.jinja2` & `bluepymm-0.8.7/bluepymm/templates/cell_template_neuron.jinja2`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.5/bluepymm/tools.py` & `bluepymm-0.8.7/bluepymm/tools.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.5/bluepymm/validate_output/main.py` & `bluepymm-0.8.7/bluepymm/validate_output/main.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.5/bluepymm.egg-info/SOURCES.txt` & `bluepymm-0.8.7/bluepymm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.5/setup.py` & `bluepymm-0.8.7/setup.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.5/tests/test_bluepymm.py` & `bluepymm-0.8.7/tests/test_bluepymm.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.5/tests/test_calculate_scores.py` & `bluepymm-0.8.7/tests/test_calculate_scores.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.5/tests/test_create_mm_sqlite.py` & `bluepymm-0.8.7/tests/test_create_mm_sqlite.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.5/tests/test_legacy.py` & `bluepymm-0.8.7/tests/test_legacy.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.5/tests/test_main.py` & `bluepymm-0.8.7/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.5/tests/test_megate_output.py` & `bluepymm-0.8.7/tests/test_megate_output.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.5/tests/test_parse_files.py` & `bluepymm-0.8.7/tests/test_parse_files.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.5/tests/test_prepare_combos.py` & `bluepymm-0.8.7/tests/test_prepare_combos.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.5/tests/test_prepare_emodel_dirs.py` & `bluepymm-0.8.7/tests/test_prepare_emodel_dirs.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.5/tests/test_process_megate_config.py` & `bluepymm-0.8.7/tests/test_process_megate_config.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.5/tests/test_reporting.py` & `bluepymm-0.8.7/tests/test_reporting.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.5/tests/test_run_combos.py` & `bluepymm-0.8.7/tests/test_run_combos.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.5/tests/test_select_combos.py` & `bluepymm-0.8.7/tests/test_select_combos.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.5/tests/test_sqlite_io.py` & `bluepymm-0.8.7/tests/test_sqlite_io.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.5/tests/test_table_processing.py` & `bluepymm-0.8.7/tests/test_table_processing.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.5/tests/test_tools.py` & `bluepymm-0.8.7/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.5/versioneer.py` & `bluepymm-0.8.7/versioneer.py`

 * *Files identical despite different names*

