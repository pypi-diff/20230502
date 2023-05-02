# Comparing `tmp/ephysiopy-1.9.13.tar.gz` & `tmp/ephysiopy-1.9.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ephysiopy-1.9.13.tar", last modified: Fri Apr 21 16:30:23 2023, max compression
+gzip compressed data, was "ephysiopy-1.9.15.tar", last modified: Tue May  2 11:59:17 2023, max compression
```

## Comparing `ephysiopy-1.9.13.tar` & `ephysiopy-1.9.15.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:30:23.399461 ephysiopy-1.9.13/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-21 16:30:14.000000 ephysiopy-1.9.13/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-21 16:30:14.000000 ephysiopy-1.9.13/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-04-21 16:30:23.399461 ephysiopy-1.9.13/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-21 16:30:14.000000 ephysiopy-1.9.13/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:30:23.395461 ephysiopy-1.9.13/ephysiopy/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-21 16:30:14.000000 ephysiopy-1.9.13/ephysiopy/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-21 16:30:14.000000 ephysiopy-1.9.13/ephysiopy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:30:23.395461 ephysiopy-1.9.13/ephysiopy/axona/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 16:30:14.000000 ephysiopy-1.9.13/ephysiopy/axona/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19336 2023-04-21 16:30:14.000000 ephysiopy-1.9.13/ephysiopy/axona/axonaIO.py
--rw-r--r--   0 runner    (1001) docker     (123)    11999 2023-04-21 16:30:14.000000 ephysiopy-1.9.13/ephysiopy/axona/file_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-21 16:30:14.000000 ephysiopy-1.9.13/ephysiopy/axona/tetrode_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-21 16:30:14.000000 ephysiopy-1.9.13/ephysiopy/axona/tintcolours.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:30:23.395461 ephysiopy-1.9.13/ephysiopy/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 16:30:14.000000 ephysiopy-1.9.13/ephysiopy/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31379 2023-04-21 16:30:14.000000 ephysiopy-1.9.13/ephysiopy/common/binning.py
--rw-r--r--   0 runner    (1001) docker     (123)    21358 2023-04-21 16:30:14.000000 ephysiopy-1.9.13/ephysiopy/common/ephys_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    40221 2023-04-21 16:30:14.000000 ephysiopy-1.9.13/ephysiopy/common/fieldcalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7148 2023-04-21 16:30:14.000000 ephysiopy-1.9.13/ephysiopy/common/gridcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-04-21 16:30:14.000000 ephysiopy-1.9.13/ephysiopy/common/mle_von_mises_vals.py
--rw-r--r--   0 runner    (1001) docker     (123)    49463 2023-04-21 16:30:14.000000 ephysiopy-1.9.13/ephysiopy/common/phasecoding.py
--rw-r--r--   0 runner    (1001) docker     (123)    24931 2023-04-21 16:30:14.000000 ephysiopy-1.9.13/ephysiopy/common/rhythmicity.py
--rw-r--r--   0 runner    (1001) docker     (123)    28784 2023-04-21 16:30:14.000000 ephysiopy-1.9.13/ephysiopy/common/spikecalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-04-21 16:30:14.000000 ephysiopy-1.9.13/ephysiopy/common/statscalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-04-21 16:30:14.000000 ephysiopy-1.9.13/ephysiopy/common/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:30:23.395461 ephysiopy-1.9.13/ephysiopy/format_converters/
--rw-r--r--   0 runner    (1001) docker     (123)    19711 2023-04-21 16:30:14.000000 ephysiopy-1.9.13/ephysiopy/format_converters/OE_Axona.py
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-04-21 16:30:14.000000 ephysiopy-1.9.13/ephysiopy/format_converters/OE_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 16:30:14.000000 ephysiopy-1.9.13/ephysiopy/format_converters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:30:23.399461 ephysiopy-1.9.13/ephysiopy/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 16:30:14.000000 ephysiopy-1.9.13/ephysiopy/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23342 2023-04-21 16:30:14.000000 ephysiopy-1.9.13/ephysiopy/io/recording.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:30:23.399461 ephysiopy-1.9.13/ephysiopy/openephys2py/
--rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-04-21 16:30:14.000000 ephysiopy-1.9.13/ephysiopy/openephys2py/KiloSort.py
--rw-r--r--   0 runner    (1001) docker     (123)    10490 2023-04-21 16:30:14.000000 ephysiopy-1.9.13/ephysiopy/openephys2py/OESettings.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 16:30:14.000000 ephysiopy-1.9.13/ephysiopy/openephys2py/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:30:23.399461 ephysiopy-1.9.13/ephysiopy/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 16:30:14.000000 ephysiopy-1.9.13/ephysiopy/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-21 16:30:14.000000 ephysiopy-1.9.13/ephysiopy/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-21 16:30:15.000000 ephysiopy-1.9.13/ephysiopy/tests/test_axona_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-04-21 16:30:15.000000 ephysiopy-1.9.13/ephysiopy/tests/test_axona_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-04-21 16:30:15.000000 ephysiopy-1.9.13/ephysiopy/tests/test_binning.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-04-21 16:30:15.000000 ephysiopy-1.9.13/ephysiopy/tests/test_dacq2py.py
--rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-04-21 16:30:15.000000 ephysiopy-1.9.13/ephysiopy/tests/test_ephys_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-04-21 16:30:15.000000 ephysiopy-1.9.13/ephysiopy/tests/test_fieldcalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-21 16:30:15.000000 ephysiopy-1.9.13/ephysiopy/tests/test_gridcell.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-21 16:30:15.000000 ephysiopy-1.9.13/ephysiopy/tests/test_openephys.py
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-04-21 16:30:15.000000 ephysiopy-1.9.13/ephysiopy/tests/test_phasecoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-04-21 16:30:15.000000 ephysiopy-1.9.13/ephysiopy/tests/test_rhythmicity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-04-21 16:30:15.000000 ephysiopy-1.9.13/ephysiopy/tests/test_spikecalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-21 16:30:15.000000 ephysiopy-1.9.13/ephysiopy/tests/test_statscalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-21 16:30:15.000000 ephysiopy-1.9.13/ephysiopy/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:30:23.399461 ephysiopy-1.9.13/ephysiopy/visualise/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 16:30:15.000000 ephysiopy-1.9.13/ephysiopy/visualise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32289 2023-04-21 16:30:15.000000 ephysiopy-1.9.13/ephysiopy/visualise/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:30:23.395461 ephysiopy-1.9.13/ephysiopy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-04-21 16:30:23.000000 ephysiopy-1.9.13/ephysiopy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-04-21 16:30:23.000000 ephysiopy-1.9.13/ephysiopy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 16:30:23.000000 ephysiopy-1.9.13/ephysiopy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-21 16:30:23.000000 ephysiopy-1.9.13/ephysiopy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-21 16:30:23.000000 ephysiopy-1.9.13/ephysiopy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-21 16:30:23.399461 ephysiopy-1.9.13/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-21 16:30:15.000000 ephysiopy-1.9.13/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:59:17.364166 ephysiopy-1.9.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-05-02 11:59:17.364166 ephysiopy-1.9.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:59:17.360166 ephysiopy-1.9.15/ephysiopy/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:59:17.360166 ephysiopy-1.9.15/ephysiopy/axona/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/axona/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19336 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/axona/axonaIO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11999 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/axona/file_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/axona/tetrode_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/axona/tintcolours.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:59:17.360166 ephysiopy-1.9.15/ephysiopy/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34032 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/common/binning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21358 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/common/ephys_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40221 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/common/fieldcalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/common/gridcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/common/mle_von_mises_vals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49500 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/common/phasecoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24931 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/common/rhythmicity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28784 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/common/spikecalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/common/statscalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/common/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:59:17.360166 ephysiopy-1.9.15/ephysiopy/format_converters/
+-rw-r--r--   0 runner    (1001) docker     (123)    19711 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/format_converters/OE_Axona.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/format_converters/OE_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/format_converters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:59:17.360166 ephysiopy-1.9.15/ephysiopy/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23796 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/io/recording.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:59:17.360166 ephysiopy-1.9.15/ephysiopy/openephys2py/
+-rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/openephys2py/KiloSort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10490 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/openephys2py/OESettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/openephys2py/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:59:17.364166 ephysiopy-1.9.15/ephysiopy/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/tests/test_axona_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/tests/test_axona_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/tests/test_binning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/tests/test_dacq2py.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/tests/test_ephys_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/tests/test_fieldcalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/tests/test_gridcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/tests/test_openephys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/tests/test_phasecoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/tests/test_rhythmicity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/tests/test_spikecalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/tests/test_statscalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:59:17.364166 ephysiopy-1.9.15/ephysiopy/visualise/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/visualise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32402 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/visualise/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:59:17.360166 ephysiopy-1.9.15/ephysiopy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-05-02 11:59:17.000000 ephysiopy-1.9.15/ephysiopy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-02 11:59:17.000000 ephysiopy-1.9.15/ephysiopy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 11:59:17.000000 ephysiopy-1.9.15/ephysiopy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-02 11:59:17.000000 ephysiopy-1.9.15/ephysiopy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-02 11:59:17.000000 ephysiopy-1.9.15/ephysiopy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-02 11:59:17.364166 ephysiopy-1.9.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/setup.py
```

### Comparing `ephysiopy-1.9.13/LICENSE` & `ephysiopy-1.9.15/LICENSE`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.13/PKG-INFO` & `ephysiopy-1.9.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ephysiopy
-Version: 1.9.13
+Version: 1.9.15
 Summary: Analysis of electrophysiology data
 Home-page: https://github.com/rhayman/ephysiopy
 Author: Robin Hayman
 Author-email: robin.hayman@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ephysiopy-1.9.13/README.md` & `ephysiopy-1.9.15/README.md`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.13/ephysiopy/axona/axonaIO.py` & `ephysiopy-1.9.15/ephysiopy/axona/axonaIO.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.13/ephysiopy/axona/file_headers.py` & `ephysiopy-1.9.15/ephysiopy/axona/file_headers.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.13/ephysiopy/axona/tetrode_dict.py` & `ephysiopy-1.9.15/ephysiopy/axona/tetrode_dict.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.13/ephysiopy/axona/tintcolours.py` & `ephysiopy-1.9.15/ephysiopy/axona/tintcolours.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.13/ephysiopy/common/binning.py` & `ephysiopy-1.9.15/ephysiopy/common/binning.py`

 * *Files 8% similar despite different names*

```diff
@@ -77,30 +77,34 @@
         self,
         xy: np.array = None,
         hdir: np.array = None,
         speed: np.array = None,
         pos_weights: np.array = None,
         ppm: int = 430,
         xyInCms: bool = False,
