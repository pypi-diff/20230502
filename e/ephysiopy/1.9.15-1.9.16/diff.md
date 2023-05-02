# Comparing `tmp/ephysiopy-1.9.15.tar.gz` & `tmp/ephysiopy-1.9.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ephysiopy-1.9.15.tar", last modified: Tue May  2 11:59:17 2023, max compression
+gzip compressed data, was "ephysiopy-1.9.16.tar", last modified: Tue May  2 12:10:29 2023, max compression
```

## Comparing `ephysiopy-1.9.15.tar` & `ephysiopy-1.9.16.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:59:17.364166 ephysiopy-1.9.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-05-02 11:59:17.364166 ephysiopy-1.9.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:59:17.360166 ephysiopy-1.9.15/ephysiopy/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:59:17.360166 ephysiopy-1.9.15/ephysiopy/axona/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/axona/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19336 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/axona/axonaIO.py
--rw-r--r--   0 runner    (1001) docker     (123)    11999 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/axona/file_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/axona/tetrode_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/axona/tintcolours.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:59:17.360166 ephysiopy-1.9.15/ephysiopy/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34032 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/common/binning.py
--rw-r--r--   0 runner    (1001) docker     (123)    21358 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/common/ephys_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    40221 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/common/fieldcalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/common/gridcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/common/mle_von_mises_vals.py
--rw-r--r--   0 runner    (1001) docker     (123)    49500 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/common/phasecoding.py
--rw-r--r--   0 runner    (1001) docker     (123)    24931 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/common/rhythmicity.py
--rw-r--r--   0 runner    (1001) docker     (123)    28784 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/common/spikecalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/common/statscalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/common/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:59:17.360166 ephysiopy-1.9.15/ephysiopy/format_converters/
--rw-r--r--   0 runner    (1001) docker     (123)    19711 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/format_converters/OE_Axona.py
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/format_converters/OE_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/format_converters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:59:17.360166 ephysiopy-1.9.15/ephysiopy/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23796 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/io/recording.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:59:17.360166 ephysiopy-1.9.15/ephysiopy/openephys2py/
--rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/openephys2py/KiloSort.py
--rw-r--r--   0 runner    (1001) docker     (123)    10490 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/openephys2py/OESettings.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/openephys2py/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:59:17.364166 ephysiopy-1.9.15/ephysiopy/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/tests/test_axona_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/tests/test_axona_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/tests/test_binning.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/tests/test_dacq2py.py
--rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/tests/test_ephys_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/tests/test_fieldcalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/tests/test_gridcell.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/tests/test_openephys.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/tests/test_phasecoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/tests/test_rhythmicity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/tests/test_spikecalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/tests/test_statscalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:59:17.364166 ephysiopy-1.9.15/ephysiopy/visualise/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/visualise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32402 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/ephysiopy/visualise/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:59:17.360166 ephysiopy-1.9.15/ephysiopy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-05-02 11:59:17.000000 ephysiopy-1.9.15/ephysiopy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-02 11:59:17.000000 ephysiopy-1.9.15/ephysiopy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 11:59:17.000000 ephysiopy-1.9.15/ephysiopy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-02 11:59:17.000000 ephysiopy-1.9.15/ephysiopy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-02 11:59:17.000000 ephysiopy-1.9.15/ephysiopy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-02 11:59:17.364166 ephysiopy-1.9.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-02 11:59:09.000000 ephysiopy-1.9.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:10:29.085597 ephysiopy-1.9.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-02 12:10:18.000000 ephysiopy-1.9.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-02 12:10:18.000000 ephysiopy-1.9.16/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-05-02 12:10:29.085597 ephysiopy-1.9.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-02 12:10:18.000000 ephysiopy-1.9.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:10:29.077597 ephysiopy-1.9.16/ephysiopy/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-02 12:10:18.000000 ephysiopy-1.9.16/ephysiopy/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-02 12:10:18.000000 ephysiopy-1.9.16/ephysiopy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:10:29.081597 ephysiopy-1.9.16/ephysiopy/axona/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 12:10:18.000000 ephysiopy-1.9.16/ephysiopy/axona/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19336 2023-05-02 12:10:18.000000 ephysiopy-1.9.16/ephysiopy/axona/axonaIO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11999 2023-05-02 12:10:18.000000 ephysiopy-1.9.16/ephysiopy/axona/file_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-02 12:10:18.000000 ephysiopy-1.9.16/ephysiopy/axona/tetrode_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-02 12:10:18.000000 ephysiopy-1.9.16/ephysiopy/axona/tintcolours.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:10:29.081597 ephysiopy-1.9.16/ephysiopy/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 12:10:18.000000 ephysiopy-1.9.16/ephysiopy/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34032 2023-05-02 12:10:18.000000 ephysiopy-1.9.16/ephysiopy/common/binning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21358 2023-05-02 12:10:18.000000 ephysiopy-1.9.16/ephysiopy/common/ephys_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40221 2023-05-02 12:10:18.000000 ephysiopy-1.9.16/ephysiopy/common/fieldcalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-05-02 12:10:18.000000 ephysiopy-1.9.16/ephysiopy/common/gridcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-05-02 12:10:18.000000 ephysiopy-1.9.16/ephysiopy/common/mle_von_mises_vals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49500 2023-05-02 12:10:18.000000 ephysiopy-1.9.16/ephysiopy/common/phasecoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24931 2023-05-02 12:10:18.000000 ephysiopy-1.9.16/ephysiopy/common/rhythmicity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28784 2023-05-02 12:10:18.000000 ephysiopy-1.9.16/ephysiopy/common/spikecalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-05-02 12:10:18.000000 ephysiopy-1.9.16/ephysiopy/common/statscalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-05-02 12:10:18.000000 ephysiopy-1.9.16/ephysiopy/common/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:10:29.081597 ephysiopy-1.9.16/ephysiopy/format_converters/
+-rw-r--r--   0 runner    (1001) docker     (123)    19711 2023-05-02 12:10:18.000000 ephysiopy-1.9.16/ephysiopy/format_converters/OE_Axona.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-05-02 12:10:18.000000 ephysiopy-1.9.16/ephysiopy/format_converters/OE_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 12:10:18.000000 ephysiopy-1.9.16/ephysiopy/format_converters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:10:29.081597 ephysiopy-1.9.16/ephysiopy/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 12:10:18.000000 ephysiopy-1.9.16/ephysiopy/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23946 2023-05-02 12:10:18.000000 ephysiopy-1.9.16/ephysiopy/io/recording.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:10:29.081597 ephysiopy-1.9.16/ephysiopy/openephys2py/
+-rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-05-02 12:10:18.000000 ephysiopy-1.9.16/ephysiopy/openephys2py/KiloSort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10490 2023-05-02 12:10:18.000000 ephysiopy-1.9.16/ephysiopy/openephys2py/OESettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 12:10:18.000000 ephysiopy-1.9.16/ephysiopy/openephys2py/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:10:29.085597 ephysiopy-1.9.16/ephysiopy/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 12:10:18.000000 ephysiopy-1.9.16/ephysiopy/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-05-02 12:10:18.000000 ephysiopy-1.9.16/ephysiopy/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-02 12:10:18.000000 ephysiopy-1.9.16/ephysiopy/tests/test_axona_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-05-02 12:10:18.000000 ephysiopy-1.9.16/ephysiopy/tests/test_axona_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-05-02 12:10:18.000000 ephysiopy-1.9.16/ephysiopy/tests/test_binning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-05-02 12:10:18.000000 ephysiopy-1.9.16/ephysiopy/tests/test_dacq2py.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-05-02 12:10:18.000000 ephysiopy-1.9.16/ephysiopy/tests/test_ephys_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-05-02 12:10:18.000000 ephysiopy-1.9.16/ephysiopy/tests/test_fieldcalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-02 12:10:18.000000 ephysiopy-1.9.16/ephysiopy/tests/test_gridcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-02 12:10:18.000000 ephysiopy-1.9.16/ephysiopy/tests/test_openephys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-05-02 12:10:18.000000 ephysiopy-1.9.16/ephysiopy/tests/test_phasecoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-05-02 12:10:18.000000 ephysiopy-1.9.16/ephysiopy/tests/test_rhythmicity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-05-02 12:10:18.000000 ephysiopy-1.9.16/ephysiopy/tests/test_spikecalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-02 12:10:18.000000 ephysiopy-1.9.16/ephysiopy/tests/test_statscalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-05-02 12:10:18.000000 ephysiopy-1.9.16/ephysiopy/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:10:29.085597 ephysiopy-1.9.16/ephysiopy/visualise/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 12:10:18.000000 ephysiopy-1.9.16/ephysiopy/visualise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32402 2023-05-02 12:10:18.000000 ephysiopy-1.9.16/ephysiopy/visualise/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:10:29.077597 ephysiopy-1.9.16/ephysiopy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-05-02 12:10:29.000000 ephysiopy-1.9.16/ephysiopy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-02 12:10:29.000000 ephysiopy-1.9.16/ephysiopy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 12:10:29.000000 ephysiopy-1.9.16/ephysiopy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-02 12:10:29.000000 ephysiopy-1.9.16/ephysiopy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-02 12:10:29.000000 ephysiopy-1.9.16/ephysiopy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-02 12:10:29.085597 ephysiopy-1.9.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-02 12:10:18.000000 ephysiopy-1.9.16/setup.py
```

### Comparing `ephysiopy-1.9.15/LICENSE` & `ephysiopy-1.9.16/LICENSE`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.15/PKG-INFO` & `ephysiopy-1.9.16/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ephysiopy
-Version: 1.9.15
+Version: 1.9.16
 Summary: Analysis of electrophysiology data
 Home-page: https://github.com/rhayman/ephysiopy
 Author: Robin Hayman
 Author-email: robin.hayman@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ephysiopy-1.9.15/README.md` & `ephysiopy-1.9.16/README.md`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.15/ephysiopy/axona/axonaIO.py` & `ephysiopy-1.9.16/ephysiopy/axona/axonaIO.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.15/ephysiopy/axona/file_headers.py` & `ephysiopy-1.9.16/ephysiopy/axona/file_headers.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.15/ephysiopy/axona/tetrode_dict.py` & `ephysiopy-1.9.16/ephysiopy/axona/tetrode_dict.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.15/ephysiopy/axona/tintcolours.py` & `ephysiopy-1.9.16/ephysiopy/axona/tintcolours.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.15/ephysiopy/common/binning.py` & `ephysiopy-1.9.16/ephysiopy/common/binning.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.15/ephysiopy/common/ephys_generic.py` & `ephysiopy-1.9.16/ephysiopy/common/ephys_generic.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.15/ephysiopy/common/fieldcalcs.py` & `ephysiopy-1.9.16/ephysiopy/common/fieldcalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.15/ephysiopy/common/gridcell.py` & `ephysiopy-1.9.16/ephysiopy/common/gridcell.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.15/ephysiopy/common/mle_von_mises_vals.py` & `ephysiopy-1.9.16/ephysiopy/common/mle_von_mises_vals.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.15/ephysiopy/common/phasecoding.py` & `ephysiopy-1.9.16/ephysiopy/common/phasecoding.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.15/ephysiopy/common/rhythmicity.py` & `ephysiopy-1.9.16/ephysiopy/common/rhythmicity.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.15/ephysiopy/common/spikecalcs.py` & `ephysiopy-1.9.16/ephysiopy/common/spikecalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.15/ephysiopy/common/statscalcs.py` & `ephysiopy-1.9.16/ephysiopy/common/statscalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.15/ephysiopy/common/utils.py` & `ephysiopy-1.9.16/ephysiopy/common/utils.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.15/ephysiopy/format_converters/OE_Axona.py` & `ephysiopy-1.9.16/ephysiopy/format_converters/OE_Axona.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.15/ephysiopy/format_converters/OE_numpy.py` & `ephysiopy-1.9.16/ephysiopy/format_converters/OE_numpy.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.15/ephysiopy/io/recording.py` & `ephysiopy-1.9.16/ephysiopy/io/recording.py`

 * *Files 1% similar despite different names*

```diff
@@ -473,16 +473,19 @@
                     os.path.join(self.path2PosData, "data_array.npy")
                 )
             pos_ts = np.load(os.path.join(self.path2PosData, "timestamps.npy"))
             # pos_ts in seconds
             pos_ts = np.ravel(pos_ts)
             if pos_data_type == "TrackMe":
                 print("Loading TrackMe data...")
