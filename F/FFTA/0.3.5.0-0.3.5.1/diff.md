# Comparing `tmp/FFTA-0.3.5.0.tar.gz` & `tmp/FFTA-0.3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FFTA-0.3.5.0.tar", last modified: Fri Jun 10 23:29:10 2022, max compression
+gzip compressed data, was "FFTA-0.3.5.1.tar", last modified: Tue May  2 20:27:38 2023, max compression
```

## Comparing `FFTA-0.3.5.0.tar` & `FFTA-0.3.5.1.tar`

### file list

```diff
@@ -1,87 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-10 23:29:10.022243 FFTA-0.3.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-10 23:29:10.014243 FFTA-0.3.5.0/FFTA.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3411 2022-06-10 23:29:09.000000 FFTA-0.3.5.0/FFTA.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1868 2022-06-10 23:29:09.000000 FFTA-0.3.5.0/FFTA.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-10 23:29:09.000000 FFTA-0.3.5.0/FFTA.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-10 23:29:09.000000 FFTA-0.3.5.0/FFTA.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-06-10 23:29:09.000000 FFTA-0.3.5.0/FFTA.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1090 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3411 2022-06-10 23:29:10.022243 FFTA-0.3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3121 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-10 23:29:10.014243 FFTA-0.3.5.0/ffta/
--rw-r--r--   0 runner    (1001) docker     (121)      478 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-10 23:29:10.014243 FFTA-0.3.5.0/ffta/acquisition/
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/acquisition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5136 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/acquisition/generate_chirp.py
--rw-r--r--   0 runner    (1001) docker     (121)     6729 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/acquisition/polling.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-10 23:29:10.018243 FFTA-0.3.5.0/ffta/analysis/
--rw-r--r--   0 runner    (1001) docker     (121)      138 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8145 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/analysis/create_movie.py
--rw-r--r--   0 runner    (1001) docker     (121)    21935 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/analysis/dist_cluster.py
--rw-r--r--   0 runner    (1001) docker     (121)    20288 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/analysis/fft.py
--rw-r--r--   0 runner    (1001) docker     (121)    12213 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/analysis/filtering.py
--rw-r--r--   0 runner    (1001) docker     (121)    12774 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/analysis/gmode_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2742 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/analysis/mask_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3744 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/analysis/proc_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2811 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/analysis/select_pixel.py
--rw-r--r--   0 runner    (1001) docker     (121)     5937 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/analysis/svd.py
--rw-r--r--   0 runner    (1001) docker     (121)    20850 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/analysis/svd_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1610 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/analysis/test_pixel.py
--rw-r--r--   0 runner    (1001) docker     (121)      924 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/analyze_pixel.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-10 23:29:10.018243 FFTA-0.3.5.0/ffta/gkpfm/
--rw-r--r--   0 runner    (1001) docker     (121)      158 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/gkpfm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3499 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/gkpfm/gkline.py
--rw-r--r--   0 runner    (1001) docker     (121)    31061 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/gkpfm/gkpixel.py
--rw-r--r--   0 runner    (1001) docker     (121)    21187 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/gkpfm/gkprocess.py
--rw-r--r--   0 runner    (1001) docker     (121)     4199 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/gkpfm/gmode_simple.py
--rw-r--r--   0 runner    (1001) docker     (121)     2201 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/gkpfm/load_excitation.py
--rw-r--r--   0 runner    (1001) docker     (121)    17070 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/gkpfm/transfer_func.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-10 23:29:10.018243 FFTA-0.3.5.0/ffta/hdf_utils/
--rw-r--r--   0 runner    (1001) docker     (121)       83 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/hdf_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13515 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/hdf_utils/analyze_h5.py
--rw-r--r--   0 runner    (1001) docker     (121)     2747 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/hdf_utils/hdf_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     5028 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/hdf_utils/plot_tfp.py
--rw-r--r--   0 runner    (1001) docker     (121)    31195 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/hdf_utils/process.py
--rw-r--r--   0 runner    (1001) docker     (121)     5254 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/line.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-10 23:29:10.018243 FFTA-0.3.5.0/ffta/load/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/load/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8580 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/load/get_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    10689 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/load/gl_ibw.py
--rw-r--r--   0 runner    (1001) docker     (121)     4242 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/load/load_commands.py
--rw-r--r--   0 runner    (1001) docker     (121)    18497 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/load/load_hdf.py
--rw-r--r--   0 runner    (1001) docker     (121)    14515 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/load/load_ringdown.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-10 23:29:10.018243 FFTA-0.3.5.0/ffta/nfmd/
--rw-r--r--   0 runner    (1001) docker     (121)    14958 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/nfmd/NFMD.py
--rw-r--r--   0 runner    (1001) docker     (121)     3403 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/nfmd/NFMDPixel.py
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/nfmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2021 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/nfmd/models.py
--rw-r--r--   0 runner    (1001) docker     (121)    40879 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/pixel.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-10 23:29:10.018243 FFTA-0.3.5.0/ffta/pixel_utils/
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/pixel_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2849 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/pixel_utils/badpixels.py
--rw-r--r--   0 runner    (1001) docker     (121)     2219 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/pixel_utils/dwavelet.py
--rw-r--r--   0 runner    (1001) docker     (121)     6262 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/pixel_utils/fitting.py
--rw-r--r--   0 runner    (1001) docker     (121)     5287 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/pixel_utils/load.py
--rw-r--r--   0 runner    (1001) docker     (121)     2689 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/pixel_utils/noise.py
--rw-r--r--   0 runner    (1001) docker     (121)     3623 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/pixel_utils/parab.py
--rw-r--r--   0 runner    (1001) docker     (121)      347 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/pixel_utils/peakdetect.py
--rw-r--r--   0 runner    (1001) docker     (121)     7656 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/pixel_utils/tfp_calc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-10 23:29:10.018243 FFTA-0.3.5.0/ffta/simulation/
--rw-r--r--   0 runner    (1001) docker     (121)      309 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3077 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/simulation/broadband_drive.py
--rw-r--r--   0 runner    (1001) docker     (121)     5887 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/simulation/calibration_curve.py
--rw-r--r--   0 runner    (1001) docker     (121)    13957 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/simulation/cantilever.py
--rw-r--r--   0 runner    (1001) docker     (121)     9489 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/simulation/electric_drive.py
--rw-r--r--   0 runner    (1001) docker     (121)     2537 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/simulation/impulse.py
--rw-r--r--   0 runner    (1001) docker     (121)     6805 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/simulation/mechanical_drive.py
--rw-r--r--   0 runner    (1001) docker     (121)     5774 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/simulation/mechanical_drive_simple.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-10 23:29:10.022243 FFTA-0.3.5.0/ffta/simulation/utils/
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/simulation/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1040 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/simulation/utils/excitation.py
--rw-r--r--   0 runner    (1001) docker     (121)     4265 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/ffta/simulation/utils/load.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-10 23:29:10.022243 FFTA-0.3.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1345 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-10 23:29:10.022243 FFTA-0.3.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3932 2022-06-10 23:25:48.000000 FFTA-0.3.5.0/tests/test_ffta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:27:38.578667 FFTA-0.3.5.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:27:38.570667 FFTA-0.3.5.1/FFTA.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-05-02 20:27:38.000000 FFTA-0.3.5.1/FFTA.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-05-02 20:27:38.000000 FFTA-0.3.5.1/FFTA.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 20:27:38.000000 FFTA-0.3.5.1/FFTA.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-02 20:27:38.000000 FFTA-0.3.5.1/FFTA.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-02 20:27:38.000000 FFTA-0.3.5.1/FFTA.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-05-02 20:27:38.578667 FFTA-0.3.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:27:38.570667 FFTA-0.3.5.1/ffta/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:27:38.570667 FFTA-0.3.5.1/ffta/_legacy_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/_legacy_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/_legacy_functions/analyze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:27:38.570667 FFTA-0.3.5.1/ffta/acquisition/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/acquisition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/acquisition/generate_chirp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/acquisition/polling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:27:38.574667 FFTA-0.3.5.1/ffta/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/analysis/create_movie.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25906 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/analysis/dist_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20348 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/analysis/fft.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13404 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/analysis/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12834 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/analysis/gmode_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/analysis/mask_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/analysis/proc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/analysis/select_pixel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/analysis/svd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20765 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/analysis/svd_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/analysis/test_pixel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/analyze_pixel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:27:38.574667 FFTA-0.3.5.1/ffta/gkpfm/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/gkpfm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/gkpfm/gkline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31024 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/gkpfm/gkpixel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21186 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/gkpfm/gkprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/gkpfm/gmode_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/gkpfm/load_excitation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19261 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/gkpfm/transfer_func.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:27:38.574667 FFTA-0.3.5.1/ffta/hdf_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/hdf_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15243 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/hdf_utils/analyze_h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/hdf_utils/hdf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/hdf_utils/plot_tfp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31115 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/hdf_utils/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/line.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:27:38.574667 FFTA-0.3.5.1/ffta/load/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/load/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8578 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/load/get_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/load/gl_ibw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/load/load_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18497 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/load/load_hdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16048 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/load/load_ringdown.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:27:38.574667 FFTA-0.3.5.1/ffta/nfmd/
+-rw-r--r--   0 runner    (1001) docker     (123)    15513 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/nfmd/NFMD.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/nfmd/NFMDPixel.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/nfmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/nfmd/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41063 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/pixel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:27:38.574667 FFTA-0.3.5.1/ffta/pixel_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/pixel_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/pixel_utils/badpixels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/pixel_utils/dwavelet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/pixel_utils/fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/pixel_utils/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/pixel_utils/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/pixel_utils/parab.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/pixel_utils/peakdetect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/pixel_utils/tfp_calc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:27:38.578667 FFTA-0.3.5.1/ffta/simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/simulation/broadband_drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/simulation/calibration_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14974 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/simulation/cantilever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9450 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/simulation/electric_drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/simulation/impulse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/simulation/mechanical_drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/simulation/mechanical_drive_simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:27:38.578667 FFTA-0.3.5.1/ffta/simulation/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/simulation/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/simulation/utils/excitation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/ffta/simulation/utils/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 20:27:38.578667 FFTA-0.3.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:27:38.578667 FFTA-0.3.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-05-02 20:23:14.000000 FFTA-0.3.5.1/tests/test_ffta.py
```

### Comparing `FFTA-0.3.5.0/FFTA.egg-info/PKG-INFO` & `FFTA-0.3.5.1/FFTA.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: FFTA
-Version: 0.3.5.0
+Version: 0.3.5.1
 Summary: Fast Free Transient Analysis
 Home-page: https://github.com/rajgiriUW/ffta/
 Author: Rajiv Giridharagopal
 Author-email: rgiri@uw.edu
 License: MIT
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 [![PyPI version](https://badge.fury.io/py/FFTA.svg)](https://badge.fury.io/py/FFTA)
 [![Documentation Status](https://readthedocs.org/projects/ffta/badge/?version=latest)](https://ffta.readthedocs.io/en/latest/?badge=latest)
 [![Coverage Status](https://coveralls.io/repos/github/rajgiriUW/ffta/badge.svg?branch=master)](https://coveralls.io/github/rajgiriUW/ffta?branch=master)
 
@@ -51,9 +50,7 @@
 ### Installation
 
 ```
 pip install ffta
 ```
 
 
-
-
```

### Comparing `FFTA-0.3.5.0/FFTA.egg-info/SOURCES.txt` & `FFTA-0.3.5.1/FFTA.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 FFTA.egg-info/requires.txt
 FFTA.egg-info/top_level.txt
 ffta/__init__.py
 ffta/__version__.py
 ffta/analyze_pixel.py
 ffta/line.py
 ffta/pixel.py
+ffta/_legacy_functions/__init__.py
+ffta/_legacy_functions/analyze.py
 ffta/acquisition/__init__.py
 ffta/acquisition/generate_chirp.py
 ffta/acquisition/polling.py
 ffta/analysis/__init__.py
 ffta/analysis/create_movie.py
 ffta/analysis/dist_cluster.py
 ffta/analysis/fft.py
```

### Comparing `FFTA-0.3.5.0/LICENSE.txt` & `FFTA-0.3.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `FFTA-0.3.5.0/PKG-INFO` & `FFTA-0.3.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: FFTA
-Version: 0.3.5.0
+Version: 0.3.5.1
 Summary: Fast Free Transient Analysis
 Home-page: https://github.com/rajgiriUW/ffta/
 Author: Rajiv Giridharagopal
 Author-email: rgiri@uw.edu
 License: MIT
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 [![PyPI version](https://badge.fury.io/py/FFTA.svg)](https://badge.fury.io/py/FFTA)
 [![Documentation Status](https://readthedocs.org/projects/ffta/badge/?version=latest)](https://ffta.readthedocs.io/en/latest/?badge=latest)
 [![Coverage Status](https://coveralls.io/repos/github/rajgiriUW/ffta/badge.svg?branch=master)](https://coveralls.io/github/rajgiriUW/ffta?branch=master)
 
@@ -51,9 +50,7 @@
 ### Installation
 
 ```
 pip install ffta
 ```
 
 
-
-
```

### Comparing `FFTA-0.3.5.0/README.md` & `FFTA-0.3.5.1/README.md`

 * *Files identical despite different names*

### Comparing `FFTA-0.3.5.0/ffta/acquisition/generate_chirp.py` & `FFTA-0.3.5.1/ffta/acquisition/generate_chirp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # -*- coding: utf-8 -*-
 """
 Created on Mon Mar 23 16:23:12 2020
 
 @author: Raj
 """
 
-import scipy.signal as sps
-import numpy as np
 import argparse
 
+import numpy as np
+import scipy.signal as sps
+
 
 def GenChirp(f_center, f_width=100e3, length=1e-2, sampling_rate=1e8, name='chirp'):
     '''
     Generates a single broad-frequency signal using SciPy chirp, writes to name.dat
     
     Important usage regarding the sampling rate:
     The sampling rate here must match that of the wave generator when you load
@@ -156,15 +157,15 @@
     
     :param beta:
     :type beta:
     
     :param sfx:
     :type sfx:
     '''
-    
+
     sample_rate = 1.0e8  # sampling rate used in Wavegenerator code
     total_samples = 800000
     pulse_samples = 700000
 
     data = np.arange(total_samples) / sample_rate
 
     data[:pulse_samples] = np.exp(-data[:pulse_samples] / tau) ** beta - 1
```

### Comparing `FFTA-0.3.5.0/ffta/acquisition/polling.py` & `FFTA-0.3.5.1/ffta/acquisition/polling.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,23 +13,24 @@
     Open Anaconda prompt
     Navigate to folder where this file is located
     
     python  polling.py "FOLDER WHERE DATA ARE BEING SAVED"
     
 '''
 
+import argparse
 import time
+
 import numpy as np
-from watchdog.observers import Observer
-from watchdog.events import FileSystemEventHandler
-from ffta import line, pixel_utils
+import pyUSID as usid
 from matplotlib import pyplot as plt
-import argparse
+from watchdog.events import FileSystemEventHandler
+from watchdog.observers import Observer
 
-import pyUSID as usid
+from ffta import line, pixel_utils
 
 
 class MyHandler(FileSystemEventHandler):
     '''
     Event Handler for polling the FFtrEFM directory for new files
     
     Every time a new file is created, this processes that .ibw as a Line
```

### Comparing `FFTA-0.3.5.0/ffta/analysis/fft.py` & `FFTA-0.3.5.1/ffta/analysis/fft.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,20 +7,25 @@
 Created on Tue Oct 20 17:42:41 2015
 
 @author: Suhas Somnath
 """
 ###############################################################################
 
 from __future__ import division, print_function, absolute_import
-import numpy as np  # for all array, data operations
+
+try:
+    from collections import Iterable
+except:
+    from collections.abc import Iterable
+from warnings import warn
+
 import matplotlib.pyplot as plt  # for all plots
-from scipy.special import erf
+import numpy as np  # for all array, data operations
 from scipy import signal as sps
-from collections import Iterable
-from warnings import warn
+from scipy.special import erf
 
 
 def get_fft_stack(image_stack):
     """
     Gets the 2D FFT for a single or stack of images by applying a blackman window
 
     :param image_stack: Either a 2D matrix [x, y] or a stack of 2D images arranged as [z or spectral, x, y]
```

### Comparing `FFTA-0.3.5.0/ffta/analysis/filtering.py` & `FFTA-0.3.5.1/ffta/analysis/filtering.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 # -*- coding: utf-8 -*-
 """
 Created on Mon Feb 26 17:15:36 2018
 
 @author: Raj
 """
 
-from .fft import FrequencyFilter
-from .gmode_utils import test_filter as gtest_filter
-import pyUSID as usid
+import warnings
+
 import numpy as np
+import pyUSID as usid
+from matplotlib import pyplot as plt
 from scipy import signal as sps
 
-from ffta.load import get_utils
-
 from ffta import pixel
-from matplotlib import pyplot as plt
-
-import warnings
+from ffta.load import get_utils
+from .fft import FrequencyFilter
+from .gmode_utils import test_filter as gtest_filter
 
 '''
 For filtering data using the pycroscopy filter command
 
 To set up a filter, you can choose any of the following:
 	Harmonic Filter: pick a frequency and bandpass filters that + 2w + 3e etc
 	Bandpass Filter: pick a specific frequency and pass that
@@ -33,387 +32,387 @@
 >>> ffta.hdf_utils.filtering.fft_filter(h5_main, hbf)
 
 
 '''
 
 
 def test_filter(hdf_file, freq_filts, parameters={}, pixelnum=[0, 0], noise_tolerance=5e-7,
-				show_plots=True, check_filter=True):
-	"""
-	Applies FFT Filter to the file at a specific line and displays the result
-
-	:param hdf_file: hdf_file to work on, e.g. hdf.file['/FF-raw'] if that's a Dataset
-		if ndarray, uses passed or default parameters
-		Use ndarray.flatten() to ensure correct dimensions
-	:type hdf_file: h5Py file or Nx1 NumPy array (preferred is NumPy array)
-		
-	:param freq_filts: Contains the filters to apply to the test signal
-	:type freq_filts: list of FrequencyFilter class objects
-		
-	:param parameters: Contains parameters in FF-raw file for constructing filters. Automatic if a Dataset/File
-		Must contain num_pts and samp_rate to be functional
-	:type parameters: dict, optional
-		
-	:param pixelnum: For extracting a specific pixel to do FFT Filtering on
-	:type pixelnum: int, optional
-	
-	:param noise_tolerance: Amount of noise below which signal is set to 0
-	:type noise_tolerance: float 0 to 1
-		
-	:param show_plots: Turns on FFT plots from Pycroscopy
-	:type show_plots : bool, optional
-		
-	:returns: tuple (filt_line, freq_filts, fig_filt, axes_filt)
-		WHERE
-		numpy.ndarray filt_line is filtered signal of hdf_file
-		list freq_filts is the filter parameters to be passed to SignalFilter
-	    matplotlib controls fig_filt, axes_filt - Only functional if show_plots is on
-	"""
-
-	reshape = False
-	ftype = str(type(hdf_file))
-	if ('h5py' in ftype) or ('Dataset' in ftype):  # hdf file
-
-		parameters = get_utils.get_params(hdf_file)
-		hdf_file = get_utils.get_pixel(hdf_file, [pixelnum[0], pixelnum[1]], array_form=True, transpose=False)
-		hdf_file = hdf_file.flatten()
-
-	if len(hdf_file.shape) == 2:
-		reshape = True
-		hdf_file = hdf_file.flatten()
+                show_plots=True, check_filter=True):
+    """
+    Applies FFT Filter to the file at a specific line and displays the result
+
+    :param hdf_file: hdf_file to work on, e.g. hdf.file['/FF-raw'] if that's a Dataset
+        if ndarray, uses passed or default parameters
+        Use ndarray.flatten() to ensure correct dimensions
+    :type hdf_file: h5Py file or Nx1 NumPy array (preferred is NumPy array)
+
+    :param freq_filts: Contains the filters to apply to the test signal
+    :type freq_filts: list of FrequencyFilter class objects
+
+    :param parameters: Contains parameters in FF-raw file for constructing filters. Automatic if a Dataset/File
+        Must contain num_pts and samp_rate to be functional
+    :type parameters: dict, optional
+
+    :param pixelnum: For extracting a specific pixel to do FFT Filtering on
+    :type pixelnum: int, optional
+
+    :param noise_tolerance: Amount of noise below which signal is set to 0
+    :type noise_tolerance: float 0 to 1
+
+    :param show_plots: Turns on FFT plots from Pycroscopy
+    :type show_plots : bool, optional
+
+    :returns: tuple (filt_line, freq_filts, fig_filt, axes_filt)
+        WHERE
+        numpy.ndarray filt_line is filtered signal of hdf_file
+        list freq_filts is the filter parameters to be passed to SignalFilter
+        matplotlib controls fig_filt, axes_filt - Only functional if show_plots is on
+    """
+
+    reshape = False
+    ftype = str(type(hdf_file))
+    if ('h5py' in ftype) or ('Dataset' in ftype):  # hdf file
+
+        parameters = get_utils.get_params(hdf_file)
+        hdf_file = get_utils.get_pixel(hdf_file, [pixelnum[0], pixelnum[1]], array_form=True, transpose=False)
+        hdf_file = hdf_file.flatten()
+
+    if len(hdf_file.shape) == 2:
+        reshape = True
+        hdf_file = hdf_file.flatten()
 
-	sh = hdf_file.shape
+    sh = hdf_file.shape
 
-	# Test filter on a single line:
-	filt_line, fig_filt, axes_filt = gtest_filter(hdf_file,
+    # Test filter on a single line:
+    filt_line, fig_filt, axes_filt = gtest_filter(hdf_file,
                                                   frequency_filters=freq_filts,
-												 noise_threshold=noise_tolerance,
-												 show_plots=show_plots)
+                                                  noise_threshold=noise_tolerance,
+                                                  show_plots=show_plots)
 
-	# If need to reshape
-	if reshape:
-		filt_line = np.reshape(filt_line, sh)
-
-	# Test filter out in Pixel
-	if check_filter:
-		plt.figure()
-		plt.plot(hdf_file, 'b')
-		plt.plot(filt_line, 'k')
-
-		h5_px_filt = pixel.Pixel(filt_line, parameters)
-		h5_px_filt.clear_filter_flags()
-		h5_px_filt.analyze()
-		h5_px_filt.plot(newplot=True)
-
-		h5_px_raw = pixel.Pixel(hdf_file, parameters)
-		h5_px_raw.analyze()
-		h5_px_raw.plot(newplot=True)
-
-	#    h5_px_raw_unfilt = pixel.Pixel(hdf_file, parameters)
-	#    h5_px_raw_unfilt.clear_filter_flags()
-	#    h5_px_raw_unfilt.analyze()
-	#    h5_px_raw_unfilt.plot(newplot=False,c1='y', c2='c')
+    # If need to reshape
+    if reshape:
+        filt_line = np.reshape(filt_line, sh)
+
+    # Test filter out in Pixel
+    if check_filter:
+        plt.figure()
+        plt.plot(hdf_file, 'b')
+        plt.plot(filt_line, 'k')
+
+        h5_px_filt = pixel.Pixel(filt_line, parameters)
+        h5_px_filt.clear_filter_flags()
+        h5_px_filt.analyze()
+        h5_px_filt.plot(newplot=True)
+
+        h5_px_raw = pixel.Pixel(hdf_file, parameters)
+        h5_px_raw.analyze()
+        h5_px_raw.plot(newplot=True)
+
+    #    h5_px_raw_unfilt = pixel.Pixel(hdf_file, parameters)
+    #    h5_px_raw_unfilt.clear_filter_flags()
+    #    h5_px_raw_unfilt.analyze()
+    #    h5_px_raw_unfilt.plot(newplot=False,c1='y', c2='c')
 
-	return filt_line, freq_filts, fig_filt, axes_filt
+    return filt_line, freq_filts, fig_filt, axes_filt
 
 
 def fft_filter(h5_main, freq_filts, noise_tolerance=5e-7, make_new=False, verbose=False):
-	"""
-	Stub for applying filter above to the entire FF image set
-	
-	:param h5_main: Dataset to work on, e.g. h5_main = px.hdf_utils.getDataSet(hdf.file, 'FF_raw')[0]
-	:type h5_main : h5py.Dataset object
-		
-	:param freq_filts: List of frequency filters usually generated in test_line above
-	:type freq_filts: list
-		
-	:param noise_tolerance: Level below which data are set to 0. Higher values = more noise (more tolerant)
-	:type noise_tolerance : float, optional
-		
-	:param make_new: Allows for re-filtering the data by creating a new folder
-	:type make_new: bool, optional
-
-	:param verbose:
-	:type verbose: bool, optional
-	
-	:returns: Filtered dataset within latest -FFT_Filtering Group
-	:rtype: Dataset
-		
-	"""
-
-	h5_filt_grp = usid.hdf_utils.check_for_old(h5_main, 'FFT_Filtering')
-
-	if make_new == True or not any(h5_filt_grp):
-
-		sig_filt = px.processing.SignalFilter(h5_main, frequency_filters=freq_filts,
-											  noise_threshold=noise_tolerance,
-											  write_filtered=True, write_condensed=False,
-											  num_pix=1, verbose=verbose, cores=2, max_mem_mb=512)
-
-		h5_filt_grp = sig_filt.compute()
-
-	else:
-		print('Taking previously computed results')
-		h5_filt = h5_filt_grp[0]['Filtered_Data']
-
-	h5_filt = h5_filt_grp['Filtered_Data']
-	usid.hdf_utils.copy_attributes(h5_main.parent, h5_filt)
-	usid.hdf_utils.copy_attributes(h5_main.parent, h5_filt.parent)
+    """
+    Stub for applying filter above to the entire FF image set
+
+    :param h5_main: Dataset to work on, e.g. h5_main = px.hdf_utils.getDataSet(hdf.file, 'FF_raw')[0]
+    :type h5_main : h5py.Dataset object
+
+    :param freq_filts: List of frequency filters usually generated in test_line above
+    :type freq_filts: list
+
+    :param noise_tolerance: Level below which data are set to 0. Higher values = more noise (more tolerant)
+    :type noise_tolerance : float, optional
+
+    :param make_new: Allows for re-filtering the data by creating a new folder
+    :type make_new: bool, optional
+
+    :param verbose:
+    :type verbose: bool, optional
+
+    :returns: Filtered dataset within latest -FFT_Filtering Group
+    :rtype: Dataset
 
-	return h5_filt
+    """
+
+    h5_filt_grp = usid.hdf_utils.check_for_old(h5_main, 'FFT_Filtering')
+
+    if make_new == True or not any(h5_filt_grp):
+
+        sig_filt = px.processing.SignalFilter(h5_main, frequency_filters=freq_filts,
+                                              noise_threshold=noise_tolerance,
+                                              write_filtered=True, write_condensed=False,
+                                              num_pix=1, verbose=verbose, cores=2, max_mem_mb=512)
+
+        h5_filt_grp = sig_filt.compute()
+
+    else:
+        print('Taking previously computed results')
+        h5_filt = h5_filt_grp[0]['Filtered_Data']
+
+    h5_filt = h5_filt_grp['Filtered_Data']
+    usid.hdf_utils.copy_attributes(h5_main.parent, h5_filt)
+    usid.hdf_utils.copy_attributes(h5_main.parent, h5_filt.parent)
+
+    return h5_filt
 
 
 def lowpass(hdf_file, parameters={}, pixelnum=[0, 0], f_cutoff=None):
-	'''
-	Interfaces to px.pycroscopy.fft.LowPassFilter
-	
-	:param hdf_file:
-	:type hdf_file:
-
-	:param parameters:
-	:type parameters: dict
-	
-	:param pixelnum: See test_filter below
-	:type pixelnum: list
-
-	:param f_cutoff: frequency to cut off. Defaults to 2*drive frequency rounded to nearest 100 kHz
-	:type f_cutoff: int
-		
-	:returns:
-	:rtype:
-	'''
-	hdf_file, num_pts, drive, samp_rate = _get_pixel_for_filtering(hdf_file, parameters, pixelnum)
+    '''
+    Interfaces to px.pycroscopy.fft.LowPassFilter
+
+    :param hdf_file:
+    :type hdf_file:
+
+    :param parameters:
+    :type parameters: dict
+
+    :param pixelnum: See test_filter below
+    :type pixelnum: list
+
+    :param f_cutoff: frequency to cut off. Defaults to 2*drive frequency rounded to nearest 100 kHz
+    :type f_cutoff: int
 
-	if not f_cutoff:
-		lpf_cutoff = np.round(drive / 1e5, decimals=0) * 2 * 1e5  # 2times the drive frequency, round up
+    :returns:
+    :rtype:
+    '''
+    hdf_file, num_pts, drive, samp_rate = _get_pixel_for_filtering(hdf_file, parameters, pixelnum)
 
-	lpf = px.processing.fft.LowPassFilter(num_pts, samp_rate, lpf_cutoff)
+    if not f_cutoff:
+        lpf_cutoff = np.round(drive / 1e5, decimals=0) * 2 * 1e5  # 2times the drive frequency, round up
 
-	return lpf
+    lpf = px.processing.fft.LowPassFilter(num_pts, samp_rate, lpf_cutoff)
+
+    return lpf
 
 
 def bandpass(hdf_file, parameters={}, pixelnum=[0, 0], f_center=None, f_width=10e3, harmonic=None, fir=False):
-	'''
-	Interfaces to pycroscopy.processing.fft.BandPassFilter
-	Note that this is effectively a Harmonic Filter of number_harmonics 1, but with finite impulse response option
-
-	:param hdf_file:
-	:type hdf_file:
-	
-	:param parameters:
-	:type parameters: dict
-	
-	:param pixelnum: See test_filter below
-	:type pixelnum: list
-	
-	:param f_center: center frequency for the specific band to pass
-	:type f_center: int
-		
-	:param f_width: width of frequency to pass
-	:type f_width: int
-	
-	:param harmonic: if specified, sets the band to this specific multiple of the drive frequency
-	:type harmonic: int
-	
-	:param fir: uses an Finite Impulse Response filter instead of a normal boxcar
-	:type fir: bool
-	
-	:returns: 1D numpy array describing the bandpass filter
-	:rtype: 1D numpy array: 
-	'''
-
-	hdf_file, num_pts, drive, samp_rate = _get_pixel_for_filtering(hdf_file, parameters, pixelnum)
-
-	# default is the 2*w signal (second harmonic for KPFM)
-	if not f_center:
-		if not harmonic:
-			f_center = drive * 2
-		else:
-			f_center = int(drive * harmonic)
+    '''
+    Interfaces to pycroscopy.processing.fft.BandPassFilter
+    Note that this is effectively a Harmonic Filter of number_harmonics 1, but with finite impulse response option
+
+    :param hdf_file:
+    :type hdf_file:
+
+    :param parameters:
+    :type parameters: dict
+
+    :param pixelnum: See test_filter below
+    :type pixelnum: list
+
+    :param f_center: center frequency for the specific band to pass
+    :type f_center: int
+
+    :param f_width: width of frequency to pass
+    :type f_width: int
+
+    :param harmonic: if specified, sets the band to this specific multiple of the drive frequency
+    :type harmonic: int
+
+    :param fir: uses an Finite Impulse Response filter instead of a normal boxcar
+    :type fir: bool
+
+    :returns: 1D numpy array describing the bandpass filter
+    :rtype: 1D numpy array:
+    '''
+
+    hdf_file, num_pts, drive, samp_rate = _get_pixel_for_filtering(hdf_file, parameters, pixelnum)
 
-	bpf = px.processing.fft.BandPassFilter(num_pts, samp_rate, f_center, f_width, fir=fir)
+    # default is the 2*w signal (second harmonic for KPFM)
+    if not f_center:
+        if not harmonic:
+            f_center = drive * 2
+        else:
+            f_center = int(drive * harmonic)
 
-	return bpf
+    bpf = px.processing.fft.BandPassFilter(num_pts, samp_rate, f_center, f_width, fir=fir)
+
+    return bpf
 
 
 def harmonic(hdf_file, parameters={}, pixelnum=[0, 0], first_harm=1, bandwidth=None, num_harmonics=5):
-	'''
-	Interfaces with px.processing.fft.HarmonicFilter
+    '''
+    Interfaces with px.processing.fft.HarmonicFilter
+
+    :param hdf_file:
+    :type hdf_file:
+
+    :param parameters:
+    :type parameters: dict
+
+    :param pixelnum: See test_filter below
+    :type pixelnum: list
+
+    :param first_harm: The first harmonic based on the drive frequency to use
+        For G-KPFM this should be explicitly set to 2
+    :type first_harm: int
+
+    :param bandwidth: bandwidth for filtering. For computational purposes this is hard-set to 2500 (2.5 kHz)
+    :type bandwidth: int
 
-	:param hdf_file:
-	:type hdf_file:
-	
-	:param parameters:
-	:type parameters: dict
-	
-	:param pixelnum: See test_filter below
-	:type pixelnum: list
-	
-	:param first_harm: The first harmonic based on the drive frequency to use
-		For G-KPFM this should be explicitly set to 2
-	:type first_harm: int
-		
-	:param bandwidth: bandwidth for filtering. For computational purposes this is hard-set to 2500 (2.5 kHz)
-	:type bandwidth: int
-		
-	:param num_harmonics: The number of harmonics to use (omega, 2*omega, 3*omega, etc)
-	:type num_harmonics: int
-	
-	:returns:
-	:rtype:
-		
-	'''
-
-	hdf_file, num_pts, drive, samp_rate = _get_pixel_for_filtering(hdf_file, parameters, pixelnum)
-
-	if not bandwidth:
-		bandwidth = 2500
-	elif bandwidth > 2500:
-		warnings.warn('Bandwidth of that level might cause errors')
-		bandwidth = 2500
+    :param num_harmonics: The number of harmonics to use (omega, 2*omega, 3*omega, etc)
+    :type num_harmonics: int
 
-	first_harm = drive * first_harm
+    :returns:
+    :rtype:
 
-	hbf = px.processing.fft.HarmonicPassFilter(num_pts, samp_rate, first_harm, bandwidth, num_harmonics)
+    '''
 
-	return hbf
+    hdf_file, num_pts, drive, samp_rate = _get_pixel_for_filtering(hdf_file, parameters, pixelnum)
+
+    if not bandwidth:
+        bandwidth = 2500
+    elif bandwidth > 2500:
+        warnings.warn('Bandwidth of that level might cause errors')
+        bandwidth = 2500
+
+    first_harm = drive * first_harm
+
+    hbf = px.processing.fft.HarmonicPassFilter(num_pts, samp_rate, first_harm, bandwidth, num_harmonics)
+
+    return hbf
 
 
 def noise_filter(hdf_file, parameters={}, pixelnum=[0, 0],
-				 centers=[10E3, 50E3, 100E3, 150E3, 200E3],
-				 widths=[20E3, 1E3, 1E3, 1E3, 1E3]):
-	'''
-	Interfaces with pycroscopy.processing.fft.NoiseBandFilter
-
-	:param hdf_file:
-	:type hdf_file:
-	
-	:param parameters:
-	:type parameters: dict
-	
-	:param pixelnum: See test_filter below
-	:type pixelnum: list
-	
-	:param centers: List of Frequencies to filter out
-	:type centers: list
-		
-	:param widths: List of frequency widths for each filter. e,g. in default case (10 kHz center, 20 kHz width) is from 0 to 20 kHz
-	:type widths: list
-	
-	:returns:
-	:rtype:
-	'''
+                 centers=[10E3, 50E3, 100E3, 150E3, 200E3],
+                 widths=[20E3, 1E3, 1E3, 1E3, 1E3]):
+    '''
+    Interfaces with pycroscopy.processing.fft.NoiseBandFilter
+
+    :param hdf_file:
+    :type hdf_file:
 
-	hdf_file, num_pts, drive, samp_rate = _get_pixel_for_filtering(hdf_file, parameters, pixelnum)
+    :param parameters:
+    :type parameters: dict
 
-	nf = px.processing.fft.NoiseBandFilter(num_pts, samp_rate, centers, widths)
+    :param pixelnum: See test_filter below
+    :type pixelnum: list
 
-	return nf
+    :param centers: List of Frequencies to filter out
+    :type centers: list
+
+    :param widths: List of frequency widths for each filter. e,g. in default case (10 kHz center, 20 kHz width) is from 0 to 20 kHz
+    :type widths: list
+
+    :returns:
+    :rtype:
+    '''
+
+    hdf_file, num_pts, drive, samp_rate = _get_pixel_for_filtering(hdf_file, parameters, pixelnum)
+
+    nf = px.processing.fft.NoiseBandFilter(num_pts, samp_rate, centers, widths)
+
+    return nf
 
 
 def _get_pixel_for_filtering(hdf_file, parameters={}, pixelnum=[0, 0]):
-	"""
-	
-	:param hdf_file:
-	:type hdf_file:
-	
-	:param parameters:
-	:type parameters: dict
-	
-	:param pixelnum: See test_filter below
-	:type pixelnum: list
-	
-	:returns: tuple (hdf_file, num_pts, drive, samp_rate)
-		WHERE
-		[type] hdf_file is...
-		int num_pts is...
-		[type] drive is...
-		[type] samp_rate is...
-	"""
-	ftype = str(type(hdf_file))
-	if ('h5py' in ftype) or ('Dataset' in ftype):  # hdf file
-
-		parameters = usid.hdf_utils.get_attributes(hdf_file)
-		hdf_file = get_utils.get_pixel(hdf_file, [pixelnum[0], pixelnum[1]], array_form=True, transpose=False)
-		hdf_file = hdf_file.flatten()
-
-	if len(hdf_file.shape) == 2:
-		hdf_file = hdf_file.flatten()
-
-	num_pts = hdf_file.shape[0]
-	drive = parameters['drive_freq']
-	samp_rate = parameters['sampling_rate']
+    """
 
-	return hdf_file, num_pts, drive, samp_rate
+    :param hdf_file:
+    :type hdf_file:
+
+    :param parameters:
+    :type parameters: dict
+
+    :param pixelnum: See test_filter below
+    :type pixelnum: list
+
+    :returns: tuple (hdf_file, num_pts, drive, samp_rate)
+        WHERE
+        [type] hdf_file is...
+        int num_pts is...
+        [type] drive is...
+        [type] samp_rate is...
+    """
+    ftype = str(type(hdf_file))
+    if ('h5py' in ftype) or ('Dataset' in ftype):  # hdf file
+
+        parameters = usid.hdf_utils.get_attributes(hdf_file)
+        hdf_file = get_utils.get_pixel(hdf_file, [pixelnum[0], pixelnum[1]], array_form=True, transpose=False)
+        hdf_file = hdf_file.flatten()
+
+    if len(hdf_file.shape) == 2:
+        hdf_file = hdf_file.flatten()
+
+    num_pts = hdf_file.shape[0]
+    drive = parameters['drive_freq']
+    samp_rate = parameters['sampling_rate']
+
+    return hdf_file, num_pts, drive, samp_rate
 
 
 # placeholder until accepted in pull request
 class BandPassFilter(FrequencyFilter):
-	def __init__(self, signal_length, samp_rate, f_center, f_width,
-				 fir=False, fir_taps=1999):
-		"""
-		Builds a bandpass filter
-		
-		:param signal_length: Points in the FFT. Assuming Signal in frequency space (ie - after FFT shifting)
-		:type signal_length: unsigned int
-		
-		:param samp_rate: sampling rate
-		:type samp_rate: unsigned integer
-		
-		:param f_center: Center frequency for filter
-		:type f_center: unsigned integer
-		
-		:param f_width: Frequency width of the pass band
-		:type f_width: unsigned integer
-		
-		:param fir: True uses a finite impulse response (FIR) response instead of a standard boxcar. FIR is causal
-		:type fir: bool, optional
-		
-		:param fir_taps: Number of taps (length of filter) for finite impulse response filter
-		:type fir_taps: int
-			
-		:returns: 1D numpy array describing the bandpass filter
-		:rtype: 1D numpy array: 
-
-		"""
-
-		if f_center >= 0.5 * samp_rate:
-			raise ValueError('Filter cutoff exceeds Nyquist rate')
-
-		self.f_center = f_center
-		self.f_width = f_width
-
-		super(BandPassFilter, self).__init__(signal_length, samp_rate)
-
-		cent = int(round(0.5 * signal_length))
-
-		# very simple boxcar
-		ind = int(round(signal_length * (f_center / samp_rate)))
-		sz = int(round(cent * f_width / samp_rate))
-
-		bpf = np.zeros(signal_length, dtype=np.float32)
-
-		# Finite Impulse Response or Boxcar
-		if not fir:
-
-			bpf[cent - ind - sz:cent - ind + sz + 1] = 1
-			bpf[cent + ind - sz:cent + ind + sz + 1] = 1
-
-		else:
-
-			freq_low = (f_center - f_width) / (0.5 * samp_rate)
-			freq_high = (f_center + f_width) / (0.5 * samp_rate)
-
-			band = [freq_low, freq_high]
-
-			taps = sps.firwin(int(fir_taps), band, pass_zero=False,
-							  window='blackman')
-			bpf = np.abs(np.fft.fftshift(np.fft.fft(taps, n=signal_length)))
-
-		self.value = bpf
-
-	def get_parms(self):
-		basic_parms = super(BandPassFilter, self).get_parms()
-		prefix = 'band_pass_'
-		this_parms = {prefix + 'start_freq': self.f_center, prefix + 'band_width': self.f_width}
-		this_parms.update(basic_parms)
-		return this_parms
+    def __init__(self, signal_length, samp_rate, f_center, f_width,
+                 fir=False, fir_taps=1999):
+        """
+        Builds a bandpass filter
+
+        :param signal_length: Points in the FFT. Assuming Signal in frequency space (ie - after FFT shifting)
+        :type signal_length: unsigned int
+
+        :param samp_rate: sampling rate
+        :type samp_rate: unsigned integer
+
+        :param f_center: Center frequency for filter
+        :type f_center: unsigned integer
+
+        :param f_width: Frequency width of the pass band
+        :type f_width: unsigned integer
+
+        :param fir: True uses a finite impulse response (FIR) response instead of a standard boxcar. FIR is causal
+        :type fir: bool, optional
+
+        :param fir_taps: Number of taps (length of filter) for finite impulse response filter
+        :type fir_taps: int
+
+        :returns: 1D numpy array describing the bandpass filter
+        :rtype: 1D numpy array:
+
+        """
+
+        if f_center >= 0.5 * samp_rate:
+            raise ValueError('Filter cutoff exceeds Nyquist rate')
+
+        self.f_center = f_center
+        self.f_width = f_width
+
+        super(BandPassFilter, self).__init__(signal_length, samp_rate)
+
+        cent = int(round(0.5 * signal_length))
+
+        # very simple boxcar
+        ind = int(round(signal_length * (f_center / samp_rate)))
+        sz = int(round(cent * f_width / samp_rate))
+
+        bpf = np.zeros(signal_length, dtype=np.float32)
+
+        # Finite Impulse Response or Boxcar
+        if not fir:
+
+            bpf[cent - ind - sz:cent - ind + sz + 1] = 1
+            bpf[cent + ind - sz:cent + ind + sz + 1] = 1
+
+        else:
+
+            freq_low = (f_center - f_width) / (0.5 * samp_rate)
+            freq_high = (f_center + f_width) / (0.5 * samp_rate)
+
+            band = [freq_low, freq_high]
+
+            taps = sps.firwin(int(fir_taps), band, pass_zero=False,
+                              window='blackman')
+            bpf = np.abs(np.fft.fftshift(np.fft.fft(taps, n=signal_length)))
+
+        self.value = bpf
+
+    def get_parms(self):
+        basic_parms = super(BandPassFilter, self).get_parms()
+        prefix = 'band_pass_'
+        this_parms = {prefix + 'start_freq': self.f_center, prefix + 'band_width': self.f_width}
+        this_parms.update(basic_parms)
+        return this_parms
```

### Comparing `FFTA-0.3.5.0/ffta/analysis/gmode_utils.py` & `FFTA-0.3.5.1/ffta/analysis/gmode_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,33 +7,38 @@
 
 Created on Thu May 05 13:29:12 2016
 
 @author: Suhas Somnath
 """
 
 from __future__ import division, print_function, absolute_import
+
 import sys
-from collections import Iterable
-from warnings import warn
+try:
+    from collections import Iterable
+except:
+    from collections.abc import Iterable
 from numbers import Number
+from warnings import warn
+
 import matplotlib.pyplot as plt
 import numpy as np
-from .fft import get_noise_floor, are_compatible_filters, build_composite_freq_filter
-
-from sidpy.hdf.hdf_utils import get_attr
-from sidpy.viz.plot_utils import set_tick_font_size, plot_curves
-
+from pyUSID import Dimension
 from pyUSID import USIDataset
 from pyUSID.io.hdf_utils import check_if_main, write_main_dataset, \
     create_results_group
-from pyUSID import Dimension
+from sidpy.hdf.hdf_utils import get_attr
+from sidpy.viz.plot_utils import set_tick_font_size, plot_curves
+
+from .fft import get_noise_floor, are_compatible_filters, build_composite_freq_filter
 
 if sys.version_info.major == 3:
     unicode = str
 
+
 # TODO: Phase rotation not implemented correctly. Find and use excitation frequency
 
 
 ###############################################################################
 
 def test_filter(resp_wfm, frequency_filters=None, noise_threshold=None, excit_wfm=None, show_plots=True,
                 plot_title=None, verbose=False):
```

### Comparing `FFTA-0.3.5.0/ffta/analysis/mask_utils.py` & `FFTA-0.3.5.1/ffta/analysis/mask_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,106 +5,106 @@
 @author: Raj
 """
 
 import numpy as np
 
 
 def load_mask_txt(path, rows=64, flip=False):
-	"""
-	Loads mask from text
+    """
+    Loads mask from text
 
-	:param path: Filepath to disk location of the mask
-	:type path: str
-		
-	:param rows: Sets a hard limit on the rows of the mask, due to Igor images being larger (rowwise)
-		than the typical G-Mode/FF-trEFM Mask size
-	:type rows: int, optional
-		
-	:param flip: Whether to flip the mask left-to-right to match CPD
-	:type flip: bool, optional
-		
-	:returns: the mask itself
-	
-	"""
-	mask = np.loadtxt(path)
-
-	if mask.shape[1] < mask.shape[0]:  # we know it's fewer rows than columns
-		mask = mask.transpose()
+    :param path: Filepath to disk location of the mask
+    :type path: str
 
-	if flip:
-		mask = np.fliplr(mask)
+    :param rows: Sets a hard limit on the rows of the mask, due to Igor images being larger (rowwise)
+        than the typical G-Mode/FF-trEFM Mask size
+    :type rows: int, optional
 
-	mask = mask[:rows, :]
+    :param flip: Whether to flip the mask left-to-right to match CPD
+    :type flip: bool, optional
 
-	return mask
+    :returns: the mask itself
+
+    """
+    mask = np.loadtxt(path)
+
+    if mask.shape[1] < mask.shape[0]:  # we know it's fewer rows than columns
+        mask = mask.transpose()
+
+    if flip:
+        mask = np.fliplr(mask)
+
+    mask = mask[:rows, :]
+
+    return mask
 
 
 def load_masks(mask):
-	"""
-	Outputs several useful mask versions
-	
-	For reference:
-		NaNs = 1s in the mask = transparent in display
-		0s = 0s in the mask = opaque in display (i.e., are exluded/masked)
-	
-	:param mask: The mask to process into various new masks
-	:type mask: ndarray 2D (rows, columns)
-		
-	:returns: tuple (mask_nan, mask_on_1D, mask_off_1D)
-		WHERE
-		2D ndarray mask_nan - all 1s are NaNs, primarily for image display. (rows, columns)
-		1D ndarray mask_on_1D - non-NaN pixels as a 1D list for distance calculation (rows*columns)
-		1D ndarray mask_off_1D - NaN pixels as a 1D list for CPD masking (rows*columns) 
-		
-	"""
-
-	mask_nan = np.copy(mask)
-
-	# tuple of coordinates
-	zeros = np.where(mask_nan == 0)
-	nans = np.where(mask_nan == 1)
-	mask_on_1D = np.array([(x, y) for x, y in zip(zeros[0], zeros[1])])
-	mask_off_1D = np.array([(x, y) for x, y in zip(nans[0], nans[1])])
+    """
+    Outputs several useful mask versions
+
+    For reference:
+        NaNs = 1s in the mask = transparent in display
+        0s = 0s in the mask = opaque in display (i.e., are exluded/masked)
+
+    :param mask: The mask to process into various new masks
+    :type mask: ndarray 2D (rows, columns)
+
+    :returns: tuple (mask_nan, mask_on_1D, mask_off_1D)
+        WHERE
+        2D ndarray mask_nan - all 1s are NaNs, primarily for image display. (rows, columns)
+        1D ndarray mask_on_1D - non-NaN pixels as a 1D list for distance calculation (rows*columns)
+        1D ndarray mask_off_1D - NaN pixels as a 1D list for CPD masking (rows*columns)
+
+    """
+
+    mask_nan = np.copy(mask)
 
-	mask_nan[mask_nan == 1] = np.nan
+    # tuple of coordinates
+    zeros = np.where(mask_nan == 0)
+    nans = np.where(mask_nan == 1)
+    mask_on_1D = np.array([(x, y) for x, y in zip(zeros[0], zeros[1])])
+    mask_off_1D = np.array([(x, y) for x, y in zip(nans[0], nans[1])])
 
-	return mask_nan, mask_on_1D, mask_off_1D
+    mask_nan[mask_nan == 1] = np.nan
+
+    return mask_nan, mask_on_1D, mask_off_1D
 
 
 def averagemask(CPDarr, mask, rows=128, nan_flag=1, avg_flag=0):
-	'''
-	Returns an averaged CPD trace given the Igor mask
+    '''
+    Returns an averaged CPD trace given the Igor mask
+
+    :param CPDarr: the CPD of n-by-samples, typically 8192 x 128 (8192 pixels, 128 CPD points)
+        Rows = 128 is default of 128x64 images
+    :type CPDarr:
+
+    :param mask: The mask to process into various new masks
+    :type mask: ndarray 2D (rows, columns)
+
+    :param rows:
+    :type rows: int
+
+    :param nan_flag: what value in the mask to set to NaN. These are IGNORED
+        1 is "transparent" in Igor mask
+        0 is "opaque/masked off" in Igor mask
+    :type nan_flag: int, 0 or 1
+
+    :param avg_flag: what values in mask to average.
+    :type avg_flag:
+
+    :returns: the averaged CPD of those pixels
+    :rtype:
+
+    '''
+    mask1D = mask.flatten()
+
+    CPDpixels = np.array([])
 
-	:param CPDarr: the CPD of n-by-samples, typically 8192 x 128 (8192 pixels, 128 CPD points)
-		Rows = 128 is default of 128x64 images
-	:type CPDarr:
-	
-	:param mask: The mask to process into various new masks
-	:type mask: ndarray 2D (rows, columns)
-	
-	:param rows:
-	:type rows: int
-	
-	:param nan_flag: what value in the mask to set to NaN. These are IGNORED  
-		1 is "transparent" in Igor mask
-		0 is "opaque/masked off" in Igor mask
-	:type nan_flag: int, 0 or 1
-		
-	:param avg_flag: what values in mask to average.
-	:type avg_flag:
-		
-	:returns: the averaged CPD of those pixels
-	:rtype:
-	
-	'''
-	mask1D = mask.flatten()
-
-	CPDpixels = np.array([])
-
-	index = [i for i in np.where(mask1D == avg_flag)[0]]
-	for i in index:
-		CPDpixels = np.append(CPDpixels, CPDarr[i, :])
+    index = [i for i in np.where(mask1D == avg_flag)[0]]
+    for i in index:
+        CPDpixels = np.append(CPDpixels, CPDarr[i, :])
 
-	CPDpixels = np.reshape(CPDpixels, [len(index), CPDarr.shape[1]])
-	CPDpixels = np.mean(CPDpixels, axis=0)
+    CPDpixels = np.reshape(CPDpixels, [len(index), CPDarr.shape[1]])
+    CPDpixels = np.mean(CPDpixels, axis=0)
 
-	return CPDpixels
+    return CPDpixels
```

### Comparing `FFTA-0.3.5.0/ffta/analysis/proc_utils.py` & `FFTA-0.3.5.1/ffta/analysis/proc_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 Created on Tue Jan 05 07:55:56 2016
 
 @author: Chris Smith, Suhas Somnath
 
 """
 
 from __future__ import division, print_function, absolute_import
+
 import itertools
+
 import numpy as np
 
 
 def get_component_slice(components, total_components=None):
     """
     Check the components object to determine how to use it to slice the dataset
 
@@ -68,15 +70,15 @@
             if len(list_of_ranges) == 1:
                 # increment the second index by 1 to be consistent with python
                 comp_slice = slice(int(list_of_ranges[0][0]), int(list_of_ranges[0][1] + 1))
 
     elif isinstance(components, slice):
         # Components is already a slice
         comp_slice = components
-        num_comps = np.arange(components.stop+1)[comp_slice].size
+        num_comps = np.arange(components.stop + 1)[comp_slice].size
 
         if total_components is not None:
             num_comps = np.min(num_comps, total_components)
 
     else:
         raise TypeError('Unsupported component type supplied to get_component_slice.  '
                         'Allowed types are integer, numpy array, list, tuple, and slice.')
```

### Comparing `FFTA-0.3.5.0/ffta/analysis/select_pixel.py` & `FFTA-0.3.5.1/ffta/analysis/select_pixel.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # -*- coding: utf-8 -*-
 """
 Created on Sun Mar 27 21:19:11 2022
 
 @author: Raj
 """
 
-from ffta.load import get_utils
-from ffta.hdf_utils.process import plot_tfp
-from ffta.hdf_utils.process import FFtrEFM
-from sidpy.hdf.hdf_utils import get_attributes
-from sidpy.viz import plot_utils
+import warnings
+
+import h5py
 import matplotlib.pyplot as plt
 from matplotlib.widgets import Cursor
-import h5py
-import warnings
+from sidpy.hdf.hdf_utils import get_attributes
+from sidpy.viz import plot_utils
+
+from ffta.hdf_utils.process import FFtrEFM
+
 
 def select(data, scale_tfp=1e6, **kwargs):
     '''
     Chooses a pixel and then displays the instantaneous frequency 
     
     :param data: The dataset to plot
     :type data: USID Dataset or FFtrEFM class object (inherits Process) or the parent Group
@@ -32,63 +33,61 @@
 		WHERE
 		numpy.ndarray filt_line is filtered signal of hdf_file
 		list freq_filts is the filter parameters to be passed to SignalFilter
 	    matplotlib controls fig_filt, axes_filt - Only functional if show_plots is on
     
     '''
 
-    fig, ax = plt.subplots(facecolor='white', figsize=(8,6))
+    fig, ax = plt.subplots(facecolor='white', figsize=(8, 6))
 
-    if isinstance(data, h5py.Dataset):    
+    if isinstance(data, h5py.Dataset):
         data = data.parent
         warnings.warn('Should specify the parent group, not a dataset')
-    
+
     if isinstance(data, FFtrEFM):
 
         img_length = data.parm_dict['FastScanSize']
         img_height = data.parm_dict['SlowScanSize']
-        
+
         num_cols = data.parm_dict['num_cols']
         num_rows = data.parm_dict['num_rows']
-        
+
         tfp = data.h5_tfp[()]
 
     elif isinstance(data, h5py.Group):
-        
+
         attr = get_attributes(data['Inst_Freq'])
         img_length = attr['FastScanSize']
         img_height = attr['SlowScanSize']
-        
+
         num_cols = attr['num_cols']
         num_rows = attr['num_rows']
-        
+
         tfp = data['tfp']
-        
+
     elif isinstance(data, h5py.Dataset):
-        
+
         attr = get_attributes(data)
         img_length = attr['FastScanSize']
         img_height = attr['SlowScanSize']
-        
+
         num_cols = attr['num_cols']
         num_rows = attr['num_rows']
-        
+
         tfp = data
-    
-    tfp = tfp[()] #numpy array
-    
+
+    tfp = tfp[()]  # numpy array
+
     kwarg = {'origin': 'lower', 'x_vec': img_length * 1e6,
              'y_vec': img_height * 1e6, 'num_ticks': 5, 'stdevs': 3, 'show_cbar': True}
-    
+
     ax.set_title('tFP Image')
-    
+
     for k, v in kwarg.items():
         if k not in kwargs:
             kwargs.update({k: v})
-    
+
     tfp_image, cbar_tfp = plot_utils.plot_map(ax, tfp * scale_tfp,
                                               cmap='inferno', **kwargs)
     cbar_tfp.set_label('Time (us)', rotation=270, labelpad=16)
     cursor = Cursor(ax, linewidth=2, vertOn=False, horizOn=False)
     plt.show()
-    
-
```

### Comparing `FFTA-0.3.5.0/ffta/analysis/svd.py` & `FFTA-0.3.5.1/ffta/analysis/svd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 # -*- coding: utf-8 -*-
 """
 Created on Wed Mar  7 22:04:39 2018
 
 @author: Raj
 """
 
-import pyUSID as usid
+import h5py
 import numpy as np
-
-from .svd_utils import SVD, rebuild_svd
-
+import pyUSID as usid
 from matplotlib import pyplot as plt
+from sidpy.viz import plot_utils
 
-from ffta.hdf_utils import hdf_utils
 from ffta.load import get_utils
-import h5py
-from sidpy.viz import plot_utils
+from .svd_utils import SVD, rebuild_svd
 
 """
 Wrapper to SVD functions, specific to ffta Class.
 
 Typical usage:
     >> h5_svd = svd.test_svd(h5_avg)
     >> clean = [0,1,2,3] # to filter to only first 4 components
@@ -173,22 +170,22 @@
     except:
         pass
 
     if savefig:
         plt.savefig('Scree_plot.png')
 
     fig_abun, axes = plot_utils.plot_map_stack(abun_maps, num_comps=num_plots, title='SVD Abundance Maps',
-                                                        color_bar_mode='single', cmap='inferno', reverse_dims=True,
-                                                        fig_mult=(3.5, 3.5), facecolor='white', **kwargs)
+                                               color_bar_mode='single', cmap='inferno', reverse_dims=True,
+                                               fig_mult=(3.5, 3.5), facecolor='white', **kwargs)
     fig_abun.tight_layout()
     if savefig:
         plt.savefig('Abundance_maps.png')
 
     fig_eigvec, axes = plot_utils.plot_curves(h5_spec_vals * 1e3, eigen_vecs, use_rainbow_plots=False,
-                                                       x_label='Time (ms)', y_label=units,
-                                                       num_plots=num_plots, subtitle_prefix='Component',
-                                                       title='SVD Eigenvectors', evenly_spaced=False, **kwargs)
+                                              x_label='Time (ms)', y_label=units,
+                                              num_plots=num_plots, subtitle_prefix='Component',
+                                              title='SVD Eigenvectors', evenly_spaced=False, **kwargs)
     fig_eigvec.tight_layout()
     if savefig:
         plt.savefig('Eigenvectors.png')
 
     return
```

### Comparing `FFTA-0.3.5.0/ffta/analysis/svd_utils.py` & `FFTA-0.3.5.1/ffta/analysis/svd_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,39 +7,40 @@
 
 Created on Mon Mar 28 09:45:08 2016
 
 @author: Suhas Somnath, Chris Smith
 """
 
 from __future__ import division, print_function, absolute_import
+
 import time
 from multiprocessing import cpu_count
-import numpy as np
-from sklearn.utils import gen_batches
-from sklearn.utils.extmath import randomized_svd
 
-from sidpy.hdf.reg_ref import get_indices_for_region_ref, create_region_reference
-from sidpy.hdf.hdf_utils import get_attr, write_simple_attrs, copy_attributes
-from sidpy.proc.comp_utils import get_available_memory
+import h5py
+import numpy as np
+from matplotlib import pyplot as plt
+from pyUSID import Dimension
+from pyUSID import USIDataset
+from pyUSID.io.anc_build_utils import calc_chunks
+from pyUSID.io.hdf_utils import find_results_groups, \
+    reshape_to_n_dims, write_main_dataset, create_results_group, \
+    create_indexed_group, find_dataset
+from pyUSID.processing.process import Process
 from sidpy.base.string_utils import format_time
 from sidpy.hdf.dtype_utils import check_dtype, stack_real_to_target_dtype
+from sidpy.hdf.hdf_utils import get_attr, write_simple_attrs, copy_attributes
+from sidpy.hdf.reg_ref import get_indices_for_region_ref, create_region_reference
+from sidpy.proc.comp_utils import get_available_memory
+# from pyUSID.viz import plot_utils
+from sidpy.viz import plot_utils
+from sklearn.utils import gen_batches
+from sklearn.utils.extmath import randomized_svd
 
-from pyUSID.processing.process import Process
 from .proc_utils import get_component_slice
-from pyUSID.io.hdf_utils import find_results_groups,  \
-    reshape_to_n_dims, write_main_dataset, create_results_group, \
-    create_indexed_group, find_dataset
-from pyUSID import Dimension
-from pyUSID.io.anc_build_utils import calc_chunks
-from pyUSID import USIDataset
 
-import h5py
-from matplotlib import pyplot as plt
-#from pyUSID.viz import plot_utils
-from sidpy.viz import plot_utils
 
 class SVD(Process):
     """
     This class provides a file-wrapper around the :meth:`sklearn.utils.extmath.randomized_svd` function.
     In other words, it extracts and then reformats the data present in the provided :class:`pyUSID.USIDataset` object,
     performs the randomized SVD operation and writes the results back to the USID HDF5 file after
     formatting the results in an USID compliant manner.
@@ -196,15 +197,14 @@
         """
         comp_dim = Dimension('Principal Component', 'a. u.', len(self.__s))
 
         h5_svd_group = create_results_group(self.h5_main, self.process_name,
                                             h5_parent_group=self._h5_target_group)
         self.h5_results_grp = h5_svd_group
         self._write_source_dset_provenance()
-        
 
         write_simple_attrs(h5_svd_group, self.parms_dict)
         write_simple_attrs(h5_svd_group, {'svd_method': 'sklearn-randomized'})
 
         h5_u = write_main_dataset(h5_svd_group, np.float32(self.__u), 'U', 'Abundance', 'a.u.', None, comp_dim,
                                   h5_pos_inds=self.h5_main.h5_pos_inds, h5_pos_vals=self.h5_main.h5_pos_vals,
                                   dtype=np.float32, chunks=calc_chunks(self.__u.shape, np.float32(0).itemsize))
@@ -277,14 +277,15 @@
 
         if cant_svd:
             max_comps = np.floor(free_mem / mem_per_comp, dtype=int)
             error_message = 'Not enough free memory for performing SVD with requested number of parameters.\n' + \
                             'Maximum possible parameters is {}.'.format(max_comps)
             raise MemoryError(error_message)
 
+
 ###############################################################################
 
 
 def simplified_kpca(kpca, source_data):
     """
     Performs kernel PCA on the provided dataset and returns the familiar
     eigenvector, eigenvalue, and scree matrices.
@@ -341,18 +342,18 @@
     
     :raise: KeyError if SVD results not found 
 
     :returns: rebu dataset
     :rtype: HDF5 Dataset
 
     """
-    
+
     if not isinstance(h5_main, USIDataset):
         h5_main = USIDataset(h5_main)
-    
+
     comp_slice, num_comps = get_component_slice(components, total_components=h5_main.shape[1])
     if isinstance(comp_slice, np.ndarray):
         comp_slice = list(comp_slice)
     dset_name = h5_main.name.split('/')[-1]
 
     # Ensuring that at least one core is available for use / 2 cores are available for other use
     max_cores = max(1, cpu_count() - 2)
@@ -392,19 +393,19 @@
 
     if cores is None:
         free_mem = max_memory - fixed_mem
     else:
         free_mem = max_memory * 2 - fixed_mem
 
     batch_size = int(round(float(free_mem) / mem_per_pix))
-    
+
     if batch_size < 0:
         print('Batches listed were negative', batch_size)
         batch_size = 100
-        
+
     batch_slices = gen_batches(h5_U.shape[0], batch_size)
 
     print('Reconstructing in batches of {} positions.'.format(batch_size))
     print('Batches should be {} Mb each.'.format(mem_per_pix * batch_size / 1024.0 ** 2))
 
     '''
     Loop over all batches.
@@ -437,15 +438,16 @@
 
     h5_main.file.flush()
 
     print('Done writing reconstructed data to file.')
 
     return h5_rebuilt
 
-def plot_svd(h5_main, savefig=False, num_plots = 16, **kwargs):
+
+def plot_svd(h5_main, savefig=False, num_plots=16, **kwargs):
     '''
     Replots the SVD showing the skree, abundance maps, and eigenvectors.
     If h5_main is a Dataset, it will default to the most recent SVD group from that
     Dataset.
     If h5_main is the results group, then it will plot the values for that group.
     
     :param h5_main:
@@ -457,69 +459,68 @@
     :param num_plots: Default number of eigenvectors and abundance plots to show
     :type num_plots: int
         
     :param kwargs: keyword arguments for svd filtering
     :type kwarrgs: dict, optional
         
     '''
-    
+
     if isinstance(h5_main, h5py.Group):
 
         _U = find_dataset(h5_main, 'U')[-1]
         _V = find_dataset(h5_main, 'V')[-1]
         units = 'arbitrary (a.u.)'
         h5_spec_vals = np.arange(_V.shape[1])
         h5_svd_group = _U.parent
 
     else:
 
         h5_svd_group = find_results_groups(h5_main, 'SVD')[-1]
         units = h5_main.attrs['quantity']
         h5_spec_vals = h5_main.get_spec_values('Time')
-    
+
     h5_U = h5_svd_group['U']
     h5_V = h5_svd_group['V']
     h5_S = h5_svd_group['S']
-    
+
     _U = USIDataset(h5_U)
     [num_rows, num_cols] = _U.pos_dim_sizes
-    
-    abun_maps = np.reshape(h5_U[:,:16], (num_rows, num_cols,-1))
+
+    abun_maps = np.reshape(h5_U[:, :16], (num_rows, num_cols, -1))
     eigen_vecs = h5_V[:16, :]
-    
+
     skree_sum = np.zeros(h5_S.shape)
     for i in range(h5_S.shape[0]):
-        skree_sum[i] = np.sum(h5_S[:i])/np.sum(h5_S)
+        skree_sum[i] = np.sum(h5_S[:i]) / np.sum(h5_S)
 
     plt.figure()
     plt.plot(skree_sum, 'bo')
     plt.title('Cumulative Variance')
     plt.xlabel('Total Components')
     plt.ylabel('Total variance ratio (a.u.)')
-    
+
     if savefig:
         plt.savefig('Cumulative_variance_plot.png')
-    
+
     fig_skree, axes = plot_utils.plot_scree(h5_S, title='Scree plot')
     fig_skree.tight_layout()
 
     if savefig:
         plt.savefig('Scree_plot.png')
-    
+
     fig_abun, axes = plot_utils.plot_map_stack(abun_maps, num_comps=num_plots, title='SVD Abundance Maps',
-                                                  color_bar_mode='single', cmap='inferno', reverse_dims=True, 
-                                                  fig_mult=(3.5,3.5), facecolor='white', **kwargs)
+                                               color_bar_mode='single', cmap='inferno', reverse_dims=True,
+                                               fig_mult=(3.5, 3.5), facecolor='white', **kwargs)
     fig_abun.tight_layout()
     if savefig:
         plt.savefig('Abundance_maps.png')
-    
 
-    fig_eigvec, axes = plot_utils.plot_curves(h5_spec_vals*1e3, eigen_vecs, use_rainbow_plots=False, 
-                                                 x_label='Time (ms)', y_label=units, 
-                                                 num_plots=num_plots, subtitle_prefix='Component', 
-                                                 title='SVD Eigenvectors', evenly_spaced=False, 
-                                                 **kwargs)
+    fig_eigvec, axes = plot_utils.plot_curves(h5_spec_vals * 1e3, eigen_vecs, use_rainbow_plots=False,
+                                              x_label='Time (ms)', y_label=units,
+                                              num_plots=num_plots, subtitle_prefix='Component',
+                                              title='SVD Eigenvectors', evenly_spaced=False,
+                                              **kwargs)
     fig_eigvec.tight_layout()
     if savefig:
         plt.savefig('Eigenvectors.png')
-    
-    return 
+
+    return
```

### Comparing `FFTA-0.3.5.0/ffta/analysis/test_pixel.py` & `FFTA-0.3.5.1/ffta/analysis/test_pixel.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,72 +1,72 @@
 # -*- coding: utf-8 -*-
 """
 Created on Thu Mar  8 13:17:12 2018
 
 @author: Raj
 """
 
-from ffta.hdf_utils import hdf_utils
 from matplotlib import pyplot as plt
 
-def test_pixel(h5_file, param_changes={}, pxls = 1, showplots = True, 
-			   verbose=True, clear_filter = False):
-	"""
-	Takes a random pixel and does standard processing.
-	
-	:param h5_file: H5 file to process
-	:type h5_file: h5Py File, path, Dataset
-		
-	:param param_changes:
-	:type param_changes: dict, optional
-	
-	:param pxls: Number of random pixels to survey
-	:type pxls: int, optional
-		
-	:param showplots: Whether to create a new plot or not. 
-	:type showplots: bool, optional
-	
-	:param verbose: To print to command line. Currently for future-proofing
-	:type verbose : bool , optional
-	
-	:param clear_filter: Whether to do filtering (FIR) or not
-	:type clear_filter: bool, optional
-		
-	
-	"""
-	# get_pixel can work on Datasets or the H5_File
-	if any(param_changes):
-		hdf_utils.change_params(h5_file, new_vals=param_changes)
-		
-	parameters = hdf_utils.get_params(h5_file)
-	cols = parameters['num_cols']
-	rows = parameters['num_rows']
-	
-	# Creates random pixels to sample
-	pixels = []
-	if pxls == 1:
-	
-		pixels.append([0,0])
-	
-	if pxls > 1:
-		
-		from numpy.random import randint
-		for i in range(pxls):
-		
-			pixels.append([randint(0,rows), randint(0,cols)])
-
-	# Analyzes all pixels
-	for rc in pixels:
-		
-		h5_px = hdf_utils.get_pixel(h5_file, rc=rc)
-		
-		if clear_filter:
-			h5_px.clear_filter_flags()
-		
-		h5_px.analyze()
-		print(rc, h5_px.tfp)
-	
-		if showplots == True:
-			plt.plot(h5_px.best_fit, 'r--')
-			plt.plot(h5_px.cut, 'g-')
-		
-	return 
+from ffta.hdf_utils import hdf_utils
+
+
+def test_pixel(h5_file, param_changes={}, pxls=1, showplots=True,
+               verbose=True, clear_filter=False):
+    """
+    Takes a random pixel and does standard processing.
+
+    :param h5_file: H5 file to process
+    :type h5_file: h5Py File, path, Dataset
+
+    :param param_changes:
+    :type param_changes: dict, optional
+
+    :param pxls: Number of random pixels to survey
+    :type pxls: int, optional
+
+    :param showplots: Whether to create a new plot or not.
+    :type showplots: bool, optional
+
+    :param verbose: To print to command line. Currently for future-proofing
+    :type verbose : bool , optional
+
+    :param clear_filter: Whether to do filtering (FIR) or not
+    :type clear_filter: bool, optional
+
+
+    """
+    # get_pixel can work on Datasets or the H5_File
+    if any(param_changes):
+        hdf_utils.change_params(h5_file, new_vals=param_changes)
+
+    parameters = hdf_utils.get_params(h5_file)
+    cols = parameters['num_cols']
+    rows = parameters['num_rows']
+
+    # Creates random pixels to sample
+    pixels = []
+    if pxls == 1:
+        pixels.append([0, 0])
+
+    if pxls > 1:
+
+        from numpy.random import randint
+        for i in range(pxls):
+            pixels.append([randint(0, rows), randint(0, cols)])
+
+    # Analyzes all pixels
+    for rc in pixels:
+
+        h5_px = hdf_utils.get_pixel(h5_file, rc=rc)
+
+        if clear_filter:
+            h5_px.clear_filter_flags()
+
+        h5_px.analyze()
+        print(rc, h5_px.tfp)
+
+        if showplots == True:
+            plt.plot(h5_px.best_fit, 'r--')
+            plt.plot(h5_px.cut, 'g-')
+
+    return
```

### Comparing `FFTA-0.3.5.0/ffta/analyze_pixel.py` & `FFTA-0.3.5.1/ffta/analyze_pixel.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # -*- coding: utf-8 -*-
 """
 Created on Wed Jan 22 12:35:38 2020
 
 @author: Raj
 """
 
-#Script that loads, analyzes, and plots fast free point scan with fit
+import matplotlib.pyplot as plt
+
+# Script that loads, analyzes, and plots fast free point scan with fit
 from ffta.pixel import Pixel
-from ffta.pixel_utils.load import signal
 from ffta.pixel_utils.load import configuration
-import matplotlib.pyplot as plt
+from ffta.pixel_utils.load import signal
 
 
 def analyze_pixel(ibw_file, param_file):
     '''
     Analyzes a single pixel
     
     :param path to \*.ibw file
@@ -25,16 +26,16 @@
     :returns: The pixel object read and analyzed
     :rtype: Pixel
         
     '''
     signal_array = signal(ibw_file)
     n_pixels, params = configuration(param_file)
     pixel = Pixel(signal_array, params=params)
-    
+
     pixel.analyze()
-    pixel.plot() 
+    pixel.plot()
     plt.xlabel('Time Step')
     plt.ylabel('Freq Shift (Hz)')
-    
+
     print('tFP is', pixel.tfp, 's')
-    
-    return pixel.tfp
+
+    return pixel.tfp
```

### Comparing `FFTA-0.3.5.0/ffta/gkpfm/gkline.py` & `FFTA-0.3.5.1/ffta/gkpfm/gkline.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,15 @@
+import time
+
 import numpy as np
-from scipy import optimize as spo
+import pyUSID as usid
+from pyUSID import Dimension
 from scipy import signal as sps
 
-import warnings
-
 import ffta
-import time
-import pyUSID as usid
-from pyUSID import Dimension
 
 
 def cpd_total(ds, params, verbose=False, ncycles=4, smooth=3):
     '''
 
     :param ds:
     :type ds:
```

### Comparing `FFTA-0.3.5.0/ffta/gkpfm/gkpixel.py` & `FFTA-0.3.5.1/ffta/gkpfm/gkpixel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # -*- coding: utf-8 -*-
 """
 Created on Tue Sep  3 11:55:14 2019
 
 @author: Raj
 """
 
-import numpy as np
+import warnings
 from math import pi
+
+import numpy as np
 import numpy.polynomial.polynomial as npPoly
+import pyUSID as usid
+from BGlib.be.analysis.utils.be_sho import SHOfunc, SHOfit
+from igor2.binarywave import load as loadibw
+from matplotlib import pyplot as plt
 from scipy.optimize import fmin_tnc
 from scipy.signal import fftconvolve, chirp
 
-from matplotlib import pyplot as plt
-from ffta.simulation.cantilever import Cantilever
-from ffta.pixel_utils.load import cantilever_params
 from ffta.pixel import Pixel
-import warnings
-
+from ffta.pixel_utils.load import cantilever_params
+from ffta.simulation.cantilever import Cantilever
 from ..analysis.fft import get_noise_floor, NoiseBandFilter
 from ..analysis.gmode_utils import test_filter
-from BGlib.be.analysis.utils.be_sho import SHOfunc, SHOfit
-from igor.binarywave import load as loadibw
-import pyUSID as usid
 
 
 class GKPixel(Pixel):
 
     def __init__(self, signal_array,
                  params,
                  can_params={},
@@ -554,21 +554,21 @@
         :type plot: bool, optional
         
         :param noise_tolerance: Use to determine noise_floor, The default is 1e-6
         :type noise_tolerance: float, optional
         
         """
         nbf = NoiseBandFilter(len(self.force), self.sampling_rate,
-                                                [2E3, 50E3, 100E3, 150E3, 200E3],
-                                                [4E3, bw, bw, bw, bw])
+                              [2E3, 50E3, 100E3, 150E3, 200E3],
+                              [4E3, bw, bw, bw, bw])
 
         filt_line, _, _ = test_filter(self.force,
                                       frequency_filters=nbf,
-                                       noise_threshold=noise_tolerance,
-                                       show_plots=plot)
+                                      noise_threshold=noise_tolerance,
+                                      show_plots=plot)
         self.force = np.real(filt_line)
         self.FORCE = np.fft.fftshift(np.fft.fft(self.force))
 
         return
 
     def plot_response(self):
         """
```

### Comparing `FFTA-0.3.5.0/ffta/gkpfm/gkprocess.py` & `FFTA-0.3.5.1/ffta/gkpfm/gkprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 # -*- coding: utf-8 -*-
 """
 Created on Tue Feb 11 18:07:06 2020
 
 @author: Raj
 """
 
-import pyUSID as usid
-import ffta
-from ffta.gkpfm.gkpixel import GKPixel
-from ffta.pixel_utils import badpixels
 import os
+import warnings
+
+import h5py
 import numpy as np
-from ffta.load import get_utils
-from sidpy.proc.comp_utils import parallel_compute
+import pyUSID as usid
+from matplotlib import pyplot as plt
+from numpy.linalg import LinAlgError
 from pyUSID import Dimension
-import h5py
-
 from scipy.ndimage import gaussian_filter1d
+from sidpy.proc.comp_utils import parallel_compute
 
+import ffta
+from ffta.gkpfm.gkpixel import GKPixel
 from ffta.hdf_utils.process import FFtrEFM
-
-from matplotlib import pyplot as plt
-from numpy.linalg import LinAlgError
-import warnings
+from ffta.load import get_utils
+from ffta.pixel_utils import badpixels
 
 '''
 To do:
     Separate the instantaneous frequency and tFP/shift calculations
 '''
```

### Comparing `FFTA-0.3.5.0/ffta/gkpfm/load_excitation.py` & `FFTA-0.3.5.1/ffta/gkpfm/load_excitation.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,74 +4,73 @@
 
 __author__ = "Rajiv Giridharagopal"
 __copyright__ = "Copyright 2018, Ginger Lab"
 __maintainer__ = "Rajiv Giridharagopal"
 __email__ = "rgiri@uw.edu"
 __status__ = "Development"
 
-import numpy as np
 import os
-import h5py
 
+import h5py
+import numpy as np
 import pyUSID as usid
-
-from igor.binarywave import load as loadibw
+from igor2.binarywave import load as loadibw
 
 
 def load_exc(ibw_folder='', pixels=64, scale=1, offset=1, verbose=False):
-	"""
-	Loads excitation files into a single .h5 file
-	
-	:param ibw_folder: The folder containing the excitation files to load
-	:type ibw_folder: string, optional
-		
-	:param pixels: How many pixels per line to divide the excitation ibw
-	:type pixels: int, optional
-		
-	:param scale: The AC signal scaling, assuming the input excitation is wrong
-	:type scale: float, optional
-		
-	:param offset: The DC offset for the excitation
-	:type offset: float, optional
-	
-	:param verbose:
-	:type verbose: bool, optional
-	
-	:returns:
-	:rtype: str
-	"""
-	if not any(ibw_folder):
-		exc_file_path = usid.io_utils.file_dialog(caption='Select any file in destination folder',
-												  file_filter='IBW Files (*.ibw)')
-		exc_file_path = '/'.join(exc_file_path.split('/')[:-1])
-
-	filelist = os.listdir(exc_file_path)
-
-	data_files = [os.path.join(exc_file_path, name)
-				  for name in filelist if name[-3:] == 'ibw']
-
-	h5_path = os.path.join(exc_file_path, 'excitation') + '.h5'
-
-	h5_file = h5py.File(h5_path, 'w')
-
-	_line0 = loadibw(data_files[0])['wave']['wData']
-	_pix0 = np.split(_line0, pixels, axis=1)[0].mean(axis=1)
-	_pix0 = scale * ((_pix0 - np.min(_pix0)) / (np.max(_line0) - np.min(_line0)) - 0.5) + offset
-
-	data = h5_file.create_dataset('excitation',
-								  shape=(len(data_files), pixels, len(_pix0)),
-								  compression='gzip')
-
-	for n, d in enumerate(data_files):
-
-		if verbose:
-			print('### Loading', d.split('/')[-1], '###')
-
-		_line = loadibw(d)['wave']['wData']
-
-		for m, l in enumerate(np.split(_line, pixels, axis=1)):
-			_pix = np.mean(l, axis=1)
-			data[n, m, :] = _pix
+    """
+    Loads excitation files into a single .h5 file
+
+    :param ibw_folder: The folder containing the excitation files to load
+    :type ibw_folder: string, optional
+
+    :param pixels: How many pixels per line to divide the excitation ibw
+    :type pixels: int, optional
+
+    :param scale: The AC signal scaling, assuming the input excitation is wrong
+    :type scale: float, optional
+
+    :param offset: The DC offset for the excitation
+    :type offset: float, optional
+
+    :param verbose:
+    :type verbose: bool, optional
+
+    :returns:
+    :rtype: str
+    """
+    if not any(ibw_folder):
+        exc_file_path = usid.io_utils.file_dialog(caption='Select any file in destination folder',
+                                                  file_filter='IBW Files (*.ibw)')
+        exc_file_path = '/'.join(exc_file_path.split('/')[:-1])
+
+    filelist = os.listdir(exc_file_path)
+
+    data_files = [os.path.join(exc_file_path, name)
+                  for name in filelist if name[-3:] == 'ibw']
+
+    h5_path = os.path.join(exc_file_path, 'excitation') + '.h5'
+
+    h5_file = h5py.File(h5_path, 'w')
+
+    _line0 = loadibw(data_files[0])['wave']['wData']
+    _pix0 = np.split(_line0, pixels, axis=1)[0].mean(axis=1)
+    _pix0 = scale * ((_pix0 - np.min(_pix0)) / (np.max(_line0) - np.min(_line0)) - 0.5) + offset
+
+    data = h5_file.create_dataset('excitation',
+                                  shape=(len(data_files), pixels, len(_pix0)),
+                                  compression='gzip')
+
+    for n, d in enumerate(data_files):
+
+        if verbose:
+            print('### Loading', d.split('/')[-1], '###')
+
+        _line = loadibw(d)['wave']['wData']
+
+        for m, l in enumerate(np.split(_line, pixels, axis=1)):
+            _pix = np.mean(l, axis=1)
+            data[n, m, :] = _pix
 
-	# self.h5_tfp = self.h5_results_grp.create_dataset('tfp', data=_arr, dtype=np.float32)
+    # self.h5_tfp = self.h5_results_grp.create_dataset('tfp', data=_arr, dtype=np.float32)
 
-	return h5_path
+    return h5_path
```

### Comparing `FFTA-0.3.5.0/ffta/hdf_utils/hdf_utils.py` & `FFTA-0.3.5.1/ffta/hdf_utils/hdf_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,15 @@
 # -*- coding: utf-8 -*-
 """
 Created on Thu Feb 22 14:28:28 2018
 
 @author: Raj
 """
-import pyUSID as usid
-
-import warnings
-import numpy as np
 import h5py
-
-from ffta.load import get_utils
-from sidpy import Dimension
+import pyUSID as usid
 
 """
 Common HDF interfacing functions
 
 _which_h5_group : Returns a group corresponding to main FFtrEFM file
 get_params : Returns the common parameters list from config file
 change_params : Changes specific parameters (replicates normal command line function)
```

### Comparing `FFTA-0.3.5.0/ffta/hdf_utils/plot_tfp.py` & `FFTA-0.3.5.1/ffta/hdf_utils/plot_tfp.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # -*- coding: utf-8 -*-
 """
 Created on Fri Mar 27 14:05:42 2020
 
 @author: Raj
 """
 
+import os
+
+import matplotlib.font_manager as fm
+import numpy as np
+import pyUSID as usid
 from matplotlib import pyplot as plt
+from mpl_toolkits.axes_grid1.anchored_artists import AnchoredSizeBar
+
 # from ffta.hdf_utils import get_utils
 from ffta.load import get_utils
 from ffta.pixel_utils import badpixels
-import pyUSID as usid
-import numpy as np
-import os
-from mpl_toolkits.axes_grid1.anchored_artists import AnchoredSizeBar
-import matplotlib.font_manager as fm
 
 
 def plot_tfps(h5_file, h5_path='/', append='', savefig=True, stdevs=2, scale=None):
     """
     Plots the relevant tfp, inst_freq, and shift values as separate image files
     
     :param h5_file:
@@ -88,65 +90,64 @@
     _, cbar_s = usid.viz.plot_utils.plot_map(ax[2], shift, x_vec=xs * 1e6, y_vec=ys * 1e6,
                                              aspect=asp, cmap='inferno', stdevs=stdevs)
 
     cbar_t.set_label('tfp (us)', rotation=270, labelpad=16)
     ax[0].set_title('tfp', fontsize=12)
 
     if scale:
-        sz = np.floor(xs*1e6 / scale)
-        ratio = int(tfp_fixed.shape[1]/sz)
+        sz = np.floor(xs * 1e6 / scale)
+        ratio = int(tfp_fixed.shape[1] / sz)
         if scale > 1:
             sz = str(scale) + ' $\mu m$'
         else:
-            sz = str(int(scale*1000)) + ' nm'
-        
+            sz = str(int(scale * 1000)) + ' nm'
+
         fontprops = fm.FontProperties(size=14, weight='bold')
-        bar1 = AnchoredSizeBar(ax[0].transData, ratio, sz, frameon=False, 
+        bar1 = AnchoredSizeBar(ax[0].transData, ratio, sz, frameon=False,
                                loc='lower right', size_vertical=2,
-                               pad=0.2, color='white', fontproperties=fontprops) 
-        
+                               pad=0.2, color='white', fontproperties=fontprops)
+
         ax[0].add_artist(bar1)
-    
+
     cbar_r.set_label('Rate (kHz)', rotation=270, labelpad=16)
     ax[1].set_title('1/tfp', fontsize=12)
 
     if scale:
-        bar1 = AnchoredSizeBar(ax[0].transData, ratio, sz, frameon=False, 
+        bar1 = AnchoredSizeBar(ax[0].transData, ratio, sz, frameon=False,
                                loc='lower right', size_vertical=2,
-                               pad=0.2, color='white', fontproperties=fontprops) 
-        ax[1].add_artist(bar1)        
+                               pad=0.2, color='white', fontproperties=fontprops)
+        ax[1].add_artist(bar1)
 
     cbar_s.set_label('shift (Hz)', rotation=270, labelpad=16)
     ax[2].set_title('shift', fontsize=12)
-    
+
     if scale:
-        bar1 = AnchoredSizeBar(ax[0].transData, ratio, sz, frameon=False, 
+        bar1 = AnchoredSizeBar(ax[0].transData, ratio, sz, frameon=False,
                                loc='lower right', size_vertical=2,
-                               pad=0.2, color='white', fontproperties=fontprops) 
-        ax[2].add_artist(bar1)        
+                               pad=0.2, color='white', fontproperties=fontprops)
+        ax[2].add_artist(bar1)
 
     fig.tight_layout()
 
     if savefig:
         path = h5_file.file.filename.replace('\\', '/')
         path = '/'.join(path.split('/')[:-1]) + '/'
         os.chdir(path)
         fig.savefig('tfp_shift_' + append + '_.tif', format='tiff')
 
     return fig, ax
 
 
-
 def get_scale(target_size, x_size):
     """
     
     :param target_size:
     :type target_size:
     
     :param x_size:
     :type x_size:
     
     :returns:
     :rtype:
     
     """
-    return
+    return
```

### Comparing `FFTA-0.3.5.0/ffta/hdf_utils/process.py` & `FFTA-0.3.5.1/ffta/hdf_utils/process.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,41 @@
 # -*- coding: utf-8 -*-
 """
 Created on Tue Feb 11 18:07:06 2020
 
 @author: Raj
 """
 
-from pyUSID.io.hdf_utils import write_main_dataset, find_dataset, create_results_group
-from pyUSID import Process
-import ffta
-from ffta.pixel import Pixel
-from ffta.pixel_utils import badpixels
-from ffta.simulation.utils.load import simulation_configuration as load_sim_config
-from ffta.simulation.utils.load import params_from_experiment as load_parm
-from ffta.simulation.impulse import impulse
-from skimage import restoration
 import os
+
+import h5py
 import numpy as np
-from ffta.load import get_utils
-from sidpy.proc.comp_utils import parallel_compute
+from matplotlib import pyplot as plt
+from pyUSID import Dimension
+from pyUSID import Process
+from pyUSID.io.hdf_utils import write_main_dataset, find_dataset, create_results_group
 from sidpy.hdf.hdf_utils import get_attributes, copy_attributes
+from sidpy.proc.comp_utils import parallel_compute
 from sidpy.viz import plot_utils
-from pyUSID import Dimension
-import h5py
+from skimage import restoration
 
-from matplotlib import pyplot as plt
+import ffta
+from ffta.load import get_utils
+from ffta.pixel import Pixel
+from ffta.pixel_utils import badpixels
+from ffta.simulation.impulse import impulse
+from ffta.simulation.utils.load import params_from_experiment as load_parm
 
 
 class FFtrEFM(Process):
     """
     This class processes the deflection data into instantaneous frequency and tFP
     Implements the pixel-by-pixel processing using ffta.pixel routines
     Abstracted using the Process class for parallel processing on image dataset
     
-    
-
     Example usage:
 
         >> from ffta.hdf_utils import process
         >> data = process.FFtrEFM(h5_main)
         >> data.test([1,2]) # tests on pixel 1,2 in row, column
         >> data.compute()
         >> data.reshape() # reshapes the tFP, shift data
@@ -720,16 +718,16 @@
         attr = get_attributes(ffprocess['Inst_Freq'])
         img_length = attr['FastScanSize']
         img_height = attr['SlowScanSize']
         
         num_cols = attr['num_cols']
         num_rows = attr['num_rows']
         
-        tfp = ffprocess['tfp']
-        shift = ffprocess['shift']
+        tfp = ffprocess['tfp'][()]
+        shift = ffprocess['shift'][()]
         
         if 'tfp_cal' in ffprocess:
             tfp_cal = ffprocess['tfp_cal'][()]
             tfp_cal_fixed, _ = badpixels.fix_array(tfp_cal, threshold=threshold)
         else:
             tfp_cal_fixed = tfp_cal = np.ones(tfp.shape)
```

### Comparing `FFTA-0.3.5.0/ffta/line.py` & `FFTA-0.3.5.1/ffta/line.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 __author__ = "Durmus U. Karatay"
 __copyright__ = "Copyright 2014, Ginger Lab"
 __maintainer__ = "Durmus U. Karatay"
 __email__ = "ukaratay@uw.edu"
 __status__ = "Development"
 
 import numpy as np
+
 from ffta import pixel
 
 
 class Line:
 
     def __init__(self, signal_array, params, n_pixels, pycroscopy=False):
         """
@@ -73,25 +74,25 @@
         
         :param pycroscopy: Pycroscopy requires different orientation, so this corrects for this effect.
         :type pycroscopy: bool, optional
 
         """
         # Pass inputs to the object.
         self.signal_array = signal_array
-        if pycroscopy: 
+        if pycroscopy:
             self.signal_array = signal_array.T
         self.n_pixels = int(n_pixels)
         self.params = params
 
         # Initialize tFP and shift arrays.
         self.tfp = np.empty(self.n_pixels)
         self.shift = np.empty(self.n_pixels)
         self.inst_freq = np.empty((self.signal_array.shape[0], self.n_pixels))
-        
-        self.avgs_per_pixel = int(self.signal_array.shape[1]/self.n_pixels)
+
+        self.avgs_per_pixel = int(self.signal_array.shape[1] / self.n_pixels)
         self.n_signals = self.signal_array.shape[0]
 
         return
 
     def analyze(self):
         """
         Analyzes the line with the given method.
@@ -105,42 +106,40 @@
         """
 
         # Split the signal array into pixels.
         pixel_signals = np.split(self.signal_array, self.n_pixels, axis=1)
 
         # Iterate over pixels and return tFP and shift arrays.
         for i, pixel_signal in enumerate(pixel_signals):
-
             p = pixel.Pixel(pixel_signal, self.params)
-            
+
             (self.tfp[i], self.shift[i], self.inst_freq[:, i]) = p.analyze()
 
         return (self.tfp, self.shift, self.inst_freq)
 
     def pixel_wise_avg(self):
         """
         Averages the line per pixel and saves the result as signal_avg_array
         This functionality is primarily used in Pycroscopy-loading functions
         
         :returns: signal_averaged time-domain signal at each pixel
         :rtype: (n_points, n_pixels) numpy array
           
         """
-        
+
         self.signal_avg_array = np.empty((self.signal_array.shape[0], self.n_pixels))
-                
+
         for i in range(self.n_pixels):
-        
-            avg = self.signal_array[:, i*self.avgs_per_pixel:(i+1)*self.avgs_per_pixel]
+            avg = self.signal_array[:, i * self.avgs_per_pixel:(i + 1) * self.avgs_per_pixel]
             self.signal_avg_array[:, i] = avg.mean(axis=1)
-        
+
         return self.signal_avg_array
-    
+
     def clear_filter_flags(self):
         """
         Removes flags from parameters for setting filters
         """
-        
-        #self.params['window'] = 0
+
+        # self.params['window'] = 0
         self.params['bandpass_filter'] = 0
-        
-        return
+
+        return
```

### Comparing `FFTA-0.3.5.0/ffta/load/get_utils.py` & `FFTA-0.3.5.1/ffta/load/get_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 # -*- coding: utf-8 -*-
 """
 Created on Fri Aug 24 13:40:54 2018
 
 @author: Raj
 """
+import h5py
+import numpy as np
 import pyUSID as usid
 import sidpy
-import h5py
 
 from ffta.line import Line
 from ffta.pixel import Pixel
 
-import numpy as np
-
 '''
 Functions for extracting certain segments from an HDF FFtrEFM file
 '''
 
 
 def get_params(h5_path, key='', verbose=False, del_indices=True):
     """
@@ -247,15 +246,15 @@
         d = h5_path[()]
         parameters = get_params(h5_path)
         r = parameters['num_rows']
         c = parameters['num_cols']
         pnts = parameters['pnts_per_pixel']
 
     if rc[1] > c or rc[0] > r:
-        err = 'row and columns must be less than ' + str(r) +  ' X ' + str(c)
+        err = 'row and columns must be less than ' + str(r) + ' X ' + str(c)
         raise ValueError(err)
 
     signal_pixel = d[rc[0] * c + rc[1]:rc[0] * c + rc[1] + pnts, :]
 
     if avg == True:
         signal_pixel = signal_pixel.mean(axis=0)
```

### Comparing `FFTA-0.3.5.0/ffta/load/gl_ibw.py` & `FFTA-0.3.5.1/ffta/load/gl_ibw.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,25 +2,24 @@
 """
 Created on Wed Feb 21 10:06:12 2018
 
 @author: Raj Giridharagopal
 """
 
 from __future__ import division, print_function, absolute_import, unicode_literals
-from os import path  # File Path formatting
-import numpy as np  # For array operations
 
-from igor import binarywave as bw
-
-from sidpy.sid import Translator # , generate_dummy_main_parms
+from os import path  # File Path formatting
 
+import h5py
+import numpy as np  # For array operations
+from igor2 import binarywave as bw
 from pyUSID.io import Dimension
 from pyUSID.io.hdf_utils import write_ind_val_dsets
 from pyUSID.io.hdf_utils import write_main_dataset, create_indexed_group
-import h5py
+from sidpy.sid import Translator  # , generate_dummy_main_parms
 
 
 class GLIBWTranslator(Translator):
     """
     Translates Ginger Lab Igor Binary Wave (.ibw) files containing images or force curves to .h5
     """
```

### Comparing `FFTA-0.3.5.0/ffta/load/load_commands.py` & `FFTA-0.3.5.1/ffta/load/load_commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 __copyright__ = "Copyright 2018, Ginger Lab"
 __maintainer__ = "Rajiv Giridharagopal"
 __email__ = "rgiri@uw.edu"
 __status__ = "Development"
 
 import h5py
 import pyUSID as usid
+
 from ffta.load import get_utils
 
 
 def hdf_commands(h5_path, ds='FF_Raw'):
     """
     Creates a bunch of typical workspace HDF5 variables for scripting use
```

### Comparing `FFTA-0.3.5.0/ffta/load/load_hdf.py` & `FFTA-0.3.5.1/ffta/load/load_hdf.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 
 __author__ = "Rajiv Giridharagopal"
 __copyright__ = "Copyright 2018, Ginger Lab"
 __maintainer__ = "Rajiv Giridharagopal"
 __email__ = "rgiri@uw.edu"
 __status__ = "Development"
 
-import numpy as np
 import os
-import h5py
 
+import h5py
+import numpy as np
 import pyUSID as usid
 import sidpy
-from sidpy.hdf.hdf_utils import get_attributes
 from pyUSID import Dimension
+from sidpy.hdf.hdf_utils import get_attributes
 
-from ffta.pixel_utils import load
-from ffta.load import gl_ibw
-from ffta.load import get_utils
 from ffta import line
+from ffta.load import get_utils
+from ffta.load import gl_ibw
+from ffta.pixel_utils import load
 
 """
 Common HDF Loading functions
 
 load_wrapper: Loads a specific ibw and FFtrEFM folder into a new H5 file
 load_folder : Takes a folder of IBW files and creates an H5 file
 load_FF : Creates FF_Raw which is the raw (r*c*averages, pnts_per_signal) Dataset
```

### Comparing `FFTA-0.3.5.0/ffta/nfmd/NFMD.py` & `FFTA-0.3.5.1/ffta/nfmd/NFMD.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 import torch
 
+import time
 
 class NFMD:
     def __init__(self, signal, num_freqs, window_size,
                  windows=None,
                  optimizer=torch.optim.SGD,
                  optimizer_opts={'lr': 1e-4},
                  max_iters=1000,
@@ -44,20 +45,23 @@
         :type device: string
             
 
         '''
         # Signal -- assumed 1D, needs to be type double
         self.x = signal.astype(np.double).flatten()
         self.n = signal.shape[0]
+        
         # Signal Decomposition options
         self.num_freqs = num_freqs
         self.window_size = window_size
         self.windows = windows
+        
         if not windows:
             self.windows = self.n
+            
         # Stochastic Gradient Descent Options
         self.optimizer = optimizer
         self.optimizer_opts = optimizer_opts
         # If the learning rate is specified, scale it by
         # window size
         if 'lr' in optimizer_opts:
             self.optimizer_opts['lr'] /= window_size
@@ -78,14 +82,16 @@
             numpy.ndarray freqs is frequency vector
             numpy.ndarray A is coefficient vector
             numpy.ndarray losses is fit loss (MSE) for each window
             List indices is list of slice objects. each slice describes fit window indices`
 
         '''
         # Compute window indices
+
+        t1 = time.time()
         self.compute_window_indices()
 
         # Determine if printing updates
         verbose = update_freq != None
 
         # lists for results
         self.freqs = []
@@ -108,16 +114,15 @@
             # Access data slice
             x_i = self.x[idx_slice].copy()
 
             # Determine number of SGD iterations to allow
             max_iters = self.max_iters
 
             if i == 0:
-                
-                max_iters = 10000
+                self.max_iters = 10000
 
             # Fit data in window to model
             loss, freqs, A = self.fit_window(x_i,
                                              freqs=prev_freqs,
                                              A=prev_A)
 
             # Store the results
@@ -125,44 +130,59 @@
             self.A.append(A)
             self.losses.append(loss)
 
             # Set the previous freqs and A variables
             prev_freqs = freqs
             prev_A = A
 
-        self.freqs = np.asarray(self.freqs)
-        self.A = np.asarray(self.A)
-        self.losses = np.asarray(self.losses)
+        #print (time.time() - t1, 's for decompose_signal')
+        t2 = time.time()
+        self.freqs = np.array(self.freqs)
+        self.A = np.array(self.A)
+        if self.device == 'cpu':
+            self.losses = [loss.detach().numpy() for loss in self.losses]
+        else:
+            self.losses = [loss.detach().cpu().numpy() for loss in self.losses]
+
+        #print (time.time() - t2, 's for detach')
 
         return self.freqs, self.A, self.losses, self.indices
 
     def compute_window_indices(self):
         '''
         Sets the 'indices' attribute with computed index slices corresponding
         to the windows used in the analysis.
         Note: this is equivalent to computing rectangular windows.
-
         '''
+
+
+        t2 = time.time()
         # Define how many points between centerpoint of windows
         increment = int(self.n / self.windows)
         window_size = self.window_size
+        
         # Initialize the indices lists
         self.indices = []
         self.mid_idcs = []
+        
         # Populate the indices lists
         for i in range(self.windows):
+        
             # Compute window slice indices
             idx_start = int(max(0, i * increment - window_size / 2))
             idx_end = int(min(self.n, i * increment + window_size / 2))
+            
             if idx_end - idx_start == window_size:
                 # Add the index slice to the indices list
                 self.indices.append(slice(idx_start, idx_end))
                 idx_mid = int((idx_end + idx_start) / 2)
                 self.mid_idcs.append(idx_mid)
 
+        #print(time.time() - t2, 's for compute_window_indices')
+
     def fit_window(self, xt, freqs=None, A=None):
         '''
         Fits a set of instantaneous frequency and component coefficient vectors
         to the provided data.
 
         :param xt: Temporal data of dimensions [T, ...]
         :typer xt: numpy.ndarray
@@ -178,19 +198,22 @@
             WHERE
             float loss is the loss for the fit window (mean squared error)
             numpy.ndarray freqs is frequency vector of instantaneous frequencies
             numpy.ndarray A is coefficient vector of component (sine/cosine) coefficients
 
         '''
         # If no frequency is provided, generate initial frequency guess:
+
         if freqs is None:
             freqs, A = self.fft(xt)
 
+        t2 = time.time()
         # Then begin SGD
         loss, freqs, A = self.sgd(xt, freqs, A, max_iters=self.max_iters)
+        print(time.time() - t2, 's for sgd')
 
         return loss, freqs, A
 
     def fft(self, xt):
         '''
         Given temporal data xt, fft performs the initial guess of the
         frequencies contained in the data using the FFT.
@@ -321,15 +344,16 @@
         # Prepare the results
         A = A.cpu().detach().numpy()
         freqs = freqs.cpu().detach().numpy()
 
         return loss, freqs, A
 
     def predict(self, T):
-        ''' Predicts the data from 1 to T.
+        '''
+        Predicts the data from 1 to T.
 
         :param T: Prediction horizon (number of timepoints T)
         :type T: int
             
         :returns: xhat from 0 to T.
         :rtype: numpy.array
```

### Comparing `FFTA-0.3.5.0/ffta/nfmd/NFMDPixel.py` & `FFTA-0.3.5.1/ffta/nfmd/NFMDPixel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-import torch
+
 from .NFMD import NFMD
 
 
 class NFMDMode:
 
     def __init__(self, IF, IA, A, t):
         '''
@@ -31,15 +31,15 @@
 
 
 class NFMDPixel:
 
     def __init__(self, signal,
                  nfmd_options={'num_freqs': 3,
                                'window_size': 320}):
-                               
+
         '''
         Initialize an NFMDPixel object for decomposing a signal into Fourier modes.
     
         :param signal: Temporal signal to be analyzed.
         :type signal: numpy.ndarray
     
         :param nmfd_options: options passed to the NFMD analysis class
```

### Comparing `FFTA-0.3.5.0/ffta/nfmd/models.py` & `FFTA-0.3.5.1/ffta/nfmd/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Model Examples
 import warnings
-from scipy import optimize
+
 import numpy as np
+from scipy import optimize
 
 warnings.filterwarnings('ignore')
 
 # Setting parameters for models with known constants
 tp = 0.001638
 decay_lambda = 1080.80
```

### Comparing `FFTA-0.3.5.0/ffta/pixel.py` & `FFTA-0.3.5.1/ffta/pixel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 """pixel.py: Contains pixel class."""
 # pylint: disable=E1101,R0902,C0103
 __author__ = "Rajiv Giridharagopal"
-__copyright__ = "Copyright 2021"
+__copyright__ = "Copyright 2023"
 __maintainer__ = "Rajiv Giridharagopal"
 __email__ = "rgiri@uw.edu"
 __status__ = "Development"
 
+import time
+import warnings
+
 import numpy as np
-from scipy import signal as sps
+import pywt
+from matplotlib import pyplot as plt
 from scipy import integrate as spg
+from scipy import signal as sps
 
+from ffta.nfmd import NFMD
+from ffta.pixel_utils import dwavelet
 from ffta.pixel_utils import noise
 from ffta.pixel_utils import parab
-from ffta.pixel_utils import dwavelet
 from ffta.pixel_utils import tfp_calc
-from ffta.nfmd import NFMD
-
-from matplotlib import pyplot as plt
-import pywt
-
-import time
-import warnings
 
 
 class Pixel:
 
-
     def __init__(self,
                  signal_array,
                  params={},
                  can_params={},
                  fit=True,
                  pycroscopy=False,
                  method='hilbert',
@@ -46,15 +44,16 @@
 
         Extracts Time-to-First-Peak (tFP) from digitized Fast-Free Time-Resolved
         Electrostatic Force Microscopy (FF-trEFM) signals [1-2]. It includes a few
         types of frequency analysis:
 
         a) Hilbert Transform
         b) Wavelet Transform
-        c) Short-Time Fourier Transform (STFT))
+        c) Short-Time Fourier Transform (STFT)
+        d) Non-stationary Fourier mode decomposition (NFMD)
             
         Attributes
         ----------
         n_points : int
             Number of points in a signal.
         n_signals : int
             Number of signals to be averaged in a pixel.
@@ -190,28 +189,29 @@
 
         # Wavelet parameters
         self.wavelet_analysis = False
         self.wavelet = 'cmor1-1'  # default complex Morlet wavelet
         self.scales = np.arange(100, 2, -1)
         self.wavelet_params = {}  # currently just optimize flag is supported
 
-        # Short Time Fourier Transform
+        # Short Time Fourier Transform parameters
         self.fft_analysis = False
         self.fft_cycles = 2
         self.fft_params = {}  # for STFT
         self.fft_time_res = 20e-6
 
-        # NFMD 
+        # NFMD parameters
         self.nfmd_analysis = False
         self.num_freqs = 2
         self.window_size = 40
         self.optimizer_opts = {'lr': 1e-4}
         self.max_iters = 100
         self.target_loss = 1e-4
         self.update_freq = None
+        self.device = 'cpu'
 
         # Misc Settings
         self.phase_fitting = False
         self.check_drive = True
         self.window = 'blackman'
         self.bandpass_filter = 1
 
@@ -399,19 +399,20 @@
 
         return
 
     def average(self):
         """
         Averages signals.
         """
-
         if self.n_signals != 1:  # if not multi-signal, don't average
 
-            # self.signal = self.signal_array.mean(axis=1)
-            self.signal = self.signal.mean(axis=1)
+            try:
+                self.signal = self.signal.mean(axis=1)
+            except:
+                self.signal = self.signal_array.mean(axis=1)
 
         return
 
     def set_drive(self):
         """
         Calculates drive frequency of averaged signals
         """
@@ -899,15 +900,16 @@
                 print('window size automatically adjusted to ', self.window_size)
 
         nfmd = NFMD(z / np.std(z),
                     num_freqs=self.num_freqs,
                     window_size=self.window_size,
                     optimizer_opts=self.optimizer_opts,
                     max_iters=self.max_iters,
-                    target_loss=self.target_loss)
+                    target_loss=self.target_loss,
+                    device=self.device)
 
         if verbose:
             freqs, A, losses, indices = nfmd.decompose_signal(self.update_freq)
         else:
             freqs, A, losses, indices = nfmd.decompose_signal()
 
         dt = 1 / self.sampling_rate
@@ -1073,15 +1075,15 @@
         a[2].set_ylabel('Phase (deg)')
         a[2].set_xlabel('Time (ms)')
 
         plt.tight_layout()
 
         return
 
-    def generate_inst_freq(self, timing=False):
+    def generate_inst_freq(self, timing=False, dc=True):
         """
         Generates the instantaneous frequency
         
         :param timing: prints the time to execute (for debugging)
         :type timing: bool, optional
             
         :returns: tuple (inst_freq, amplitude, phase)
@@ -1091,15 +1093,15 @@
             [type] phase is...
         """
 
         if timing:
             t1 = time.time()
 
         # Remove DC component, first.
-        if self.method != 'nfmd':
+        if dc:
             self.remove_dc()
         else:
             self.signal = np.copy(self.signal_array)
 
         # Phase-lock signals.
         # self.phase_lock()
 
@@ -1152,15 +1154,15 @@
             self.hilbert()
 
             # Filter out oscillatory noise from amplitude
             if self.filter_amplitude:
                 self.amplitude_filter()
 
         else:
-            raise ValueError('Invalid analysis method! Valid options: hilbert, wavelet, fft')
+            raise ValueError('Invalid analysis method! Valid options: hilbert, wavelet, fft, nfmd')
 
         if timing:
             print('Time:', time.time() - t1, 's')
 
         # Filter out oscillatory noise from instantaneous frequency
         if self.filter_frequency:
             self.frequency_filter()
```

### Comparing `FFTA-0.3.5.0/ffta/pixel_utils/dwavelet.py` & `FFTA-0.3.5.1/ffta/pixel_utils/dwavelet.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """dwavelet.py: contains functions used in DWT calculations."""
 
-import pywt
 import numpy as np
+import pywt
 
 
 def dwt_denoise(signal, fLow, fHigh, sampling_rate):
     """
     Uses Discrete Wavelet Transform to denoise signal
     around a desired frequency band.
```

### Comparing `FFTA-0.3.5.0/ffta/pixel_utils/fitting.py` & `FFTA-0.3.5.1/ffta/pixel_utils/fitting.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,14 +147,15 @@
     popt = minimize(cost, pinit, method='TNC', options={'disp': False},
                     bounds=[(-10000, -1.0),
                             (5e-7, 0.1),
                             (1e-5, 0.1)])
 
     return popt.x
 
+
 def fit_product_unbound(Q, drive_freq, t, inst_freq):
     """
     Fit without any bound constraints
     
     :param Q:
     :type Q:
     
@@ -166,15 +167,15 @@
     
     :param inst_freq:
     :type inst_freq:
     
     :returns:
     :rtype:
     """
-    
+
     # Initial guess for relaxation constant.
     inv_beta = Q / (np.pi * drive_freq)
 
     # Cost function to minimize.
     cost = lambda p: np.sum((ddho_freq_product(t, *p) - inst_freq) ** 2)
 
     # bounded optimization using scipy.minimize
@@ -234,18 +235,18 @@
     :rtype:
     """
     # Cost function to minimize.
     cost = lambda p: np.sum((cut_exp(t, *p) - inst_freq) ** 2)
 
     pinit = [inst_freq.max() - inst_freq.min(), inst_freq.min(), 1e-4]
 
-#    popt = minimize(cost, pinit, method='TNC', options={'disp': False},
-#                    bounds=[(1e-5, 1000),
-#                            (np.abs(inst_freq.min()) * -2, np.abs(inst_freq.max()) * 2),
-#                             (1e-6, 0.1)])
+    #    popt = minimize(cost, pinit, method='TNC', options={'disp': False},
+    #                    bounds=[(1e-5, 1000),
+    #                            (np.abs(inst_freq.min()) * -2, np.abs(inst_freq.max()) * 2),
+    #                             (1e-6, 0.1)])
 
     popt = minimize(cost, pinit, method='TNC', options={'disp': False})
 
     return popt.x
 
 
 def fit_ringdown(t, cut):
```

### Comparing `FFTA-0.3.5.0/ffta/pixel_utils/load.py` & `FFTA-0.3.5.1/ffta/pixel_utils/load.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,20 @@
 __copyright__ = "Copyright 2018, Ginger Lab"
 __maintainer__ = "Rajiv Giridharagopal"
 __email__ = "rgiri@uw.edu"
 __status__ = "Development"
 
 import configparser
 import sys
-from igor.binarywave import load as loadibw
-from numpy.lib.npyio import loadtxt
 from os.path import splitext
+
 import numpy as np
 import pandas as pd
+from igor2.binarywave import load as loadibw
+from numpy.lib.npyio import loadtxt
 
 
 def signal(path, skiprows=0):
     """
     Loads .ibw or ASCII files and return it as a numpy.ndarray.
 
     :param path: Path to signal file.
```

### Comparing `FFTA-0.3.5.0/ffta/pixel_utils/noise.py` & `FFTA-0.3.5.1/ffta/pixel_utils/noise.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,84 +8,83 @@
 
 import numpy as np
 import scipy.linalg as spl
 import scipy.spatial.distance as spsd
 
 
 def phase_lock(signal_array, tidx, cidx):
-	"""
-	Aligns signals of a pixel on the rising edge of first zeros, if they are
-	not aligned due to phase jitter of analog-to-digital converter.
-
-	:param signal_array: 2D real-valued signal array.
-	:type signal_array: (n_points, n_signals), array_like
-	
-	:param tidx: Time to trigger from the start of signals as index.
-	:type tidx: int
-	
-	:param cidx: Period of the signal as number of points,
-		i.e. drive_freq/sampling_rate
-	:type cidx: int
-		
-	:returns: tuple (new_signal_array, tidx)
-		WHERE
-		array_like new_signal_array is phase-locked signal array in format (n_points, n_signals)
-		int tidx is index of trigger after phase-locking.
-
-	"""
-
-	# Initialize variables.
-	n_points, n_signals = signal_array.shape
-
-	above = signal_array[:cidx, :] > 0
-	below = np.logical_not(above)
-	left_shifted_above = above[1:, :]
-
-	idxs = (left_shifted_above[:, :] & below[0:-1, :]).argmax(axis=0)
-
-	# Have all signals same length by cutting them from both ends.
-	total_cut = int(idxs.max() + idxs.min() + 1)
-	new_signal_array = np.empty((n_points - total_cut, n_signals))
-	tidx -= int(idxs.mean())  # Shift trigger index by average amount.
+    """
+    Aligns signals of a pixel on the rising edge of first zeros, if they are
+    not aligned due to phase jitter of analog-to-digital converter.
 
-	# Cut signals.
-	for i, idx in enumerate(idxs):
+    :param signal_array: 2D real-valued signal array.
+    :type signal_array: (n_points, n_signals), array_like
 
-		new_signal_array[:, i] = signal_array[idx:-(total_cut - idx), i]
+    :param tidx: Time to trigger from the start of signals as index.
+    :type tidx: int
 
-	return new_signal_array, tidx
+    :param cidx: Period of the signal as number of points,
+        i.e. drive_freq/sampling_rate
+    :type cidx: int
+
+    :returns: tuple (new_signal_array, tidx)
+        WHERE
+        array_like new_signal_array is phase-locked signal array in format (n_points, n_signals)
+        int tidx is index of trigger after phase-locking.
+
+    """
+
+    # Initialize variables.
+    n_points, n_signals = signal_array.shape
+
+    above = signal_array[:cidx, :] > 0
+    below = np.logical_not(above)
+    left_shifted_above = above[1:, :]
+
+    idxs = (left_shifted_above[:, :] & below[0:-1, :]).argmax(axis=0)
+
+    # Have all signals same length by cutting them from both ends.
+    total_cut = int(idxs.max() + idxs.min() + 1)
+    new_signal_array = np.empty((n_points - total_cut, n_signals))
+    tidx -= int(idxs.mean())  # Shift trigger index by average amount.
+
+    # Cut signals.
+    for i, idx in enumerate(idxs):
+        new_signal_array[:, i] = signal_array[idx:-(total_cut - idx), i]
+
+    return new_signal_array, tidx
 
 
 def pca_discard(signal_array, k):
-	"""
-	Discards noisy signals using Principal Component Analysis and Mahalonobis
-	distance.
+    """
+    Discards noisy signals using Principal Component Analysis and Mahalonobis
+    distance.
+
+    :param signal_array: 2D real-valued signal array.
+    :type signal_array: (n_points, n_signals), array_like
 
-	:param signal_array: 2D real-valued signal array.
-	:type signal_array: (n_points, n_signals), array_like
+    :param k: Number of eigenvectors to use, can't be bigger than n_signals.
+    :type k: int
 
-	:param k: Number of eigenvectors to use, can't be bigger than n_signals.
-	:type k: int
-		
-	:returns: indices of noisy signals.
-	:rtype: array
+    :returns: indices of noisy signals.
+    :rtype: array
 
-	"""
+    """
 
-	# Get the size of signals.
-	n_points, n_signals = signal_array.shape
+    # Get the size of signals.
+    n_points, n_signals = signal_array.shape
 
-	# Remove the mean from all signals.
-	mean_signal = signal_array.mean(axis=1).reshape(n_points, 1)
-	signal_array = signal_array - mean_signal
+    # Remove the mean from all signals.
+    mean_signal = signal_array.mean(axis=1).reshape(n_points, 1)
+    signal_array = signal_array - mean_signal
 
-	# Calculate the biggest eigenvector of covariance matrix.
-	_, eigvec = spl.eigh(np.dot(signal_array.T, signal_array),
-						 eigvals=(n_signals - k, n_signals - 1))
+    # Calculate the biggest eigenvector of covariance matrix.
+    _, eigvec = spl.eigh(np.dot(signal_array.T, signal_array),
+                         eigvals=(n_signals - k, n_signals - 1))
 
-	eigsig = np.dot(signal_array, eigvec)  # Convert it to eigensignal.
+    eigsig = np.dot(signal_array, eigvec)  # Convert it to eigensignal.
 
-	weights = np.dot(eigsig.T, signal_array) / spl.norm(eigsig)
-	mean = weights.mean(axis=1).reshape(1, k)
-	idx = np.where(spsd.cdist(weights.T, mean, 'mahalanobis') > 2)
+    weights = np.dot(eigsig.T, signal_array) / spl.norm(eigsig)
+    mean = weights.mean(axis=1).reshape(1, k)
+    idx = np.where(spsd.cdist(weights.T, mean, 'mahalanobis') > 2)
 
-	return idx
+    return idx
```

### Comparing `FFTA-0.3.5.0/ffta/pixel_utils/parab.py` & `FFTA-0.3.5.1/ffta/pixel_utils/parab.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,154 +1,154 @@
 """parab.py: Parabola fit around three points to find a true vertex."""
 
 import numpy as np
 
 
 def fit_peak(f, x):
-	'''
-	Uses solution to parabola to fit peak and two surrounding points
-	This assumes there is a peak (i.e. parabola second deriv is negative)
-	
-	If interested, this is educational to see with sympy
-	 import sympy
-	 y1, y2, y3 = sympy.symbols('y1 y2 y3')
-	 A = sympy.Matrix([[(-1)**2, -1, 1],[0**2, 0, 1],[(1)**2,1,1]]) 
-	 C = sympy.Matrix([[y1],[y2],[y3]])
-	 D = A.inv().multiply(C)
-	 D contains the values of a, b, c in ax**2 + bx + c
-	 Peak position is at x = -D[1]/(2D[0])   
-	
-	:param f: array of f(x)
-	:type f: array 
-	
-	:param x: array of indices corresponding to f
-	:type x: array 
-	
-	:returns: tuple (findex, yindex, xindex)
-		WHERE
-		[type] findex is...
-		[type] yindex is...
-		[type] xindex is...
-	'''
-
-	pk = np.argmax(f)
-
-	y1 = f[pk - 1]
-	y2 = f[pk]
-	y3 = f[pk + 1]
-
-	a = 0.5 * y1 - y2 + 0.5 * y3
-	b = -0.5 * y1 + 0.5 * y3
-	c = y2
-
-	xindex = -b / (2 * a)
-	findex = xindex * (x[1] - x[0]) + x[1]
-	yindex = a * xindex ** 2 + b * xindex + c
+    '''
+    Uses solution to parabola to fit peak and two surrounding points
+    This assumes there is a peak (i.e. parabola second deriv is negative)
+
+    If interested, this is educational to see with sympy
+     import sympy
+     y1, y2, y3 = sympy.symbols('y1 y2 y3')
+     A = sympy.Matrix([[(-1)**2, -1, 1],[0**2, 0, 1],[(1)**2,1,1]])
+     C = sympy.Matrix([[y1],[y2],[y3]])
+     D = A.inv().multiply(C)
+     D contains the values of a, b, c in ax**2 + bx + c
+     Peak position is at x = -D[1]/(2D[0])
+
+    :param f: array of f(x)
+    :type f: array
+
+    :param x: array of indices corresponding to f
+    :type x: array
+
+    :returns: tuple (findex, yindex, xindex)
+        WHERE
+        [type] findex is...
+        [type] yindex is...
+        [type] xindex is...
+    '''
+
+    pk = np.argmax(f)
+
+    y1 = f[pk - 1]
+    y2 = f[pk]
+    y3 = f[pk + 1]
+
+    a = 0.5 * y1 - y2 + 0.5 * y3
+    b = -0.5 * y1 + 0.5 * y3
+    c = y2
+
+    xindex = -b / (2 * a)
+    findex = xindex * (x[1] - x[0]) + x[1]
+    yindex = a * xindex ** 2 + b * xindex + c
 
-	return findex, yindex, xindex
+    return findex, yindex, xindex
 
 
 def ridge_finder(spectrogram, freq_bin):
-	'''
-	Uses parabolda to fit peak and two surrounding points
-	This takes a spectrogram and the frequency bin spacing and wraps parab.fit_2d
-	
-	:param spectrogram: Returned by scipy.signal.spectrogram or stft or cwt
-		Arranged in (frequencies, times) shape
-	:type spectrogram: ndarray 
-		
-	:param freq_bin: arrays corresponding the frequencies in the spectrogram
-	:type freq_bin: ndarray
-		
-	:returns: tuple (xindex, yindex)
-		WHERE
-		ndarray xindex is 1D array of the frequency bins returned by parabolic approximation
-		ndarray yindex is 1D array of the peak values at the xindices supplied
-	'''
-	_argmax = np.argmax(np.abs(spectrogram), axis=0)
-	cols = spectrogram.shape[1]
-
-	# generate a (3, cols) matrix of the spectrogram values
-	maxspec = np.array([spectrogram[(_argmax - 1, range(cols))],
-						spectrogram[(_argmax, range(cols))],
-						spectrogram[(_argmax + 1, range(cols))]])
+    '''
+    Uses parabolda to fit peak and two surrounding points
+    This takes a spectrogram and the frequency bin spacing and wraps parab.fit_2d
+
+    :param spectrogram: Returned by scipy.signal.spectrogram or stft or cwt
+        Arranged in (frequencies, times) shape
+    :type spectrogram: ndarray
+
+    :param freq_bin: arrays corresponding the frequencies in the spectrogram
+    :type freq_bin: ndarray
+
+    :returns: tuple (xindex, yindex)
+        WHERE
+        ndarray xindex is 1D array of the frequency bins returned by parabolic approximation
+        ndarray yindex is 1D array of the peak values at the xindices supplied
+    '''
+    _argmax = np.argmax(np.abs(spectrogram), axis=0)
+    cols = spectrogram.shape[1]
+
+    # generate a (3, cols) matrix of the spectrogram values
+    maxspec = np.array([spectrogram[(_argmax - 1, range(cols))],
+                        spectrogram[(_argmax, range(cols))],
+                        spectrogram[(_argmax + 1, range(cols))]])
 
-	return fit_2d(maxspec, _argmax, freq_bin)
+    return fit_2d(maxspec, _argmax, freq_bin)
 
 
 def fit_2d(f, p, dx):
-	'''
-	Uses solution to parabola to fit peak and two surrounding points
-	This assumes there is a peak (i.e. parabola second deriv is negative).
-	
-	This is a broadcast version for speed purposes
-	
-	:param f: 2D array f(x) of size (3 , samples)
-	:type f: 2D array
-	
-	:param p: peak positions for f
-	:type p: 1D array
-
-	:param dx: frequency (x values) of f
-	:type dx: 1D array 
-
-	:returns: tuple (findex, yindex, xindex)
-		WHERE
-		[type] findex is...
-		[type] yindex is...
-		[type] xindex is...	
-	'''
-
-	if f.shape[0] != 3:
-		raise ValueError('Must be exactly 3 rows')
-
-	a = 0.5 * f[0, :] - f[1, :] + 0.5 * f[2, :]
-	b = -0.5 * f[0, :] + 0.5 * f[2, :]
-	c = f[1, :]
-
-	xindex = -b / (2 * a)
-	findex = xindex * (dx[1] - dx[0]) + dx[p]
-	yindex = a * (xindex ** 2) + b * xindex + c
+    '''
+    Uses solution to parabola to fit peak and two surrounding points
+    This assumes there is a peak (i.e. parabola second deriv is negative).
 
-	return findex, yindex, xindex
+    This is a broadcast version for speed purposes
+
+    :param f: 2D array f(x) of size (3 , samples)
+    :type f: 2D array
+
+    :param p: peak positions for f
+    :type p: 1D array
+
+    :param dx: frequency (x values) of f
+    :type dx: 1D array
+
+    :returns: tuple (findex, yindex, xindex)
+        WHERE
+        [type] findex is...
+        [type] yindex is...
+        [type] xindex is...
+    '''
+
+    if f.shape[0] != 3:
+        raise ValueError('Must be exactly 3 rows')
+
+    a = 0.5 * f[0, :] - f[1, :] + 0.5 * f[2, :]
+    b = -0.5 * f[0, :] + 0.5 * f[2, :]
+    c = f[1, :]
+
+    xindex = -b / (2 * a)
+    findex = xindex * (dx[1] - dx[0]) + dx[p]
+    yindex = a * (xindex ** 2) + b * xindex + c
+
+    return findex, yindex, xindex
 
 
 def fit_peak_old(f, x):
-	"""
-	Uses parabola equation to fit to the peak and two surrounding points
-	
-	:param f:
-	:type f: array
-	
-	:param x: index of peak, typically just argmax
-	:type x:
-
-	:returns: tuple (xindex, yindex)
-		WHERE
-		[type] xindex is...
-		[type] yindex is...
-	"""
-
-	x1 = x - 1
-	x2 = x
-	x3 = x + 1
-
-	y1 = f[x - 1]
-	y2 = f[x]
-	y3 = f[x + 1]
-
-	d = (x1 - x3) * (x1 - x2) * (x2 - x3)
-
-	A = (x1 * (y3 - y2) + x2 * (y1 - y3) + x3 * (y2 - y1)) / d
-
-	B = (x1 ** 2.0 * (y2 - y3) +
-		 x2 ** 2.0 * (y3 - y1) +
-		 x3 ** 2.0 * (y1 - y2)) / d
-
-	C = (x2 * x3 * (x2 - x3) * y1 +
-		 x3 * x1 * (x3 - x1) * y2 +
-		 x1 * x2 * (x1 - x2) * y3) / d
+    """
+    Uses parabola equation to fit to the peak and two surrounding points
+
+    :param f:
+    :type f: array
+
+    :param x: index of peak, typically just argmax
+    :type x:
+
+    :returns: tuple (xindex, yindex)
+        WHERE
+        [type] xindex is...
+        [type] yindex is...
+    """
+
+    x1 = x - 1
+    x2 = x
+    x3 = x + 1
+
+    y1 = f[x - 1]
+    y2 = f[x]
+    y3 = f[x + 1]
+
+    d = (x1 - x3) * (x1 - x2) * (x2 - x3)
+
+    A = (x1 * (y3 - y2) + x2 * (y1 - y3) + x3 * (y2 - y1)) / d
+
+    B = (x1 ** 2.0 * (y2 - y3) +
+         x2 ** 2.0 * (y3 - y1) +
+         x3 ** 2.0 * (y1 - y2)) / d
+
+    C = (x2 * x3 * (x2 - x3) * y1 +
+         x3 * x1 * (x3 - x1) * y2 +
+         x1 * x2 * (x1 - x2) * y3) / d
 
-	xindex = -B / (2.0 * A)
-	yindex = C - B ** 2.0 / (4.0 * A)
+    xindex = -B / (2.0 * A)
+    yindex = C - B ** 2.0 / (4.0 * A)
 
-	return xindex, yindex
+    return xindex, yindex
```

### Comparing `FFTA-0.3.5.0/ffta/pixel_utils/tfp_calc.py` & `FFTA-0.3.5.1/ffta/pixel_utils/tfp_calc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # -*- coding: utf-8 -*-
 
 """tfp.py: Routines for fitting the frequency/phase/amplitude to extract tFP/shift """
 
-from . import fitting
 import numpy as np
 from scipy import interpolate as spi
 from scipy import optimize as spo
 
+from . import fitting
+
 
 def find_minimum(pix, cut):
     """
     Finds when the minimum of instantaneous frequency happens using spline fitting
     
     :param pix: pixel object to analyze
     :type pix: ffta.pixel.Pixel object
@@ -85,17 +86,17 @@
     pix.best_fit : ndarray
         Best-fit line calculated from popt and fit function
 
     '''
 
     # Fit the cut to the model.
     try:
-        
+
         popt = fitting.fit_product(pix.Q, pix.drive_freq, t, cut)
-        
+
     except:
 
         popt = fitting.fit_product_unbound(pix.Q, pix.drive_freq, t, cut)
 
     A, tau1, tau2 = popt
 
     # Analytical minimum of the fit.
```

### Comparing `FFTA-0.3.5.0/ffta/simulation/broadband_drive.py` & `FFTA-0.3.5.1/ffta/simulation/broadband_drive.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 __author__ = "Rajiv Giridharagopal"
 __copyright__ = "Copyright 2020, Ginger Lab"
 __email__ = "rgiri@uw.edu"
 __status__ = "Production"
 
 from math import pi
+
 from scipy.signal import chirp
 
 from .cantilever import Cantilever
-from .utils import excitation
 
 # Set constant 2 * pi.
 PI2 = 2 * pi
 
 
 class BroadbandPulse(Cantilever):
```

### Comparing `FFTA-0.3.5.0/ffta/simulation/calibration_curve.py` & `FFTA-0.3.5.1/ffta/simulation/calibration_curve.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,24 +2,23 @@
 """
 Created on Thu Mar  4 10:27:55 2021
 
 @author: Raj
 """
 
 import numpy as np
+import pandas as pd
+from matplotlib import pyplot as plt
+from scipy.interpolate import InterpolatedUnivariateSpline as ius
+from scipy.signal import medfilt
 
+from ffta.pixel_utils.load import configuration
 from .mechanical_drive import MechanicalDrive
 from .utils.load import params_from_experiment as load_parm
 from .utils.load import simulation_configuration as load_sim_config
-from ffta.pixel_utils.load import configuration
-from scipy.interpolate import InterpolatedUnivariateSpline as ius
-from scipy.signal import medfilt
-
-from matplotlib import pyplot as plt
-import pandas as pd
 
 
 def cal_curve(can_path, param_cfg, taus_range=[-7, -3], plot=True, **kwargs):
     '''
     Generates a calibration curve for a given cantilever given some particular
     parameters.
 
@@ -67,24 +66,24 @@
         can_params['res_freq'] = parms['drive_freq']
         sim_params['trigger'] = parms['trigger']
         sim_params['total_time'] = parms['total_time']
         sim_params['sampling_rate'] = parms['sampling_rate']
 
     if len(taus_range) != 2 or (taus_range[1] <= taus_range[0]):
         raise ValueError('Range must be ascending and 2-items')
-    
+
     # Check if given as log or actual values
     if taus_range[0] < 0 or taus_range[1] < 0:
         _rlo = taus_range[0]
         _rhi = taus_range[1]
-    
+
     else:
         _rlo = np.log10(taus_range[0])
         _rhi = np.log10(taus_range[1])
-        
+
     taus = np.logspace(_rlo, _rhi, 50)
     tfps = []
 
     for t in taus:
         force_params['tau'] = t
         cant = MechanicalDrive(can_params, force_params, sim_params)
         Z, _ = cant.simulate()
@@ -154,14 +153,15 @@
     df.index.name = 'taus'
     df.to_csv('Calibration_Curve.csv')
 
     print('Do not forget that the spline is in log-space')
 
     return taus, tfps, spl
 
+
 def reconstruct_cal_curve(csv_file):
     '''
     Reconstruct the calibration curve from a saved CSV
     
     :param csv_file: path to CSV file
     :type csv_file: str
     
@@ -170,15 +170,15 @@
         ndarray taus is the single exponential taus that were simulated
         ndarray tfps is the measured time to first peaks
         UnivariateSpline spl is spline object of the calibration curve. To scale an image, type spl(x)
                
     '''
 
     df = pd.read_csv(csv_file)
-    
+
     taus = df['taus']
     tfps = df['tfps']
     spl = ius(tfps, taus, k=4)
-    
-    print ('Note that taus, tfps, and cal_curve are in log-space')
+
+    print('Note that taus, tfps, and cal_curve are in log-space')
 
     return taus, tfps, spl
```

### Comparing `FFTA-0.3.5.0/ffta/simulation/cantilever.py` & `FFTA-0.3.5.1/ffta/simulation/cantilever.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """simulate.py: Contains Cantilever class."""
 # pylint: disable=E1101,R0902,C0103
 __copyright__ = "Copyright 2020, Ginger Lab"
 __author__ = "Rajiv Giridharaogpal"
 __email__ = "rgiri@uw.edu"
 __status__ = "Production"
 
-import numpy as np
 from math import pi
+
+import numpy as np
 from scipy.integrate import odeint
 
 from ..pixel import Pixel
 
 # Set constant 2 * pi.
 PI2 = 2 * pi
 
@@ -21,15 +22,14 @@
 
     This class contains the functions needed to simulate. To create a class that
     simulates a subset, it needs to overload the following functions:
     force(self, t)
     omega(self, t)
     dZdt(self, t) if the given ODE form will not work
 
-
     Attributes
     ----------
     amp : float
         Amplitude of the cantilever in meters.
     beta : float
         Damping factor of the cantilever in rad/s.
     delta : float
@@ -65,14 +65,29 @@
     >>> params = load.simulation_configuration(params_file)
     >>>
     >>> c = cantilever.Cantilever(*params)
     >>> Z, infodict = c.simulate()
     >>> c.analyze()
     >>> c.analyze(roi=0.004) # can change the parameters as desired
 
+    To correctly construct this, Cantilever requires the following parameters
+    passed in the dictionaries can_params, force_params, and sim_params.
+    Note: the dictionaries are functionally the same, you could leave force_params
+    and sim_params blank and only create can_params.    
+
+    Minimum parameters needed:
+        amp = float (in m)
+        or:
+            amp_invols = float (in m/V)
+            soft_amp = float (in V)
+        drive_freq = float (in Hz)
+        res_freq = float (in Hz)
+        k = float (in N/m)
+        q_factor = float
+        total_time = float (in seconds)
 
     :param can_params: Parameters for cantilever properties. The dictionary contains:
         amp_invols = float (in m/V)
         def_invols = float (in m/V)
         soft_amp = float (in V)
         drive_freq = float (in Hz)
         res_freq = float (in Hz)
@@ -93,61 +108,75 @@
     :param sim_params: Parameters for simulation. The dictionary contains:
         trigger = float (in seconds)
         total_time = float (in seconds)
         sampling_rate = int (in Hz)
     :type sim_params: dict
     """
 
-    def __init__(self, can_params, force_params, sim_params):
+    def __init__(self, 
+                 can_params={}, 
+                 force_params={}, 
+                 sim_params={}):
 
         # Initialize cantilever parameters and calculate some others.
         for key, value in can_params.items():
             setattr(self, key, value)
+        
+        # Initialize force parameters and calculate some others.
+        for key, value in force_params.items():
+            setattr(self, key, value)
 
+        # Initialize simulation parameters.
+        for key, value in sim_params.items():
+            setattr(self, key, value)
+        
         self.w0 = PI2 * self.res_freq  # Radial resonance frequency.
         self.wd = PI2 * self.drive_freq  # Radial drive frequency.
-
+        
         if not np.allclose(self.w0, self.wd):
+            print(self.w0, self.wd)
             print('Resonance and Drive not equal. Make sure simulation is long enough!')
 
+        if not hasattr(self, 'tau'):
+            self.tau = 0
+
+        self.delta_w = 0
         self.beta = self.w0 / (2 * self.q_factor)  # Damping factor.
         self.mass = self.k / (self.w0 ** 2)  # Mass of the cantilever in kg.
-        self.amp = self.soft_amp * self.amp_invols  # Amplitude in meters.
+        
+        if hasattr(self, 'soft_amp') and hasattr(self, 'amp_invols'):
+            self.amp = self.soft_amp * self.amp_invols  # Amplitude in meters.
 
         # Calculate reduced driving force and phase in equilibrium.
         np.seterr(divide='ignore')  # suprress divide-by-0 warning in arctan
         self.f0 = self.amp * np.sqrt((self.w0 ** 2 - self.wd ** 2) ** 2 +
                                      4 * self.beta ** 2 * self.wd ** 2)
         self.delta = np.abs(np.arctan(np.divide(2 * self.wd * self.beta,
                                                 self.w0 ** 2 - self.wd ** 2)))
-
-        # Initialize force parameters and calculate some others.
-        for key, value in force_params.items():
-            setattr(self, key, value)
-
-        self.delta_w = PI2 * self.delta_freq  # Frequency shift in radians.
-        self.fe = self.es_force / self.mass  # Reduced electrostatic force.
-
-        # Initialize simulation parameters.
-        for key, value in sim_params.items():
-            setattr(self, key, value)
+        self.fe = 0 
+        
+        if hasattr(self, 'delta_freq'):
+            self.delta_w = PI2 * self.delta_freq  # Frequency shift in radians.
+        
+        if hasattr(self, 'es_force'):
+            self.fe = self.es_force / self.mass  # Reduced electrostatic force.
 
         # Calculate time axis for simulated tip motion without extra cycles
         num_pts = int(self.total_time * self.sampling_rate)
         self.t_Z = np.linspace(0, self.total_time, num=num_pts)
 
         # Calculate frequency axis for simulated tip_motion without extra cycles.
         self.freq_Z = np.linspace(0, int(self.sampling_rate / 2), num=int(num_pts / 2 + 1))
 
         # Create a Pixel class-compatible params file
         self.fit_params = {}
         self.parameters = force_params
         self.parameters.update(**sim_params)
         self.can_params = can_params
-        self.create_parameters(self.parameters, self.can_params)
+        #self.create_parameters(self.parameters, self.can_params)
 
         return
 
     def set_conditions(self, trigger_phase=180):
         """
         Sets initial conditions and other simulation parameters.
```

### Comparing `FFTA-0.3.5.0/ffta/simulation/electric_drive.py` & `FFTA-0.3.5.1/ffta/simulation/electric_drive.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 """simulate.py: Contains Cantilever class."""
 # pylint: disable=E1101,R0902,C0103
 __author__ = "Rajiv Giridharagopal"
 __copyright__ = "Copyright 2020, Ginger Lab"
 __email__ = "rgiri@uw.edu"
 __status__ = "Production"
 
-import numpy as np
 from math import pi
-from scipy.integrate import odeint
+
+import numpy as np
 
 from .cantilever import Cantilever
 from .utils import excitation
 
 # Set constant 2 * pi.
 PI2 = 2 * pi
 
 
 class ElectricDrive(Cantilever):
-    
 
     def __init__(self, can_params, force_params, sim_params, v_array=[], v_step=np.nan,
                  func=excitation.single_exp, func_args=[]):
         """Damped Driven Harmonic Oscillator Simulator for AFM Cantilevers under Electric drive
 
         Simulates a DDHO under excitation with given parameters.
```

### Comparing `FFTA-0.3.5.0/ffta/simulation/impulse.py` & `FFTA-0.3.5.1/ffta/simulation/impulse.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 # -*- coding: utf-8 -*-
 """
 Created on Sun May  8 13:59:18 2022
 
 @author: Raj
 """
 
-import numpy as np
-
 from .mechanical_drive import MechanicalDrive
 from .utils.load import params_from_experiment as load_parm
-from .utils.load import simulation_configuration as load_sim_config
-from ffta.pixel_utils.load import configuration
 
 
-def impulse(can_path, param_cfg=None, voltage = None, plot=False, **kwargs):
+def impulse(can_path, param_cfg=None, voltage=None, plot=False, **kwargs):
     '''
     Generates the impulse force response for a given cantilever given some particular
     parameters.
     
     :param can_path: Path to cantilever parameters.txt file 
     :type can_path: str
 
@@ -32,35 +28,35 @@
     
     :param kwargs: Passed to pixel.analyze (n_taps, method, etc)
     :type kwargs:
     
     '''
     if isinstance(can_path, str) and isinstance(param_cfg, str):
         can_params, force_params, sim_params, _, parms = load_parm(can_path, param_cfg)
-    elif isinstance(can_path, list) and isinstance(param_cfg, dict): #passing dictionaries directly
+    elif isinstance(can_path, list) and isinstance(param_cfg, dict):  # passing dictionaries directly
         can_params, force_params, sim_params = can_path
         parms = param_cfg
         can_params['drive_freq'] = parms['drive_freq']
         can_params['res_freq'] = parms['drive_freq']
         sim_params['trigger'] = parms['trigger']
         sim_params['total_time'] = parms['total_time']
         sim_params['sampling_rate'] = parms['sampling_rate']
     else:
         raise ValueError('Missing correct parameters path')
     # Use input voltage to calculate expected frequency shift with which to simulate
     if voltage:
-        k = can_params['k'] # N/m 
+        k = can_params['k']  # N/m
         resf = can_params['res_freq']
-        dFdz = force_params['dFdz'] # I think these values are off by 1000 somewhere
-        #dFdz = dFdz * 4 *k / resf , note dFdz is already saved scaled!!!
-        
-        delta_f =  resf / (4*k) * dFdz * voltage**2  # Marohn and others
+        dFdz = force_params['dFdz']  # I think these values are off by 1000 somewhere
+        # dFdz = dFdz * 4 *k / resf , note dFdz is already saved scaled!!!
+
+        delta_f = resf / (4 * k) * dFdz * voltage ** 2  # Marohn and others
         force_params['delta_freq'] = delta_f
-        force_params['es_force'] = (voltage / (force_params['lift_height']*1e-9))*1.6e-19
+        force_params['es_force'] = (voltage / (force_params['lift_height'] * 1e-9)) * 1.6e-19
         # #omega0 = resf * np.ones(len(voltage)) - delta_f
-    
-    force_params['tau'] = 1e-8 #"impulse"
+
+    force_params['tau'] = 1e-8  # "impulse"
     cant = MechanicalDrive(can_params, force_params, sim_params)
     Z, _ = cant.simulate()
     pix = cant.analyze(plot=plot, **kwargs)
-    
-    return pix, cant
+
+    return pix, cant
```

### Comparing `FFTA-0.3.5.0/ffta/simulation/mechanical_drive.py` & `FFTA-0.3.5.1/ffta/simulation/mechanical_drive.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 __author__ = "Rajiv Giridharagopal"
 __copyright__ = "Copyright 2020, Ginger Lab"
 __email__ = "rgiri@uw.edu"
 __status__ = "Production"
 
-import numpy as np
 from math import pi
-from scipy.integrate import odeint
+
+import numpy as np
 
 from .cantilever import Cantilever
 from .utils import excitation
 
 # Set constant 2 * pi.
 PI2 = 2 * pi
```

### Comparing `FFTA-0.3.5.0/ffta/simulation/mechanical_drive_simple.py` & `FFTA-0.3.5.1/ffta/simulation/mechanical_drive_simple.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 __author__ = "Rajiv Giridharagopal"
 __copyright__ = "Copyright 2020, Ginger Lab"
 __email__ = "rgiri@uw.edu"
 __status__ = "Production"
 
-import numpy as np
 from math import pi
-from scipy.integrate import odeint
+
+import numpy as np
 
 from .cantilever import Cantilever
 from .utils import excitation
 
 # Set constant 2 * pi.
 PI2 = 2 * pi
 
 
 class MechanicalDrive_Simple(Cantilever):
 
-    def __init__(self, can_params, force_params, sim_params,
+    def __init__(self, 
+                 can_params={}, 
+                 force_params={}, 
+                 sim_params={},
                  w_array=[]):
         """Damped Driven Harmonic Oscillator Simulator for AFM Cantilevers under 
         Mechanical drive (i.e. conventional DDHO)
 
-        Simulates a DDHO under excitation with explicitly supplied resonance frequency shift
-        and NO electrostatic force change
+        Simulates a DDHO under excitation with explicitly supplied resonance 
+        frequency shift and NO electrostatic force change
 
         Attributes
         ----------
         Z : ndarray
             ODE integration of the DDHO response
 
         Method
@@ -44,15 +47,15 @@
         --------
         >>> from ffta.simulation import mechanical_drive
         >>> from ffta.simulation.utils import load
         >>>
         >>> params_file = '../examples/sim_params.cfg'
         >>> params = load.simulation_configuration(params_file)
         >>>
-        >>> c = mechanical_dirve.MechanicalDrive(*params)
+        >>> c = mechanical_dirve.MechanicalDrive_Simple(*params)
         >>> Z, infodict = c.simulate()
         >>> c.analyze()
         >>> c.analyze(roi=0.004) # can change the parameters as desired
         >>>
         >>> # To supply an arbitary v_array
         >>> n_points = int(params[2]['total_time'] * params[2]['sampling_rate'])
         >>> v_array = np.ones(n_points) # create just a flat excitation
@@ -97,15 +100,15 @@
         parms = [can_params, force_params, sim_params]
         super(MechanicalDrive_Simple, self).__init__(*parms)
 
         # Did user supply a voltage pulse themselves 
         if len(w_array) != int(self.total_time * self.sampling_rate):
             print(int(self.total_time * self.sampling_rate))
             print(len(w_array))
-            raise ValueError('v_array must match sampling rate/length of parameters')
+            raise ValueError('w_array must match sampling rate/length of parameters')
 
         self.w_array = w_array
 
         return
 
     def omega(self, t):
         """
```

### Comparing `FFTA-0.3.5.0/ffta/simulation/utils/excitation.py` & `FFTA-0.3.5.1/ffta/simulation/utils/excitation.py`

 * *Files identical despite different names*

### Comparing `FFTA-0.3.5.0/ffta/simulation/utils/load.py` & `FFTA-0.3.5.1/ffta/simulation/utils/load.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 """
 Created on Tue May 12 11:23:17 2020
 
 @author: Raj
 """
 
 import configparser
+import urllib
+
 from ffta.pixel_utils.load import cantilever_params
 from ffta.pixel_utils.load import configuration
-import urllib
+
 
 def simulation_configuration(path, is_url=False):
     """
     Reads an ASCII file with relevant parameters for simulation.
 
     Parameters
     ----------
@@ -104,15 +106,15 @@
 
     params_cfg : string
         Path to parameters.cfg file (from FFtrEFM experiment, in the data folder)
     '''
 
     can = cantilever_params(can_params_file)
     _, par = configuration(params_cfg)
-    
+
     if isinstance(params_cfg, dict):
         par = params_cfg
 
     can_params = {}
     can_params['amp_invols'] = can['Initial']['AMPINVOLS']
     can_params['def_invols'] = can['Initial']['DEFINVOLS']
     can_params['soft_amp'] = 0.3
```

### Comparing `FFTA-0.3.5.0/setup.py` & `FFTA-0.3.5.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,17 +19,17 @@
     author='Rajiv Giridharagopal',
     author_email='rgiri@uw.edu',
     license='MIT',
     url='https://github.com/rajgiriUW/ffta/',
 
     packages=find_packages(exclude=['xop', 'docs', 'data', 'notebooks']),
 
-    install_requires=['numpy>=1.18.1',
+    install_requires=['numpy>=1.20.0',
                       'scipy>=1.4.1',
-                      'igor>=0.3',
+                      'igor2>=0.5.2',
                       'numexpr>=2.7.1',
                       'pyUSID>=0.0.10',
                       'pywavelets>=1.1.1',
                       'sidpy>=0.0.5',
                       'pandas>=1.1.0',
                       'BGlib>=0.0.3',
                       'torch>=1.6.0',
```

### Comparing `FFTA-0.3.5.0/tests/test_ffta.py` & `FFTA-0.3.5.1/tests/test_ffta.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import os
 import sys
-import pytest
+
 import numpy as np
-import h5py
 
 sys.path.insert(0, '..')
 
 import ffta
 import pyUSID as usid
-from ffta.simulation import mechanical_drive
 
+from ffta.simulation.mechanical_drive import MechanicalDrive
+from ffta.simulation.utils.load import simulation_configuration
+from ffta.simulation.utils import excitation
 
 # Testing of standard process flow
 class TestFFTA:
     ff_folder = 'tests/testdata'
     ff_file = 'tests/testdata/FF_H5.h5'
 
     def delete_old_h5(self):
@@ -30,15 +31,15 @@
         except:
             print('###### Error with old .h5 file')
 
     def test_load_data_files(self):
         self.delete_old_h5()
         h5_path, data_files, parm_dict = ffta.load.load_hdf.load_folder(folder_path=self.ff_folder)
         assert (len(data_files) == 8)
-        assert (len(parm_dict.items()) == 23)        
+        assert (len(parm_dict.items()) == 23)
         assert (type(h5_path) == str)
 
     def test_load_FF(self):
         self.delete_old_h5()
         h5_path, data_files, parm_dict = ffta.load.load_hdf.load_folder(folder_path=self.ff_folder)
         h5_path = h5_path.replace('\\', '/')  # travis
         h5_avg = ffta.load.load_hdf.load_FF(data_files, parm_dict, h5_path)
@@ -113,7 +114,31 @@
 
     # def test_pixel_nfmd(self):
     #     self.load_deflection()
     #     pix = ffta.pixel.Pixel(self.Z, trigger=5e-4, total_time=5e-3, roi=1e-3, method='nfmd')
     #     pix.analyze()
     #
     #     assert (pix.tfp > 1e-6 and pix.tfp < 500e-4)
+
+class TestSimulation:
+
+    if 'testdata' in os.getcwd():
+        os.chdir('..')
+        os.chdir('..')
+    path = r'tests/example_sim_params.cfg'
+
+    def test_read_sim_config(self):
+        can_params, force_params, sim_params = simulation_configuration(self.path)
+        assert (force_params['es_force'] == 3e-09 and force_params['delta_freq'] == -277.53 
+                and force_params['tau'] ==1e-05)
+        return
+
+    def test_mech_drive(self):
+        can_params, force_params, sim_params = simulation_configuration(self.path)
+        cant = MechanicalDrive(can_params, force_params, sim_params)
+        assert (cant.tau == 1e-5)
+
+        Z, info = cant.simulate()
+        assert(len(Z.shape) > 0)
+
+        return
+
```

