# Comparing `tmp/strax-1.4.3.tar.gz` & `tmp/strax-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strax-1.4.3.tar", last modified: Tue Apr 25 03:20:13 2023, max compression
+gzip compressed data, was "strax-1.5.0.tar", last modified: Tue May  2 19:36:47 2023, max compression
```

## Comparing `strax-1.4.3.tar` & `strax-1.5.0.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:20:13.889692 strax-1.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-04-25 03:20:09.000000 strax-1.4.3/CODE-OF-CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-25 03:20:09.000000 strax-1.4.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    18362 2023-04-25 03:20:09.000000 strax-1.4.3/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-04-25 03:20:09.000000 strax-1.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-25 03:20:09.000000 strax-1.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    26071 2023-04-25 03:20:13.889692 strax-1.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-25 03:20:09.000000 strax-1.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:20:13.873692 strax-1.4.3/bin/
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-04-25 03:20:09.000000 strax-1.4.3/bin/rechunker
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:20:13.873692 strax-1.4.3/extra_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-25 03:20:09.000000 strax-1.4.3/extra_requirements/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-25 03:20:09.000000 strax-1.4.3/extra_requirements/requirements-tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-25 03:20:09.000000 strax-1.4.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-25 03:20:13.889692 strax-1.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-04-25 03:20:09.000000 strax-1.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:20:13.877692 strax-1.4.3/strax/
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-25 03:20:09.000000 strax-1.4.3/strax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-25 03:20:09.000000 strax-1.4.3/strax/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14225 2023-04-25 03:20:09.000000 strax-1.4.3/strax/chunk.py
--rw-r--r--   0 runner    (1001) docker     (123)    11166 2023-04-25 03:20:09.000000 strax-1.4.3/strax/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    93514 2023-04-25 03:20:09.000000 strax-1.4.3/strax/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    12111 2023-04-25 03:20:09.000000 strax-1.4.3/strax/corrections.py
--rw-r--r--   0 runner    (1001) docker     (123)    10810 2023-04-25 03:20:09.000000 strax-1.4.3/strax/dtypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-25 03:20:09.000000 strax-1.4.3/strax/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    20577 2023-04-25 03:20:09.000000 strax-1.4.3/strax/mailbox.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-25 03:20:09.000000 strax-1.4.3/strax/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:20:13.881692 strax-1.4.3/strax/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-25 03:20:09.000000 strax-1.4.3/strax/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-04-25 03:20:09.000000 strax-1.4.3/strax/plugins/cut_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-04-25 03:20:09.000000 strax-1.4.3/strax/plugins/loop_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-25 03:20:09.000000 strax-1.4.3/strax/plugins/merge_only_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-04-25 03:20:09.000000 strax-1.4.3/strax/plugins/overlap_window_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-04-25 03:20:09.000000 strax-1.4.3/strax/plugins/parrallel_source_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    27174 2023-04-25 03:20:09.000000 strax-1.4.3/strax/plugins/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:20:13.885692 strax-1.4.3/strax/processing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 03:20:09.000000 strax-1.4.3/strax/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-04-25 03:20:09.000000 strax-1.4.3/strax/processing/data_reduction.py
--rw-r--r--   0 runner    (1001) docker     (123)    11792 2023-04-25 03:20:09.000000 strax-1.4.3/strax/processing/general.py
--rw-r--r--   0 runner    (1001) docker     (123)    23837 2023-04-25 03:20:09.000000 strax-1.4.3/strax/processing/hitlets.py
--rw-r--r--   0 runner    (1001) docker     (123)    19284 2023-04-25 03:20:09.000000 strax-1.4.3/strax/processing/peak_building.py
--rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-04-25 03:20:09.000000 strax-1.4.3/strax/processing/peak_merging.py
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-04-25 03:20:09.000000 strax-1.4.3/strax/processing/peak_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    13732 2023-04-25 03:20:09.000000 strax-1.4.3/strax/processing/peak_splitting.py
--rw-r--r--   0 runner    (1001) docker     (123)    14551 2023-04-25 03:20:09.000000 strax-1.4.3/strax/processing/pulse_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-04-25 03:20:09.000000 strax-1.4.3/strax/processing/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    12991 2023-04-25 03:20:09.000000 strax-1.4.3/strax/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    19611 2023-04-25 03:20:09.000000 strax-1.4.3/strax/run_selection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:20:13.885692 strax-1.4.3/strax/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 03:20:09.000000 strax-1.4.3/strax/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28547 2023-04-25 03:20:09.000000 strax-1.4.3/strax/storage/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     7709 2023-04-25 03:20:09.000000 strax-1.4.3/strax/storage/file_rechunker.py
--rw-r--r--   0 runner    (1001) docker     (123)    14439 2023-04-25 03:20:09.000000 strax-1.4.3/strax/storage/files.py
--rw-r--r--   0 runner    (1001) docker     (123)    14031 2023-04-25 03:20:09.000000 strax-1.4.3/strax/storage/mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-04-25 03:20:09.000000 strax-1.4.3/strax/storage/zipfiles.py
--rw-r--r--   0 runner    (1001) docker     (123)    11197 2023-04-25 03:20:09.000000 strax-1.4.3/strax/testutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    23951 2023-04-25 03:20:09.000000 strax-1.4.3/strax/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:20:13.877692 strax-1.4.3/strax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    26071 2023-04-25 03:20:13.000000 strax-1.4.3/strax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-04-25 03:20:13.000000 strax-1.4.3/strax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 03:20:13.000000 strax-1.4.3/strax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 03:20:13.000000 strax-1.4.3/strax.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-25 03:20:13.000000 strax-1.4.3/strax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-25 03:20:13.000000 strax-1.4.3/strax.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:20:13.889692 strax-1.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 03:20:09.000000 strax-1.4.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11542 2023-04-25 03:20:09.000000 strax-1.4.3/tests/test_child_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-04-25 03:20:09.000000 strax-1.4.3/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    16586 2023-04-25 03:20:09.000000 strax-1.4.3/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    17852 2023-04-25 03:20:09.000000 strax-1.4.3/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-04-25 03:20:09.000000 strax-1.4.3/tests/test_corrections.py
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-04-25 03:20:09.000000 strax-1.4.3/tests/test_cut_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-25 03:20:09.000000 strax-1.4.3/tests/test_data_reduction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-04-25 03:20:09.000000 strax-1.4.3/tests/test_fixed_plugin_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    12413 2023-04-25 03:20:09.000000 strax-1.4.3/tests/test_general_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-25 03:20:09.000000 strax-1.4.3/tests/test_get_zarr.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-25 03:20:09.000000 strax-1.4.3/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    20240 2023-04-25 03:20:09.000000 strax-1.4.3/tests/test_hitlet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-04-25 03:20:09.000000 strax-1.4.3/tests/test_inline_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-25 03:20:09.000000 strax-1.4.3/tests/test_lone_hit_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-04-25 03:20:09.000000 strax-1.4.3/tests/test_loop_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     5212 2023-04-25 03:20:09.000000 strax-1.4.3/tests/test_mailbox.py
--rw-r--r--   0 runner    (1001) docker     (123)    11602 2023-04-25 03:20:09.000000 strax-1.4.3/tests/test_mongo_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)    12609 2023-04-25 03:20:09.000000 strax-1.4.3/tests/test_multi_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-04-25 03:20:09.000000 strax-1.4.3/tests/test_overlap_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-25 03:20:09.000000 strax-1.4.3/tests/test_peak_merging.py
--rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-04-25 03:20:09.000000 strax-1.4.3/tests/test_peak_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-04-25 03:20:09.000000 strax-1.4.3/tests/test_peak_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-04-25 03:20:09.000000 strax-1.4.3/tests/test_peak_splitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-04-25 03:20:09.000000 strax-1.4.3/tests/test_pulse_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-04-25 03:20:09.000000 strax-1.4.3/tests/test_saving.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-04-25 03:20:09.000000 strax-1.4.3/tests/test_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    11286 2023-04-25 03:20:09.000000 strax-1.4.3/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    16531 2023-04-25 03:20:09.000000 strax-1.4.3/tests/test_superruns.py
--rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-04-25 03:20:09.000000 strax-1.4.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:36:47.352210 strax-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-05-02 19:36:44.000000 strax-1.5.0/CODE-OF-CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-02 19:36:44.000000 strax-1.5.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    18803 2023-05-02 19:36:44.000000 strax-1.5.0/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-02 19:36:44.000000 strax-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-02 19:36:44.000000 strax-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    26592 2023-05-02 19:36:47.352210 strax-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-02 19:36:44.000000 strax-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:36:47.332210 strax-1.5.0/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-05-02 19:36:44.000000 strax-1.5.0/bin/rechunker
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:36:47.332210 strax-1.5.0/extra_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-02 19:36:44.000000 strax-1.5.0/extra_requirements/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-02 19:36:44.000000 strax-1.5.0/extra_requirements/requirements-tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-02 19:36:44.000000 strax-1.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-02 19:36:47.352210 strax-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-02 19:36:44.000000 strax-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:36:47.336210 strax-1.5.0/strax/
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-02 19:36:44.000000 strax-1.5.0/strax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-02 19:36:44.000000 strax-1.5.0/strax/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14225 2023-05-02 19:36:44.000000 strax-1.5.0/strax/chunk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11166 2023-05-02 19:36:44.000000 strax-1.5.0/strax/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93514 2023-05-02 19:36:44.000000 strax-1.5.0/strax/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12111 2023-05-02 19:36:44.000000 strax-1.5.0/strax/corrections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-05-02 19:36:44.000000 strax-1.5.0/strax/dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-05-02 19:36:44.000000 strax-1.5.0/strax/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20577 2023-05-02 19:36:44.000000 strax-1.5.0/strax/mailbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-02 19:36:44.000000 strax-1.5.0/strax/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:36:47.340210 strax-1.5.0/strax/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-02 19:36:44.000000 strax-1.5.0/strax/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-02 19:36:44.000000 strax-1.5.0/strax/plugins/cut_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-05-02 19:36:44.000000 strax-1.5.0/strax/plugins/loop_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-02 19:36:44.000000 strax-1.5.0/strax/plugins/merge_only_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-05-02 19:36:44.000000 strax-1.5.0/strax/plugins/overlap_window_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-05-02 19:36:44.000000 strax-1.5.0/strax/plugins/parrallel_source_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27174 2023-05-02 19:36:44.000000 strax-1.5.0/strax/plugins/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:36:47.344210 strax-1.5.0/strax/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 19:36:44.000000 strax-1.5.0/strax/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-05-02 19:36:44.000000 strax-1.5.0/strax/processing/data_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11787 2023-05-02 19:36:44.000000 strax-1.5.0/strax/processing/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23837 2023-05-02 19:36:44.000000 strax-1.5.0/strax/processing/hitlets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19284 2023-05-02 19:36:44.000000 strax-1.5.0/strax/processing/peak_building.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-05-02 19:36:44.000000 strax-1.5.0/strax/processing/peak_merging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-05-02 19:36:44.000000 strax-1.5.0/strax/processing/peak_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13818 2023-05-02 19:36:44.000000 strax-1.5.0/strax/processing/peak_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14551 2023-05-02 19:36:44.000000 strax-1.5.0/strax/processing/pulse_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-05-02 19:36:44.000000 strax-1.5.0/strax/processing/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12991 2023-05-02 19:36:44.000000 strax-1.5.0/strax/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19611 2023-05-02 19:36:44.000000 strax-1.5.0/strax/run_selection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:36:47.344210 strax-1.5.0/strax/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 19:36:44.000000 strax-1.5.0/strax/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28547 2023-05-02 19:36:44.000000 strax-1.5.0/strax/storage/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7709 2023-05-02 19:36:44.000000 strax-1.5.0/strax/storage/file_rechunker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14439 2023-05-02 19:36:44.000000 strax-1.5.0/strax/storage/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14031 2023-05-02 19:36:44.000000 strax-1.5.0/strax/storage/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-05-02 19:36:44.000000 strax-1.5.0/strax/storage/zipfiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11197 2023-05-02 19:36:44.000000 strax-1.5.0/strax/testutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23951 2023-05-02 19:36:44.000000 strax-1.5.0/strax/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:36:47.340210 strax-1.5.0/strax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    26592 2023-05-02 19:36:47.000000 strax-1.5.0/strax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-05-02 19:36:47.000000 strax-1.5.0/strax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 19:36:47.000000 strax-1.5.0/strax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 19:36:47.000000 strax-1.5.0/strax.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-02 19:36:47.000000 strax-1.5.0/strax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-02 19:36:47.000000 strax-1.5.0/strax.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:36:47.352210 strax-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 19:36:44.000000 strax-1.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11542 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_child_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16586 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17852 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_corrections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_cut_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_data_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_fixed_plugin_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12413 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_general_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_get_zarr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20240 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_hitlet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_inline_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_lone_hit_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_loop_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5212 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_mailbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11602 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_mongo_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12609 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_multi_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_overlap_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_peak_merging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_peak_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_peak_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_peak_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_pulse_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_saving.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11286 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16531 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_superruns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_utils.py
```

### Comparing `strax-1.4.3/CODE-OF-CONDUCT.md` & `strax-1.5.0/CODE-OF-CONDUCT.md`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/CONTRIBUTING.md` & `strax-1.5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/HISTORY.md` & `strax-1.5.0/HISTORY.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,44 +1,54 @@
+1.5.0 / 2023-05-02
+---------------------
+* Fix ipython version by @dachengx in https://github.com/AxFoundation/strax/pull/719
+* Do not change channel when sort_by_time by @dachengx in https://github.com/AxFoundation/strax/pull/718
+* Save hits level information(hits time difference) in peaks by @dachengx in https://github.com/AxFoundation/strax/pull/716
+
+**Full Changelog**: https://github.com/AxFoundation/strax/compare/v1.4.3...v1.5.0
+
+
 1.4.3 / 2023-04-22
 ---------------------
 * Select max gaps from positive gaps by @dachengx in https://github.com/AxFoundation/strax/pull/708
 
 New Contributors
 * @dachengx made their first contribution in https://github.com/AxFoundation/strax/pull/708
 
 **Full Changelog**: https://github.com/AxFoundation/strax/compare/v1.4.2...v1.4.3
 
+
 1.4.2 / 2023-03-08
 ---------------------
 * Patch md access in the rechunker by @JoranAngevaare in https://github.com/AxFoundation/strax/pull/711
 * Raise compression errors if unable by @JoranAngevaare in https://github.com/AxFoundation/strax/pull/714
 
-
 **Full Changelog**: https://github.com/AxFoundation/strax/compare/v1.4.1...v1.4.2
 
 
 1.4.1 / 2023-02-13
 ---------------------
 * Rechunker using Mailbox by @JoranAngevaare in https://github.com/AxFoundation/strax/pull/710
 
-
 **Full Changelog**: https://github.com/AxFoundation/strax/compare/v1.4.0...v1.4.1
 
+
 1.4.0 / 2022-10-17
 ---------------------
 * Add capability for building summed waveform over channel subset by @DCichon in https://github.com/AxFoundation/strax/pull/565
 * Fixed delta peak timestamp problem by @FaroutYLq in https://github.com/AxFoundation/strax/pull/702
 
 Notes
  -  Breaking changes in the peak-building chain due to #565
 New Contributors
  - @DCichon made their first contribution in https://github.com/AxFoundation/strax/pull/565
 
 **Full Changelog**: https://github.com/AxFoundation/strax/compare/v1.3.0...v1.4.0
 
+
 1.3.0 / 2022-09-09
 ---------------------
 * Restructure plugins by @JoranAngevaare in https://github.com/AxFoundation/strax/pull/700
 * Numpy caching of data in online monitor storage by @JoranAngevaare in https://github.com/AxFoundation/strax/pull/698
 * Fix overflow bug in sort_by_time add little test by @WenzDaniel in https://github.com/AxFoundation/strax/pull/695
 * Refactor in preparation for PyMongo 4.0 by @JoranAngevaare in https://github.com/AxFoundation/strax/pull/656
 * Plugin log property by @jmosbacher in https://github.com/AxFoundation/strax/pull/588
```