-        cmsPerBin: int = 3,
+        binsize: int = 3,
         smooth_sz: int = 5,
     ):
         self.xy = xy
         self.dir = hdir
         self.speed = speed
         self._pos_weights = pos_weights
         self._ppm = ppm  # pixels per metre
-        self._cmsPerBin = cmsPerBin
+        self._binsize = binsize
         self._inCms = xyInCms
-        self._binsize = None  # has setter and getter - see below
+        self._nBins = None
+        self._binedges = None  # has setter and getter - see below
         self._x_lims = None
         self._y_lims = None
         self._smooth_sz = smooth_sz
         self._smoothingType = "gaussian"  # 'boxcar' or 'gaussian'
         self.whenToSmooth = "before"  # or 'after'
+        self._var2Bin = VariableToBin.XY
+        self._mapType = MapType.RATE
+        self._calcBinEdges()
 
     @property
     def inCms(self):
         # Whether the units are in cms or not
         return self._inCms
 
     @inCms.setter
@@ -111,26 +115,74 @@
     def ppm(self):
         # Get the current pixels per metre (ppm)
         return self._ppm
 
     @ppm.setter
     def ppm(self, value):
         self._ppm = value
-        self._binsize = self._calcBinSize(self.cmsPerBin)
+        # self._binedges = self._calcBinEdges(self.binsize)
 
     @property
-    def binsize(self):
-        # Returns binsize calculated in _calcBinSize and based on cmsPerBin
-        if self._binsize is None:
-            self._binsize = self._calcBinSize(self.cmsPerBin)
-        return self._binsize
+    def var2Bin(self):
+        return self._var2Bin
 
-    @binsize.setter
-    def binsize(self, value):
-        self._binsize = value
+    @var2Bin.setter
+    def var2Bin(self, value):
+        self._var2Bin = value
+        # self._calcBinEdges()
+
+    @property
+    def mapType(self):
+        return self._mapType
+
+    @mapType.setter
+    def mapType(self, value):
+        self._mapType = value
+
+    @property
+    def nBins(self):
+        '''
+        The number of bins for each dim
+        '''
+        if self.binsize:
+            return len(self._binedges[0]), len(self._binedges[1])
+        else:
+            return None
+
+    @nBins.setter
+    def nBins(self, value):
+        '''
+        Sets the number of bins
+        '''
+        if self.var2Bin == VariableToBin.XY:
+            x_lims, y_lims = self._getXYLimits()
+            if len(value) == 1:
+                _x = np.linspace(x_lims[0], x_lims[1], int(value[0]))
+                _y = np.linspace(y_lims[0], y_lims[1], int(value[0]))
+            elif len(value) == 2:
+                _x = np.linspace(x_lims[0], x_lims[1], int(value[0]))
+                _y = np.linspace(y_lims[0], y_lims[1], int(value[1]))
+            self._binedges = _y, _x
+        elif self.var2Bin == VariableToBin.DIR:
+            self._binedges = [np.linspace(0, 360 + self.binsize, value[0])]
+        elif self.var2Bin == VariableToBin.SPEED:
+            maxspeed = np.max(self.speed)
+            self._binedges = [np.linspace(0, maxspeed, value[0])]
+        self._calcBinDims()
+
+    @property
+    def binedges(self):
+        # Returns binedges calculated in _calcBinEdges and based on cmsPerBin
+        # if self._binedges is None:
+        #     self._binedges = self._calcBinEdges(self.binsize)
+        return self._binedges
+
+    @binedges.setter
+    def binedges(self, value):
+        self._binedges = value
 
     @property
     def x_lims(self):
         return self._x_lims
 
     @x_lims.setter
     def x_lims(self, value):