+                n_pos_chans = int(
+                    self.settings.processors['TrackMe'].channel_count)
                 pos_data = loadTrackMePluginData(
-                    Path(os.path.join(self.path2PosData, "continuous.dat")))
+                    Path(os.path.join(self.path2PosData, "continuous.dat")),
+                    n_channels=n_pos_chans)
                 pos_ts = loadTrackMeTimestamps(
                     Path(self.path2PosData))
                 pos_ts = pos_ts[0:len(pos_data)]
             sample_rate = self.settings.processors[pos_data_type].sample_rate
             sample_rate = float(sample_rate)
             xyTS = pos_ts - recording_start_time
             if self.sync_message_file is not None:
```

### Comparing `ephysiopy-1.9.15/ephysiopy/openephys2py/KiloSort.py` & `ephysiopy-1.9.16/ephysiopy/openephys2py/KiloSort.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.15/ephysiopy/openephys2py/OESettings.py` & `ephysiopy-1.9.16/ephysiopy/openephys2py/OESettings.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.15/ephysiopy/tests/conftest.py` & `ephysiopy-1.9.16/ephysiopy/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.15/ephysiopy/tests/test_axona_headers.py` & `ephysiopy-1.9.16/ephysiopy/tests/test_axona_headers.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.15/ephysiopy/tests/test_axona_io.py` & `ephysiopy-1.9.16/ephysiopy/tests/test_axona_io.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.15/ephysiopy/tests/test_binning.py` & `ephysiopy-1.9.16/ephysiopy/tests/test_binning.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.15/ephysiopy/tests/test_dacq2py.py` & `ephysiopy-1.9.16/ephysiopy/tests/test_dacq2py.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.15/ephysiopy/tests/test_ephys_generic.py` & `ephysiopy-1.9.16/ephysiopy/tests/test_ephys_generic.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.15/ephysiopy/tests/test_fieldcalcs.py` & `ephysiopy-1.9.16/ephysiopy/tests/test_fieldcalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.15/ephysiopy/tests/test_gridcell.py` & `ephysiopy-1.9.16/ephysiopy/tests/test_gridcell.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.15/ephysiopy/tests/test_phasecoding.py` & `ephysiopy-1.9.16/ephysiopy/tests/test_phasecoding.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.15/ephysiopy/tests/test_rhythmicity.py` & `ephysiopy-1.9.16/ephysiopy/tests/test_rhythmicity.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.15/ephysiopy/tests/test_spikecalcs.py` & `ephysiopy-1.9.16/ephysiopy/tests/test_spikecalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.15/ephysiopy/tests/test_statscalcs.py` & `ephysiopy-1.9.16/ephysiopy/tests/test_statscalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.15/ephysiopy/tests/test_utils.py` & `ephysiopy-1.9.16/ephysiopy/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.15/ephysiopy/visualise/plotting.py` & `ephysiopy-1.9.16/ephysiopy/visualise/plotting.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.15/ephysiopy.egg-info/PKG-INFO` & `ephysiopy-1.9.16/ephysiopy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ephysiopy
-Version: 1.9.15
+Version: 1.9.16
 Summary: Analysis of electrophysiology data
 Home-page: https://github.com/rhayman/ephysiopy
 Author: Robin Hayman
 Author-email: robin.hayman@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ephysiopy-1.9.15/ephysiopy.egg-info/SOURCES.txt` & `ephysiopy-1.9.16/ephysiopy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.15/setup.py` & `ephysiopy-1.9.16/setup.py`

 * *Files identical despite different names*