### Comparing `strax-1.4.3/LICENSE` & `strax-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/PKG-INFO` & `strax-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strax
-Version: 1.4.3
+Version: 1.5.0
 Summary: Streaming analysis for xenon TPCs
 Home-page: https://github.com/AxFoundation/strax
 Author: Jelle Aalbers
 License: UNKNOWN
 Description: # strax
         Streaming analysis for xenon experiments
         
@@ -22,51 +22,61 @@
         
         Strax is an analysis framework for pulse-only digitization data, specialized for live data reduction at speeds of 50-100 MB(raw) / core / sec. For more information, please see the [strax documentation](https://strax.readthedocs.io).
         
         Strax' primary aim is to support noble liquid TPC dark matter searches, such as XENONnT. The XENON-specific algorithms live in the separate package [straxen](https://github.com/XENONnT/straxen). If you want to try out strax, you probably want to start there. This package only contains the core framework and basic algorithms any TPCs would want to use.
         
         
         
+        1.5.0 / 2023-05-02
+        ---------------------
+        * Fix ipython version by @dachengx in https://github.com/AxFoundation/strax/pull/719
+        * Do not change channel when sort_by_time by @dachengx in https://github.com/AxFoundation/strax/pull/718
+        * Save hits level information(hits time difference) in peaks by @dachengx in https://github.com/AxFoundation/strax/pull/716
+        
+        **Full Changelog**: https://github.com/AxFoundation/strax/compare/v1.4.3...v1.5.0
+        
+        
         1.4.3 / 2023-04-22
         ---------------------
         * Select max gaps from positive gaps by @dachengx in https://github.com/AxFoundation/strax/pull/708
         
         New Contributors
         * @dachengx made their first contribution in https://github.com/AxFoundation/strax/pull/708
         
         **Full Changelog**: https://github.com/AxFoundation/strax/compare/v1.4.2...v1.4.3
         
+        
         1.4.2 / 2023-03-08
         ---------------------
         * Patch md access in the rechunker by @JoranAngevaare in https://github.com/AxFoundation/strax/pull/711
         * Raise compression errors if unable by @JoranAngevaare in https://github.com/AxFoundation/strax/pull/714
         
-        
         **Full Changelog**: https://github.com/AxFoundation/strax/compare/v1.4.1...v1.4.2
         
         
         1.4.1 / 2023-02-13
         ---------------------
         * Rechunker using Mailbox by @JoranAngevaare in https://github.com/AxFoundation/strax/pull/710
         
-        
         **Full Changelog**: https://github.com/AxFoundation/strax/compare/v1.4.0...v1.4.1
         
+        
         1.4.0 / 2022-10-17
         ---------------------
         * Add capability for building summed waveform over channel subset by @DCichon in https://github.com/AxFoundation/strax/pull/565
         * Fixed delta peak timestamp problem by @FaroutYLq in https://github.com/AxFoundation/strax/pull/702
         
         Notes
          -  Breaking changes in the peak-building chain due to #565
         New Contributors
          - @DCichon made their first contribution in https://github.com/AxFoundation/strax/pull/565
         
         **Full Changelog**: https://github.com/AxFoundation/strax/compare/v1.3.0...v1.4.0
         
+        
         1.3.0 / 2022-09-09
         ---------------------
         * Restructure plugins by @JoranAngevaare in https://github.com/AxFoundation/strax/pull/700
         * Numpy caching of data in online monitor storage by @JoranAngevaare in https://github.com/AxFoundation/strax/pull/698
         * Fix overflow bug in sort_by_time add little test by @WenzDaniel in https://github.com/AxFoundation/strax/pull/695
         * Refactor in preparation for PyMongo 4.0 by @JoranAngevaare in https://github.com/AxFoundation/strax/pull/656
         * Plugin log property by @jmosbacher in https://github.com/AxFoundation/strax/pull/588
```

### Comparing `strax-1.4.3/README.md` & `strax-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/bin/rechunker` & `strax-1.5.0/bin/rechunker`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/setup.py` & `strax-1.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 with open('README.md') as file:
     readme = file.read()
 
 with open('HISTORY.md') as file:
     history = file.read()
 
 setuptools.setup(name='strax',
-                 version='1.4.3',
+                 version='1.5.0',
                  description='Streaming analysis for xenon TPCs',
                  author='Jelle Aalbers',
                  url='https://github.com/AxFoundation/strax',
                  setup_requires=['pytest-runner'],
                  install_requires=requires,
                  tests_require=requires + tests_requires,
                  long_description=readme + '\n\n' + history,
```

### Comparing `strax-1.4.3/strax/__init__.py` & `strax-1.5.0/strax/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # flake8: noqa
-__version__ = '1.4.3'
+__version__ = '1.5.0'
 
 # Glue the package together
 # See https://www.youtube.com/watch?v=0oTh1CXRaQ0 if this confuses you
 # The order of subpackes is not invariant, since we use strax.xxx inside strax
 from .utils import *
 from .chunk import *
 from .dtypes import *
```

### Comparing `strax-1.4.3/strax/chunk.py` & `strax-1.5.0/strax/chunk.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/strax/config.py` & `strax-1.5.0/strax/config.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/strax/context.py` & `strax-1.5.0/strax/context.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/strax/corrections.py` & `strax-1.5.0/strax/corrections.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/strax/dtypes.py` & `strax-1.5.0/strax/dtypes.py`

 * *Files 4% similar despite different names*

```diff
@@ -162,31 +162,35 @@
     """
     if n_samples < 2:
         raise ValueError('n_samples must be at least 2!')
 
     dtype = hitlet_dtype()
     additional_fields = [(('Hitlet data in PE/sample with ZLE (only the first length samples are filled)', 'data'),
                            np.float32, n_samples),
-                         (('Dummy field required for splitting',
+                         (('Dummy max_gap required for splitting',
                            'max_gap'), np.int32),
+                         (('Dummy max_diff required for splitting',
+                           'max_diff'), np.int32),
+                         (('Dummy min_diff required for splitting',
+                           'min_diff'), np.int32),
                          (('Maximum interior goodness of split',
                            'max_goodness_of_split'), np.float32),
                          ]
 
     return dtype + additional_fields
 
 
-def peak_dtype(n_channels=100, n_sum_wv_samples=200, n_widths=11, digitize_top=True):
+def peak_dtype(n_channels=100, n_sum_wv_samples=200, n_widths=11, digitize_top=True, hits_timing=True):
     """Data type for peaks - ranges across all channels in a detector
     Remember to set channel to -1 (todo: make enum)
     """
     if n_channels == 1:
         raise ValueError("Must have more than one channel")
         # Otherwise array changes shape?? badness ensues
-    dtype =  peak_interval_dtype + [
+    dtype = peak_interval_dtype + [
         # For peaklets this is likely to be overwritten:
         (('Classification of the peak(let)',
           'type'), np.int8),
         (('Integral across channels [PE]',
           'area'), np.float32),
         (('Integral per channel [PE]',
           'area_per_channel'), np.float32, n_channels),
@@ -205,18 +209,25 @@
         (('Channel within tight range of mean',
           'tight_coincidence'), np.int16),
         (('Largest gap between hits inside peak [ns]',
           'max_gap'), np.int32),
         (('Maximum interior goodness of split',
           'max_goodness_of_split'), np.float32),
     ]
+    if hits_timing:
+        dtype += [
+            (('Largest time difference between apexes of hits inside peak [ns]',
+              'max_diff'), np.int32),
+            (('Smallest time difference between apexes of hits inside peak [ns]',
+              'min_diff'), np.int32),
+        ]
     if digitize_top:
         top_field = (('Waveform data in PE/sample (not PE/ns!), top array',
                       'data_top'), np.float32, n_sum_wv_samples)
-        dtype.insert(5, top_field)
+        dtype.insert(9, top_field)
     return dtype
 
 
 def copy_to_buffer(source: np.ndarray,
                    buffer: np.ndarray,
                    func_name: str,
                    field_names: ty.Tuple[str] = None):
```

### Comparing `strax-1.4.3/strax/io.py` & `strax-1.5.0/strax/io.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/strax/mailbox.py` & `strax-1.5.0/strax/mailbox.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/strax/plugins/cut_plugin.py` & `strax-1.5.0/strax/plugins/cut_plugin.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/strax/plugins/loop_plugin.py` & `strax-1.5.0/strax/plugins/loop_plugin.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/strax/plugins/merge_only_plugin.py` & `strax-1.5.0/strax/plugins/merge_only_plugin.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/strax/plugins/overlap_window_plugin.py` & `strax-1.5.0/strax/plugins/overlap_window_plugin.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/strax/plugins/parrallel_source_plugin.py` & `strax-1.5.0/strax/plugins/parrallel_source_plugin.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/strax/plugins/plugin.py` & `strax-1.5.0/strax/plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/strax/processing/data_reduction.py` & `strax-1.5.0/strax/processing/data_reduction.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/strax/processing/general.py` & `strax-1.5.0/strax/processing/general.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,23 +12,23 @@
 @export
 def sort_by_time(x):
     """Sorts things. Either by time or by time, then channel if both
     fields are in the given array.
     """
     if len(x) == 0:
         return x
-    
+
     if 'channel' in x.dtype.names:
         min_channel = x['channel'].min()
-        channel = x['channel']
+        channel = x['channel'].copy()
         if min_channel < 0:
             channel -= min_channel
     else:
         channel = np.ones(len(x))
-        
+
     max_time_difference = (np.iinfo(np.int64).max - 10) / (channel.max()+1)
     # Subtract 10 to have some extra margin, just in case.
     # Use absolute to account for peaks which are channel -1.
     _time_range_too_large = (x['time'].max() - x['time'].min()) > max_time_difference
     if not _time_range_too_large:
         # Faster sorting:
         x = _sort_by_time_and_channel(x, channel, channel.max()+1)
```

### Comparing `strax-1.4.3/strax/processing/hitlets.py` & `strax-1.5.0/strax/processing/hitlets.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/strax/processing/peak_building.py` & `strax-1.5.0/strax/processing/peak_building.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/strax/processing/peak_merging.py` & `strax-1.5.0/strax/processing/peak_merging.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/strax/processing/peak_properties.py` & `strax-1.5.0/strax/processing/peak_properties.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/strax/processing/peak_splitting.py` & `strax-1.5.0/strax/processing/peak_splitting.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,15 +154,18 @@
                 r['time'] = p['time'] + prev_split_i * p['dt']
                 r['channel'] = p['channel']
                 # Set the dt to the original (lowest) dt first;
                 # this may change when the sum waveform of the new peak
                 # is computed
                 r['dt'] = orig_dt
                 r['length'] = (split_i - prev_split_i) * p['dt'] / orig_dt
-                r['max_gap'] = -1  # Too lazy to compute this
+                # Too lazy to compute these
+                r['max_gap'] = -1
+                r['max_diff'] = -1
+                r['min_diff'] = -1
                 if r['length'] <= 0:
                     print(p['data'])
                     print(prev_split_i, split_i)
                     raise ValueError("Attempt to create invalid peak!")
 
                 offset += 1
                 if offset == len(new_peaks):
```

### Comparing `strax-1.4.3/strax/processing/pulse_processing.py` & `strax-1.5.0/strax/processing/pulse_processing.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/strax/processing/statistics.py` & `strax-1.5.0/strax/processing/statistics.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/strax/processor.py` & `strax-1.5.0/strax/processor.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/strax/run_selection.py` & `strax-1.5.0/strax/run_selection.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/strax/storage/common.py` & `strax-1.5.0/strax/storage/common.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/strax/storage/file_rechunker.py` & `strax-1.5.0/strax/storage/file_rechunker.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/strax/storage/files.py` & `strax-1.5.0/strax/storage/files.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/strax/storage/mongo.py` & `strax-1.5.0/strax/storage/mongo.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/strax/storage/zipfiles.py` & `strax-1.5.0/strax/storage/zipfiles.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/strax/testutils.py` & `strax-1.5.0/strax/testutils.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/strax/utils.py` & `strax-1.5.0/strax/utils.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/strax.egg-info/PKG-INFO` & `strax-1.5.0/strax.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strax
-Version: 1.4.3
+Version: 1.5.0
 Summary: Streaming analysis for xenon TPCs
 Home-page: https://github.com/AxFoundation/strax
 Author: Jelle Aalbers
 License: UNKNOWN
 Description: # strax
         Streaming analysis for xenon experiments
         
@@ -22,51 +22,61 @@
         
         Strax is an analysis framework for pulse-only digitization data, specialized for live data reduction at speeds of 50-100 MB(raw) / core / sec. For more information, please see the [strax documentation](https://strax.readthedocs.io).
         
         Strax' primary aim is to support noble liquid TPC dark matter searches, such as XENONnT. The XENON-specific algorithms live in the separate package [straxen](https://github.com/XENONnT/straxen). If you want to try out strax, you probably want to start there. This package only contains the core framework and basic algorithms any TPCs would want to use.
         
         
         
+        1.5.0 / 2023-05-02
+        ---------------------
+        * Fix ipython version by @dachengx in https://github.com/AxFoundation/strax/pull/719
+        * Do not change channel when sort_by_time by @dachengx in https://github.com/AxFoundation/strax/pull/718
+        * Save hits level information(hits time difference) in peaks by @dachengx in https://github.com/AxFoundation/strax/pull/716
+        
+        **Full Changelog**: https://github.com/AxFoundation/strax/compare/v1.4.3...v1.5.0
+        
+        
         1.4.3 / 2023-04-22
         ---------------------
         * Select max gaps from positive gaps by @dachengx in https://github.com/AxFoundation/strax/pull/708
         
         New Contributors
         * @dachengx made their first contribution in https://github.com/AxFoundation/strax/pull/708
         
         **Full Changelog**: https://github.com/AxFoundation/strax/compare/v1.4.2...v1.4.3
         
+        
         1.4.2 / 2023-03-08
         ---------------------
         * Patch md access in the rechunker by @JoranAngevaare in https://github.com/AxFoundation/strax/pull/711
         * Raise compression errors if unable by @JoranAngevaare in https://github.com/AxFoundation/strax/pull/714
         
-        
         **Full Changelog**: https://github.com/AxFoundation/strax/compare/v1.4.1...v1.4.2
         
         
         1.4.1 / 2023-02-13
         ---------------------
         * Rechunker using Mailbox by @JoranAngevaare in https://github.com/AxFoundation/strax/pull/710
         
-        
         **Full Changelog**: https://github.com/AxFoundation/strax/compare/v1.4.0...v1.4.1
         
+        
         1.4.0 / 2022-10-17
         ---------------------
         * Add capability for building summed waveform over channel subset by @DCichon in https://github.com/AxFoundation/strax/pull/565
         * Fixed delta peak timestamp problem by @FaroutYLq in https://github.com/AxFoundation/strax/pull/702
         
         Notes
          -  Breaking changes in the peak-building chain due to #565
         New Contributors
          - @DCichon made their first contribution in https://github.com/AxFoundation/strax/pull/565
         
         **Full Changelog**: https://github.com/AxFoundation/strax/compare/v1.3.0...v1.4.0
         
+        
         1.3.0 / 2022-09-09
         ---------------------
         * Restructure plugins by @JoranAngevaare in https://github.com/AxFoundation/strax/pull/700
         * Numpy caching of data in online monitor storage by @JoranAngevaare in https://github.com/AxFoundation/strax/pull/698
         * Fix overflow bug in sort_by_time add little test by @WenzDaniel in https://github.com/AxFoundation/strax/pull/695
         * Refactor in preparation for PyMongo 4.0 by @JoranAngevaare in https://github.com/AxFoundation/strax/pull/656
         * Plugin log property by @jmosbacher in https://github.com/AxFoundation/strax/pull/588
```

### Comparing `strax-1.4.3/strax.egg-info/SOURCES.txt` & `strax-1.5.0/strax.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/tests/test_child_plugins.py` & `strax-1.5.0/tests/test_child_plugins.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/tests/test_config.py` & `strax-1.5.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/tests/test_context.py` & `strax-1.5.0/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/tests/test_core.py` & `strax-1.5.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/tests/test_corrections.py` & `strax-1.5.0/tests/test_corrections.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/tests/test_cut_plugin.py` & `strax-1.5.0/tests/test_cut_plugin.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/tests/test_data_reduction.py` & `strax-1.5.0/tests/test_data_reduction.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/tests/test_fixed_plugin_cache.py` & `strax-1.5.0/tests/test_fixed_plugin_cache.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/tests/test_general_processing.py` & `strax-1.5.0/tests/test_general_processing.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/tests/test_get_zarr.py` & `strax-1.5.0/tests/test_get_zarr.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/tests/test_helpers.py` & `strax-1.5.0/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/tests/test_hitlet.py` & `strax-1.5.0/tests/test_hitlet.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/tests/test_inline_plugin.py` & `strax-1.5.0/tests/test_inline_plugin.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/tests/test_lone_hit_integration.py` & `strax-1.5.0/tests/test_lone_hit_integration.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/tests/test_loop_plugins.py` & `strax-1.5.0/tests/test_loop_plugins.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/tests/test_mailbox.py` & `strax-1.5.0/tests/test_mailbox.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/tests/test_mongo_frontend.py` & `strax-1.5.0/tests/test_mongo_frontend.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/tests/test_multi_output.py` & `strax-1.5.0/tests/test_multi_output.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/tests/test_overlap_plugin.py` & `strax-1.5.0/tests/test_overlap_plugin.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/tests/test_peak_merging.py` & `strax-1.5.0/tests/test_peak_merging.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/tests/test_peak_processing.py` & `strax-1.5.0/tests/test_peak_processing.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/tests/test_peak_properties.py` & `strax-1.5.0/tests/test_peak_properties.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/tests/test_peak_splitting.py` & `strax-1.5.0/tests/test_peak_splitting.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/tests/test_pulse_processing.py` & `strax-1.5.0/tests/test_pulse_processing.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/tests/test_saving.py` & `strax-1.5.0/tests/test_saving.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/tests/test_statistics.py` & `strax-1.5.0/tests/test_statistics.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/tests/test_storage.py` & `strax-1.5.0/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/tests/test_superruns.py` & `strax-1.5.0/tests/test_superruns.py`

 * *Files identical despite different names*

### Comparing `strax-1.4.3/tests/test_utils.py` & `strax-1.5.0/tests/test_utils.py`

 * *Files identical despite different names*