@@ -158,22 +210,22 @@
         return self._pos_weights
 
     @pos_weights.setter
     def pos_weights(self, value):
         self._pos_weights = value
 
     @property
-    def cmsPerBin(self):
+    def binsize(self):
         # The number of cms per bin of the binned up map
-        return self._cmsPerBin
+        return self._binsize
 
-    @cmsPerBin.setter
-    def cmsPerBin(self, value):
-        self._cmsPerBin = value
-        self._binsize = self._calcBinSize(self.cmsPerBin)
+    @binsize.setter
+    def binsize(self, value):
+        self._binsize = value
+        self._binedges = self._calcBinEdges(self.binsize)
 
     @property
     def smooth_sz(self):
         # The size of the smoothing window applied to the binned data
         return self._smooth_sz
 
     @smooth_sz.setter
@@ -185,114 +237,143 @@
         # The type of smoothing to do - legal values are 'boxcar' or 'gaussian'
         return self._smoothingType
 
     @smoothingType.setter
     def smoothingType(self, value):
         self._smoothingType = value
 
-    def _calcBinSize(self, cmsPerBin: int = 3) -> tuple:
-        """
-        Aims to get the right number of bins for x and y dims given the ppm
-        in the set header and the x and y extent
-
-        Parameters
-        ----------
-        cmsPerBin : int, optional, default = 3
-            The number of cms per bin OR degrees for directional binning
-
-        Returns
-        -------
-        2-tuple: each member an array of bin edges for x and y
-        """
+    def _getXYLimits(self):
+        '''
+        Gets the min/max of the x/y data
+        '''
         x_lims = getattr(self, "x_lims", None)
         y_lims = getattr(self, "y_lims", None)
         if x_lims is None:
             x_lims = (np.nanmin(self.xy[0]), np.nanmax(self.xy[0]))
         if y_lims is None:
             y_lims = (np.nanmin(self.xy[1]), np.nanmax(self.xy[1]))
+        self.x_lims = x_lims
+        self.y_lims = y_lims
+        return x_lims, y_lims
+
+    def _calcBinDims(self):
+        try:
+            self._binDims = [len(b) for b in self._binedges]
+        except TypeError:
+            self._binDims = len(self._binedges)
 
-        n_x = np.ceil((x_lims[1] - x_lims[0]) / cmsPerBin)
-        n_y = np.ceil((y_lims[1] - y_lims[0]) / cmsPerBin)
-        _x = np.linspace(x_lims[0], x_lims[1], int(n_x))
-        _y = np.linspace(y_lims[0], y_lims[1], int(n_y))
+    def _calcBinEdges(self, binsize: int = 3) -> tuple:
+        """
+        Aims to get the right number of bins for the variable to be
+        binned
 
-        return _y, _x
+        Parameters
+        ----------
+        binsize : int, optional, default = 3
+            The number of cms per bin for XY
+            OR degrees for DIR
+            OR cm/s for SPEED
 
-    def getMap(self, spkWeights, varType="xy", mapType="rate", smoothing=True):
+        Returns
+        -------
+        tuple: each member an array of bin edges
+        """
+        if self.var2Bin == VariableToBin.DIR:
+            self.binedges = np.arange(0, 360 + binsize, binsize)
+        elif self.var2Bin == VariableToBin.SPEED:
+            maxspeed = np.max(self.speed)
+            # assume min speed = 0
+            self.binedges = np.arange(0, maxspeed, binsize)
+        else:  # self.var2Bin == VariableToBin.XY:
+            x_lims, y_lims = self._getXYLimits()
+            n_x = np.ceil((x_lims[1] - x_lims[0]) / binsize)
+            n_y = np.ceil((y_lims[1] - y_lims[0]) / binsize)
+            _x = np.linspace(x_lims[0], x_lims[1], int(n_x))
+            _y = np.linspace(y_lims[0], y_lims[1], int(n_y))
+            self.binedges = _y, _x
+        self._calcBinDims()
+        return self.binedges
+
+    def getMap(self, spkWeights,
+               varType=VariableToBin.XY,
+               mapType=MapType.RATE,
+               smoothing=True):
         """
         Bins up the variable type varType and returns a tuple of
         (rmap, binnedPositionDir) or
         (rmap, binnedPostionX, binnedPositionY)
 
         Parameters
         ----------
         spkWeights : array_like
             Shape equal to number of positions samples captured and consists of
             position weights. For example, if there were 5 positions
             recorded and a cell spiked once in position 2 and 5 times in
             position 3 and nothing anywhere else then pos_weights looks
             like: [0 0 1 5 0]
-        varType : str, optional, default 'xy'
-            The variable to bin up. Legal values are: 'xy', 'dir', and 'speed'
-        mapType : str, optional, default 'rate'
-            If 'rate' then the binned up spikes are divided by varType.
-            Otherwise return binned up position. Options are 'rate' or 'pos'
+        varType : Enum value - see Variable2Bin defined at top of this file
+            The variable to bin up. Legal values are: XY, DIR and SPEED
+        mapType : enum value - see MapType defined at top of this file
+            If RATE then the binned up spikes are divided by varType.
+            Otherwise return binned up position. Options are RATE or POS
         smoothing : bool, optional, default True
             Whether to smooth the data or not
 
         Returns
         -------
         binned_data, binned_pos : tuple
             This is either a 2-tuple or a 3-tuple depening on whether binned
             pos (mapType 'pos') or binned spikes (mapType 'rate') is asked
             for respectively
 
         """
-        sample = getattr(self, varType, "xy")
+        if varType == VariableToBin.DIR:
+            sample = self.dir
+        elif varType == VariableToBin.SPEED:
+            sample = self.speed
+        elif varType == VariableToBin.XY:
+            sample = self.xy
+        else:
+            raise ValueError("Unrecognized variable to bin.")
         assert sample is not None
-        # might happen if head direction not supplied for example
 
-        if "xy" in varType:
-            self.binsize = self._calcBinSize(self.cmsPerBin)
-        elif "dir" in varType:
-            self.binsize = np.arange(0, 360 + self.cmsPerBin, self.cmsPerBin)
-        elif "speed" in varType:
-            self.binsize = np.arange(0, 50, 1)
+        self.var2Bin = varType
+        self._calcBinEdges(self.binsize)
 
         binned_pos, binned_pos_edges = self._binData(
                                                      sample,
-                                                     self.binsize,
+                                                     self._binedges,
                                                      self.pos_weights)
         nanIdx = binned_pos == 0
 
-        if "pos" in mapType:  # return just binned up position
+        if mapType == MapType.POS:  # return just binned up position
             if smoothing:
-                if "dir" in varType:
+                if varType == VariableToBin.DIR:
                     binned_pos = self._circPadSmooth(
                         binned_pos, n=self.smooth_sz)
                 else:
                     binned_pos = blurImage(
                         binned_pos, self.smooth_sz, ftype=self.smoothingType
                     )
             return binned_pos, binned_pos_edges
 
-        binned_spk, _ = self._binData(sample, self.binsize, spkWeights)
+        binned_spk, _ = self._binData(sample, self._binedges, spkWeights)
         # binned_spk is returned as a tuple of the binned data and the bin
         # edges
         if "after" in self.whenToSmooth:
             rmap = binned_spk / binned_pos
-            if "dir" in varType:
+            if varType == VariableToBin.DIR:
                 rmap = self._circPadSmooth(rmap, self.smooth_sz)
             else:
                 rmap = blurImage(
                     rmap, self.smooth_sz, ftype=self.smoothingType)
         else:  # default case
             if not smoothing:
                 return binned_spk / binned_pos, binned_pos_edges
-            if "dir" in varType:
+            if varType == VariableToBin.DIR:
                 binned_pos = self._circPadSmooth(binned_pos, self.smooth_sz)
                 binned_spk = self._circPadSmooth(binned_spk, self.smooth_sz)
                 rmap = binned_spk / binned_pos
             else:
                 binned_pos = blurImage(
                     binned_pos, self.smooth_sz, ftype=self.smoothingType
                 )
@@ -366,14 +447,16 @@
         entries of h)
         """
         if weights is None:
             weights = np.ones_like(var)
         dims = weights.ndim
         if dims == 1 and var.ndim == 1:
             var = var[np.newaxis, :]
+            # if self.var2Bin != VariableToBin.XY and len(bin_edges) != 1:
+            #     bin_edges = self._calcBinEdges(self.binsize)
             bin_edges = bin_edges[np.newaxis, :]
         elif dims > 1 and var.ndim == 1:
             var = var[np.newaxis, :]
             bin_edges = bin_edges[np.newaxis, :]
         else:
             var = np.flipud(var)
         weights = np.atleast_2d(weights)  # needed for list comp below
```

### Comparing `ephysiopy-1.9.13/ephysiopy/common/ephys_generic.py` & `ephysiopy-1.9.15/ephysiopy/common/ephys_generic.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.13/ephysiopy/common/fieldcalcs.py` & `ephysiopy-1.9.15/ephysiopy/common/fieldcalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.13/ephysiopy/common/mle_von_mises_vals.py` & `ephysiopy-1.9.15/ephysiopy/common/mle_von_mises_vals.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.13/ephysiopy/common/phasecoding.py` & `ephysiopy-1.9.15/ephysiopy/common/phasecoding.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import matplotlib
+import matplotlib.cm
 import matplotlib.pyplot as plt
 import numpy as np
 from ephysiopy.common.binning import RateMap
 from ephysiopy.common.ephys_generic import PosCalcsGeneric
 from ephysiopy.common.rhythmicity import LFPOscillations
 from ephysiopy.common.utils import bwperim
 from scipy import ndimage, optimize, signal
@@ -142,16 +143,16 @@
             xy[0, :],
             xy[1, :],
             ppm=self.ppm,
             cm=True,
         )
         P.postprocesspos(tracker_params={"AxonaBadValue": 1023})
         # ... do the ratemap creation here once
-        R = RateMap(P.xy, P.dir, P.speed)
-        R.cmsPerBin = self.cms_per_bin
+        R = RateMap(P.xy, P.dir, P.speed, xyInCms=True)
+        R.binsize = self.cms_per_bin
         R.smooth_sz = self.field_smoothing_kernel_len
         R.ppm = self.ppm
         spk_times_in_pos_samples = self.getSpikePosIndices(spike_ts)
         spk_weights = np.bincount(
             spk_times_in_pos_samples, minlength=len(self.pos_ts))
         self.spk_times_in_pos_samples = spk_times_in_pos_samples
         self.spk_weights = spk_weights
@@ -300,15 +301,15 @@
         #     for reg in rp:
         #         print(reg.filled_area)
         #     markers = skimage.morphology.remove_small_objects(
         #         lb, min_size=4000, connectivity=4, in_place=True)
         if plot:
             fig = plt.figure()
             ax = fig.add_subplot(211)
-            ax.pcolormesh(ye, xe, rmap, cmap=matplotlib.colormaps["jet"],
+            ax.pcolormesh(ye, xe, rmap, cmap=matplotlib.cm.get_cmap("jet"),
                           edgecolors="face")
             ax.set_title("Smoothed ratemap + peaks")
             ax.xaxis.set_visible(False)
             ax.yaxis.set_visible(False)
             ax.set_aspect("equal")
             xlim = ax.get_xlim()
             ylim = ax.get_ylim()
@@ -621,15 +622,15 @@
                 interpolation="nearest"
             )
             plt.colorbar(imm, orientation="horizontal")
             ax.set_aspect("equal")
             # add a custom colorbar for colors in runVals
 
             # create a custom colormap for the plot
-            cmap = matplotlib.colormaps["hsv"]
+            cmap = matplotlib.cm.get_cmap("hsv")
             cmaplist = [cmap(i) for i in range(cmap.N)]
             cmaplist[0] = (1, 1, 1, 1)
             cmap = cmap.from_list("Perim cmap", cmaplist, cmap.N)
             bounds = np.linspace(0, 360, cmap.N)
             norm = matplotlib.colors.BoundaryNorm(bounds, cmap.N)
 
             imm = ax.imshow(
```

### Comparing `ephysiopy-1.9.13/ephysiopy/common/rhythmicity.py` & `ephysiopy-1.9.15/ephysiopy/common/rhythmicity.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.13/ephysiopy/common/spikecalcs.py` & `ephysiopy-1.9.15/ephysiopy/common/spikecalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.13/ephysiopy/common/statscalcs.py` & `ephysiopy-1.9.15/ephysiopy/common/statscalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.13/ephysiopy/common/utils.py` & `ephysiopy-1.9.15/ephysiopy/common/utils.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.13/ephysiopy/format_converters/OE_Axona.py` & `ephysiopy-1.9.15/ephysiopy/format_converters/OE_Axona.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.13/ephysiopy/format_converters/OE_numpy.py` & `ephysiopy-1.9.15/ephysiopy/format_converters/OE_numpy.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.13/ephysiopy/io/recording.py` & `ephysiopy-1.9.15/ephysiopy/io/recording.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,30 +65,36 @@
     h = new_array["h"][0]
     x = new_array["x"] * w
     y = new_array["y"] * h
     pos_data = np.array([np.ravel(x), np.ravel(y)]).T
     return pos_data
 
 
-def loadTrackMePluginData(pname: Path) -> np.ndarray:
-    mmap = memmapBinaryFile(str(pname), n_channels=4)
+def loadTrackMePluginData(pname: Path, n_channels: int = 4) -> np.ndarray:
+    mmap = memmapBinaryFile(str(pname), n_channels)
     return np.array(mmap[0:2, :]).T
 
 
 def loadTrackMeTTLTimestamps(pname: Path) -> np.ndarray:
     ts = np.load(os.path.join(pname, "timestamps.npy"))
     states = np.load(os.path.join(pname, "states.npy"))
     return ts[states > 0]
 
 
 def loadTrackMeTimestamps(pname: Path) -> np.ndarray:
     ts = np.load(os.path.join(pname, "timestamps.npy"))
     return ts
 
 
+def loadTrackMeFrameCount(pname: Path, n_channels: int = 4) -> np.ndarray:
+    data = memmapBinaryFile(str(pname), n_channels)
+    # framecount data is always last column in continuous.dat file
+    return np.array(data[-1, :]).T
+
+
 class RecordingKind(Enum):
     FPGA = 1
     NEUROPIXELS = 2
     ACQUISITIONBOARD = 3
     NWB = 4
 
 
@@ -105,14 +111,15 @@
 
 class TrialInterface(FigureMaker, metaclass=abc.ABCMeta):
     def __init__(self, pname: Path, **kwargs) -> None:
         assert os.path.exists(pname)
         self._pname = pname
         self._settings = None
         self._PosCalcs = None
+        self._RateMap = None
         self._pos_data_type = None
         self._sync_message_file = None
         self._clusterData = None  # Kilosort or .cut / .clu file
         self._recording_start_time = None
         self._ttl_data = None
         self._accelerometer_data = None
         self._path2PosData = None
@@ -158,14 +165,22 @@
         return self._PosCalcs
 
     @PosCalcs.setter
     def PosCalcs(self, val):
         self._PosCalcs = val
 
     @property
+    def RateMap(self):
+        return self._RateMap
+
+    @RateMap.setter
+    def RateMap(self, value):
+        self._RateMap = value
+
+    @property
     def pos_data_type(self):
         return self._pos_data_type
 
     @pos_data_type.setter
     def pos_data_type(self, val):
         self._pos_data_type = val
 
@@ -256,15 +271,19 @@
         raise NotImplementedError
 
     @abc.abstractmethod
     def load_ttl(self, *args, **kwargs):
         raise NotImplementedError
 
     @abc.abstractmethod
-    def get_spike_times(self, cluster: int, tetrode: int = None, *args, **kwargs):
+    def get_spike_times(self,
+                        cluster: int,
+                        tetrode: int = None,
+                        *args,
+                        **kwargs):
         """Returns the times of an individual cluster"""
         raise NotImplementedError
 
 
 class AxonaTrial(TrialInterface):
     def __init__(self, pname: Path, **kwargs) -> None:
         super().__init__(pname, **kwargs)
@@ -345,41 +364,40 @@
         rec_method = [i for i in self.settings.processors.keys()
                       if i in record_methods][0]
         if 'Sources/' in rec_method:
             tmp_rec_method = rec_method.lstrip('Sources/')
             self.rec_kind = Xml2RecordingKind[tmp_rec_method]
         else:
             self.rec_kind = Xml2RecordingKind[rec_method]
-        
+
         # Attempt to find the files contained in the parent directory
         # related to the recording with the default experiment and
         # recording name
         self.find_files(pname)
         self.sample_rate = None
         self.sample_rate = self.settings.processors[rec_method].sample_rate
         if self.sample_rate is None:
             if self.rec_kind == RecordingKind.NEUROPIXELS:
                 self.sample_rate = 30000
+        else:  # rubbish fix - many strs need casting to int/float
+            self.sample_rate = float(self.sample_rate)
         self.channel_count = self.settings.processors[rec_method].channel_count
         if self.channel_count is None:
             if self.rec_kind == RecordingKind.NEUROPIXELS:
                 self.channel_count = 384
         self.kilodata = None
 
-    def __load_kilo__(self):
-        """Loads KiloSort data"""
-        self.kilodata = KiloSortSession(self.pname)
-        self.kilodata.load()
-        self.kilodata.removeNoiseClusters()
-
     def get_spike_times(self, cluster: int, tetrode: int = None,
                         *args, **kwargs):
-        ts = self.kilodata.spk_times
-        times = ts[self.kilodata.spk_clusters == cluster]
-        return times.astype(np.int64) / self.sample_rate
+        ts = self.clusterData.spk_times
+        if cluster in self.clusterData.spk_clusters:
+            times = ts[self.clusterData.spk_clusters == cluster]
+            return times.astype(np.int64) / self.sample_rate
+        else:
+            warnings.warn("Cluster not present")
 
     def load_lfp(self, pname: Path, *args, **kwargs):
         '''
         Valid kwargs are:
         'target_sample_rate' - int
             the sample rate to downsample to from the original
         '''
@@ -451,27 +469,26 @@
                     self.path2PosData, "data_array.npy"))
             if pos_data_type == "TrackingPlugin":
                 print("Loading Tracking Plugin data...")
                 pos_data = loadTrackingPluginData(
                     os.path.join(self.path2PosData, "data_array.npy")
                 )
             pos_ts = np.load(os.path.join(self.path2PosData, "timestamps.npy"))
+            # pos_ts in seconds
             pos_ts = np.ravel(pos_ts)
             if pos_data_type == "TrackMe":
                 print("Loading TrackMe data...")
                 pos_data = loadTrackMePluginData(
                     Path(os.path.join(self.path2PosData, "continuous.dat")))
-                # pos_ts = loadTrackMeTTLTimestamps(self.path2EventsData)
                 pos_ts = loadTrackMeTimestamps(
                     Path(self.path2PosData))
                 pos_ts = pos_ts[0:len(pos_data)]
-            pos_timebase = getattr(self, "pos_timebase", 3e4)
-            sample_rate = np.floor(1 / np.mean(np.diff(pos_ts) / pos_timebase))
+            sample_rate = self.settings.processors[pos_data_type].sample_rate
+            sample_rate = float(sample_rate)
             xyTS = pos_ts - recording_start_time
-            # xyTS = xyTS / pos_timebase  # convert to seconds
             if self.sync_message_file is not None:
                 recording_start_time = xyTS[0]
 
             P = PosCalcsGeneric(
                 pos_data[:, 0],
                 pos_data[:, 1],
                 cm=cm,
```

### Comparing `ephysiopy-1.9.13/ephysiopy/openephys2py/KiloSort.py` & `ephysiopy-1.9.15/ephysiopy/openephys2py/KiloSort.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.13/ephysiopy/openephys2py/OESettings.py` & `ephysiopy-1.9.15/ephysiopy/openephys2py/OESettings.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.13/ephysiopy/tests/conftest.py` & `ephysiopy-1.9.15/ephysiopy/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.13/ephysiopy/tests/test_axona_headers.py` & `ephysiopy-1.9.15/ephysiopy/tests/test_axona_headers.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.13/ephysiopy/tests/test_axona_io.py` & `ephysiopy-1.9.15/ephysiopy/tests/test_axona_io.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.13/ephysiopy/tests/test_binning.py` & `ephysiopy-1.9.15/ephysiopy/tests/test_binning.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Sequence
 
 import numpy as np
 import pytest
-from ephysiopy.common.binning import RateMap
+from ephysiopy.common.binning import RateMap, VariableToBin, MapType
 
 
 @pytest.fixture
 def standard_Ratemap(basic_PosCalcs):
     """Returns a Ratemap instance with a random walk as x,y"""
     P = basic_PosCalcs
     P.postprocesspos(tracker_params={"AxonaBadValue": 1023})
@@ -15,27 +15,27 @@
     # P.dir = P.dir[0:10 * P.sample_rate]
     # P.speed = P.speed[0:10 * P.sample_rate]
     # P.npos = 10 * P.sample_rate
     return RateMap(P.xy, P.dir, P.speed)
 
 
 def test_calc_bin_size(standard_Ratemap):
-    bs = standard_Ratemap._calcBinSize()
+    bs = standard_Ratemap._calcBinEdges()
     print(f"Using {standard_Ratemap.ppm} ppm")
     assert isinstance(bs, (np.ndarray, list, Sequence))
 
 
 def test_bin_data(standard_Ratemap):
     R = standard_Ratemap
     xy = getattr(R, "xy")
-    xy_bins = R.binsize
+    xy_bins = R.binedges
     hd = getattr(R, "dir")
     R.inCms
     R.inCms = True
-    hd_bins = np.arange(0, 360 + R.cmsPerBin, R.cmsPerBin)
+    hd_bins = np.arange(0, 360 + R.binsize, R.binsize)
     samples = [xy, hd]
     bins = [xy_bins, hd_bins]
     pw2d = np.zeros(shape=[2, len(hd)])
     pw2d[0, :] = R.pos_weights
     pw2d[1, :] = R.pos_weights
     pw = [R.pos_weights, pw2d]
     for sample in zip(samples, bins, pw):
@@ -53,16 +53,16 @@
     n_pos = len(standard_Ratemap.pos_weights)
     spk_weights = np.random.rand(n_pos)
     spk_weights[spk_weights >= 0.95] = 1
     spk_weights[spk_weights >= 0.99] = 2
     spk_weights[spk_weights >= 0.99] = 3
     spk_weights[spk_weights < 0.95] = 0
 
-    vars_2_bin = ["xy", "dir", "speed"]
-    map_types = ["rate", "pos"]
+    vars_2_bin = [VariableToBin.XY, VariableToBin.DIR, VariableToBin.SPEED]
+    map_types = [MapType.RATE, MapType.POS]
     smoothing_when = ["after", "before"]
     do_smooth = [True, False]
     # There is a member variable to smooth before or after dividing
     # binned spikes by the spatial variable that needs to be set in the
     # iteration below
 
     for var in vars_2_bin:
```

### Comparing `ephysiopy-1.9.13/ephysiopy/tests/test_dacq2py.py` & `ephysiopy-1.9.15/ephysiopy/tests/test_dacq2py.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.13/ephysiopy/tests/test_ephys_generic.py` & `ephysiopy-1.9.15/ephysiopy/tests/test_ephys_generic.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.13/ephysiopy/tests/test_fieldcalcs.py` & `ephysiopy-1.9.15/ephysiopy/tests/test_fieldcalcs.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 import pytest
 from ephysiopy.common import fieldcalcs
+from ephysiopy.tests.test_binning import standard_Ratemap
 
 
 def test_limit_to_one(basic_ratemap):
     _, middle_field, _ = fieldcalcs.limit_to_one(basic_ratemap)
     assert isinstance(middle_field, np.ndarray)
     basic_ratemap[1::, :] = np.nan
     fieldcalcs.limit_to_one(basic_ratemap)
@@ -112,17 +113,20 @@
     assert isinstance(measures, dict)
     fieldcalcs.grid_field_props(
         basic_ratemap, min_distance=10,
         maxima='single',
         step=15)
 
 
-def test_deform_SAC(basic_ratemap):
-    from ephysiopy.common.binning import RateMap
-    R = RateMap()
+def test_deform_SAC(standard_Ratemap):
+    R = standard_Ratemap
+    n_pos = len(R.pos_weights)
+    spk_weights = np.random.rand(n_pos)
+    spk_weights[spk_weights >= 0.95] = 1
+    basic_ratemap, _ = R.getMap(spk_weights)
     sac = R.autoCorr2D(
         basic_ratemap, ~np.isfinite(basic_ratemap))
     from skimage import transform
     A = transform.AffineTransform(
         scale=[1, 1.15], translation=[0, -15])
     sac = transform.warp(sac, A.inverse)
     deformed_SAC = fieldcalcs.deform_SAC(sac)
@@ -132,22 +136,24 @@
     nodwell = ~np.isfinite(A)
     sac = R.autoCorr2D(A, nodwell)
     fieldcalcs.deform_SAC(sac)
     fieldcalcs.deform_SAC(
         sac, np.array([[3, 9], [10, 2]]), np.array([[1, 9], [10, 2]]))
 
 
-def test_get_grid_orientation(basic_ratemap):
-    from ephysiopy.common.gridcell import SAC
-    S = SAC()
-    nodwell = ~np.isfinite(basic_ratemap)
-    sac = S.autoCorr2D(basic_ratemap, nodwell)
+def test_get_grid_orientation(standard_Ratemap):
+    n_pos = len(standard_Ratemap.pos_weights)
+    spk_weights = np.random.rand(n_pos)
+    spk_weights[spk_weights >= 0.95] = 1
+    basic_ratemap, _ = standard_Ratemap.getMap(spk_weights)
+    sac = standard_Ratemap.autoCorr2D(
+        basic_ratemap, ~np.isfinite(basic_ratemap))
     measures = fieldcalcs.grid_field_props(sac, allProps=True)
     peak_coords = measures['closest_peak_coords']
     fieldcalcs.grid_orientation(peak_coords, np.arange(len(peak_coords)))
     A = np.zeros_like(basic_ratemap)
     A[3:10, 3:8] = 10
     nodwell = ~np.isfinite(A)
-    sac = S.autoCorr2D(A, nodwell)
+    sac = standard_Ratemap.autoCorr2D(A, nodwell)
     measures = fieldcalcs.grid_field_props(sac, allProps=True)
     peak_coords = measures['closest_peak_coords']
     fieldcalcs.grid_orientation(peak_coords, np.arange(len(peak_coords)))
```

### Comparing `ephysiopy-1.9.13/ephysiopy/tests/test_phasecoding.py` & `ephysiopy-1.9.15/ephysiopy/tests/test_phasecoding.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-import numpy as np
-from ephysiopy.io.recording import AxonaTrial
-from ephysiopy.common.phasecoding import phasePrecession2D
-from ephysiopy.common.phasecoding import phase_precession_config as ppc
-
-
-def test_phase_precession_2d_setup(path_to_axona_data):
-    T = AxonaTrial(path_to_axona_data)
-    T.load_pos_data(path_to_axona_data)
-    T.load_lfp(path_to_axona_data, "EEG")
-    spike_ts = T.TETRODE.get_spike_samples(1, 1)
-    pp2d = phasePrecession2D(
-        T.EEGCalcs.sig,
-        250.,
-        T.PosCalcs.xy,
-        spike_ts,
-        T.PosCalcs.xyTS,
-        ppc)
-    # test setting some properties
-    pp2d.ts = range(10)
-
-
-def test_perform_regression(path_to_axona_data):
-    T = AxonaTrial(path_to_axona_data)
-    T.load_pos_data(path_to_axona_data)
-    T.load_lfp(path_to_axona_data, "EEG")
-    spike_ts = T.TETRODE.get_spike_samples(1, 1)
-    pp2d = phasePrecession2D(T.EEGCalcs.sig,
-                             250.,
-                             T.PosCalcs.xy,
-                             spike_ts,
-                             T.PosCalcs.xyTS,
-                             ppc)
-    pp2d.performRegression()
-    # do the regression with different options
-    peaksXY, _, labels, _ = pp2d.partitionFields()
-    posD, runD = pp2d.getPosProps(labels, peaksXY)
-    pp2d.getThetaProps()
-    spkD = pp2d.getSpikeProps(posD["runLabel"],
-                              runD["meanDir"],
-                              runD["runDurationInPosBins"])
-    pp2d._ppRegress(spkD, whichSpk="last")
-    # the following test fails..
-    # pp2d._ppRegress(spkD, whichSpk="mean")
-
-
-def test_pos_props_with_events(path_to_axona_data):
-    T = AxonaTrial(path_to_axona_data)
-    T.load_pos_data(path_to_axona_data)
-    T.load_lfp(path_to_axona_data, "EEG")
-    T.load_ttl()
-    spike_ts = T.TETRODE.get_spike_samples(1, 1)
-    pp2d = phasePrecession2D(T.EEGCalcs.sig,
-                             250.,
-                             T.PosCalcs.xy,
-                             spike_ts,
-                             T.PosCalcs.xyTS,
-                             ppc)
-    laser_events = np.array(
-        np.ceil(T.ttl_data['on'] /
-                T.ttl_data.timebase *
-                T.PosCalcs.sample_rate)).astype(int)
-    peaksXY, _, labels, _ = pp2d.partitionFields()
-    pp2d.getPosProps(
-        labels, peaksXY, laserEvents=laser_events, plot=True)
-
-
-def test_circ_circ_corr(path_to_axona_data):
-    T = AxonaTrial(path_to_axona_data)
-    T.load_pos_data(path_to_axona_data)
-    T.load_lfp(path_to_axona_data)
-    spike_ts = T.TETRODE.get_spike_samples(1, 1)
-    pp2d = phasePrecession2D(T.EEGCalcs.sig,
-                             250.,
-                             T.PosCalcs.xy,
-                             spike_ts,
-                             T.PosCalcs.xyTS,
-                             ppc)
-    pp2d._circCircCorrTLinear(
-        theta=T.PosCalcs.dir[0:10].data,
-        phi=np.random.vonmises(0, 4, 10),
-        k=10,
-        conf=True)
-
-    pp2d._circCircCorrTLinear(
-        theta=T.PosCalcs.dir[0:3].data,
-        phi=np.random.vonmises(0, 4, 3),
-        k=3,
-        conf=True)
+# import numpy as np
+# from ephysiopy.io.recording import AxonaTrial
+# from ephysiopy.common.phasecoding import phasePrecession2D
+# from ephysiopy.common.phasecoding import phase_precession_config as ppc
+
+
+# def test_phase_precession_2d_setup(path_to_axona_data):
+#     T = AxonaTrial(path_to_axona_data)
+#     T.load_pos_data(path_to_axona_data)
+#     T.load_lfp(path_to_axona_data, "EEG")
+#     spike_ts = T.TETRODE.get_spike_samples(1, 1)
+#     pp2d = phasePrecession2D(
+#         T.EEGCalcs.sig,
+#         250.,
+#         T.PosCalcs.xy,
+#         spike_ts,
+#         T.PosCalcs.xyTS,
+#         ppc)
+#     # test setting some properties
+#     pp2d.ts = range(10)
+
+
+# def test_perform_regression(path_to_axona_data):
+#     T = AxonaTrial(path_to_axona_data)
+#     T.load_pos_data(path_to_axona_data)
+#     T.load_lfp(path_to_axona_data, "EEG")
+#     spike_ts = T.TETRODE.get_spike_samples(1, 1)
+#     pp2d = phasePrecession2D(T.EEGCalcs.sig,
+#                              250.,
+#                              T.PosCalcs.xy,
+#                              spike_ts,
+#                              T.PosCalcs.xyTS,
+#                              ppc)
+#     pp2d.performRegression()
+#     # do the regression with different options
+#     peaksXY, _, labels, _ = pp2d.partitionFields()
+#     posD, runD = pp2d.getPosProps(labels, peaksXY)
+#     pp2d.getThetaProps()
+#     spkD = pp2d.getSpikeProps(posD["runLabel"],
+#                               runD["meanDir"],
+#                               runD["runDurationInPosBins"])
+#     pp2d._ppRegress(spkD, whichSpk="last")
+#     # the following test fails..
+#     # pp2d._ppRegress(spkD, whichSpk="mean")
+
+
+# def test_pos_props_with_events(path_to_axona_data):
+#     T = AxonaTrial(path_to_axona_data)
+#     T.load_pos_data(path_to_axona_data)
+#     T.load_lfp(path_to_axona_data, "EEG")
+#     T.load_ttl()
+#     spike_ts = T.TETRODE.get_spike_samples(1, 1)
+#     pp2d = phasePrecession2D(T.EEGCalcs.sig,
+#                              250.,
+#                              T.PosCalcs.xy,
+#                              spike_ts,
+#                              T.PosCalcs.xyTS,
+#                              ppc)
+#     laser_events = np.array(
+#         np.ceil(T.ttl_data['on'] /
+#                 T.ttl_data.timebase *
+#                 T.PosCalcs.sample_rate)).astype(int)
+#     peaksXY, _, labels, _ = pp2d.partitionFields()
+#     pp2d.getPosProps(
+#         labels, peaksXY, laserEvents=laser_events, plot=True)
+
+
+# def test_circ_circ_corr(path_to_axona_data):
+#     T = AxonaTrial(path_to_axona_data)
+#     T.load_pos_data(path_to_axona_data)
+#     T.load_lfp(path_to_axona_data)
+#     spike_ts = T.TETRODE.get_spike_samples(1, 1)
+#     pp2d = phasePrecession2D(T.EEGCalcs.sig,
+#                              250.,
+#                              T.PosCalcs.xy,
+#                              spike_ts,
+#                              T.PosCalcs.xyTS,
+#                              ppc)
+#     pp2d._circCircCorrTLinear(
+#         theta=T.PosCalcs.dir[0:10].data,
+#         phi=np.random.vonmises(0, 4, 10),
+#         k=10,
+#         conf=True)
+
+#     pp2d._circCircCorrTLinear(
+#         theta=T.PosCalcs.dir[0:3].data,
+#         phi=np.random.vonmises(0, 4, 3),
+#         k=3,
+#         conf=True)
```

### Comparing `ephysiopy-1.9.13/ephysiopy/tests/test_rhythmicity.py` & `ephysiopy-1.9.15/ephysiopy/tests/test_rhythmicity.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.13/ephysiopy/tests/test_spikecalcs.py` & `ephysiopy-1.9.15/ephysiopy/tests/test_spikecalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.13/ephysiopy/tests/test_statscalcs.py` & `ephysiopy-1.9.15/ephysiopy/tests/test_statscalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.13/ephysiopy/tests/test_utils.py` & `ephysiopy-1.9.15/ephysiopy/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.13/ephysiopy/visualise/plotting.py` & `ephysiopy-1.9.15/ephysiopy/visualise/plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import matplotlib.pylab as plt
 import matplotlib.transforms as transforms
 import numpy as np
 from matplotlib.patches import Rectangle
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 
 from ephysiopy.axona import tintcolours as tcols
-from ephysiopy.common.binning import RateMap
+from ephysiopy.common.binning import RateMap, VariableToBin
 from ephysiopy.common.spikecalcs import SpikeCalcsGeneric
 
 
 # Decorators
 def stripAxes(func):
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
@@ -38,15 +38,14 @@
 
 class FigureMaker(object):
     '''
     A mixin class for TrialInterface that deals solely with
     producing graphical output
     '''
     def __init__(self):
-        self.data_loaded = False
         self.PosCalcs = None
 
     def initialise(self):
         xy = getattr(self.PosCalcs, "xy")
         hdir = getattr(self.PosCalcs, "dir")
         speed = getattr(self.PosCalcs, "speed")
         ppm = getattr(self.PosCalcs, "ppm")
@@ -54,20 +53,19 @@
         setattr(self, "npos", xy.shape[1])
         pos_weights = None
         if hdir is not None:
             if np.ma.is_masked(hdir):
                 pos_weights = np.array(~hdir.mask).astype(int)
             else:
                 pos_weights = np.ones_like(hdir)
-        self.RateMapMaker = RateMap(
+        self.RateMap = RateMap(
             xy=xy, hdir=hdir, speed=speed, pos_weights=pos_weights, ppm=ppm,
-            xyInCms=True, cmsPerBin=cmsPerBin)
-        self.RateMapMaker.x_lims = getattr(self, 'x_lims', None)  # 2-tuple
-        self.RateMapMaker.y_lims = getattr(self, 'y_lims', None)
-        self.data_loaded = True
+            xyInCms=True, binsize=cmsPerBin)
+        self.RateMap.x_lims = getattr(self, 'x_lims', None)  # 2-tuple
+        self.RateMap.y_lims = getattr(self, 'y_lims', None)
 
     def getSpikePosIndices(self, spk_times: np.ndarray):
         pos_times = getattr(self.PosCalcs, 'xyTS')
         idx = np.searchsorted(pos_times, spk_times)
         idx[idx == len(pos_times)] = idx[idx == len(pos_times)] - 1
         return idx
 
@@ -85,19 +83,20 @@
         except IndexError:
             pass
         return fig
 
     @stripAxes
     def makeRateMap(self, spk_times: np.ndarray,
                     ax: matplotlib.axes = None) -> matplotlib.axes:
-        self.initialise()
+        if not self.RateMap:
+            self.initialise()
         spk_times_in_pos_samples = self.getSpikePosIndices(spk_times)
         spk_weights = np.bincount(
             spk_times_in_pos_samples, minlength=self.npos)
-        rmap = self.RateMapMaker.getMap(spk_weights)
+        rmap = self.RateMap.getMap(spk_weights)
         ratemap = np.ma.MaskedArray(rmap[0], np.isnan(rmap[0]), copy=True)
         x, y = np.meshgrid(rmap[1][1][0:-1].data, rmap[1][0][0:-1].data)
         vmax = np.nanmax(np.ravel(ratemap))
         if ax is None:
             fig = plt.figure()
             ax = fig.add_subplot(111)
         ax.pcolormesh(
@@ -106,15 +105,16 @@
         ax.set_aspect('equal')
         return ax
 
     @stripAxes
     def makeSpikePathPlot(self, spk_times: np.ndarray = None,
                           ax: matplotlib.axes = None,
                           **kwargs) -> matplotlib.axes:
-        self.initialise()
+        if not self.RateMap:
+            self.initialise()
         if 'c' in kwargs:
             col = kwargs.pop('c')
         else:
             col = tcols.colours[1]
         if ax is None:
             fig = plt.figure()
             ax = fig.add_subplot(111)
@@ -126,46 +126,48 @@
             ax.plot(self.PosCalcs.xy[0, idx],
                     self.PosCalcs.xy[1, idx], 's', c=col, **kwargs)
         return ax
 
     @stripAxes
     def makeSAC(self, spk_times: np.array = None,
                 ax: matplotlib.axes = None, **kwargs) -> matplotlib.axes:
-        self.initialise()
+        if not self.RateMap:
+            self.initialise()
         spk_times_in_pos_samples = self.getSpikePosIndices(spk_times)
         spk_weights = np.bincount(
             spk_times_in_pos_samples, minlength=self.npos)
-        rmap = self.RateMapMaker.getMap(spk_weights)
-        from ephysiopy.common import gridcell
-        S = gridcell.SAC()
+        rmap = self.RateMap.getMap(spk_weights)
         nodwell = ~np.isfinite(rmap[0])
-        sac = S.autoCorr2D(rmap[0], nodwell)
+        sac = self.RateMap.autoCorr2D(rmap[0], nodwell)
+        from ephysiopy.common.gridcell import SAC
+        S = SAC()
         measures = S.getMeasures(sac)
         if ax is None:
             fig = plt.figure()
             ax = fig.add_subplot(111)
         ax = self.show_SAC(sac, measures, ax)
         return ax
 
     @stripAxes
     def makeHDPlot(self, spk_times: np.array = None,
                    ax: matplotlib.axes = None, **kwargs) -> matplotlib.axes:
-        self.initialise()
+        if not self.RateMap:
+            self.initialise()
         spk_times_in_pos_samples = self.getSpikePosIndices(spk_times)
         spk_weights = np.bincount(
             spk_times_in_pos_samples, minlength=self.npos)
-        rmap = self.RateMapMaker.getMap(spk_weights, 'dir')
+        rmap = self.RateMap.getMap(spk_weights, varType=VariableToBin.DIR)
         if ax is None:
             fig = plt.figure()
             ax = fig.add_subplot(111, projection='polar')
         # need to deal with the case where the axis is supplied but
         # is not polar. deal with polar first
         theta = np.deg2rad(rmap[1][0])
         ax.clear()
-        r = rmap[0]
+        r = rmap[0]  # in samples so * pos sample_rate
         r = np.insert(r, -1, r[0])
         if 'polar' in ax.name:
             ax.plot(theta, r)
             if 'fill' in kwargs:
                 ax.fill(theta, r, alpha=0.5)
             ax.set_aspect('equal')
         else:
@@ -177,15 +179,15 @@
             angles = self.PosCalcs.dir[spk_times_in_pos_samples]
             r, th = mean_resultant_vector(np.deg2rad(angles))
             ax.plot([th, th], [0, r*np.max(rmap[0])], 'r')
         if 'polar' in ax.name:
             ax.set_thetagrids([0, 90, 180, 270])
         return ax
 
-    @stripAxes
+    # @stripAxes
     def makeSpeedVsRatePlot(
             self, spk_times: np.array, minSpeed: float = 0.0,
             maxSpeed: float = 40.0, sigma: float = 3.0,
             ax: matplotlib.axes = None, **kwargs) -> matplotlib.axes:
         """
         Plots the instantaneous firing rate of a cell against running speed
         Also outputs a couple of measures as with Kropff et al., 2015; the
```

### Comparing `ephysiopy-1.9.13/ephysiopy.egg-info/PKG-INFO` & `ephysiopy-1.9.15/ephysiopy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ephysiopy
-Version: 1.9.13
+Version: 1.9.15
 Summary: Analysis of electrophysiology data
 Home-page: https://github.com/rhayman/ephysiopy
 Author: Robin Hayman
 Author-email: robin.hayman@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ephysiopy-1.9.13/ephysiopy.egg-info/SOURCES.txt` & `ephysiopy-1.9.15/ephysiopy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.13/setup.py` & `ephysiopy-1.9.15/setup.py`

 * *Files identical despite different names*

